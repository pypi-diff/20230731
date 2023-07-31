# Comparing `tmp/python-tackerclient-1.8.0.tar.gz` & `tmp/python-tackerclient-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-tackerclient-1.8.0.tar", last modified: Fri Sep  3 11:33:03 2021, max compression
+gzip compressed data, was "python-tackerclient-1.9.0.tar", last modified: Fri Jan  7 14:38:44 2022, max compression
```

## Comparing `python-tackerclient-1.8.0.tar` & `python-tackerclient-1.9.0.tar`

### file list

```diff
@@ -1,254 +1,254 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.354190 python-tackerclient-1.8.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1386 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/.pylintrc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4252 2021-09-03 11:33:03.000000 python-tackerclient-1.8.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15517 2021-09-03 11:33:03.000000 python-tackerclient-1.8.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1209 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3191 2021-09-03 11:33:03.354190 python-tackerclient-1.8.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1692 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.310192 python-tackerclient-1.8.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.310192 python-tackerclient-1.8.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.310192 python-tackerclient-1.8.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5309 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/doc/source/cli/commands.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/doc/source/cli/vnf_package_commands.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2921 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.310192 python-tackerclient-1.8.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      942 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5116 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/doc/source/contributor/developing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1146 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1492 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.310192 python-tackerclient-1.8.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1641 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.310192 python-tackerclient-1.8.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/doc/source/reference/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      997 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/lower-constraints.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.314192 python-tackerclient-1.8.0/python_tackerclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3191 2021-09-03 11:33:03.000000 python-tackerclient-1.8.0/python_tackerclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9322 2021-09-03 11:33:03.000000 python-tackerclient-1.8.0/python_tackerclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-09-03 11:33:03.000000 python-tackerclient-1.8.0/python_tackerclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5155 2021-09-03 11:33:03.000000 python-tackerclient-1.8.0/python_tackerclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-09-03 11:33:03.000000 python-tackerclient-1.8.0/python_tackerclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-09-03 11:33:03.000000 python-tackerclient-1.8.0/python_tackerclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2021-09-03 11:33:03.000000 python-tackerclient-1.8.0/python_tackerclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2021-09-03 11:33:03.000000 python-tackerclient-1.8.0/python_tackerclient.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.302192 python-tackerclient-1.8.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.318191 python-tackerclient-1.8.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/notes/add-creating-ns-vnffg-from-template-213eee7f1820aa0c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/notes/add-vnffg-and-vnf-ids-to-ns-list-commands-9d462efc103f8ecb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/notes/bug-1750865-04c3ebd0c3f8af29.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/notes/bug-1754556-53268d3081fa18d1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/notes/bug-1754793-54446bcd0a4e84aa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/notes/bug-1754926-06ac4d7ffd17b5ce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/notes/clustering-service-cli-e15cc6627de293fa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/notes/del-project_and_user_id-e9dd396f83a162d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/notes/deprecate-direct-yaml-cli-input-812564bab1b99b4b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/notes/deprecate-infra-mgmt-driver-attributes-e371624c50accee8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/notes/deprecated-tacker-command-29121558bd748082.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/notes/drop-py-2-7-b2052825c4b92b52.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/notes/multi-delete-support-in-tacker-acd4a7e86114f0be.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/notes/network-services-descriptor-06f6abe90adb40f3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/notes/new-commmand-vnf-resource-list-d5422ab917f0892f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/notes/remove-passing-mgmt-and-infra-driver-from-client-c9135f84480b2cae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/notes/tacker-support-python-openstackclient-b88b20b80b872229.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/notes/update-vim-without-config-c3b637741889eff6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/notes/vnf-inline-template-25f6a0b66f7407a1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/notes/vnfd-vnf-vim-name-mandatory-in-tacker-cli-dfe802af6de5c80e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/notes/vnffg-client-abd7d7f06860b91d.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.322191 python-tackerclient-1.8.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.322191 python-tackerclient-1.8.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.322191 python-tackerclient-1.8.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8504 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      644 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6107 2021-09-03 11:33:03.354190 python-tackerclient-1.8.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/setup.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      294 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tacker_test.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.322191 python-tackerclient-1.8.0/tackerclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14816 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.326191 python-tackerclient-1.8.0/tackerclient/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1205 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/common/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3785 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/common/clientmanager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1221 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/common/command.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1148 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/common/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5865 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/common/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3368 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/common/extension.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14635 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/common/serializer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5806 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2614 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/common/validators.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.326191 python-tackerclient-1.8.0/tackerclient/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.326191 python-tackerclient-1.8.0/tackerclient/osc/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.326191 python-tackerclient-1.8.0/tackerclient/osc/common/vnflcm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/common/vnflcm/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1758 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/common/vnflcm/vnflcm_versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1919 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4348 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/sdk_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7872 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.326191 python-tackerclient-1.8.0/tackerclient/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/v1/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.326191 python-tackerclient-1.8.0/tackerclient/osc/v1/events/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/v1/events/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4210 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/v1/events/events.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.330191 python-tackerclient-1.8.0/tackerclient/osc/v1/nfvo/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/v1/nfvo/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9347 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/v1/nfvo/ns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7870 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/v1/nfvo/nsd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9931 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/v1/nfvo/vim.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20864 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/v1/nfvo/vnffg.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7786 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/v1/nfvo/vnffgd.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.330191 python-tackerclient-1.8.0/tackerclient/osc/v1/vnflcm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/v1/vnflcm/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.330191 python-tackerclient-1.8.0/tackerclient/osc/v1/vnflcm/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1707 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/v1/vnflcm/samples/change_ext_conn_vnf_instance_param_sample.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2517 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/v1/vnflcm/samples/instantiate_vnf_instance_param_sample.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/v1/vnflcm/samples/scale_vnf_instance_param_sample.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/v1/vnflcm/samples/update_vnf_instance_param_sample.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20811 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/v1/vnflcm/vnflcm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10290 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/v1/vnflcm/vnflcm_op_occs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.330191 python-tackerclient-1.8.0/tackerclient/osc/v1/vnfm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/v1/vnfm/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17461 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/v1/vnfm/vnf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8015 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/v1/vnfm/vnfd.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.330191 python-tackerclient-1.8.0/tackerclient/osc/v1/vnfpkgm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/v1/vnfpkgm/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19486 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/osc/v1/vnfpkgm/vnf_package.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33600 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.330191 python-tackerclient-1.8.0/tackerclient/tacker/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tacker/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2556 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tacker/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.330191 python-tackerclient-1.8.0/tackerclient/tacker/v1_0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26569 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tacker/v1_0/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.334191 python-tackerclient-1.8.0/tackerclient/tacker/v1_0/events/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tacker/v1_0/events/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3181 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tacker/v1_0/events/events.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1011 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tacker/v1_0/extension.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.334191 python-tackerclient-1.8.0/tackerclient/tacker/v1_0/nfvo/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tacker/v1_0/nfvo/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5045 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tacker/v1_0/nfvo/ns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3324 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tacker/v1_0/nfvo/nsd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4822 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tacker/v1_0/nfvo/vim.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3646 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tacker/v1_0/nfvo/vim_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7259 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tacker/v1_0/nfvo/vnfcluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8135 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tacker/v1_0/nfvo/vnffg.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3389 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tacker/v1_0/nfvo/vnffgd.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.334191 python-tackerclient-1.8.0/tackerclient/tacker/v1_0/vnfm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tacker/v1_0/vnfm/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12482 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tacker/v1_0/vnfm/vnf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3819 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tacker/v1_0/vnfm/vnfd.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.334191 python-tackerclient-1.8.0/tackerclient/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.338191 python-tackerclient-1.8.0/tackerclient/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.338191 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2786 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.338191 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3964 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/common/test_vnflcm_versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.342191 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/samples/vnf_update_config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        3 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/samples/vnf_update_config_file_with_empty_dict.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/samples/vnf_update_empty_config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/samples/vnf_update_empty_param.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/samples/vnf_update_invalid_format_config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/samples/vnf_update_invalid_format_param.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/samples/vnf_update_param.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        3 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/samples/vnf_update_param_file_with_empty_dict.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.342191 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.342191 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2551 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.302192 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.342191 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9191 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/etsi_nfv_sol001_common_types.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    67244 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/etsi_nfv_sol001_vnfd_types.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7726 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_df_simple.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_top.vnfd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1542 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_types.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.346191 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/TOSCA-Metadata/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/TOSCA-Metadata/TOSCA.meta
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.306192 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.346191 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9125 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/etsi_nfv_sol001_common_types.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    67211 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/etsi_nfv_sol001_vnfd_types.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7726 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_df_simple.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_top.vnfd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1542 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_types.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.346191 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Scripts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Scripts/install.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.346191 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/TOSCA-Metadata/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/TOSCA-Metadata/TOSCA.meta
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33930 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/test_vnf_package.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35824 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/test_vnflcm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18266 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/test_vnflcm_op_occs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.346191 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/vnf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/vnf/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12082 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/vnf/test_vnf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6767 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/vnf_package_fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5768 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/vnflcm_fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3373 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/vnflcm_op_occs_fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.346191 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1248 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v2/test_vnflcm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14453 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/test_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4764 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/test_casual_args.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33751 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/test_cli10.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1939 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/test_cli10_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1317 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/test_command_meta.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2541 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/test_http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7149 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3116 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/test_ssl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5090 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4099 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/test_validators.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.350191 python-tackerclient-1.8.0/tackerclient/tests/unit/vm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/vm/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.350191 python-tackerclient-1.8.0/tackerclient/tests/unit/vm/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/vm/samples/vim_config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/vm/samples/vim_config_with_false_cert_verify.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/vm/samples/vim_config_without_auth_url.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/vm/samples/vim_k8s_bearer_token.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/vm/samples/vim_k8s_bearer_token_without_auth_url.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/vm/samples/vim_k8s_config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/vm/samples/vim_k8s_config_without_auth_url.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/vm/samples/vnffg_update_file.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2797 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/vm/test_cli10_v10_event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8270 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/vm/test_cli10_vim.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7011 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/vm/test_cli10_vim_k8s.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6970 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/vm/test_cli10_vim_k8s_with_bearer_token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21202 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/vm/test_cli10_vnf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5560 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/vm/test_cli10_vnfd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4815 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/vm/test_cli10_vnffg.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4387 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/vm/test_cli10_vnffgd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4525 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/tests/unit/vm/test_vim_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.350191 python-tackerclient-1.8.0/tackerclient/v1_0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/v1_0/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    49499 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/v1_0/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      759 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tackerclient/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-03 11:33:03.350191 python-tackerclient-1.8.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tools/tacker.bash_completion
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1634 2021-09-03 11:32:27.000000 python-tackerclient-1.8.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.596289 python-tackerclient-1.9.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1386 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/.pylintrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4328 2022-01-07 14:38:44.000000 python-tackerclient-1.9.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15793 2022-01-07 14:38:44.000000 python-tackerclient-1.9.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1209 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3291 2022-01-07 14:38:44.596289 python-tackerclient-1.9.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1692 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.580289 python-tackerclient-1.9.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.580289 python-tackerclient-1.9.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.580289 python-tackerclient-1.9.0/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5309 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/doc/source/cli/commands.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/doc/source/cli/vnf_package_commands.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2921 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.584288 python-tackerclient-1.9.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      942 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5116 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/doc/source/contributor/developing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1146 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1492 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.584288 python-tackerclient-1.9.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1641 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.584288 python-tackerclient-1.9.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.584288 python-tackerclient-1.9.0/python_tackerclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3291 2022-01-07 14:38:44.000000 python-tackerclient-1.9.0/python_tackerclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9323 2022-01-07 14:38:44.000000 python-tackerclient-1.9.0/python_tackerclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-01-07 14:38:44.000000 python-tackerclient-1.9.0/python_tackerclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5231 2022-01-07 14:38:44.000000 python-tackerclient-1.9.0/python_tackerclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-01-07 14:38:44.000000 python-tackerclient-1.9.0/python_tackerclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2022-01-07 14:38:44.000000 python-tackerclient-1.9.0/python_tackerclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2022-01-07 14:38:44.000000 python-tackerclient-1.9.0/python_tackerclient.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.576288 python-tackerclient-1.9.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.584288 python-tackerclient-1.9.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/notes/add-creating-ns-vnffg-from-template-213eee7f1820aa0c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/notes/add-vnffg-and-vnf-ids-to-ns-list-commands-9d462efc103f8ecb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/notes/bug-1750865-04c3ebd0c3f8af29.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/notes/bug-1754556-53268d3081fa18d1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/notes/bug-1754793-54446bcd0a4e84aa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/notes/bug-1754926-06ac4d7ffd17b5ce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/notes/clustering-service-cli-e15cc6627de293fa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/notes/del-project_and_user_id-e9dd396f83a162d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/notes/deprecate-direct-yaml-cli-input-812564bab1b99b4b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/notes/deprecate-infra-mgmt-driver-attributes-e371624c50accee8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/notes/deprecated-tacker-command-29121558bd748082.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/notes/drop-py-2-7-b2052825c4b92b52.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/notes/multi-delete-support-in-tacker-acd4a7e86114f0be.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/notes/network-services-descriptor-06f6abe90adb40f3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/notes/new-commmand-vnf-resource-list-d5422ab917f0892f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/notes/remove-passing-mgmt-and-infra-driver-from-client-c9135f84480b2cae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/notes/tacker-support-python-openstackclient-b88b20b80b872229.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/notes/update-vim-without-config-c3b637741889eff6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/notes/vnf-inline-template-25f6a0b66f7407a1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/notes/vnfd-vnf-vim-name-mandatory-in-tacker-cli-dfe802af6de5c80e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/notes/vnffg-client-abd7d7f06860b91d.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.584288 python-tackerclient-1.9.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.584288 python-tackerclient-1.9.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.584288 python-tackerclient-1.9.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8504 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      644 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6262 2022-01-07 14:38:44.600288 python-tackerclient-1.9.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/setup.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      294 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tacker_test.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.588288 python-tackerclient-1.9.0/tackerclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14816 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.588288 python-tackerclient-1.9.0/tackerclient/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1205 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/common/_i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3785 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/common/clientmanager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1221 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/common/command.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1148 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/common/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5865 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/common/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3368 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/common/extension.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14635 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/common/serializer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5806 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2614 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/common/validators.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.588288 python-tackerclient-1.9.0/tackerclient/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.588288 python-tackerclient-1.9.0/tackerclient/osc/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.588288 python-tackerclient-1.9.0/tackerclient/osc/common/vnflcm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/common/vnflcm/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1758 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/common/vnflcm/vnflcm_versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1919 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4348 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/sdk_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7872 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.588288 python-tackerclient-1.9.0/tackerclient/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.588288 python-tackerclient-1.9.0/tackerclient/osc/v1/events/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/v1/events/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4210 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/v1/events/events.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.588288 python-tackerclient-1.9.0/tackerclient/osc/v1/nfvo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/v1/nfvo/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9347 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/v1/nfvo/ns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7870 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/v1/nfvo/nsd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9931 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/v1/nfvo/vim.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20864 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/v1/nfvo/vnffg.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7786 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/v1/nfvo/vnffgd.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.588288 python-tackerclient-1.9.0/tackerclient/osc/v1/vnflcm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/v1/vnflcm/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.588288 python-tackerclient-1.9.0/tackerclient/osc/v1/vnflcm/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1707 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/v1/vnflcm/samples/change_ext_conn_vnf_instance_param_sample.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2517 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/v1/vnflcm/samples/instantiate_vnf_instance_param_sample.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/v1/vnflcm/samples/scale_vnf_instance_param_sample.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/v1/vnflcm/samples/update_vnf_instance_param_sample.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20811 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/v1/vnflcm/vnflcm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11678 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/v1/vnflcm/vnflcm_op_occs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.588288 python-tackerclient-1.9.0/tackerclient/osc/v1/vnfm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/v1/vnfm/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17461 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/v1/vnfm/vnf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8015 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/v1/vnfm/vnfd.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.588288 python-tackerclient-1.9.0/tackerclient/osc/v1/vnfpkgm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/v1/vnfpkgm/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19486 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/osc/v1/vnfpkgm/vnf_package.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33600 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.588288 python-tackerclient-1.9.0/tackerclient/tacker/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tacker/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2556 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tacker/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.588288 python-tackerclient-1.9.0/tackerclient/tacker/v1_0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26569 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tacker/v1_0/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.588288 python-tackerclient-1.9.0/tackerclient/tacker/v1_0/events/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tacker/v1_0/events/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3181 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tacker/v1_0/events/events.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1011 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tacker/v1_0/extension.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.592288 python-tackerclient-1.9.0/tackerclient/tacker/v1_0/nfvo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tacker/v1_0/nfvo/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5045 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tacker/v1_0/nfvo/ns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3324 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tacker/v1_0/nfvo/nsd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4822 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tacker/v1_0/nfvo/vim.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3646 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tacker/v1_0/nfvo/vim_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7259 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tacker/v1_0/nfvo/vnfcluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8135 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tacker/v1_0/nfvo/vnffg.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3389 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tacker/v1_0/nfvo/vnffgd.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.592288 python-tackerclient-1.9.0/tackerclient/tacker/v1_0/vnfm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tacker/v1_0/vnfm/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12482 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tacker/v1_0/vnfm/vnf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3819 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tacker/v1_0/vnfm/vnfd.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.592288 python-tackerclient-1.9.0/tackerclient/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.592288 python-tackerclient-1.9.0/tackerclient/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.592288 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2786 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.592288 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3964 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/common/test_vnflcm_versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.592288 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/samples/vnf_update_config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        3 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/samples/vnf_update_config_file_with_empty_dict.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/samples/vnf_update_empty_config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/samples/vnf_update_empty_param.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/samples/vnf_update_invalid_format_config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/samples/vnf_update_invalid_format_param.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/samples/vnf_update_param.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        3 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/samples/vnf_update_param_file_with_empty_dict.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.592288 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.592288 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2551 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.580289 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.596289 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9191 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/etsi_nfv_sol001_common_types.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    67244 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/etsi_nfv_sol001_vnfd_types.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7726 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_df_simple.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_top.vnfd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1542 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_types.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.596289 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/TOSCA-Metadata/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/TOSCA-Metadata/TOSCA.meta
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.580289 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.596289 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9125 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/etsi_nfv_sol001_common_types.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    67211 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/etsi_nfv_sol001_vnfd_types.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7726 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_df_simple.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_top.vnfd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1542 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_types.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.596289 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Scripts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Scripts/install.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.596289 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/TOSCA-Metadata/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/TOSCA-Metadata/TOSCA.meta
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33930 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/test_vnf_package.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35824 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/test_vnflcm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20523 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/test_vnflcm_op_occs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.596289 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/vnf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/vnf/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12082 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/vnf/test_vnf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6767 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/vnf_package_fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5768 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/vnflcm_fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3373 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/vnflcm_op_occs_fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.596289 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1248 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v2/test_vnflcm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14453 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/test_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4764 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/test_casual_args.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33751 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/test_cli10.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1939 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/test_cli10_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1317 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/test_command_meta.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2541 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/test_http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7149 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3116 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/test_ssl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5090 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4099 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/test_validators.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.596289 python-tackerclient-1.9.0/tackerclient/tests/unit/vm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/vm/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.596289 python-tackerclient-1.9.0/tackerclient/tests/unit/vm/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/vm/samples/vim_config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/vm/samples/vim_config_with_false_cert_verify.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/vm/samples/vim_config_without_auth_url.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/vm/samples/vim_k8s_bearer_token.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/vm/samples/vim_k8s_bearer_token_without_auth_url.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/vm/samples/vim_k8s_config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/vm/samples/vim_k8s_config_without_auth_url.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/vm/samples/vnffg_update_file.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2797 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/vm/test_cli10_v10_event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8270 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/vm/test_cli10_vim.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7011 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/vm/test_cli10_vim_k8s.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6970 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/vm/test_cli10_vim_k8s_with_bearer_token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21202 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/vm/test_cli10_vnf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5560 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/vm/test_cli10_vnfd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4815 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/vm/test_cli10_vnffg.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4387 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/vm/test_cli10_vnffgd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4525 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/tests/unit/vm/test_vim_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.596289 python-tackerclient-1.9.0/tackerclient/v1_0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/v1_0/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    49798 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/v1_0/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      759 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tackerclient/version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-01-07 14:38:44.596289 python-tackerclient-1.9.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tools/tacker.bash_completion
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1494 2022-01-07 14:38:10.000000 python-tackerclient-1.9.0/tox.ini
```

### Comparing `python-tackerclient-1.8.0/.pylintrc` & `python-tackerclient-1.9.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/AUTHORS` & `python-tackerclient-1.9.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 Dirk Mueller <dirk@dmllr.de>
 Donghun Cha <dcha94@dcn.ssu.ac.kr>
 Doug Hellmann <doug@doughellmann.com>
 Flavio Percoco <flaper87@gmail.com>
 Ghanshyam Mann <gmann@ghanshyammann.com>
 Hervé Beraud <hberaud@redhat.com>
 Hideki Saito <saito@fgrep.org>
+Hiromu Asahina <hiromu.asahina.az@hco.ntt.co.jp>
 Hiroo Kitamura <hiroo.kitamura@ntt-at.co.jp>
 Hiroya Nakaya <nakaya.hr@ncos.nec.co.jp>
 Isaku Yamahata <isaku.yamahata@intel.com>
 Itsuro Oda <oda@valinux.co.jp>
 Janki <jankihchhatbar@gmail.com>
 Janki <jchhatba@redhat.com>
 Janki Chhatbar <jankihchhatbar@gmail.com>
@@ -87,14 +88,15 @@
 howardlee <lihongweibj@inspur.com>
 huxining <xining@unitedstack.com>
 jacky06 <zhang.min@99cloud.net>
 janki <jchhatba@redhat.com>
 ji-xuepeng <ji.xuepeng@zte.com.cn>
 kavithahr <kavitha.r@nectechnologies.in>
 lingyongxu <lyxu@fiberhome.com>
+maaoyu <maaoyu@inspur.com>
 nirajsingh <niraj.singh@nttdata.com>
 pengyuesheng <pengyuesheng@gohighsec.com>
 prankul mahajan <prankul.mahajan88@gmail.com>
 qingszhao <zhao.daqing@99cloud.net>
 rajat29 <rajat.sharma@nectechnologies.in>
 ricolin <rico.l@inwinstack.com>
 rtmdk <rtmdk@163.com>
```

### Comparing `python-tackerclient-1.8.0/CONTRIBUTING.rst` & `python-tackerclient-1.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/ChangeLog` & `python-tackerclient-1.9.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 CHANGES
 =======
 
+1.9.0
+-----
+
+* Update python testing classifier
+* Support of Cancel VNF command in openstackclient
+* Add Python3 yoga unit tests
+* Drop test for lower constraints
+* Update master for stable/xena
+
 1.8.0
 -----
 
 * Multi version API support
 * Remove use of testtools.helpers.safe\_hasattr
 * Remove broken link from Python-TackerClient guide
 * Correct YAML load warning
 * vnfConfigurableProperties missing in VNF show
 
 1.7.0
 -----
 
 * Use assertCountEqual instead of assertItemsEqual
 * Update min version of tox
+* setup.cfg: Replace dashes with underscores
 * Add Python3 xena unit tests
 * Adds support force delete VNFFG
 * Fix failing UT in TestListVnfLcmOp
+* Update master for stable/wallaby
 
 1.6.0
 -----
 
 * CLI for Individual VNF LCM Operation Occurrence
 * Support CLI for Getting List of VNF LCM Operation Occurrences
 * Support of Retry VNF command in openstackclient
```

### Comparing `python-tackerclient-1.8.0/HACKING.rst` & `python-tackerclient-1.9.0/HACKING.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/LICENSE` & `python-tackerclient-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/PKG-INFO` & `python-tackerclient-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-tackerclient
-Version: 1.8.0
+Version: 1.9.0
 Summary: CLI and Client Library for OpenStack Tacker
 Home-page: https://docs.openstack.org/python-tackerclient/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -86,8 +86,10 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
```

### Comparing `python-tackerclient-1.8.0/README.rst` & `python-tackerclient-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/doc/source/cli/commands.rst` & `python-tackerclient-1.9.0/doc/source/cli/commands.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/doc/source/conf.py` & `python-tackerclient-1.9.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/doc/source/contributor/contributing.rst` & `python-tackerclient-1.9.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/doc/source/contributor/developing.rst` & `python-tackerclient-1.9.0/doc/source/contributor/developing.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/doc/source/contributor/index.rst` & `python-tackerclient-1.9.0/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/doc/source/index.rst` & `python-tackerclient-1.9.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/doc/source/install/index.rst` & `python-tackerclient-1.9.0/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/doc/source/reference/index.rst` & `python-tackerclient-1.9.0/doc/source/reference/index.rst`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/python_tackerclient.egg-info/PKG-INFO` & `python-tackerclient-1.9.0/python_tackerclient.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-tackerclient
-Version: 1.8.0
+Version: 1.9.0
 Summary: CLI and Client Library for OpenStack Tacker
 Home-page: https://docs.openstack.org/python-tackerclient/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -86,8 +86,10 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
```

### Comparing `python-tackerclient-1.8.0/python_tackerclient.egg-info/SOURCES.txt` & `python-tackerclient-1.9.0/python_tackerclient.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 AUTHORS
 CONTRIBUTING.rst
 ChangeLog
 HACKING.rst
 LICENSE
 MANIFEST.in
 README.rst
-lower-constraints.txt
 requirements.txt
 setup.cfg
 setup.py
 tacker_test.sh
 test-requirements.txt
 tox.ini
 doc/requirements.txt
@@ -28,15 +27,14 @@
 doc/source/install/index.rst
 doc/source/reference/index.rst
 python_tackerclient.egg-info/PKG-INFO
 python_tackerclient.egg-info/SOURCES.txt
 python_tackerclient.egg-info/dependency_links.txt
 python_tackerclient.egg-info/entry_points.txt
 python_tackerclient.egg-info/not-zip-safe
-python_tackerclient.egg-info/pbr.json
 python_tackerclient.egg-info/requires.txt
 python_tackerclient.egg-info/top_level.txt
 releasenotes/notes/add-creating-ns-vnffg-from-template-213eee7f1820aa0c.yaml
 releasenotes/notes/add-vnffg-and-vnf-ids-to-ns-list-commands-9d462efc103f8ecb.yaml
 releasenotes/notes/bug-1750865-04c3ebd0c3f8af29.yaml
 releasenotes/notes/bug-1754556-53268d3081fa18d1.yaml
 releasenotes/notes/bug-1754793-54446bcd0a4e84aa.yaml
@@ -64,14 +62,16 @@
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
 releasenotes/source/stein.rst
 releasenotes/source/train.rst
 releasenotes/source/unreleased.rst
 releasenotes/source/ussuri.rst
 releasenotes/source/victoria.rst
+releasenotes/source/wallaby.rst
+releasenotes/source/xena.rst
 releasenotes/source/_static/.placeholder
 releasenotes/source/_templates/.placeholder
 tackerclient/__init__.py
 tackerclient/client.py
 tackerclient/i18n.py
 tackerclient/shell.py
 tackerclient/version.py
```

### Comparing `python-tackerclient-1.8.0/python_tackerclient.egg-info/entry_points.txt` & `python-tackerclient-1.9.0/python_tackerclient.egg-info/entry_points.txt`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 vnf_show = tackerclient.osc.v1.vnfm.vnf:ShowVNF
 vnflcm_change-ext-conn = tackerclient.osc.v1.vnflcm.vnflcm:ChangeExtConnVnfLcm
 vnflcm_create = tackerclient.osc.v1.vnflcm.vnflcm:CreateVnfLcm
 vnflcm_delete = tackerclient.osc.v1.vnflcm.vnflcm:DeleteVnfLcm
 vnflcm_heal = tackerclient.osc.v1.vnflcm.vnflcm:HealVnfLcm
 vnflcm_instantiate = tackerclient.osc.v1.vnflcm.vnflcm:InstantiateVnfLcm
 vnflcm_list = tackerclient.osc.v1.vnflcm.vnflcm:ListVnfLcm
+vnflcm_op_cancel = tackerclient.osc.v1.vnflcm.vnflcm_op_occs:CancelVnfLcmOp
 vnflcm_op_fail = tackerclient.osc.v1.vnflcm.vnflcm_op_occs:FailVnfLcmOp
 vnflcm_op_list = tackerclient.osc.v1.vnflcm.vnflcm_op_occs:ListVnfLcmOp
 vnflcm_op_retry = tackerclient.osc.v1.vnflcm.vnflcm_op_occs:RetryVnfLcmOp
 vnflcm_op_rollback = tackerclient.osc.v1.vnflcm.vnflcm_op_occs:RollbackVnfLcmOp
 vnflcm_op_show = tackerclient.osc.v1.vnflcm.vnflcm_op_occs:ShowVnfLcmOp
 vnflcm_scale = tackerclient.osc.v1.vnflcm.vnflcm:ScaleVnfLcm
 vnflcm_show = tackerclient.osc.v1.vnflcm.vnflcm:ShowVnfLcm
```

### Comparing `python-tackerclient-1.8.0/releasenotes/source/conf.py` & `python-tackerclient-1.9.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/requirements.txt` & `python-tackerclient-1.9.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/setup.cfg` & `python-tackerclient-1.9.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 [metadata]
 name = python-tackerclient
 summary = CLI and Client Library for OpenStack Tacker
-description-file = 
+description_file = 
 	README.rst
 author = OpenStack
-author-email = openstack-discuss@lists.openstack.org
-home-page = https://docs.openstack.org/python-tackerclient/
-python-requires = >=3.6
+author_email = openstack-discuss@lists.openstack.org
+home_page = https://docs.openstack.org/python-tackerclient/
+python_requires = >=3.6
 classifier = 
 	Environment :: OpenStack
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
 
 [files]
 packages = 
 	tackerclient
 
 [entry_points]
 console_scripts = 
@@ -90,14 +92,15 @@
 	vnflcm_terminate = tackerclient.osc.v1.vnflcm.vnflcm:TerminateVnfLcm
 	vnflcm_delete = tackerclient.osc.v1.vnflcm.vnflcm:DeleteVnfLcm
 	vnflcm_heal = tackerclient.osc.v1.vnflcm.vnflcm:HealVnfLcm
 	vnflcm_update = tackerclient.osc.v1.vnflcm.vnflcm:UpdateVnfLcm
 	vnflcm_scale = tackerclient.osc.v1.vnflcm.vnflcm:ScaleVnfLcm
 	vnflcm_change-ext-conn = tackerclient.osc.v1.vnflcm.vnflcm:ChangeExtConnVnfLcm
 	vnflcm_op_rollback = tackerclient.osc.v1.vnflcm.vnflcm_op_occs:RollbackVnfLcmOp
+	vnflcm_op_cancel = tackerclient.osc.v1.vnflcm.vnflcm_op_occs:CancelVnfLcmOp
 	vnflcm_op_fail = tackerclient.osc.v1.vnflcm.vnflcm_op_occs:FailVnfLcmOp
 	vnflcm_op_retry = tackerclient.osc.v1.vnflcm.vnflcm_op_occs:RetryVnfLcmOp
 	vnflcm_op_list = tackerclient.osc.v1.vnflcm.vnflcm_op_occs:ListVnfLcmOp
 	vnflcm_op_show = tackerclient.osc.v1.vnflcm.vnflcm_op_occs:ShowVnfLcmOp
 	vnflcm_versions = tackerclient.osc.common.vnflcm.vnflcm_versions:VnfLcmVersions
 openstack.tackerclient.v2 = 
 	vnflcm_create = tackerclient.osc.v1.vnflcm.vnflcm:CreateVnfLcm
```

### Comparing `python-tackerclient-1.8.0/setup.py` & `python-tackerclient-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/client.py` & `python-tackerclient-1.9.0/tackerclient/client.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/common/_i18n.py` & `python-tackerclient-1.9.0/tackerclient/common/_i18n.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/common/clientmanager.py` & `python-tackerclient-1.9.0/tackerclient/common/clientmanager.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/common/command.py` & `python-tackerclient-1.9.0/tackerclient/common/command.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/common/constants.py` & `python-tackerclient-1.9.0/tackerclient/common/constants.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/common/exceptions.py` & `python-tackerclient-1.9.0/tackerclient/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/common/extension.py` & `python-tackerclient-1.9.0/tackerclient/common/extension.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/common/serializer.py` & `python-tackerclient-1.9.0/tackerclient/common/serializer.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/common/utils.py` & `python-tackerclient-1.9.0/tackerclient/common/utils.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/common/validators.py` & `python-tackerclient-1.9.0/tackerclient/common/validators.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/i18n.py` & `python-tackerclient-1.9.0/tackerclient/i18n.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/osc/common/vnflcm/vnflcm_versions.py` & `python-tackerclient-1.9.0/tackerclient/osc/common/vnflcm/vnflcm_versions.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/osc/plugin.py` & `python-tackerclient-1.9.0/tackerclient/osc/plugin.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/osc/sdk_utils.py` & `python-tackerclient-1.9.0/tackerclient/osc/sdk_utils.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/osc/utils.py` & `python-tackerclient-1.9.0/tackerclient/osc/utils.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/osc/v1/events/events.py` & `python-tackerclient-1.9.0/tackerclient/osc/v1/events/events.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/osc/v1/nfvo/ns.py` & `python-tackerclient-1.9.0/tackerclient/osc/v1/nfvo/ns.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/osc/v1/nfvo/nsd.py` & `python-tackerclient-1.9.0/tackerclient/osc/v1/nfvo/nsd.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/osc/v1/nfvo/vim.py` & `python-tackerclient-1.9.0/tackerclient/osc/v1/nfvo/vim.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/osc/v1/nfvo/vnffg.py` & `python-tackerclient-1.9.0/tackerclient/osc/v1/nfvo/vnffg.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/osc/v1/nfvo/vnffgd.py` & `python-tackerclient-1.9.0/tackerclient/osc/v1/nfvo/vnffgd.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/osc/v1/vnflcm/samples/change_ext_conn_vnf_instance_param_sample.json` & `python-tackerclient-1.9.0/tackerclient/osc/v1/vnflcm/samples/change_ext_conn_vnf_instance_param_sample.json`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/osc/v1/vnflcm/samples/instantiate_vnf_instance_param_sample.json` & `python-tackerclient-1.9.0/tackerclient/osc/v1/vnflcm/samples/instantiate_vnf_instance_param_sample.json`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/osc/v1/vnflcm/vnflcm.py` & `python-tackerclient-1.9.0/tackerclient/osc/v1/vnflcm/vnflcm.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/osc/v1/vnflcm/vnflcm_op_occs.py` & `python-tackerclient-1.9.0/tackerclient/osc/v1/vnflcm/vnflcm_op_occs.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,14 +97,55 @@
         client = self.app.client_manager.tackerclient
         result = client.rollback_vnf_instance(parsed_args.vnf_lcm_op_occ_id)
         if not result:
             print((_('Rollback request for LCM operation %(id)s has been'
                      ' accepted') % {'id': parsed_args.vnf_lcm_op_occ_id}))
 
 
+class CancelVnfLcmOp(command.ShowOne):
+    _description = _("Cancel VNF Instance")
+
+    def get_parser(self, prog_name):
+        """Add arguments to parser.
+
+        Args:
+            prog_name ([type]): program name
+
+        Returns:
+            parser([ArgumentParser]):
+        """
+        parser = super(CancelVnfLcmOp, self).get_parser(prog_name)
+        parser.add_argument(
+            _VNF_LCM_OP_OCC_ID,
+            metavar="<vnf-lcm-op-occ-id>",
+            help=_('VNF lifecycle management operation occurrence ID.'))
+        parser.add_argument(
+            "--cancel-mode",
+            default='GRACEFUL',
+            metavar="<cancel-mode>",
+            choices=['GRACEFUL', 'FORCEFUL'],
+            help=_("Cancel mode can be 'GRACEFUL' or 'FORCEFUL'. "
+                   "Default is 'GRACEFUL'"))
+        return parser
+
+    def take_action(self, parsed_args):
+        """Execute cancel_vnf_instance and output comment.
+
+        Args:
+            parsed_args ([Namespace]): arguments of CLI.
+        """
+        client = self.app.client_manager.tackerclient
+        result = client.cancel_vnf_instance(
+            parsed_args.vnf_lcm_op_occ_id,
+            {'cancelMode': parsed_args.cancel_mode})
+        if not result:
+            print((_('Cancel request for LCM operation %(id)s has been'
+                     ' accepted') % {'id': parsed_args.vnf_lcm_op_occ_id}))
+
+
 class FailVnfLcmOp(command.ShowOne):
     _description = _("Fail VNF Instance")
 
     def get_parser(self, prog_name):
         """Add arguments to parser.
 
         Args:
```

### Comparing `python-tackerclient-1.8.0/tackerclient/osc/v1/vnfm/vnf.py` & `python-tackerclient-1.9.0/tackerclient/osc/v1/vnfm/vnf.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/osc/v1/vnfm/vnfd.py` & `python-tackerclient-1.9.0/tackerclient/osc/v1/vnfm/vnfd.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/osc/v1/vnfpkgm/vnf_package.py` & `python-tackerclient-1.9.0/tackerclient/osc/v1/vnfpkgm/vnf_package.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/shell.py` & `python-tackerclient-1.9.0/tackerclient/shell.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tacker/client.py` & `python-tackerclient-1.9.0/tackerclient/tacker/client.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tacker/v1_0/__init__.py` & `python-tackerclient-1.9.0/tackerclient/tacker/v1_0/__init__.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tacker/v1_0/events/events.py` & `python-tackerclient-1.9.0/tackerclient/tacker/v1_0/events/events.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tacker/v1_0/extension.py` & `python-tackerclient-1.9.0/tackerclient/tacker/v1_0/extension.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tacker/v1_0/nfvo/ns.py` & `python-tackerclient-1.9.0/tackerclient/tacker/v1_0/nfvo/ns.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tacker/v1_0/nfvo/nsd.py` & `python-tackerclient-1.9.0/tackerclient/tacker/v1_0/nfvo/nsd.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tacker/v1_0/nfvo/vim.py` & `python-tackerclient-1.9.0/tackerclient/tacker/v1_0/nfvo/vim.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tacker/v1_0/nfvo/vim_utils.py` & `python-tackerclient-1.9.0/tackerclient/tacker/v1_0/nfvo/vim_utils.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tacker/v1_0/nfvo/vnfcluster.py` & `python-tackerclient-1.9.0/tackerclient/tacker/v1_0/nfvo/vnfcluster.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tacker/v1_0/nfvo/vnffg.py` & `python-tackerclient-1.9.0/tackerclient/tacker/v1_0/nfvo/vnffg.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tacker/v1_0/nfvo/vnffgd.py` & `python-tackerclient-1.9.0/tackerclient/tacker/v1_0/nfvo/vnffgd.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tacker/v1_0/vnfm/vnf.py` & `python-tackerclient-1.9.0/tackerclient/tacker/v1_0/vnfm/vnf.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tacker/v1_0/vnfm/vnfd.py` & `python-tackerclient-1.9.0/tackerclient/tacker/v1_0/vnfm/vnfd.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/osc/base.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/osc/base.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/osc/common/test_vnflcm_versions.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/osc/common/test_vnflcm_versions.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/client.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/client.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/etsi_nfv_sol001_common_types.yaml` & `python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/etsi_nfv_sol001_common_types.yaml`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/etsi_nfv_sol001_vnfd_types.yaml` & `python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/etsi_nfv_sol001_vnfd_types.yaml`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_df_simple.yaml` & `python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_df_simple.yaml`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_top.vnfd.yaml` & `python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_top.vnfd.yaml`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_types.yaml` & `python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package/Definitions/helloworld3_types.yaml`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/etsi_nfv_sol001_common_types.yaml` & `python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/etsi_nfv_sol001_common_types.yaml`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/etsi_nfv_sol001_vnfd_types.yaml` & `python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/etsi_nfv_sol001_vnfd_types.yaml`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_df_simple.yaml` & `python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_df_simple.yaml`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_top.vnfd.yaml` & `python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_top.vnfd.yaml`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_types.yaml` & `python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/fixture_data/sample_vnf_package_artifacts/Definitions/helloworld3_types.yaml`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/test_vnf_package.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/test_vnf_package.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/test_vnflcm.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/test_vnflcm.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/test_vnflcm_op_occs.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/test_vnflcm_op_occs.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from io import StringIO
 import os
 import sys
 
+import ddt
 from oslo_utils.fixture import uuidsentinel
 from unittest import mock
 
 from tackerclient.common import exceptions
 from tackerclient.osc import utils as tacker_osc_utils
 from tackerclient.osc.v1.vnflcm import vnflcm_op_occs
 from tackerclient.tests.unit.osc import base
@@ -53,14 +54,78 @@
         self.header = {'content-type': 'application/json'}
         self.app = mock.Mock()
         self.app_args = mock.Mock()
         self.client_manager = self.cs
         self.app.client_manager.tackerclient = self.client_manager
 
 
+@ddt.ddt
+class TestCancelVnfLcmOp(TestVnfLcm):
+
+    def setUp(self):
+        super(TestCancelVnfLcmOp, self).setUp()
+        self.cancel_vnf_lcm = vnflcm_op_occs.CancelVnfLcmOp(
+            self.app, self.app_args, cmd_name='vnflcm op cancel')
+
+    @ddt.data('GRACEFUL', 'FORCEFUL')
+    def test_take_action(self, cancel_mode):
+        """take_action normal system test"""
+
+        arglist = ['--cancel-mode', cancel_mode,
+                   uuidsentinel.vnf_lcm_op_occ_id]
+        verifylist = [('cancel_mode', cancel_mode),
+                      ('vnf_lcm_op_occ_id', uuidsentinel.vnf_lcm_op_occ_id)]
+
+        parsed_args = self.check_parser(
+            self.cancel_vnf_lcm, arglist, verifylist)
+        url = os.path.join(
+            self.url,
+            'vnflcm/v1/vnf_lcm_op_occs',
+            uuidsentinel.vnf_lcm_op_occ_id,
+            'cancel')
+        self.requests_mock.register_uri(
+            'POST', url, headers=self.header, json={})
+
+        sys.stdout = buffer = StringIO()
+        self.cancel_vnf_lcm.take_action(parsed_args)
+
+        actual_message = buffer.getvalue().strip()
+
+        expected_message = (
+            'Cancel request for LCM operation ' +
+            uuidsentinel.vnf_lcm_op_occ_id +
+            ' has been accepted')
+
+        self.assertEqual(expected_message, actual_message)
+
+    def test_terminate_no_options(self):
+        self.assertRaises(base.ParserException, self.check_parser,
+                          self.cancel_vnf_lcm, [], [])
+
+    def test_take_action_vnf_lcm_op_occ_id_not_found(self):
+        """take_action abnomaly system test"""
+
+        arglist = [uuidsentinel.vnf_lcm_op_occ_id]
+        verifylist = [('vnf_lcm_op_occ_id', uuidsentinel.vnf_lcm_op_occ_id)]
+
+        parsed_args = self.check_parser(
+            self.cancel_vnf_lcm, arglist, verifylist)
+        url = os.path.join(
+            self.url,
+            'vnflcm/v1/vnf_lcm_op_occs',
+            uuidsentinel.vnf_lcm_op_occ_id,
+            'cancel')
+        self.requests_mock.register_uri(
+            'POST', url, headers=self.header, status_code=404, json={})
+
+        self.assertRaises(exceptions.TackerClientException,
+                          self.cancel_vnf_lcm.take_action,
+                          parsed_args)
+
+
 class TestRollbackVnfLcmOp(TestVnfLcm):
 
     def setUp(self):
         super(TestRollbackVnfLcmOp, self).setUp()
         self.rollback_vnf_lcm = vnflcm_op_occs.RollbackVnfLcmOp(
             self.app, self.app_args, cmd_name='vnflcm op rollback')
```

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/vnf/test_vnf.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/vnf/test_vnf.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/vnf_package_fakes.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/vnf_package_fakes.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/vnflcm_fakes.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/vnflcm_fakes.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v1/vnflcm_op_occs_fakes.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v1/vnflcm_op_occs_fakes.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/osc/v2/test_vnflcm.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/osc/v2/test_vnflcm.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/test_auth.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/test_casual_args.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/test_casual_args.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/test_cli10.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/test_cli10.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/test_cli10_extensions.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/test_cli10_extensions.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/test_command_meta.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/test_command_meta.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/test_http.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/test_http.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/test_shell.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/test_shell.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/test_ssl.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/test_ssl.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/test_utils.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/test_validators.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/test_validators.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/vm/test_cli10_v10_event.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/vm/test_cli10_v10_event.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/vm/test_cli10_vim.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/vm/test_cli10_vim.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/vm/test_cli10_vim_k8s.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/vm/test_cli10_vim_k8s.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/vm/test_cli10_vim_k8s_with_bearer_token.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/vm/test_cli10_vim_k8s_with_bearer_token.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/vm/test_cli10_vnf.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/vm/test_cli10_vnf.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/vm/test_cli10_vnfd.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/vm/test_cli10_vnfd.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/vm/test_cli10_vnffg.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/vm/test_cli10_vnffg.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/vm/test_cli10_vnffgd.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/vm/test_cli10_vnffgd.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/tests/unit/vm/test_vim_utils.py` & `python-tackerclient-1.9.0/tackerclient/tests/unit/vm/test_vim_utils.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tackerclient/v1_0/client.py` & `python-tackerclient-1.9.0/tackerclient/v1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -948,14 +948,19 @@
 
     @APIParamsCall
     def rollback_vnf_instance(self, occ_id):
         return self.post((self.vnf_lcm_op_occs_path + "/rollback") % occ_id,
                          headers=self.headers)
 
     @APIParamsCall
+    def cancel_vnf_instance(self, occ_id, body):
+        return self.post((self.vnf_lcm_op_occs_path + "/cancel") % occ_id,
+                         body=body)
+
+    @APIParamsCall
     def fail_vnf_instance(self, occ_id):
         return self.post((self.vnf_lcm_op_occs_path + "/fail") % occ_id,
                          headers=self.headers)
 
     @APIParamsCall
     def change_ext_conn_vnf_instance(self, vnf_id, body):
         return self.post((self.vnf_instance_path + "/change_ext_conn") %
@@ -1272,14 +1277,17 @@
 
     def update_vnf_instance(self, vnf_id, body):
         return self.vnf_lcm_client.update_vnf_instance(vnf_id, body)
 
     def rollback_vnf_instance(self, occ_id):
         return self.vnf_lcm_client.rollback_vnf_instance(occ_id)
 
+    def cancel_vnf_instance(self, occ_id, body):
+        return self.vnf_lcm_client.cancel_vnf_instance(occ_id, body)
+
     def fail_vnf_instance(self, occ_id):
         return self.vnf_lcm_client.fail_vnf_instance(occ_id)
 
     def retry_vnf_instance(self, occ_id):
         return self.vnf_lcm_client.retry_vnf_instance(occ_id)
 
     def update_vnf_package(self, vnf_package, body):
```

### Comparing `python-tackerclient-1.8.0/tackerclient/version.py` & `python-tackerclient-1.9.0/tackerclient/version.py`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tools/tacker.bash_completion` & `python-tackerclient-1.9.0/tools/tacker.bash_completion`

 * *Files identical despite different names*

### Comparing `python-tackerclient-1.8.0/tox.ini` & `python-tackerclient-1.9.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = py38,py36,pep8,docs
+envlist = py39,py38,py36,pep8,docs
 minversion = 3.18.0
 skipsdist = True
 ignore_basepython_conflict = True
 
 [testenv]
 basepython = python3
 setenv = VIRTUAL_ENV={envdir}
@@ -48,13 +48,7 @@
 # W504 line break after binary operator
 ignore = E125,W504
 show-source = true
 exclude=.venv,.git,.tox,dist,doc,*lib/python*,*egg,tools
 # F821 undefined name 'unicode'
 # if isinstance(config, str) or isinstance(config, unicode):
 builtins = unicode
-
-[testenv:lower-constraints]
-deps =
-  -c{toxinidir}/lower-constraints.txt
-  -r{toxinidir}/test-requirements.txt
-  -r{toxinidir}/requirements.txt
```

