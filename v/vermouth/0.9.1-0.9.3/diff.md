# Comparing `tmp/vermouth-0.9.1.tar.gz` & `tmp/vermouth-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vermouth-0.9.1.tar", last modified: Thu Dec 22 12:17:35 2022, max compression
+gzip compressed data, was "vermouth-0.9.3.tar", last modified: Mon Jul 31 09:03:35 2023, max compression
```

## Comparing `vermouth-0.9.1.tar` & `vermouth-0.9.3.tar`

### file list

```diff
@@ -1,681 +1,704 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.141742 vermouth-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2022-12-22 12:17:23.000000 vermouth-0.9.1/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2022-12-22 12:17:23.000000 vermouth-0.9.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.037742 vermouth-0.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.045742 vermouth-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2022-12-22 12:17:23.000000 vermouth-0.9.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2022-12-22 12:17:23.000000 vermouth-0.9.1/.github/workflows/run_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16528 2022-12-22 12:17:23.000000 vermouth-0.9.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      659 2022-12-22 12:17:23.000000 vermouth-0.9.1/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)    11528 2022-12-22 12:17:23.000000 vermouth-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2022-12-22 12:17:35.141742 vermouth-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2022-12-22 12:17:23.000000 vermouth-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.045742 vermouth-0.9.1/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2022-12-22 12:17:23.000000 vermouth-0.9.1/bin/embed_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    38644 2022-12-22 12:17:23.000000 vermouth-0.9.1/bin/martinize2
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2022-12-22 12:17:23.000000 vermouth-0.9.1/bin/run_martinize2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.045742 vermouth-0.9.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2022-12-22 12:17:23.000000 vermouth-0.9.1/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.045742 vermouth-0.9.1/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.045742 vermouth-0.9.1/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:23.000000 vermouth-0.9.1/doc/source/_static/.empty_for_git
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.045742 vermouth-0.9.1/doc/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2022-12-22 12:17:23.000000 vermouth-0.9.1/doc/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2022-12-22 12:17:23.000000 vermouth-0.9.1/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2022-12-22 12:17:23.000000 vermouth-0.9.1/doc/source/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2022-12-22 12:17:23.000000 vermouth-0.9.1/doc/source/file_formats.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2022-12-22 12:17:23.000000 vermouth-0.9.1/doc/source/general_overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6334 2022-12-22 12:17:23.000000 vermouth-0.9.1/doc/source/graph_algorithms.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2022-12-22 12:17:23.000000 vermouth-0.9.1/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15596 2022-12-22 12:17:23.000000 vermouth-0.9.1/doc/source/martinize2_workflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-22 12:17:23.000000 vermouth-0.9.1/doc/source/processors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      213 2022-12-22 12:17:23.000000 vermouth-0.9.1/doc/source/technical_background.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.045742 vermouth-0.9.1/doc/source/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.045742 vermouth-0.9.1/doc/source/tutorials/1_simple_protein_aa/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-22 12:17:23.000000 vermouth-0.9.1/doc/source/tutorials/1_simple_protein_aa/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.045742 vermouth-0.9.1/doc/source/tutorials/2_simple_protein_cg/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-22 12:17:23.000000 vermouth-0.9.1/doc/source/tutorials/2_simple_protein_cg/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.045742 vermouth-0.9.1/doc/source/tutorials/3_membrane_protein/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2022-12-22 12:17:23.000000 vermouth-0.9.1/doc/source/tutorials/3_membrane_protein/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.045742 vermouth-0.9.1/doc/source/tutorials/4_branched_polymer/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-22 12:17:23.000000 vermouth-0.9.1/doc/source/tutorials/4_branched_polymer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.045742 vermouth-0.9.1/doc/source/tutorials/5_glycosylated_protein/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2022-12-22 12:17:23.000000 vermouth-0.9.1/doc/source/tutorials/5_glycosylated_protein/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.045742 vermouth-0.9.1/doc/source/tutorials/6_adding_residues_links/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-22 12:17:23.000000 vermouth-0.9.1/doc/source/tutorials/6_adding_residues_links/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.045742 vermouth-0.9.1/doc/source/tutorials/7_adding_modifications/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2022-12-22 12:17:23.000000 vermouth-0.9.1/doc/source/tutorials/7_adding_modifications/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      405 2022-12-22 12:17:23.000000 vermouth-0.9.1/doc/source/tutorials/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.045742 vermouth-0.9.1/maintainers/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2022-12-22 12:17:23.000000 vermouth-0.9.1/maintainers/head_template_data
--rw-r--r--   0 runner    (1001) docker     (123)      587 2022-12-22 12:17:23.000000 vermouth-0.9.1/maintainers/head_template_py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2022-12-22 12:17:23.000000 vermouth-0.9.1/maintainers/releasing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.037742 vermouth-0.9.1/maintainers/vim/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.049742 vermouth-0.9.1/maintainers/vim/syntax/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2022-12-22 12:17:23.000000 vermouth-0.9.1/maintainers/vim/syntax/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2022-12-22 12:17:23.000000 vermouth-0.9.1/maintainers/vim/syntax/ff.vim
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-22 12:17:23.000000 vermouth-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2022-12-22 12:17:23.000000 vermouth-0.9.1/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2022-12-22 12:17:23.000000 vermouth-0.9.1/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2022-12-22 12:17:35.141742 vermouth-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2022-12-22 12:17:23.000000 vermouth-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.049742 vermouth-0.9.1/vermouth/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/citation_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.049742 vermouth-0.9.1/vermouth/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.037742 vermouth-0.9.1/vermouth/data/force_fields/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.049742 vermouth-0.9.1/vermouth/data/force_fields/amber/
--rw-r--r--   0 runner    (1001) docker     (123)    31320 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/amber/aminoacids.rtp
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/amber/modifications.ff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.053742 vermouth-0.9.1/vermouth/data/force_fields/charmm/
--rw-r--r--   0 runner    (1001) docker     (123)    17350 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/charmm/aminoacids.rtp
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/charmm/modifications.ff
--rw-r--r--   0 runner    (1001) docker     (123)  1891817 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/charmm/small_molecule_charmm.ff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.053742 vermouth-0.9.1/vermouth/data/force_fields/elnedyn21/
--rw-r--r--   0 runner    (1001) docker     (123)    13718 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/elnedyn21/aminoacids.ff
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/elnedyn21/citations.bib
--rw-r--r--   0 runner    (1001) docker     (123)      622 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/elnedyn21/general.ff
--rw-r--r--   0 runner    (1001) docker     (123)      390 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/elnedyn21/modifications.ff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.053742 vermouth-0.9.1/vermouth/data/force_fields/elnedyn22/
--rw-r--r--   0 runner    (1001) docker     (123)    13733 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/elnedyn22/aminoacids.ff
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/elnedyn22/citations.bib
--rw-r--r--   0 runner    (1001) docker     (123)      622 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/elnedyn22/general.ff
--rw-r--r--   0 runner    (1001) docker     (123)      486 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/elnedyn22/modifications.ff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.053742 vermouth-0.9.1/vermouth/data/force_fields/elnedyn22p/
--rw-r--r--   0 runner    (1001) docker     (123)    15732 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/elnedyn22p/aminoacids.ff
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/elnedyn22p/citations.bib
--rw-r--r--   0 runner    (1001) docker     (123)      622 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/elnedyn22p/general.ff
--rw-r--r--   0 runner    (1001) docker     (123)      390 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/elnedyn22p/modifications.ff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.053742 vermouth-0.9.1/vermouth/data/force_fields/gromos/
--rw-r--r--   0 runner    (1001) docker     (123)    62511 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/gromos/aminoacids.rtp
--rw-r--r--   0 runner    (1001) docker     (123)     9113 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/gromos/cofactors.ff
--rw-r--r--   0 runner    (1001) docker     (123)      397 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/gromos/modifications.ff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.057742 vermouth-0.9.1/vermouth/data/force_fields/martini22/
--rw-r--r--   0 runner    (1001) docker     (123)    21153 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/martini22/aminoacids.ff
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/martini22/citations.bib
--rw-r--r--   0 runner    (1001) docker     (123)      622 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/martini22/general.ff
--rw-r--r--   0 runner    (1001) docker     (123)      586 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/martini22/modifications.ff
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/martini22/nucleotides.ff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.057742 vermouth-0.9.1/vermouth/data/force_fields/martini22p/
--rw-r--r--   0 runner    (1001) docker     (123)    20954 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/martini22p/aminoacids.ff
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/martini22p/citations.bib
--rw-r--r--   0 runner    (1001) docker     (123)      622 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/martini22p/general.ff
--rw-r--r--   0 runner    (1001) docker     (123)      390 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/martini22p/modifications.ff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.057742 vermouth-0.9.1/vermouth/data/force_fields/martini3001/
--rw-r--r--   0 runner    (1001) docker     (123)    31166 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/martini3001/aminoacids.ff
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/martini3001/citations.bib
--rw-r--r--   0 runner    (1001) docker     (123)      622 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/martini3001/general.ff
--rw-r--r--   0 runner    (1001) docker     (123)      942 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/martini3001/modifications.ff
--rw-r--r--   0 runner    (1001) docker     (123)    10570 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/martini3001/small_molecule_martini3.ff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.057742 vermouth-0.9.1/vermouth/data/force_fields/martini30b32/
--rw-r--r--   0 runner    (1001) docker     (123)    20017 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/martini30b32/aminoacids.ff
--rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/martini30b32/citations.bib
--rw-r--r--   0 runner    (1001) docker     (123)      159 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/martini30b32/modifications.ff
--rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/martini30b32/small_molecules.ff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.057742 vermouth-0.9.1/vermouth/data/force_fields/martini30dev/
--rw-r--r--   0 runner    (1001) docker     (123)    21438 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/martini30dev/aminoacids.ff
--rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/martini30dev/citations.bib
--rw-r--r--   0 runner    (1001) docker     (123)      321 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/force_fields/martini30dev/modifications.ff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.069742 vermouth-0.9.1/vermouth/data/mappings/
--rwxr-xr-x   0 runner    (1001) docker     (123)      996 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/ala.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      204 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/ala.gromos.map
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/arg.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/arg.charmm36.martini22p.map
--rw-r--r--   0 runner    (1001) docker     (123)      432 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/arg.gromos.map
--rwxr-xr-x   0 runner    (1001) docker     (123)     1114 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/asn.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/asn.charmm36.martini22p.map
--rw-r--r--   0 runner    (1001) docker     (123)      311 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/asn.gromos.map
--rwxr-xr-x   0 runner    (1001) docker     (123)     1097 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/asp.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/asp.charmm36.martini22p.map
--rw-r--r--   0 runner    (1001) docker     (123)      274 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/asp.gromos.map
--rw-r--r--   0 runner    (1001) docker     (123)      262 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/asp0.gromos.map
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/chol.charmm36.map
--rwxr-xr-x   0 runner    (1001) docker     (123)      996 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/cys.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      247 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/cys.gromos.map
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/dmpc.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/dopc.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/dppc.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/dppg.charmm36.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.077742 vermouth-0.9.1/vermouth/data/mappings/elnedyn/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/ala.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/arg.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/asn.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/asp.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/chol.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/cys.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/dmpc.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/dopc.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/dppc.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/dppg.charmm36.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.077742 vermouth-0.9.1/vermouth/data/mappings/elnedyn/elnedyn22p/
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/elnedyn22p/arg.charmm36.elnedyn22p.map
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/elnedyn22p/asn.charmm36.elnedyn22p.map
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/elnedyn22p/asp.charmm36.elnedyn22p.map
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/elnedyn22p/gln.charmm36.elnedyn22p.map
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/elnedyn22p/glu.charmm36.elnedyn22p.map
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/elnedyn22p/lys.charmm36.elnedyn22p.map
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/elnedyn22p/ser.charmm36.elnedyn22p.map
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/elnedyn22p/thr.charmm36.elnedyn22p.map
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/gln.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/glu.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      806 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/gly.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/his.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/ile.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/leu.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/lys.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/met.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      797 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/modifications.elnedyn21.mapping
--rw-r--r--   0 runner    (1001) docker     (123)      996 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/modifications.elnedyn22.mapping
--rw-r--r--   0 runner    (1001) docker     (123)      801 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/modifications.elnedyn22p.mapping
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/phe.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/popc.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/pope.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/popg.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/pops.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/pro.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/ser.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/thr.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/trp.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/tyr.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      865 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn/val.charmm36.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.081742 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/ala.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/arg.charmm36.elnedyn22p.map
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/arg.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/asn.charmm36.elnedyn22p.map
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/asn.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/asp.charmm36.elnedyn22p.map
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/asp.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/cys.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/gln.charmm36.elnedyn22p.map
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/gln.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/glu.charmm36.elnedyn22p.map
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/glu.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      809 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/gly.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/his.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/ile.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/leu.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/lys.charmm36.elnedyn22p.map
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/lys.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/met.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      797 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/modifications.mapping
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/phe.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/pro.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/ser.charmm36.elnedyn22p.map
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/ser.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/thr.charmm36.elnedyn22p.map
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/thr.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/trp.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/tyr.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      868 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/elnedyn21/val.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      757 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/fmn.gromos.map
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/gln.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/gln.charmm36.martini22p.map
--rw-r--r--   0 runner    (1001) docker     (123)      330 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/gln.gromos.map
--rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/glu.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/glu.charmm36.martini22p.map
--rw-r--r--   0 runner    (1001) docker     (123)      328 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/glu.gromos.map
--rw-r--r--   0 runner    (1001) docker     (123)      312 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/glu0.gromos.map
--rwxr-xr-x   0 runner    (1001) docker     (123)      794 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/gly.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      186 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/gly.gromos.map
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/his.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      393 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/his.gromos.map
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/hsd.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/hse.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/hsp.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/ile.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      282 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/ile.gromos.map
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/leu.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      275 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/leu.gromos.map
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/lys.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/lys.charmm36.martini22p.map
--rw-r--r--   0 runner    (1001) docker     (123)      368 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/lys.gromos.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.093742 vermouth-0.9.1/vermouth/data/mappings/martini3001/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/ala.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/ala.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      342 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/antr.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/arg.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/arg.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/ash.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/asn.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/asn.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/asp.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/asp.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/aspp.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      230 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/bald.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      222 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/benz.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      184 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/c3.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      256 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/chxe.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      248 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/cpen.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      305 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/cume.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/cys.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/cys.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      208 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/diol.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      237 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/diox.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      286 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/dman.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      273 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/eben.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      187 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/fura.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/glh.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/gln.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/gln.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/glu.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/glu.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/glup.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      820 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/gly.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)      823 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/gly.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/hid.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/hie.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/hip.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/his.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/his.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/hsd.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/hse.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/hsp.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/ile.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/ile.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      194 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/imia.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      250 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/inda.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      263 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/indo.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/leu.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/leu.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/lsn.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/lyn.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/lys.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/lys.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      266 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/mboa.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      238 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/mcpe.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      252 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/meob.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/met.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/met.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      300 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/mind.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/modifications.amber.mapping
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/modifications.charmm36.mapping
--rw-r--r--   0 runner    (1001) docker     (123)      282 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/mxyl.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      275 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/naft.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      228 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/nitb.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      282 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/oxyl.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      264 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/pcro.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/phe.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/phe.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      211 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/phen.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      256 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/phmk.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      203 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/prld.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/pro.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/pro.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      286 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/pxyl.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      205 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/pyr1.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      196 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/pyrd.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      196 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/pyrl.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      196 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/pyrm.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      266 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/qinl.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/ser.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/ser.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      263 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/sm139.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      252 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/styr.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      179 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/thaz.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      201 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/thf.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      187 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/thip.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      255 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/thp.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/thr.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/thr.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      232 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/tolu.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/trp.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/trp.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/tyr.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/tyr.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/val.amber.map
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/val.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      241 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/zimi.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      247 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/zthp.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      238 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini3001/zthz.charmm36.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.093742 vermouth-0.9.1/vermouth/data/mappings/martini30b32/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini30b32/ala.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini30b32/arg.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini30b32/asn.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini30b32/asp.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      223 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini30b32/benz.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini30b32/cys.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini30b32/gln.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini30b32/glu.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      824 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini30b32/gly.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini30b32/his.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini30b32/hsd.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini30b32/ile.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini30b32/leu.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini30b32/lys.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini30b32/met.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      376 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini30b32/modifications.mapping
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini30b32/phe.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini30b32/pro.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini30b32/ser.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini30b32/thr.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini30b32/trp.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini30b32/tyr.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/martini30b32/val.charmm36.map
--rwxr-xr-x   0 runner    (1001) docker     (123)     1184 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/met.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      278 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/met.gromos.map
--rw-r--r--   0 runner    (1001) docker     (123)      370 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/modifications.gromos.mapping
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/modifications.mapping
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/nad.gromos.map
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/phe.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      501 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/phe.gromos.map
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/popc.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/pope.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/popg.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/pops.charmm36.map
--rwxr-xr-x   0 runner    (1001) docker     (123)      996 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/pro.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      229 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/pro.gromos.map
--rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/ser.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/ser.charmm36.martini22p.map
--rw-r--r--   0 runner    (1001) docker     (123)      257 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/ser.gromos.map
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/thr.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/thr.charmm36.martini22p.map
--rw-r--r--   0 runner    (1001) docker     (123)      283 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/thr.gromos.map
--rw-r--r--   0 runner    (1001) docker     (123)      677 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/tpp.gromos.map
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/trp.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      732 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/trp.gromos.map
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/tyr.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      584 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/tyr.gromos.map
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/val.charmm36.map
--rw-r--r--   0 runner    (1001) docker     (123)      248 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/mappings/val.gromos.map
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/data/quotes.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.093742 vermouth-0.9.1/vermouth/dssp/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/dssp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21618 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/dssp/dssp.py
--rw-r--r--   0 runner    (1001) docker     (123)    15338 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/edge_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)    43401 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/ffinput.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/file_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/forcefield.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.101742 vermouth-0.9.1/vermouth/gmx/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/gmx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/gmx/gro.py
--rw-r--r--   0 runner    (1001) docker     (123)    10564 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/gmx/itp.py
--rw-r--r--   0 runner    (1001) docker     (123)    17698 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/gmx/itp_read.py
--rw-r--r--   0 runner    (1001) docker     (123)    18294 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/gmx/rtp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13322 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/graph_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.101742 vermouth-0.9.1/vermouth/graphing/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11617 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/graphing/grappa.py
--rw-r--r--   0 runner    (1001) docker     (123)    43888 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/ismags.py
--rw-r--r--   0 runner    (1001) docker     (123)    10113 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/log_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20367 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/map_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    32810 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/map_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    51750 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/molecule.py
--rw-r--r--   0 runner    (1001) docker     (123)    18045 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/parser_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.101742 vermouth-0.9.1/vermouth/pdb/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/pdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19935 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/pdb/pdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.101742 vermouth-0.9.1/vermouth/processors/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/add_molecule_edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/annotate_mut_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/apply_posres.py
--rw-r--r--   0 runner    (1001) docker     (123)    20081 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/apply_rubber_band.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/attach_mass.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/average_beads.py
--rw-r--r--   0 runner    (1001) docker     (123)    16024 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/canonicalize_modifications.py
--rw-r--r--   0 runner    (1001) docker     (123)    12422 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/do_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    35821 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/do_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/go_vs_includes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/gro_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/locate_charge_dummies.py
--rw-r--r--   0 runner    (1001) docker     (123)    14592 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/make_bonds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/merge_all_molecules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/merge_chains.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/name_moltype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/pdb_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/rename_modified_residues.py
--rw-r--r--   0 runner    (1001) docker     (123)    22938 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/repair_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/set_molecule_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/sort_molecule_atoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/processors/tune_cystein_bridges.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.109742 vermouth-0.9.1/vermouth/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.113742 vermouth-0.9.1/vermouth/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   127980 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/1bta.pdb
--rw-r--r--   0 runner    (1001) docker     (123)   127980 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/1bta_mutated.pdb
--rw-r--r--   0 runner    (1001) docker     (123)   390258 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/2QWO.pdb
--rw-r--r--   0 runner    (1001) docker     (123)   789750 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/2dn2.pdb
--rw-r--r--   0 runner    (1001) docker     (123)  3325374 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/6E8W.pdb
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/ala5.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      997 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/ala5_cg.pdb
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/dna-short.pdb
--rw-r--r--   0 runner    (1001) docker     (123)    15814 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/dssp_1bta.ssd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.037742 vermouth-0.9.1/vermouth/tests/data/force_fields/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.113742 vermouth-0.9.1/vermouth/tests/data/force_fields/martini-test/
--rw-r--r--   0 runner    (1001) docker     (123)    20132 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/force_fields/martini-test/aminoacids.ff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.113742 vermouth-0.9.1/vermouth/tests/data/force_fields/pepplane/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/force_fields/pepplane/ala.ff
--rw-r--r--   0 runner    (1001) docker     (123)      622 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/force_fields/pepplane/general.ff
--rw-r--r--   0 runner    (1001) docker     (123)      252 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/force_fields/pepplane/modifications.ff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.113742 vermouth-0.9.1/vermouth/tests/data/force_fields/universal-test/
--rw-r--r--   0 runner    (1001) docker     (123)    26194 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/force_fields/universal-test/aminoacids.rtp
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/force_fields/universal-test/modifications.ff
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/heme.pdb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.041742 vermouth-0.9.1/vermouth/tests/data/integration_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.041742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.113742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/dipro-termini/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/dipro-termini/README
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/dipro-termini/aa.pdb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.113742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/dipro-termini/martinize2/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/dipro-termini/martinize2/cg.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      406 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/dipro-termini/martinize2/citation
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/dipro-termini/martinize2/command
--rw-r--r--   0 runner    (1001) docker     (123)      987 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/dipro-termini/martinize2/molecule_0.itp
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/dipro-termini/martinize2/topol.top
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.113742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/README
--rw-r--r--   0 runner    (1001) docker     (123)    36099 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/aa.pdb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.117742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/cg.pdb
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/chain_A.ssd
--rw-r--r--   0 runner    (1001) docker     (123)      419 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/citation
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/command
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/molecule_0.itp
--rw-r--r--   0 runner    (1001) docker     (123)      867 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/screen.output
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/topol.top
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.117742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/README
--rw-r--r--   0 runner    (1001) docker     (123)    58725 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/aa.pdb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.117742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/
--rw-r--r--   0 runner    (1001) docker     (123)     8927 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/cg.pdb
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/chain_A.ssd
--rw-r--r--   0 runner    (1001) docker     (123)      348 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/citation
--rw-r--r--   0 runner    (1001) docker     (123)      138 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/command
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/molecule_0.itp
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/screen.output
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/topol.top
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.117742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/README
--rw-r--r--   0 runner    (1001) docker     (123)    24624 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/aa.pdb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.117742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/cg.pdb
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/chain_A.ssd
--rw-r--r--   0 runner    (1001) docker     (123)      519 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/citation
--rw-r--r--   0 runner    (1001) docker     (123)       90 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/command
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/molecule_0.itp
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/screen.output
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/topol.top
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.041742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.117742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5/README
--rw-r--r--   0 runner    (1001) docker     (123)   362933 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5/aa.pdb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.121742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/
--rw-r--r--   0 runner    (1001) docker     (123)    64614 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/cg.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/cg.top
--rw-r--r--   0 runner    (1001) docker     (123)    48477 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/chain_.ssd
--rw-r--r--   0 runner    (1001) docker     (123)      407 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/citation
--rw-r--r--   0 runner    (1001) docker     (123)      117 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/command
--rw-r--r--   0 runner    (1001) docker     (123)   130905 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/molecule_0.itp
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/screen.output
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.117742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/README
--rw-r--r--   0 runner    (1001) docker     (123)   362933 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/aa.pdb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.121742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/
--rw-r--r--   0 runner    (1001) docker     (123)    64614 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/cg.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/cg.top
--rw-r--r--   0 runner    (1001) docker     (123)    48477 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/chain_.ssd
--rw-r--r--   0 runner    (1001) docker     (123)      407 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/citation
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/command
--rw-r--r--   0 runner    (1001) docker     (123)   130856 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/molecule_0.itp
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/screen.output
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.121742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/3i40/
--rw-r--r--   0 runner    (1001) docker     (123)    63828 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/3i40/3i40.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      293 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/3i40/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.125742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/
--rw-r--r--   0 runner    (1001) docker     (123)    11537 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/cg.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/cg.top
--rw-r--r--   0 runner    (1001) docker     (123)    11526 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/chain_A.ssd
--rw-r--r--   0 runner    (1001) docker     (123)    11526 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/chain_C.ssd
--rw-r--r--   0 runner    (1001) docker     (123)      407 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/citation
--rw-r--r--   0 runner    (1001) docker     (123)      114 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/command
--rw-r--r--   0 runner    (1001) docker     (123)    22543 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/insulin_dimer.itp
--rw-r--r--   0 runner    (1001) docker     (123)    18292 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/molecule_0.itp
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/screen.output
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.125742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/
--rw-r--r--   0 runner    (1001) docker     (123)   159513 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/6LFO_gap.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      386 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.125742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/
--rw-r--r--   0 runner    (1001) docker     (123)    55693 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/cg.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/cg.top
--rw-r--r--   0 runner    (1001) docker     (123)    10933 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/chain_R.ssd
--rw-r--r--   0 runner    (1001) docker     (123)      407 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/citation
--rw-r--r--   0 runner    (1001) docker     (123)      151 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/command
--rw-r--r--   0 runner    (1001) docker     (123)   111329 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/molecule_0.itp
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/screen.output
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.125742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_chain/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_chain/README
--rw-r--r--   0 runner    (1001) docker     (123)    63828 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_chain/aa.pdb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.125742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/
--rw-r--r--   0 runner    (1001) docker     (123)    11537 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/cg.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/cg.top
--rw-r--r--   0 runner    (1001) docker     (123)    11526 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/chain_A.ssd
--rw-r--r--   0 runner    (1001) docker     (123)      407 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/citation
--rw-r--r--   0 runner    (1001) docker     (123)      134 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/command
--rw-r--r--   0 runner    (1001) docker     (123)    20955 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/molecule_0.itp
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/screen.output
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.125742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_region/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_region/README
--rw-r--r--   0 runner    (1001) docker     (123)    63828 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_region/aa.pdb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.129742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/
--rw-r--r--   0 runner    (1001) docker     (123)    11537 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/cg.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/cg.top
--rw-r--r--   0 runner    (1001) docker     (123)    11526 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/chain_A.ssd
--rw-r--r--   0 runner    (1001) docker     (123)      407 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/citation
--rw-r--r--   0 runner    (1001) docker     (123)      133 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/command
--rw-r--r--   0 runner    (1001) docker     (123)    19283 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/molecule_0.itp
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/screen.output
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.129742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/bpti/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/bpti/README
--rw-r--r--   0 runner    (1001) docker     (123)    71928 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/bpti/aa.pdb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.133742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/
--rw-r--r--   0 runner    (1001) docker     (123)    12336 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/cg.pdb
--rw-r--r--   0 runner    (1001) docker     (123)    12453 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/chain_A.ssd
--rw-r--r--   0 runner    (1001) docker     (123)      519 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/citation
--rw-r--r--   0 runner    (1001) docker     (123)      124 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/command
--rw-r--r--   0 runner    (1001) docker     (123)    18978 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/molecule_0.itp
--rw-r--r--   0 runner    (1001) docker     (123)    26495 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/screen.output
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/topol.top
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.133742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme/README
--rw-r--r--   0 runner    (1001) docker     (123)   125469 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme/aa.pdb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.133742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/
--rw-r--r--   0 runner    (1001) docker     (123)    27432 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/cg.pdb
--rw-r--r--   0 runner    (1001) docker     (123)    23245 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/chain_A.ssd
--rw-r--r--   0 runner    (1001) docker     (123)       34 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/citation
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/command
--rw-r--r--   0 runner    (1001) docker     (123)    47269 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/molecule_0.itp
--rw-r--r--   0 runner    (1001) docker     (123)    37646 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/screen.output
--rw-r--r--   0 runner    (1001) docker     (123)    47488 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/test.itp
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/topol.top
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.137742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/README
--rw-r--r--   0 runner    (1001) docker     (123)   125469 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/aa.pdb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.137742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/
--rw-r--r--   0 runner    (1001) docker     (123)    28494 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/cg.pdb
--rw-r--r--   0 runner    (1001) docker     (123)    23245 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/chain_A.ssd
--rw-r--r--   0 runner    (1001) docker     (123)      407 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/citation
--rw-r--r--   0 runner    (1001) docker     (123)      107 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/command
--rw-r--r--   0 runner    (1001) docker     (123)    56460 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/molecule_0.itp
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/screen.output
--rw-r--r--   0 runner    (1001) docker     (123)    47488 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/test.itp
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/topol.top
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.137742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/villin/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/villin/README
--rw-r--r--   0 runner    (1001) docker     (123)    23380 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/villin/aa.pdb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.141742 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/villin/martinize2/
--rw-r--r--   0 runner    (1001) docker     (123)    10307 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/villin/martinize2/cg.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      502 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/villin/martinize2/citation
--rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/villin/martinize2/command
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/villin/martinize2/molecule_0.itp
--rw-r--r--   0 runner    (1001) docker     (123)      873 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/villin/martinize2/screen.output
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/villin/martinize2/topol.top
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.041742 vermouth-0.9.1/vermouth/tests/data/mappings/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.041742 vermouth-0.9.1/vermouth/tests/data/mappings/universal-test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.141742 vermouth-0.9.1/vermouth/tests/data/mappings/universal-test/martini-test/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/mappings/universal-test/martini-test/ser.mapping
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.141742 vermouth-0.9.1/vermouth/tests/data/mappings/universal-test/pepplane/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/mappings/universal-test/pepplane/ala.mapping
--rw-r--r--   0 runner    (1001) docker     (123)      916 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/mappings/universal-test/pepplane/modifications.mapping
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/data/tri_alanine.pdb
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/datafiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.141742 vermouth-0.9.1/vermouth/tests/gmx/
--rw-r--r--   0 runner    (1001) docker     (123)    20533 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/gmx/test_gro.py
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/gmx/test_itp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/helper_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.141742 vermouth-0.9.1/vermouth/tests/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7263 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/integration_tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8695 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/molecule_strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.141742 vermouth-0.9.1/vermouth/tests/pdb/
--rw-r--r--   0 runner    (1001) docker     (123)    11495 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/pdb/test_read_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/pdb/test_write_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_add_molecule_edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     9768 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_annotate_mut_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)    19313 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_apply_rubber_band.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_average_beads.py
--rw-r--r--   0 runner    (1001) docker     (123)    23516 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_do_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    17880 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_dssp.py
--rw-r--r--   0 runner    (1001) docker     (123)    19473 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_edge_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)    39944 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_ff_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    21519 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_ffinput.py
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_file_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_forcefield.py
--rw-r--r--   0 runner    (1001) docker     (123)     8143 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_go_vs_includes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14890 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14825 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_grappa.py
--rw-r--r--   0 runner    (1001) docker     (123)    19965 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_ismags.py
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_itp_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9587 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    12376 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_make_bonds.py
--rw-r--r--   0 runner    (1001) docker     (123)    18981 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_map_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    16734 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_map_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_mapping_integrative.py
--rw-r--r--   0 runner    (1001) docker     (123)    44701 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_molecule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6161 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_name_moltype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_native_forcefield.py
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_ptm_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    17176 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_repair_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_section_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5164 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_set_molecule_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_sort_molecule_atoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_tune_cystein_bridges.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/truncating_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2022-12-22 12:17:23.000000 vermouth-0.9.1/vermouth/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 12:17:35.049742 vermouth-0.9.1/vermouth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2022-12-22 12:17:34.000000 vermouth-0.9.1/vermouth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    29858 2022-12-22 12:17:35.000000 vermouth-0.9.1/vermouth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 12:17:34.000000 vermouth-0.9.1/vermouth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 12:17:34.000000 vermouth-0.9.1/vermouth.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-22 12:17:34.000000 vermouth-0.9.1/vermouth.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-22 12:17:34.000000 vermouth-0.9.1/vermouth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-22 12:17:34.000000 vermouth-0.9.1/vermouth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.787004 vermouth-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-31 09:03:20.000000 vermouth-0.9.3/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-31 09:03:20.000000 vermouth-0.9.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.615004 vermouth-0.9.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.635004 vermouth-0.9.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-31 09:03:20.000000 vermouth-0.9.3/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-31 09:03:20.000000 vermouth-0.9.3/.github/workflows/run_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16528 2023-07-31 09:03:20.000000 vermouth-0.9.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-31 09:03:20.000000 vermouth-0.9.3/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-07-31 09:03:20.000000 vermouth-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-07-31 09:03:35.787004 vermouth-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-07-31 09:03:20.000000 vermouth-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.639004 vermouth-0.9.3/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-07-31 09:03:20.000000 vermouth-0.9.3/bin/embed_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38489 2023-07-31 09:03:20.000000 vermouth-0.9.3/bin/martinize2
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-31 09:03:20.000000 vermouth-0.9.3/bin/run_martinize2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.639004 vermouth-0.9.3/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-31 09:03:20.000000 vermouth-0.9.3/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.639004 vermouth-0.9.3/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.639004 vermouth-0.9.3/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:20.000000 vermouth-0.9.3/doc/source/_static/.empty_for_git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.639004 vermouth-0.9.3/doc/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-31 09:03:20.000000 vermouth-0.9.3/doc/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-07-31 09:03:20.000000 vermouth-0.9.3/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-07-31 09:03:20.000000 vermouth-0.9.3/doc/source/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-31 09:03:20.000000 vermouth-0.9.3/doc/source/file_formats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-31 09:03:20.000000 vermouth-0.9.3/doc/source/general_overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-07-31 09:03:20.000000 vermouth-0.9.3/doc/source/graph_algorithms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-31 09:03:20.000000 vermouth-0.9.3/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15596 2023-07-31 09:03:20.000000 vermouth-0.9.3/doc/source/martinize2_workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-31 09:03:20.000000 vermouth-0.9.3/doc/source/processors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-31 09:03:20.000000 vermouth-0.9.3/doc/source/technical_background.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.639004 vermouth-0.9.3/doc/source/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.639004 vermouth-0.9.3/doc/source/tutorials/1_simple_protein_aa/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-31 09:03:20.000000 vermouth-0.9.3/doc/source/tutorials/1_simple_protein_aa/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.639004 vermouth-0.9.3/doc/source/tutorials/2_simple_protein_cg/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-31 09:03:20.000000 vermouth-0.9.3/doc/source/tutorials/2_simple_protein_cg/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.639004 vermouth-0.9.3/doc/source/tutorials/3_membrane_protein/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-31 09:03:20.000000 vermouth-0.9.3/doc/source/tutorials/3_membrane_protein/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.639004 vermouth-0.9.3/doc/source/tutorials/4_branched_polymer/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-31 09:03:20.000000 vermouth-0.9.3/doc/source/tutorials/4_branched_polymer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.639004 vermouth-0.9.3/doc/source/tutorials/5_glycosylated_protein/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-31 09:03:20.000000 vermouth-0.9.3/doc/source/tutorials/5_glycosylated_protein/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.643004 vermouth-0.9.3/doc/source/tutorials/6_adding_residues_links/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-31 09:03:20.000000 vermouth-0.9.3/doc/source/tutorials/6_adding_residues_links/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.643004 vermouth-0.9.3/doc/source/tutorials/7_adding_modifications/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-31 09:03:20.000000 vermouth-0.9.3/doc/source/tutorials/7_adding_modifications/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-31 09:03:20.000000 vermouth-0.9.3/doc/source/tutorials/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.643004 vermouth-0.9.3/maintainers/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-31 09:03:20.000000 vermouth-0.9.3/maintainers/head_template_data
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-31 09:03:20.000000 vermouth-0.9.3/maintainers/head_template_py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-31 09:03:20.000000 vermouth-0.9.3/maintainers/releasing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.619004 vermouth-0.9.3/maintainers/vim/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.643004 vermouth-0.9.3/maintainers/vim/syntax/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-31 09:03:20.000000 vermouth-0.9.3/maintainers/vim/syntax/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-31 09:03:20.000000 vermouth-0.9.3/maintainers/vim/syntax/ff.vim
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-31 09:03:20.000000 vermouth-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-31 09:03:20.000000 vermouth-0.9.3/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-31 09:03:20.000000 vermouth-0.9.3/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-31 09:03:35.787004 vermouth-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-31 09:03:20.000000 vermouth-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.647004 vermouth-0.9.3/vermouth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/citation_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.647004 vermouth-0.9.3/vermouth/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.627004 vermouth-0.9.3/vermouth/data/force_fields/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.651004 vermouth-0.9.3/vermouth/data/force_fields/amber/
+-rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/amber/aminoacids.rtp
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/amber/modifications.ff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.651004 vermouth-0.9.3/vermouth/data/force_fields/charmm/
+-rw-r--r--   0 runner    (1001) docker     (123)    17278 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/charmm/aminoacids.rtp
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/charmm/modifications.ff
+-rw-r--r--   0 runner    (1001) docker     (123)  1891817 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/charmm/small_molecule_charmm.ff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.655004 vermouth-0.9.3/vermouth/data/force_fields/elnedyn21/
+-rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/elnedyn21/aminoacids.ff
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/elnedyn21/citations.bib
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/elnedyn21/general.ff
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/elnedyn21/modifications.ff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.655004 vermouth-0.9.3/vermouth/data/force_fields/elnedyn22/
+-rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/elnedyn22/aminoacids.ff
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/elnedyn22/citations.bib
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/elnedyn22/general.ff
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/elnedyn22/modifications.ff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.655004 vermouth-0.9.3/vermouth/data/force_fields/elnedyn22p/
+-rw-r--r--   0 runner    (1001) docker     (123)    15732 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/elnedyn22p/aminoacids.ff
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/elnedyn22p/citations.bib
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/elnedyn22p/general.ff
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/elnedyn22p/modifications.ff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.655004 vermouth-0.9.3/vermouth/data/force_fields/gromos/
+-rw-r--r--   0 runner    (1001) docker     (123)    62511 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/gromos/aminoacids.rtp
+-rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/gromos/cofactors.ff
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/gromos/modifications.ff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.655004 vermouth-0.9.3/vermouth/data/force_fields/martini22/
+-rw-r--r--   0 runner    (1001) docker     (123)    21152 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/martini22/aminoacids.ff
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/martini22/citations.bib
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/martini22/general.ff
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/martini22/modifications.ff
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/martini22/nucleotides.ff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.659004 vermouth-0.9.3/vermouth/data/force_fields/martini22p/
+-rw-r--r--   0 runner    (1001) docker     (123)    20954 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/martini22p/aminoacids.ff
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/martini22p/citations.bib
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/martini22p/general.ff
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/martini22p/modifications.ff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.659004 vermouth-0.9.3/vermouth/data/force_fields/martini3001/
+-rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/martini3001/aminoacids.ff
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/martini3001/citations.bib
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/martini3001/general.ff
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/martini3001/modifications.ff
+-rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/martini3001/small_molecule_martini3.ff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.659004 vermouth-0.9.3/vermouth/data/force_fields/martini30b32/
+-rw-r--r--   0 runner    (1001) docker     (123)    20017 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/martini30b32/aminoacids.ff
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/martini30b32/citations.bib
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/martini30b32/modifications.ff
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/martini30b32/small_molecules.ff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.659004 vermouth-0.9.3/vermouth/data/force_fields/martini30dev/
+-rw-r--r--   0 runner    (1001) docker     (123)    21438 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/martini30dev/aminoacids.ff
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/martini30dev/citations.bib
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/force_fields/martini30dev/modifications.ff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.683004 vermouth-0.9.3/vermouth/data/mappings/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      996 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/ala.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/ala.gromos.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/arg.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/arg.charmm36.martini22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/arg.gromos.map
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1114 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/asn.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/asn.charmm36.martini22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/asn.gromos.map
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1097 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/asp.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/asp.charmm36.martini22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/asp.gromos.map
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/asp0.gromos.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/chol.charmm36.map
+-rwxr-xr-x   0 runner    (1001) docker     (123)      996 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/cys.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/cys.gromos.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/dmpc.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/dopc.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/dppc.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/dppg.charmm36.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.691004 vermouth-0.9.3/vermouth/data/mappings/elnedyn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/ala.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/arg.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/asn.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/asp.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/chol.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/cys.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/dmpc.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/dopc.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/dppc.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/dppg.charmm36.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.691004 vermouth-0.9.3/vermouth/data/mappings/elnedyn/elnedyn22p/
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/elnedyn22p/arg.charmm36.elnedyn22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/elnedyn22p/asn.charmm36.elnedyn22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/elnedyn22p/asp.charmm36.elnedyn22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/elnedyn22p/gln.charmm36.elnedyn22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/elnedyn22p/glu.charmm36.elnedyn22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/elnedyn22p/lys.charmm36.elnedyn22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/elnedyn22p/ser.charmm36.elnedyn22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/elnedyn22p/thr.charmm36.elnedyn22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/gln.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/glu.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/gly.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/his.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/ile.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/leu.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/lys.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/met.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/modifications.elnedyn21.mapping
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/modifications.elnedyn22.mapping
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/modifications.elnedyn22p.mapping
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/phe.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/popc.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/pope.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/popg.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/pops.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/pro.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/ser.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/thr.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/trp.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/tyr.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn/val.charmm36.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.699004 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/ala.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/arg.charmm36.elnedyn22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/arg.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/asn.charmm36.elnedyn22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/asn.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/asp.charmm36.elnedyn22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/asp.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/cys.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/gln.charmm36.elnedyn22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/gln.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/glu.charmm36.elnedyn22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/glu.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/gly.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/his.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/ile.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/leu.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/lys.charmm36.elnedyn22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/lys.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/met.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/modifications.mapping
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/phe.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/pro.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/ser.charmm36.elnedyn22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/ser.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/thr.charmm36.elnedyn22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/thr.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/trp.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/tyr.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/elnedyn21/val.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/fmn.gromos.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/gln.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/gln.charmm36.martini22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/gln.gromos.map
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/glu.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/glu.charmm36.martini22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/glu.gromos.map
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/glu0.gromos.map
+-rwxr-xr-x   0 runner    (1001) docker     (123)      794 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/gly.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/gly.gromos.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/his.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/his.gromos.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/hsd.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/hse.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/hsp.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/ile.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/ile.gromos.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/leu.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/leu.gromos.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/lys.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/lys.charmm36.martini22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/lys.gromos.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.719004 vermouth-0.9.3/vermouth/data/mappings/martini3001/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/ala.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/ala.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/antr.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/arg.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/arg.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/ash.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/asn.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/asn.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/asp.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/asp.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/aspp.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/bald.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/benz.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/c3.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/chxe.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/cpen.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/cume.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/cys.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/cys.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/diol.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/diox.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/dman.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/eben.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/fura.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/glh.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/gln.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/gln.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/glu.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/glu.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/glup.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/gly.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/gly.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/hid.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/hie.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/hip.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/his.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/his.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/hsd.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/hse.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/hsp.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/ile.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/ile.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/imia.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/inda.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/indo.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/leu.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/leu.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/lsn.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/lyn.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/lys.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/lys.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/mboa.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/mcpe.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/meob.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/met.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/met.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/mind.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/modifications.amber.mapping
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/modifications.charmm36.mapping
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/mxyl.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/naft.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/nitb.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/oxyl.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/pcro.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/phe.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/phe.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/phen.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/phmk.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/prld.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/pro.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/pro.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/pxyl.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/pyr1.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/pyrd.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/pyrl.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/pyrm.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/qinl.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/ser.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/ser.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/sm139.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/styr.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/thaz.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/thf.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/thip.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/thp.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/thr.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/thr.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/tolu.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/trp.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/trp.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/tyr.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/tyr.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/val.amber.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/val.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/zimi.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/zthp.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini3001/zthz.charmm36.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.723004 vermouth-0.9.3/vermouth/data/mappings/martini30b32/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini30b32/ala.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini30b32/arg.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini30b32/asn.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini30b32/asp.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini30b32/benz.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini30b32/cys.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini30b32/gln.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini30b32/glu.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini30b32/gly.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini30b32/his.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini30b32/hsd.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini30b32/ile.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini30b32/leu.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini30b32/lys.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini30b32/met.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini30b32/modifications.mapping
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini30b32/phe.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini30b32/pro.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini30b32/ser.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini30b32/thr.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini30b32/trp.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini30b32/tyr.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/martini30b32/val.charmm36.map
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1184 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/met.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/met.gromos.map
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/modifications.gromos.mapping
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/modifications.mapping
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/nad.gromos.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/phe.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/phe.gromos.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/popc.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/pope.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/popg.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/pops.charmm36.map
+-rwxr-xr-x   0 runner    (1001) docker     (123)      996 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/pro.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/pro.gromos.map
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/ser.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/ser.charmm36.martini22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/ser.gromos.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/thr.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/thr.charmm36.martini22p.map
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/thr.gromos.map
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/tpp.gromos.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/trp.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/trp.gromos.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/tyr.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/tyr.gromos.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/val.charmm36.map
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/mappings/val.gromos.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/data/quotes.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.723004 vermouth-0.9.3/vermouth/dssp/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/dssp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22140 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/dssp/dssp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15338 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/edge_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44487 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/ffinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/forcefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.723004 vermouth-0.9.3/vermouth/gmx/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/gmx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/gmx/gro.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10682 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/gmx/itp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17698 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/gmx/itp_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18294 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/gmx/rtp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13322 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/graph_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.723004 vermouth-0.9.3/vermouth/graphing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11617 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/graphing/grappa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43888 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/ismags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/log_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20367 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/map_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32810 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/map_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51890 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18045 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/parser_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.727004 vermouth-0.9.3/vermouth/pdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/pdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20974 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/pdb/pdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.731004 vermouth-0.9.3/vermouth/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/add_molecule_edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/annotate_mut_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/apply_posres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20081 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/apply_rubber_band.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/attach_mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/average_beads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16024 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/canonicalize_modifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/do_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/do_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/go_vs_includes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/gro_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/locate_charge_dummies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14592 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/make_bonds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/merge_all_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/merge_chains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/name_moltype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/pdb_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/rename_modified_residues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/repair_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/set_molecule_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/sort_molecule_atoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/processors/tune_cystein_bridges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.739004 vermouth-0.9.3/vermouth/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.747004 vermouth-0.9.3/vermouth/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   127980 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/1bta.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)   127980 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/1bta_mutated.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)   390258 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/2QWO.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)   789750 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/2dn2.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)  3325374 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/6E8W.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/ala5.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/ala5_cg.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/dna-short.pdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.751004 vermouth-0.9.3/vermouth/tests/data/dssp_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/dssp_tests/dssp_1bta.ssd
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/dssp_tests/mini-protein1_betasheet.pdb.v2.2.1-3b2-deb_cv1.ssd
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/dssp_tests/mini-protein1_betasheet.pdb.v3.0.0-3b1-deb_cv1.ssd
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/dssp_tests/mini-protein2_helix.pdb.v2.2.1-3b2-deb_cv1.ssd
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/dssp_tests/mini-protein2_helix.pdb.v3.0.0-3b1-deb_cv1.ssd
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/dssp_tests/mini-protein3_trp-cage.pdb.v2.2.1-3b2-deb_cv1.ssd
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/dssp_tests/mini-protein3_trp-cage.pdb.v3.0.0-3b1-deb_cv1.ssd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.627004 vermouth-0.9.3/vermouth/tests/data/force_fields/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.751004 vermouth-0.9.3/vermouth/tests/data/force_fields/martini-test/
+-rw-r--r--   0 runner    (1001) docker     (123)    20132 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/force_fields/martini-test/aminoacids.ff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.751004 vermouth-0.9.3/vermouth/tests/data/force_fields/pepplane/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/force_fields/pepplane/ala.ff
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/force_fields/pepplane/general.ff
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/force_fields/pepplane/modifications.ff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.751004 vermouth-0.9.3/vermouth/tests/data/force_fields/universal-test/
+-rw-r--r--   0 runner    (1001) docker     (123)    26194 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/force_fields/universal-test/aminoacids.rtp
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/force_fields/universal-test/modifications.ff
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/heme.pdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.631004 vermouth-0.9.3/vermouth/tests/data/integration_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.631004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.751004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/dipro-termini/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/dipro-termini/README
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/dipro-termini/aa.pdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.751004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/dipro-termini/martinize2/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/dipro-termini/martinize2/cg.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/dipro-termini/martinize2/citation
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/dipro-termini/martinize2/command
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/dipro-termini/martinize2/molecule_0.itp
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/dipro-termini/martinize2/topol.top
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.751004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/README
+-rw-r--r--   0 runner    (1001) docker     (123)    36099 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/aa.pdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.755004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/cg.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/chain_A.ssd
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/citation
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/command
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/molecule_0.itp
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/screen.output
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/topol.top
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.755004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/README
+-rw-r--r--   0 runner    (1001) docker     (123)    58725 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/aa.pdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.755004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/
+-rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/cg.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/chain_A.ssd
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/citation
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/command
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/molecule_0.itp
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/screen.output
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/topol.top
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.755004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/README
+-rw-r--r--   0 runner    (1001) docker     (123)    24624 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/aa.pdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.759004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/cg.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/chain_A.ssd
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/citation
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/command
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/molecule_0.itp
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/screen.output
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/topol.top
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.631004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.759004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5/README
+-rw-r--r--   0 runner    (1001) docker     (123)   362933 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5/aa.pdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.763004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/
+-rw-r--r--   0 runner    (1001) docker     (123)    64614 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/cg.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/cg.top
+-rw-r--r--   0 runner    (1001) docker     (123)    48477 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/chain_.ssd
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/citation
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/command
+-rw-r--r--   0 runner    (1001) docker     (123)   130905 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/molecule_0.itp
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/screen.output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.759004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/README
+-rw-r--r--   0 runner    (1001) docker     (123)   362933 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/aa.pdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.763004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/
+-rw-r--r--   0 runner    (1001) docker     (123)    64614 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/cg.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/cg.top
+-rw-r--r--   0 runner    (1001) docker     (123)    48477 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/chain_.ssd
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/citation
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/command
+-rw-r--r--   0 runner    (1001) docker     (123)   130856 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/molecule_0.itp
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/screen.output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.763004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/3i40/
+-rw-r--r--   0 runner    (1001) docker     (123)    63828 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/3i40/3i40.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/3i40/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.767004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11537 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/cg.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/cg.top
+-rw-r--r--   0 runner    (1001) docker     (123)    11526 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/chain_A.ssd
+-rw-r--r--   0 runner    (1001) docker     (123)    11526 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/chain_C.ssd
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/citation
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/command
+-rw-r--r--   0 runner    (1001) docker     (123)    22543 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/insulin_dimer.itp
+-rw-r--r--   0 runner    (1001) docker     (123)    18292 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/molecule_0.itp
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/screen.output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.767004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/
+-rw-r--r--   0 runner    (1001) docker     (123)   159513 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/6LFO_gap.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.767004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/
+-rw-r--r--   0 runner    (1001) docker     (123)    55693 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/cg.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/cg.top
+-rw-r--r--   0 runner    (1001) docker     (123)    10933 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/chain_R.ssd
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/citation
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/command
+-rw-r--r--   0 runner    (1001) docker     (123)   111329 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/molecule_0.itp
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/screen.output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.767004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_chain/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_chain/README
+-rw-r--r--   0 runner    (1001) docker     (123)    63828 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_chain/aa.pdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.771004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11537 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/cg.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/cg.top
+-rw-r--r--   0 runner    (1001) docker     (123)    11526 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/chain_A.ssd
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/citation
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/command
+-rw-r--r--   0 runner    (1001) docker     (123)    20955 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/molecule_0.itp
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/screen.output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.771004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_region/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_region/README
+-rw-r--r--   0 runner    (1001) docker     (123)    63828 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_region/aa.pdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.771004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11537 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/cg.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/cg.top
+-rw-r--r--   0 runner    (1001) docker     (123)    11526 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/chain_A.ssd
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/citation
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/command
+-rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/molecule_0.itp
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/screen.output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.771004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/bpti/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/bpti/README
+-rw-r--r--   0 runner    (1001) docker     (123)    71928 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/bpti/aa.pdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.775004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/
+-rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/cg.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/chain_A.ssd
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/citation
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/command
+-rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/molecule_0.itp
+-rw-r--r--   0 runner    (1001) docker     (123)    26495 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/screen.output
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/topol.top
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.775004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme/README
+-rw-r--r--   0 runner    (1001) docker     (123)   125469 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme/aa.pdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.775004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/
+-rw-r--r--   0 runner    (1001) docker     (123)    27432 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/cg.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)    23245 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/chain_A.ssd
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/citation
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/command
+-rw-r--r--   0 runner    (1001) docker     (123)    47269 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/molecule_0.itp
+-rw-r--r--   0 runner    (1001) docker     (123)    37646 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/screen.output
+-rw-r--r--   0 runner    (1001) docker     (123)    47488 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/test.itp
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/topol.top
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.779004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/README
+-rw-r--r--   0 runner    (1001) docker     (123)   125469 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/aa.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)    28493 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/cg.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)    23245 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/chain_A.ssd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.779004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/
+-rw-r--r--   0 runner    (1001) docker     (123)    28494 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/cg.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)    23245 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/chain_A.ssd
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/citation
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/command
+-rw-r--r--   0 runner    (1001) docker     (123)    56460 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/molecule_0.itp
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/screen.output
+-rw-r--r--   0 runner    (1001) docker     (123)    47488 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/test.itp
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/topol.top
+-rw-r--r--   0 runner    (1001) docker     (123)    56460 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/molecule_0.itp
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/topol.top
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.779004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/prot_modf_charmm/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/prot_modf_charmm/README
+-rw-r--r--   0 runner    (1001) docker     (123)   151339 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/prot_modf_charmm/input.pdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.783004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/prot_modf_charmm/martinize2/
+-rw-r--r--   0 runner    (1001) docker     (123)    28493 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/prot_modf_charmm/martinize2/cg.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/prot_modf_charmm/martinize2/cg.top
+-rw-r--r--   0 runner    (1001) docker     (123)    23245 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/prot_modf_charmm/martinize2/chain_.ssd
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/prot_modf_charmm/martinize2/citation
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/prot_modf_charmm/martinize2/command
+-rw-r--r--   0 runner    (1001) docker     (123)    56361 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/prot_modf_charmm/martinize2/molecule_0.itp
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/prot_modf_charmm/martinize2/screen.output
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/prot_modf_charmm/martinize2/sys.top
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.783004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/villin/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/villin/README
+-rw-r--r--   0 runner    (1001) docker     (123)    23380 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/villin/aa.pdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.783004 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/villin/martinize2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/villin/martinize2/cg.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/villin/martinize2/citation
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/villin/martinize2/command
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/villin/martinize2/molecule_0.itp
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/villin/martinize2/screen.output
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/villin/martinize2/topol.top
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.635004 vermouth-0.9.3/vermouth/tests/data/mappings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.635004 vermouth-0.9.3/vermouth/tests/data/mappings/universal-test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.783004 vermouth-0.9.3/vermouth/tests/data/mappings/universal-test/martini-test/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/mappings/universal-test/martini-test/ser.mapping
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.783004 vermouth-0.9.3/vermouth/tests/data/mappings/universal-test/pepplane/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/mappings/universal-test/pepplane/ala.mapping
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/mappings/universal-test/pepplane/modifications.mapping
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/data/tri_alanine.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/datafiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.783004 vermouth-0.9.3/vermouth/tests/gmx/
+-rw-r--r--   0 runner    (1001) docker     (123)    20593 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/gmx/test_gro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/gmx/test_itp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/helper_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.787004 vermouth-0.9.3/vermouth/tests/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/integration_tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/molecule_strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.787004 vermouth-0.9.3/vermouth/tests/pdb/
+-rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/pdb/test_read_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/pdb/test_write_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_add_molecule_edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_annotate_mut_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19313 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_apply_rubber_band.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_average_beads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_do_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21052 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_dssp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_edge_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_ff_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21519 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_ffinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_forcefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_go_vs_includes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14890 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_grappa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19965 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_ismags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_itp_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_make_bonds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18981 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_map_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16734 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_map_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_mapping_integrative.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44701 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_name_moltype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_native_forcefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_ptm_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_repair_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_section_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_set_molecule_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_sort_molecule_atoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_tune_cystein_bridges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/truncating_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-07-31 09:03:20.000000 vermouth-0.9.3/vermouth/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:35.647004 vermouth-0.9.3/vermouth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-07-31 09:03:35.000000 vermouth-0.9.3/vermouth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31435 2023-07-31 09:03:35.000000 vermouth-0.9.3/vermouth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:03:35.000000 vermouth-0.9.3/vermouth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:03:35.000000 vermouth-0.9.3/vermouth.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-31 09:03:35.000000 vermouth-0.9.3/vermouth.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-31 09:03:35.000000 vermouth-0.9.3/vermouth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 09:03:35.000000 vermouth-0.9.3/vermouth.egg-info/top_level.txt
```

### Comparing `vermouth-0.9.1/.github/workflows/deploy.yml` & `vermouth-0.9.3/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/.github/workflows/run_tests.yml` & `vermouth-0.9.3/.github/workflows/run_tests.yml`

 * *Files 7% similar despite different names*

```diff
@@ -51,23 +51,24 @@
         pip install --upgrade setuptools pip
     - name: Install package and requirements
       run: |
         pip install --upgrade .
         pip install -r requirements-tests.txt
         
     - name: Run pytest with codecoverage
-      run: |
-        coverage run --source=vermouth $(which pytest) -vv vermouth --hypothesis-show-statistics
-        coverage report --omit='*/bin/pytest'
-        
+      run:  pytest vermouth --cov=vermouth --cov-report=xml --hypothesis-show-statistics
     - if: ${{ matrix.WITH_CODECOV }}
-      name: Report code coverage 
-      run: |
-        codecov
-        
+      name: Upload coverage codecov   
+      uses: codecov/codecov-action@v3 
+      with:
+            token: ${{ secrets.CODECOV_TOKEN }}
+            files: ./coverage.xml
+            fail_ci_if_error: true
+            verbose: true
+            
   lint:
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python 3.10
       uses: actions/setup-python@v4
```

### Comparing `vermouth-0.9.1/.pylintrc` & `vermouth-0.9.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/.zenodo.json` & `vermouth-0.9.3/.zenodo.json`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/LICENSE` & `vermouth-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/PKG-INFO` & `vermouth-0.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vermouth
-Version: 0.9.1
+Version: 0.9.3
 Home-page: https://github.com/marrink-lab/vermouth-martinize
 Author: P C Kroon
 Author-email: p.c.kroon@rug.nl
 License: Apache 2.0
 Keywords: martini MD martinize
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -81,14 +81,24 @@
 At the moment, martinize2 tries to reproduce the interface of the original
 Martinize. You can find explanations on how to use Martinize on the [Martini
 tutorials]; in most cases, replacing calls to `martinize.py` by calls to
 `martinize2` should produce similar results.
 
 The documentation of the vermouth python library will come soon.
 
+## Citation
+```
+@article{kroon2022martinize2,
+  title={Martinize2 and Vermouth: Unified Framework for Topology Generation},
+  author={Kroon, Peter C and Gr{\"u}newald, Fabian and Barnoud, Jonathan and van Tilburg, Marco 
+          and Souza, Paulo CT and Wassenaar, Tsjerk A and Marrink, Siewert-Jan},
+  journal={arXiv preprint arXiv:2212.01191},
+  year={2022}}
+```
+
 ## License
 
 Martinize2 and vermouth are distributed under the Apache 2.0 license.
 
     Copyright 2018 University of Groningen
 
 	Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `vermouth-0.9.1/README.md` & `vermouth-0.9.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -57,14 +57,24 @@
 At the moment, martinize2 tries to reproduce the interface of the original
 Martinize. You can find explanations on how to use Martinize on the [Martini
 tutorials]; in most cases, replacing calls to `martinize.py` by calls to
 `martinize2` should produce similar results.
 
 The documentation of the vermouth python library will come soon.
 
+## Citation
+```
+@article{kroon2022martinize2,
+  title={Martinize2 and Vermouth: Unified Framework for Topology Generation},
+  author={Kroon, Peter C and Gr{\"u}newald, Fabian and Barnoud, Jonathan and van Tilburg, Marco 
+          and Souza, Paulo CT and Wassenaar, Tsjerk A and Marrink, Siewert-Jan},
+  journal={arXiv preprint arXiv:2212.01191},
+  year={2022}}
+```
+
 ## License
 
 Martinize2 and vermouth are distributed under the Apache 2.0 license.
 
     Copyright 2018 University of Groningen
 
 	Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `vermouth-0.9.1/bin/embed_test.py` & `vermouth-0.9.3/bin/embed_test.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/bin/martinize2` & `vermouth-0.9.3/bin/martinize2`

 * *Files 22% similar despite different names*

```diff
@@ -32,144 +32,173 @@
 from vermouth import DATA_PATH
 from vermouth.dssp import dssp
 from vermouth.dssp.dssp import (
     AnnotateDSSP,
     AnnotateMartiniSecondaryStructures,
     AnnotateResidues,
 )
-from vermouth.log_helpers import (StyleAdapter, BipolarFormatter,
-                                  CountingHandler, TypeAdapter,
-                                  ignore_warnings_and_count,)
+from vermouth.log_helpers import (
+    StyleAdapter,
+    BipolarFormatter,
+    CountingHandler,
+    TypeAdapter,
+    ignore_warnings_and_count,
+)
 from vermouth import selectors
 from vermouth.map_input import (
     read_mapping_directory,
     generate_all_self_mappings,
-    combine_mappings
+    combine_mappings,
 )
 from vermouth.citation_parser import citation_formatter
 
 # TODO Since vermouth's __init__.py does some logging (KDTree), this may or may
 # not work as intended. Investigation required.
 
-LOGGER = TypeAdapter(logging.getLogger('vermouth'))
+LOGGER = TypeAdapter(logging.getLogger("vermouth"))
 
-PRETTY_FORMATTER = logging.Formatter(fmt='{levelname:>8} - {type} - {message}',
-                                     style='{')
-DETAILED_FORMATTER = logging.Formatter(fmt='{levelname:>8} - {type} - {name} - {message}',
-                                       style='{')
+PRETTY_FORMATTER = logging.Formatter(
+    fmt="{levelname:>8} - {type} - {message}", style="{"
+)
+DETAILED_FORMATTER = logging.Formatter(
+    fmt="{levelname:>8} - {type} - {name} - {message}", style="{"
+)
 
 COUNTER = CountingHandler()
 
 # Control above what level message we want to count
 COUNTER.setLevel(logging.WARNING)
 
 CONSOLE_HANDLER = logging.StreamHandler()
-FORMATTER = BipolarFormatter(DETAILED_FORMATTER,
-                             PRETTY_FORMATTER,
-                             logging.DEBUG,
-                             logger=LOGGER)
+FORMATTER = BipolarFormatter(
+    DETAILED_FORMATTER, PRETTY_FORMATTER, logging.DEBUG, logger=LOGGER
+)
 CONSOLE_HANDLER.setFormatter(FORMATTER)
 LOGGER.addHandler(CONSOLE_HANDLER)
 LOGGER.addHandler(COUNTER)
 
 LOGGER = StyleAdapter(LOGGER)
 
-VERSION = 'martinize with vermouth {}'.format(vermouth.__version__)
+VERSION = "martinize with vermouth {}".format(vermouth.__version__)
 
 
 def read_system(path, ignore_resnames=(), ignh=None, modelidx=None):
     """
     Read a system from a PDB or GRO file.
 
     This function guesses the file type based on the file extension.
 
     The resulting system does not have a force field and may not have edges.
     """
     system = vermouth.System()
     file_extension = path.suffix.upper()[1:]  # We do not keep the dot
-    if file_extension in ['PDB', 'ENT']:
-        vermouth.PDBInput(str(path), exclude=ignore_resnames, ignh=ignh,
-                          modelidx=modelidx).run_system(system)
-    elif file_extension in ['GRO']:
-        vermouth.GROInput(str(path), exclude=ignore_resnames, ignh=ignh).run_system(system)
+    if file_extension in ["PDB", "ENT"]:
+        vermouth.PDBInput(
+            str(path), exclude=ignore_resnames, ignh=ignh, modelidx=modelidx
+        ).run_system(system)
+    elif file_extension in ["GRO"]:
+        vermouth.GROInput(str(path), exclude=ignore_resnames, ignh=ignh).run_system(
+            system
+        )
     else:
         raise ValueError('Unknown file extension "{}".'.format(file_extension))
     return system
 
 
-def pdb_to_universal(system, delete_unknown=False, force_field=None,
-                     modifications=None, mutations=None,
-                     bonds_from_name=True, bonds_from_dist=True, bonds_fudge=1,
-                     write_graph=None, write_repair=None, write_canon=None):
+def pdb_to_universal(
+    system,
+    delete_unknown=False,
+    force_field=None,
+    modifications=None,
+    mutations=None,
+    bonds_from_name=True,
+    bonds_from_dist=True,
+    bonds_fudge=1,
+    write_graph=None,
+    write_repair=None,
+    write_canon=None,
+):
     """
     Convert a system read from the PDB to a clean canonical atomistic system.
     """
     if force_field is None:
-        force_field = vermouth.forcefield.get_native_force_field('charmm')
+        force_field = vermouth.forcefield.get_native_force_field("charmm")
     if modifications is None:
         modifications = []
     if mutations is None:
         mutations = []
     canonicalized = system.copy()
     canonicalized.force_field = force_field
 
-    LOGGER.info('Guessing the bonds.', type='step')
-    vermouth.MakeBonds(allow_name=bonds_from_name,
-                       allow_dist=bonds_from_dist,
-                       fudge=bonds_fudge).run_system(canonicalized)
+    LOGGER.info("Guessing the bonds.", type="step")
+    vermouth.MakeBonds(
+        allow_name=bonds_from_name, allow_dist=bonds_from_dist, fudge=bonds_fudge
+    ).run_system(canonicalized)
     vermouth.MergeNucleicStrands().run_system(canonicalized)
     if write_graph is not None:
-        vermouth.pdb.write_pdb(canonicalized, str(write_graph), omit_charges=True,
-                               defer_writing=False)
+        vermouth.pdb.write_pdb(
+            canonicalized, str(write_graph), omit_charges=True, defer_writing=False
+        )
 
-    LOGGER.debug('Annotating required mutations and modifications.', type='step')
+    LOGGER.debug("Annotating required mutations and modifications.", type="step")
     vermouth.AnnotateMutMod(modifications, mutations).run_system(canonicalized)
-    LOGGER.info('Repairing the graph.', type='step')
-    vermouth.RepairGraph(delete_unknown=delete_unknown, include_graph=False).run_system(canonicalized)
+    LOGGER.info("Repairing the graph.", type="step")
+    vermouth.RepairGraph(delete_unknown=delete_unknown, include_graph=False).run_system(
+        canonicalized
+    )
     if write_repair is not None:
-        vermouth.pdb.write_pdb(canonicalized, str(write_repair),
-                               omit_charges=True, nan_missing_pos=True, 
-                               defer_writing=False)
-    LOGGER.info('Dealing with modifications.', type='step')
+        vermouth.pdb.write_pdb(
+            canonicalized,
+            str(write_repair),
+            omit_charges=True,
+            nan_missing_pos=True,
+            defer_writing=False,
+        )
+    LOGGER.info("Dealing with modifications.", type="step")
     vermouth.CanonicalizeModifications().run_system(canonicalized)
     if write_canon is not None:
-        vermouth.pdb.write_pdb(canonicalized, str(write_canon),
-                               omit_charges=True, nan_missing_pos=True,
-                               defer_writing=False)
-    vermouth.AttachMass(attribute='mass').run_system(canonicalized)
-    vermouth.SortMoleculeAtoms().run_system(canonicalized) # was system
+        vermouth.pdb.write_pdb(
+            canonicalized,
+            str(write_canon),
+            omit_charges=True,
+            nan_missing_pos=True,
+            defer_writing=False,
+        )
+    vermouth.AttachMass(attribute="mass").run_system(canonicalized)
     return canonicalized
 
 
 def martinize(system, mappings, to_ff, delete_unknown=False):
     """
     Convert a system from one force field to an other at lower resolution.
     """
-    LOGGER.info('Creating the graph at the target resolution.', type='step')
-    vermouth.DoMapping(mappings=mappings,
-                       to_ff=to_ff,
-                       delete_unknown=delete_unknown,
-                       attribute_keep=('cgsecstruct', 'chain'),
-                       attribute_must=('resname',),
-                       attribute_stash=('resid',)).run_system(system)
-    LOGGER.info('Averaging the coordinates.', type='step')
+    LOGGER.info("Creating the graph at the target resolution.", type="step")
+    vermouth.DoMapping(
+        mappings=mappings,
+        to_ff=to_ff,
+        delete_unknown=delete_unknown,
+        attribute_keep=("cgsecstruct", "chain"),
+        attribute_must=("resname",),
+        attribute_stash=("resid",),
+    ).run_system(system)
+    LOGGER.info("Averaging the coordinates.", type="step")
     vermouth.DoAverageBead(ignore_missing_graphs=True).run_system(system)
-    LOGGER.info('Applying the links.', type='step')
+    LOGGER.info("Applying the links.", type="step")
     vermouth.DoLinks().run_system(system)
-    LOGGER.info('Placing the charge dummies.', type='step')
+    LOGGER.info("Placing the charge dummies.", type="step")
     vermouth.LocateChargeDummies().run_system(system)
     return system
 
 
 def write_gmx_topology(system, top_path, defines=(), header=()):
     """
     Writes a Gromacs .top file for the specified system.
     """
     if not system.molecules:
-        raise ValueError('No molecule in the system. Nothing to write.')
+        raise ValueError("No molecule in the system. Nothing to write.")
 
     # Write the ITP files for the molecule types, and prepare writing the
     # [ molecules ] section of the top file.
     # * We write one ITP file for each different moltype in the system, the
     #   moltype being defined by the name provided under the "moltype" meta of
     #   the molecules. If more than one molecule share the same moltype, we use
     #   the first one to write the ITP file.
@@ -181,63 +210,67 @@
     moltype_count = []  # items will be [moltype, number of molecules]
 
     # Iterate over groups of successive molecules with the same moltypes. We
     # shall *NOT* sort the molecules before hand, as groups of successive
     # molecules with the same moltype can be interupted by other moltypes, and
     # we want to reflect these interuptions in the [ molecules ] section of the
     # top file.
-    molecule_groups = itertools.groupby(system.molecules, key=lambda x: x.meta['moltype'])
+    molecule_groups = itertools.groupby(
+        system.molecules, key=lambda x: x.meta["moltype"]
+    )
     for moltype, molecules in molecule_groups:
         molecule = next(molecules)
         if moltype not in moltype_written:
             # A given moltype can appear more than once in the sequence of
             # molecules, without being uninterupted by other moltypes. Even in
             # that case, we want to write the ITP only once.
-            with deferred_open('{}.itp'.format(moltype), 'w') as outfile:
+            with deferred_open("{}.itp".format(moltype), "w") as outfile:
                 # here we format and merge all citations
-                header[-1] = header[-1]+"\n"
+                header[-1] = header[-1] + "\n"
                 header.append("Pleas cite the following papers:")
                 for citation in molecule.citations:
-                    cite_string =  citation_formatter(molecule.force_field.citations[citation])
+                    cite_string = citation_formatter(
+                        molecule.force_field.citations[citation]
+                    )
                     LOGGER.info("Please cite: " + cite_string)
                     header.append(cite_string)
                 vermouth.gmx.itp.write_molecule_itp(molecule, outfile, header=header)
-            this_moltype_len = len(molecule.meta['moltype'])
+            this_moltype_len = len(molecule.meta["moltype"])
             if this_moltype_len > max_name_length:
                 max_name_length = this_moltype_len
             moltype_written.add(moltype)
         # We already removed one element from the "molecules" generator, do not
         # forget to count it in the number of molecules in that group.
         moltype_count.append([moltype, 1 + len(list(molecules))])
 
     # Write the top file
-    template = textwrap.dedent("""\
+    template = textwrap.dedent(
+        """\
         {defines}
         #include "martini.itp"
         {includes}
 
         [ system ]
         Title of the system
 
         [ molecules ]
         {molecules}
-    """)
-    include_string = '\n'.join(
-        '#include "{}.itp"'.format(molecule_type)
-        for molecule_type, _ in moltype_count
-    )
-    molecule_string = '\n'.join(
-        '{mtype:<{length}}    {num}'
-        .format(mtype=mtype, num=num, length=max_name_length)
-        for mtype, num in moltype_count
+    """
+    )
+    include_string = "\n".join(
+        '#include "{}.itp"'.format(molecule_type) for molecule_type, _ in moltype_count
     )
-    define_string = '\n'.join(
-        '#define {}'.format(define) for define in defines
+    molecule_string = "\n".join(
+        "{mtype:<{length}}    {num}".format(
+            mtype=mtype, num=num, length=max_name_length
+        )
+        for mtype, num in moltype_count
     )
-    with deferred_open(str(top_path), 'w') as outfile:
+    define_string = "\n".join("#define {}".format(define) for define in defines)
+    with deferred_open(str(top_path), "w") as outfile:
         outfile.write(
             textwrap.dedent(
                 template.format(
                     includes=include_string,
                     molecules=molecule_string,
                     defines=define_string,
                 )
@@ -267,20 +300,22 @@
     argparse.ArgumentError
         Raised when the value cannot be converted.
     """
     try:
         result = float(value)
     except ValueError:
         lowered = value.lower()
-        if lowered in ('auto', 'none'):
+        if lowered in ("auto", "none"):
             return lowered
         raise argparse.ArgumentError(
-            argument='-cys',
-            message=('The value of the "cys" option must be "auto", "none", '
-                     'or a distance in nanometers.'),
+            argument="-cys",
+            message=(
+                'The value of the "cys" option must be "auto", "none", '
+                "or a distance in nanometers."
+            ),
         )
     else:
         return result
 
 
 def maxwarn(value):
     """
@@ -305,21 +340,23 @@
         A warning type and the associated count to ignore. Either element can be
         None if not specified.
 
     Raises
     ------
     argparse.ArgumentTypeError
     """
-    msg = ("Values for the -maxwarn option must be the name of a "
-           "warning type, a number, or following the format "
-           "'<warning-type>:<count>' where <warning-type> is the name "
-           "of the warning type to ignore, and <count> is the number of "
-           "warning of that type to ignore. "
-           "'{value}' is not a valid value.".format(value=value))
-    splitted = value.split(':')
+    msg = (
+        "Values for the -maxwarn option must be the name of a "
+        "warning type, a number, or following the format "
+        "'<warning-type>:<count>' where <warning-type> is the name "
+        "of the warning type to ignore, and <count> is the number of "
+        "warning of that type to ignore. "
+        "'{value}' is not a valid value.".format(value=value)
+    )
+    splitted = value.split(":")
     if len(splitted) == 1:
         try:
             count = int(value)
         except ValueError:
             # The value is not an int, so a warning type to ignore an
             # an unspecified number of
             return (value, None)
@@ -330,420 +367,665 @@
             count = int(splitted[1])
         except ValueError:
             pass  # The exception will be raised at the end of the function
         else:
             return (splitted[0], count)
     raise argparse.ArgumentTypeError(msg)
 
+
 def entry():
     """
     Parses commandline arguments and performs the logic.
     """
     parser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
-    parser.add_argument('-V', '--version', action='version', version=VERSION)
+    parser.add_argument("-V", "--version", action="version", version=VERSION)
+
+    file_group = parser.add_argument_group("Input and output files")
+    file_group.add_argument(
+        "-f", dest="inpath", required=False, type=Path, help="Input file (PDB|GRO)"
+    )
+    file_group.add_argument(
+        "-x",
+        dest="outpath",
+        required=False,
+        type=Path,
+        help="Output coarse grained structure (PDB)",
+    )
+    file_group.add_argument(
+        "-o", dest="top_path", type=Path, help="Output topology (TOP)"
+    )
+    file_group.add_argument(
+        "-sep",
+        dest="keep_duplicate_itp",
+        action="store_true",
+        default=False,
+        help="Write separate topologies for identical chains",
+    )
+    file_group.add_argument(
+        "-merge",
+        dest="merge_chains",
+        type=lambda x: x.split(","),
+        action="append",
+        help="Merge chains: e.g. -merge A,B,C (+)",
+    )
+    file_group.add_argument(
+        "-resid",
+        dest="resid_handling",
+        type=str,
+        default="mol",
+        help="How to handle resid. Choice of mol or input.\n"
+        "mol: resids are numbered from 1 to n for each molecule\n"
+        "input: resids are the same as in the input pdb",
+    )
+    file_group.add_argument(
+        "-ignore",
+        dest="ignore_res",
+        nargs="+",
+        default=[],
+        action="append",
+        type=lambda x: x.split(","),
+        help="Ignore residues with that name: e.g. " "-ignore HOH,LIG (+)",
+    )
+    file_group.add_argument(
+        "-ignh",
+        dest="ignore_h",
+        default=False,
+        action="store_true",
+        help="Ignore all Hydrogen atoms in the input file",
+    )
+    file_group.add_argument(
+        "-model",
+        dest="modelidx",
+        default=None,
+        type=int,
+        help="Which MODEL to select. Only meaningful for" " PDB files.",
+    )
+    file_group.add_argument(
+        "-bonds-from",
+        dest="bonds_from",
+        choices=["name", "distance", "none", "both"],
+        default="both",
+        help="How to determine connectivity in the input. "
+        "If 'none', only bonds from the input file (CONECT)"
+        " will be used.",
+    )
+    file_group.add_argument(
+        "-bonds-fudge",
+        dest="bonds_fudge",
+        type=float,
+        default=1.2,
+        help="Factor with which Van der Waals"
+        " radii should be scaled when determining bonds "
+        "based on distances.",
+    )
+
+    ff_group = parser.add_argument_group("Force field selection")
+    ff_group.add_argument(
+        "-ff", dest="to_ff", default="martini3001", help="Which forcefield to use"
+    )
+    ff_group.add_argument(
+        "-from",
+        dest="from_ff",
+        default="charmm",
+        help="Force field of the original structure.",
+    )
+    ff_group.add_argument(
+        "-ff-dir",
+        dest="extra_ff_dir",
+        action="append",
+        type=Path,
+        default=[],
+        help="Additional repository for custom force fields.",
+    )
+    ff_group.add_argument(
+        "-map-dir",
+        dest="extra_map_dir",
+        action="append",
+        type=Path,
+        default=[],
+        help="Additional repository for mapping files.",
+    )
+    ff_group.add_argument(
+        "-list-ff",
+        action="store_true",
+        dest="list_ff",
+        help="List all known force fields, and exit.",
+    )
+    ff_group.add_argument(
+        "-list-blocks",
+        action="store_true",
+        dest="list_blocks",
+        help="List all Blocks and Modifications known to the" " force field, and exit.",
+    )
 
-    file_group = parser.add_argument_group('Input and output files')
-    file_group.add_argument('-f', dest='inpath', required=False, type=Path,
-                            help='Input file (PDB|GRO)')
-    file_group.add_argument('-x', dest='outpath', required=False, type=Path,
-                            help='Output coarse grained structure (PDB)')
-    file_group.add_argument('-o', dest='top_path', type=Path,
-                            help='Output topology (TOP)')
-    file_group.add_argument('-sep', dest='keep_duplicate_itp',
-                            action='store_true', default=False,
-                            help='Write separate topologies for identical chains')
-    file_group.add_argument('-merge', dest='merge_chains',
-                            type=lambda x: x.split(','), action='append',
-                            help='Merge chains: e.g. -merge A,B,C (+)')
-    file_group.add_argument('-resid', dest='resid_handling',
-                            type=str, default='mol',
-                            help="How to handle resid. Choice of mol or input.\n"
-                                 "mol: resids are numbered from 1 to n for each molecule\n"
-                                 "input: resids are the same as in the input pdb")
-    file_group.add_argument('-ignore', dest='ignore_res', nargs='+',
-                            default=[], action='append', type=lambda x: x.split(','),
-                            help='Ignore residues with that name: e.g. '
-                            '-ignore HOH,LIG (+)')
-    file_group.add_argument('-ignh', dest='ignore_h', default=False,
-                            action='store_true',
-                            help='Ignore all Hydrogen atoms in the input file')
-    file_group.add_argument('-model', dest='modelidx', default=None, type=int,
-                            help='Which MODEL to select. Only meaningful for'
-                            ' PDB files.')
-    file_group.add_argument('-bonds-from', dest='bonds_from',
-                            choices=['name', 'distance', 'none', 'both'],
-                            default='both',
-                            help="How to determine connectivity in the input. "
-                            "If 'none', only bonds from the input file (CONECT)"
-                            " will be used.")
-    file_group.add_argument('-bonds-fudge', dest='bonds_fudge', type=float,
-                            default=1.2, help='Factor with which Van der Waals'
-                            ' radii should be scaled when determining bonds '
-                            'based on distances.')
-
-    ff_group = parser.add_argument_group('Force field selection')
-    ff_group.add_argument('-ff', dest='to_ff', default='martini3001',
-                          help='Which forcefield to use')
-    ff_group.add_argument('-from', dest='from_ff', default='charmm',
-                          help='Force field of the original structure.')
-    ff_group.add_argument('-ff-dir', dest='extra_ff_dir', action='append',
-                          type=Path, default=[],
-                          help='Additional repository for custom force fields.')
-    ff_group.add_argument('-map-dir', dest='extra_map_dir', action='append',
-                          type=Path, default=[],
-                          help='Additional repository for mapping files.')
-    ff_group.add_argument('-list-ff', action='store_true', dest='list_ff',
-                          help='List all known force fields, and exit.')
-    ff_group.add_argument('-list-blocks', action='store_true', dest='list_blocks',
-                          help='List all Blocks and Modifications known to the'
-                          ' force field, and exit.')
-
-    posres_group = parser.add_argument_group('Position restraints')
-    posres_group.add_argument('-p', dest='posres', type=str.lower,
-                              choices=('none', 'all', 'backbone'), default='none',
-                              help='Output position restraints (none/all/backbone)')
-    posres_group.add_argument('-pf', dest='posres_fc', type=float, default=1000,
-                              help='Position restraints force constant in kJ/mol/nm^2')
-    secstruct_group = parser.add_argument_group('Secondary structure handling')
+    posres_group = parser.add_argument_group("Position restraints")
+    posres_group.add_argument(
+        "-p",
+        dest="posres",
+        type=str.lower,
+        choices=("none", "all", "backbone"),
+        default="none",
+        help="Output position restraints (none/all/backbone)",
+    )
+    posres_group.add_argument(
+        "-pf",
+        dest="posres_fc",
+        type=float,
+        default=1000,
+        help="Position restraints force constant in kJ/mol/nm^2",
+    )
+    secstruct_group = parser.add_argument_group("Secondary structure handling")
     secstruct_exclusion = secstruct_group.add_mutually_exclusive_group()
-    secstruct_exclusion.add_argument('-dssp', nargs='?', const='dssp',
-                                     help='DSSP executable for determining structure')
-    secstruct_exclusion.add_argument('-ss', dest='ss', type=str.upper,
-                                     metavar='SEQUENCE',
-                                     help=('Manually set the secondary '
-                                           'structure of the proteins.'))
-    secstruct_exclusion.add_argument('-collagen', action='store_true', default=False,
-                                     help='Use collagen parameters')
-    secstruct_group.add_argument('-ed', dest='extdih', action='store_true', default=False,
-                                 help=('Use dihedrals for extended regions '
-                                       'rather than elastic bonds'))
-
-    rb_group = parser.add_argument_group('Protein elastic network')
-    rb_group.add_argument('-elastic', action='store_true', default=False,
-                          help='Write elastic bonds')
-    rb_group.add_argument('-ef', dest='rb_force_constant', type=float, default=500,
-                          help='Elastic bond force constant Fc in kJ/mol/nm^2')
-    rb_group.add_argument('-el', dest='rb_lower_bound', type=float, default=0,
-                          help='Elastic bond lower cutoff: F = Fc if rij < lo')
-    rb_group.add_argument('-eu', dest='rb_upper_bound', type=float, default=0.9,
-                          help='Elastic bond upper cutoff: F = 0  if rij > up')
-    rb_group.add_argument('-ermd', dest='res_min_dist', type=int,
-                          help=('The minimum separation between two residues to have an RB '
-                                'the default value is set by the force-field.'),
-                          default=None)
-    rb_group.add_argument('-ea', dest='rb_decay_factor', type=float, default=0,
-                          help='Elastic bond decay factor a')
-    rb_group.add_argument('-ep', dest='rb_decay_power', type=float, default=1,
-                          help='Elastic bond decay power p')
-    rb_group.add_argument('-em', dest='rb_minimum_force', type=float, default=0,
-                          help='Remove elastic bonds with force constant lower than this')
-    rb_group.add_argument('-eb', dest='rb_selection',
-                          type=lambda x: x.split(','), default=None,
-                          help='Comma separated list of bead names for elastic bonds')
-    rb_group.add_argument('-eunit', dest='rb_unit', default='molecule',
-                          help=('Establish what is the structural unit for the '
-                                'elastic network. Bonds are only created within'
-                                ' a unit. Options are molecule, chain, all, or a'
-                                'specified region defined by resids, with following'
-                                'format: <start_resid_1>:<end_resid_1>, <start_resid_2>:<end_resid_2>...'))
-    go_group = parser.add_argument_group('Virtual site based GoMartini')
-    go_group.add_argument('-govs-includes', action='store_true', default=False,
-                          help='Write include statements to use Vitrual Site Go Martini.')
-    go_group.add_argument('-govs-moltype', default='molecule_0',
-                          help=('Set the name of the molecule when using '
-                                'Virtual Sites GoMartini.'))
-    prot_group = parser.add_argument_group('Protein description')
-    prot_group.add_argument('-scfix', dest='scfix',
-                            action='store_true', default=False,
-                            help='Apply side chain corrections.')
-    prot_group.add_argument('-cys', dest='cystein_bridge',
-                            type=_cys_argument,
-                            default='none', help='Cystein bonds')
-    prot_group.add_argument('-mutate', dest='mutations', action='append',
-                            type=lambda s: s.split(':'), default=[],
-                            help='Mutate a residue. Desired mutation is '
-                            'specified as, e.g. A-PHE45:ALA. The format is '
-                            '<chain>-<resname><resid>:<new resname>. Elements '
-                            'of the specification can be omitted as required.')
-    prot_group.add_argument('-modify', dest='modifications', action='append',
-                            type=lambda s: s.split(':'), default=[],
-                            help='Add a modification to a residue. Desired '
-                            'modification is specified as, e.g. A-ASP45:ASP0. '
-                            'The format is <chain>-<resname><resid>:<modification>.'
-                            ' Elements of the specification can be omitted as '
-                            'required.')
-    prot_group.add_argument('-nter', dest='modifications', action='append',
-                            type=lambda s: ['nter', s], default=[],
-                            help='Shorthand for patching N-termini. An '
-                            'N-terminus is defined as a residue which is '
-                            'connected to 1 other residue, and has the highest '
-                            'resid.')
-    prot_group.add_argument('-cter', dest='modifications', action='append',
-                            type=lambda s: ['cter', s], default=[],
-                            help='Shorthand for patching C-termini. A '
-                            'C-terminus is defined as a residue which is '
-                            'connected to 1 other residue, and has the lowest '
-                            'resid.')
+    secstruct_exclusion.add_argument(
+        "-dssp",
+        nargs="?",
+        const="dssp",
+        help="DSSP executable for determining structure",
+    )
+    secstruct_exclusion.add_argument(
+        "-ss",
+        dest="ss",
+        type=str.upper,
+        metavar="SEQUENCE",
+        help=("Manually set the secondary " "structure of the proteins."),
+    )
+    secstruct_exclusion.add_argument(
+        "-collagen", action="store_true", default=False, help="Use collagen parameters"
+    )
+    secstruct_group.add_argument(
+        "-ed",
+        dest="extdih",
+        action="store_true",
+        default=False,
+        help=("Use dihedrals for extended regions " "rather than elastic bonds"),
+    )
+
+    rb_group = parser.add_argument_group("Protein elastic network")
+    rb_group.add_argument(
+        "-elastic", action="store_true", default=False, help="Write elastic bonds"
+    )
+    rb_group.add_argument(
+        "-ef",
+        dest="rb_force_constant",
+        type=float,
+        default=500,
+        help="Elastic bond force constant Fc in kJ/mol/nm^2",
+    )
+    rb_group.add_argument(
+        "-el",
+        dest="rb_lower_bound",
+        type=float,
+        default=0,
+        help="Elastic bond lower cutoff: F = Fc if rij < lo",
+    )
+    rb_group.add_argument(
+        "-eu",
+        dest="rb_upper_bound",
+        type=float,
+        default=0.9,
+        help="Elastic bond upper cutoff: F = 0  if rij > up",
+    )
+    rb_group.add_argument(
+        "-ermd",
+        dest="res_min_dist",
+        type=int,
+        help=(
+            "The minimum separation between two residues to have an RB "
+            "the default value is set by the force-field."
+        ),
+        default=None,
+    )
+    rb_group.add_argument(
+        "-ea",
+        dest="rb_decay_factor",
+        type=float,
+        default=0,
+        help="Elastic bond decay factor a",
+    )
+    rb_group.add_argument(
+        "-ep",
+        dest="rb_decay_power",
+        type=float,
+        default=1,
+        help="Elastic bond decay power p",
+    )
+    rb_group.add_argument(
+        "-em",
+        dest="rb_minimum_force",
+        type=float,
+        default=0,
+        help="Remove elastic bonds with force constant lower than this",
+    )
+    rb_group.add_argument(
+        "-eb",
+        dest="rb_selection",
+        type=lambda x: x.split(","),
+        default=None,
+        help="Comma separated list of bead names for elastic bonds",
+    )
+    rb_group.add_argument(
+        "-eunit",
+        dest="rb_unit",
+        default="molecule",
+        help=(
+            "Establish what is the structural unit for the "
+            "elastic network. Bonds are only created within"
+            " a unit. Options are molecule, chain, all, or a"
+            "specified region defined by resids, with following"
+            "format: <start_resid_1>:<end_resid_1>, <start_resid_2>:<end_resid_2>..."
+        ),
+    )
+    go_group = parser.add_argument_group("Virtual site based GoMartini")
+    go_group.add_argument(
+        "-govs-includes",
+        action="store_true",
+        default=False,
+        help="Write include statements to use Vitrual Site Go Martini.",
+    )
+    go_group.add_argument(
+        "-govs-moltype",
+        default="molecule_0",
+        help=("Set the name of the molecule when using " "Virtual Sites GoMartini."),
+    )
+    prot_group = parser.add_argument_group("Protein description")
+    prot_group.add_argument(
+        "-scfix",
+        dest="scfix",
+        action="store_true",
+        default=False,
+        help="Apply side chain corrections.",
+    )
+    prot_group.add_argument(
+        "-cys",
+        dest="cystein_bridge",
+        type=_cys_argument,
+        default="none",
+        help="Cystein bonds",
+    )
+    prot_group.add_argument(
+        "-mutate",
+        dest="mutations",
+        action="append",
+        type=lambda s: s.split(":"),
+        default=[],
+        help="Mutate a residue. Desired mutation is "
+        "specified as, e.g. A-PHE45:ALA. The format is "
+        "<chain>-<resname><resid>:<new resname>. Elements "
+        "of the specification can be omitted as required.",
+    )
+    prot_group.add_argument(
+        "-modify",
+        dest="modifications",
+        action="append",
+        type=lambda s: s.split(":"),
+        default=[],
+        help="Add a modification to a residue. Desired "
+        "modification is specified as, e.g. A-ASP45:ASP0. "
+        "The format is <chain>-<resname><resid>:<modification>."
+        " Elements of the specification can be omitted as "
+        "required.",
+    )
+    prot_group.add_argument(
+        "-nter",
+        dest="modifications",
+        action="append",
+        type=lambda s: ["nter", s],
+        default=[],
+        help="Shorthand for patching N-termini. An "
+        "N-terminus is defined as a residue which is "
+        "connected to 1 other residue, and has the highest "
+        "resid.",
+    )
+    prot_group.add_argument(
+        "-cter",
+        dest="modifications",
+        action="append",
+        type=lambda s: ["cter", s],
+        default=[],
+        help="Shorthand for patching C-termini. A "
+        "C-terminus is defined as a residue which is "
+        "connected to 1 other residue, and has the lowest "
+        "resid.",
+    )
     # Unfortunately there's no action=extend_const. append_const *almost* does
     # what we need, but it makes the resulting list too deep:
     # [[['cter', 'COOH-ter'], ['nter', 'NH2-ter']], ['ASP3', 'ASP0']]
-    prot_group.add_argument('-nt', dest='neutral_termini',
-                            action='store_true', default=False,
-                            help='Set neutral termini (charged is default). '
-                            'Alias for "-nter NH2-ter -cter COOH-ter"')
-
-    debug_group = parser.add_argument_group('Debugging options')
-    debug_group.add_argument('-write-graph', type=Path, default=None,
-                             help='Write the graph as PDB after the MakeBonds step.')
-    debug_group.add_argument('-write-repair', type=Path, default=None,
-                             help=('Write the graph as PDB after the '
-                                   'RepairGraph step. The resulting file may '
-                                   'contain "nan" coordinates making it '
-                                   'unreadable by most softwares.'))
-    debug_group.add_argument('-write-canon', type=Path, default=None,
-                             help=('Write the graph as PDB after the '
-                                   'CanonicalizeModifications step. The '
-                                   'resulting file may contain "nan" '
-                                   'coordinates making it unreadable by most '
-                                   'software.'))
-    debug_group.add_argument('-v', dest='verbosity', action='count',
-                             help='Enable debug logging output. Can be given '
-                                  'multiple times.', default=0)
-    debug_group.add_argument('-maxwarn', dest='maxwarn', type=maxwarn,
-                             action='append', nargs='+', default=[],
-                             help='The maximum number of allowed warnings. If '
-                             'more warnings are encountered no output files are'
-                             ' written.')
+    prot_group.add_argument(
+        "-nt",
+        dest="neutral_termini",
+        action="store_true",
+        default=False,
+        help="Set neutral termini (charged is default). "
+        'Alias for "-nter NH2-ter -cter COOH-ter"',
+    )
+
+    debug_group = parser.add_argument_group("Debugging options")
+    debug_group.add_argument(
+        "-write-graph",
+        type=Path,
+        default=None,
+        help="Write the graph as PDB after the MakeBonds step.",
+    )
+    debug_group.add_argument(
+        "-write-repair",
+        type=Path,
+        default=None,
+        help=(
+            "Write the graph as PDB after the "
+            "RepairGraph step. The resulting file may "
+            'contain "nan" coordinates making it '
+            "unreadable by most softwares."
+        ),
+    )
+    debug_group.add_argument(
+        "-write-canon",
+        type=Path,
+        default=None,
+        help=(
+            "Write the graph as PDB after the "
+            "CanonicalizeModifications step. The "
+            'resulting file may contain "nan" '
+            "coordinates making it unreadable by most "
+            "software."
+        ),
+    )
+    debug_group.add_argument(
+        "-v",
+        dest="verbosity",
+        action="count",
+        help="Enable debug logging output. Can be given " "multiple times.",
+        default=0,
+    )
+    debug_group.add_argument(
+        "-maxwarn",
+        dest="maxwarn",
+        type=maxwarn,
+        action="append",
+        nargs="+",
+        default=[],
+        help="The maximum number of allowed warnings. If "
+        "more warnings are encountered no output files are"
+        " written.",
+    )
 
     args = parser.parse_args()
 
     loglevels = {0: logging.INFO, 1: logging.DEBUG, 2: 5}
     LOGGER.setLevel(loglevels[args.verbosity])
 
     known_force_fields = vermouth.forcefield.find_force_fields(
-        Path(DATA_PATH) / 'force_fields'
+        Path(DATA_PATH) / "force_fields"
+    )
+    known_mappings = read_mapping_directory(
+        Path(DATA_PATH) / "mappings", known_force_fields
     )
-    known_mappings = read_mapping_directory(Path(DATA_PATH) / 'mappings',
-                                            known_force_fields)
 
     # Add user force fields and mappings
     for directory in args.extra_ff_dir:
         try:
             vermouth.forcefield.find_force_fields(directory, known_force_fields)
         except FileNotFoundError:
             msg = '"{}" given to the -ff-dir option should be a directory.'
             raise ValueError(msg.format(directory))
     for directory in args.extra_map_dir:
         try:
-            partial_mapping = read_mapping_directory(directory,
-                                                     known_force_fields)
+            partial_mapping = read_mapping_directory(directory, known_force_fields)
         except NotADirectoryError:
             msg = '"{}" given to the -map-dir option should be a directory.'
             raise ValueError(msg.format(directory))
         combine_mappings(known_mappings, partial_mapping)
 
     if args.list_ff:
-        print('The following force fields are known:')
+        print("The following force fields are known:")
         for idx, ff_name in enumerate(reversed(list(known_force_fields)), 1):
-            print('{:3d}. {}'.format(idx, ff_name))
+            print("{:3d}. {}".format(idx, ff_name))
         parser.exit()
 
     # Build self mappings
     partial_mapping = generate_all_self_mappings(known_force_fields.values())
     combine_mappings(known_mappings, partial_mapping)
 
     from_ff = args.from_ff
     if args.to_ff not in known_force_fields:
         raise ValueError('Unknown force field "{}".'.format(args.to_ff))
     if args.from_ff not in known_force_fields:
         raise ValueError('Unknown force field "{}".'.format(args.from_ff))
-    #if from_ff not in known_mappings or args.to_ff not in known_mappings[from_ff]:
+    # if from_ff not in known_mappings or args.to_ff not in known_mappings[from_ff]:
     #    raise ValueError('No mapping known to go from "{}" to "{}".'
     #                     .format(from_ff, args.to_ff))
 
     if args.list_blocks:
-        print('The following Blocks are known to force field {}:'.format(args.from_ff))
-        print(', '.join(known_force_fields[args.from_ff].blocks))
-        print('The following Modifications are known to force field {}:'.format(args.from_ff))
-        print(', '.join(known_force_fields[args.from_ff].modifications))
+        print("The following Blocks are known to force field {}:".format(args.from_ff))
+        print(", ".join(known_force_fields[args.from_ff].blocks))
+        print(
+            "The following Modifications are known to force field {}:".format(
+                args.from_ff
+            )
+        )
+        print(", ".join(known_force_fields[args.from_ff].modifications))
         print()
-        print('The following Blocks are known to force field {}:'.format(args.to_ff))
-        print(', '.join(known_force_fields[args.to_ff].blocks))
-        print('The following Modifications are known to force field {}:'.format(args.to_ff))
-        print(', '.join(known_force_fields[args.to_ff].modifications))
+        print("The following Blocks are known to force field {}:".format(args.to_ff))
+        print(", ".join(known_force_fields[args.to_ff].blocks))
+        print(
+            "The following Modifications are known to force field {}:".format(
+                args.to_ff
+            )
+        )
+        print(", ".join(known_force_fields[args.to_ff].modifications))
         parser.exit()
 
     if args.elastic and args.govs_includes:
-        parser.error('A rubber band elastic network and GoMartini are not '
-                     'compatible. The -elastic and -govs-include flags cannot '
-                     'be used together.')
+        parser.error(
+            "A rubber band elastic network and GoMartini are not "
+            "compatible. The -elastic and -govs-include flags cannot "
+            "be used together."
+        )
 
-    if args.to_ff.startswith('elnedyn'):
+    if args.to_ff.startswith("elnedyn"):
         # FIXME: This type of thing should be added to the FF itself.
-        LOGGER.info('The forcefield {} must always be used with an elastic '
-                    'network. Enabling it now.', args.to_ff)
+        LOGGER.info(
+            "The forcefield {} must always be used with an elastic "
+            "network. Enabling it now.",
+            args.to_ff,
+        )
         args.elastic = True
 
     file_extension = args.inpath.suffix.upper()[1:]  # We do not keep the dot
-    if file_extension in ['GRO'] and args.modelidx is not None:
+    if file_extension in ["GRO"] and args.modelidx is not None:
         parser.error("GRO files don't know the concept of models.")
     if args.modelidx is None:
         # Set a sane default value. Can't do this using argparse machinery,
         # since we need to be able to check whether the flag was given.
         args.modelidx = 1
 
-    bonds_from_name = args.bonds_from in ('name', 'both')
-    bonds_from_dist = args.bonds_from in ('distance', 'both')
-
+    bonds_from_name = args.bonds_from in ("name", "both")
+    bonds_from_dist = args.bonds_from in ("distance", "both")
 
     # args.ignore_res is a pretty deep list: given "-ignore HOH CU,LIG -ignore LIG2"
     # it'll contain [[['HOH'], ['CU', 'LIG']], [['LIG2']]]
     ignore_res = set()
     for grp in args.ignore_res:
         ignore_res.update(*grp)
 
     if args.neutral_termini:
-        args.modifications.append(['cter', 'COOH-ter'])
-        args.modifications.append(['nter', 'NH2-ter'])
+        args.modifications.append(["cter", "COOH-ter"])
+        args.modifications.append(["nter", "NH2-ter"])
     else:
         if args.modifications:
             resspecs, mods = zip(*args.modifications)
         else:
             resspecs, mods = [], []
-        if not any('cter' in resspec for resspec in resspecs):
-            args.modifications.append(['cter', 'C-ter'])
-        if not any('nter' in resspec for resspec in resspecs):
-            args.modifications.append(['nter', 'N-ter'])
+        if not any("cter" in resspec for resspec in resspecs):
+            args.modifications.append(["cter", "C-ter"])
+        if not any("nter" in resspec for resspec in resspecs):
+            args.modifications.append(["nter", "N-ter"])
 
     # Reading the input structure.
     # So far, we assume we only go from atomistic to martini. We want the
     # input structure to be a clean universal system.
     # For now at least, we silently delete molecules with unknown blocks.
-    system = read_system(args.inpath, ignore_resnames=ignore_res,
-                         ignh=args.ignore_h, modelidx=args.modelidx)
+    system = read_system(
+        args.inpath,
+        ignore_resnames=ignore_res,
+        ignh=args.ignore_h,
+        modelidx=args.modelidx,
+    )
     system = pdb_to_universal(
         system,
         delete_unknown=True,
         force_field=known_force_fields[from_ff],
         bonds_from_name=bonds_from_name,
         bonds_from_dist=bonds_from_dist,
         bonds_fudge=args.bonds_fudge,
         modifications=args.modifications,
         mutations=args.mutations,
         write_graph=args.write_graph,
         write_repair=args.write_repair,
         write_canon=args.write_canon,
     )
 
-    LOGGER.info('Read input.', type='step')
+    LOGGER.info("Read input.", type="step")
     for molecule in system.molecules:
-        LOGGER.debug("Read molecule {}.", molecule, type='step')
+        LOGGER.debug("Read molecule {}.", molecule, type="step")
 
     target_ff = known_force_fields[args.to_ff]
     if args.dssp is not None:
-        AnnotateDSSP(executable=args.dssp, savedir='.').run_system(system)
+        AnnotateDSSP(executable=args.dssp, savedir=".").run_system(system)
         AnnotateMartiniSecondaryStructures().run_system(system)
     elif args.ss is not None:
-        AnnotateResidues(attribute='secstruct', sequence=args.ss,
-                         molecule_selector=selectors.is_protein).run_system(system)
+        AnnotateResidues(
+            attribute="secstruct",
+            sequence=args.ss,
+            molecule_selector=selectors.is_protein,
+        ).run_system(system)
         AnnotateMartiniSecondaryStructures().run_system(system)
     elif args.collagen:
-        if not target_ff.has_feature('collagen'):
-            LOGGER.warning('The force field "{}" does not have specific '
-                           'parameters for collagen (-collagen).',
-                           target_ff.name, type='missing-feature')
-        AnnotateResidues(attribute='cgsecstruct', sequence='F',
-                         molecule_selector=selectors.is_protein).run_system(system)
-    if args.extdih and not target_ff.has_feature('extdih'):
-        LOGGER.warning('The force field "{}" does not define dihedral '
-                       'angles for extended regions of proteins (-extdih).',
-                       target_ff.name, type='missing-feature')
+        if not target_ff.has_feature("collagen"):
+            LOGGER.warning(
+                'The force field "{}" does not have specific '
+                "parameters for collagen (-collagen).",
+                target_ff.name,
+                type="missing-feature",
+            )
+        AnnotateResidues(
+            attribute="cgsecstruct",
+            sequence="F",
+            molecule_selector=selectors.is_protein,
+        ).run_system(system)
+    if args.extdih and not target_ff.has_feature("extdih"):
+        LOGGER.warning(
+            'The force field "{}" does not define dihedral '
+            "angles for extended regions of proteins (-extdih).",
+            target_ff.name,
+            type="missing-feature",
+        )
     vermouth.SetMoleculeMeta(extdih=args.extdih).run_system(system)
-    if args.scfix and not target_ff.has_feature('scfix'):
-        LOGGER.warning('The force field "{}" does not define angle and '
-                       'torsion for the side chain corrections (-scfix).',
-                       target_ff.name, type='missing-feature')
+    if args.scfix and not target_ff.has_feature("scfix"):
+        LOGGER.warning(
+            'The force field "{}" does not define angle and '
+            "torsion for the side chain corrections (-scfix).",
+            target_ff.name,
+            type="missing-feature",
+        )
     vermouth.SetMoleculeMeta(scfix=args.scfix).run_system(system)
 
-    ss_sequence = list(itertools.chain(*(
-        dssp.sequence_from_residues(molecule, 'secstruct')
-        for molecule in system.molecules
-        if selectors.is_protein(molecule)
-    )))
+    ss_sequence = list(
+        itertools.chain(
+            *(
+                dssp.sequence_from_residues(molecule, "secstruct")
+                for molecule in system.molecules
+                if selectors.is_protein(molecule)
+            )
+        )
+    )
 
-    if args.cystein_bridge == 'none':
+    if args.cystein_bridge == "none":
         vermouth.RemoveCysteinBridgeEdges().run_system(system)
-    elif args.cystein_bridge != 'auto':
+    elif args.cystein_bridge != "auto":
         vermouth.AddCysteinBridgesThreshold(args.cystein_bridge).run_system(system)
 
     # Run martinize on the system.
     system = martinize(
         system,
         mappings=known_mappings,
         to_ff=known_force_fields[args.to_ff],
         delete_unknown=True,
     )
 
     # Apply position restraints if required.
-    if args.posres != 'none':
-        LOGGER.info('Applying position restraints.', type='step')
-        node_selectors = {'all': selectors.select_all,
-                          'backbone': selectors.select_backbone}
+    if args.posres != "none":
+        LOGGER.info("Applying position restraints.", type="step")
+        node_selectors = {
+            "all": selectors.select_all,
+            "backbone": selectors.select_backbone,
+        }
         node_selector = node_selectors[args.posres]
         vermouth.ApplyPosres(node_selector, args.posres_fc).run_system(system)
 
     if args.govs_includes:
         # The way Virtual Site GoMartini works has to be in sync with
         # Sebastian's create_goVirt.py script, until the method is fully
         # implemented in vermouth. One call of martinize2 must create a single
         # molecule, regardless of the number of fragments in the input.
         # The molecule type name is provided as an input with the -govs-moltype
         # flag to be consistent with the name provided to Sebastian's script.
         # The name cannot be guessed because a system may need to be composed
         # from multiple calls to martinize2 and create_goVirt.py.
-        LOGGER.info('Adding includes for Virtual Site Go Martini.', type='step')
-        LOGGER.info('The output topology will require files generated by '
-                    '"create_goVirt.py".')
+        LOGGER.info("Adding includes for Virtual Site Go Martini.", type="step")
+        LOGGER.info(
+            "The output topology will require files generated by " '"create_goVirt.py".'
+        )
         vermouth.MergeAllMolecules().run_system(system)
         vermouth.SetMoleculeMeta(moltype=args.govs_moltype).run_system(system)
         vermouth.GoVirtIncludes().run_system(system)
-        defines = ('GO_VIRT',)
+        defines = ("GO_VIRT",)
     else:
         # Merge chains if required.
         if args.merge_chains:
             for chain_set in args.merge_chains:
                 vermouth.MergeChains(chain_set).run_system(system)
         vermouth.NameMolType(deduplicate=not args.keep_duplicate_itp).run_system(system)
         defines = ()
 
     # Apply a rubber band elastic network is required.
     if args.elastic:
-        LOGGER.info('Setting the rubber bands.', type='step')
-        if args.rb_unit == 'molecule':
+        LOGGER.info("Setting the rubber bands.", type="step")
+        if args.rb_unit == "molecule":
             domain_criterion = vermouth.processors.apply_rubber_band.always_true
-        elif args.rb_unit == 'all':
+        elif args.rb_unit == "all":
             vermouth.MergeAllMolecules().run_system(system)
             domain_criterion = vermouth.processors.apply_rubber_band.always_true
-        elif args.rb_unit == 'chain':
+        elif args.rb_unit == "chain":
             domain_criterion = vermouth.processors.apply_rubber_band.same_chain
         else:
-            regions = [tuple([int(i) for i in apair.split(':')]) for apair in args.rb_unit.split(',')]
+            regions = [
+                tuple([int(i) for i in apair.split(":")])
+                for apair in args.rb_unit.split(",")
+            ]
             if any(len(region) != 2 for region in regions):
-                message = 'Faulty resid interval for elastic network unit: "{}".'.format(args.rb_unit)
+                message = (
+                    'Faulty resid interval for elastic network unit: "{}".'.format(
+                        args.rb_unit
+                    )
+                )
                 LOGGER.critical(message)
                 raise ValueError(message)
             else:
-                domain_criterion = vermouth.processors.apply_rubber_band.make_same_region_criterion(regions)
+                domain_criterion = (
+                    vermouth.processors.apply_rubber_band.make_same_region_criterion(
+                        regions
+                    )
+                )
 
         if args.rb_selection is not None:
             selector = functools.partial(
                 selectors.proto_select_attribute_in,
-                attribute='atomname',
+                attribute="atomname",
                 values=args.rb_selection,
             )
         else:
             selector = selectors.select_backbone
         rubber_band_processor = vermouth.ApplyRubberBand(
             lower_bound=args.rb_lower_bound,
             upper_bound=args.rb_upper_bound,
@@ -759,60 +1041,70 @@
 
     # Here we need to add the resids from the PDB back if that is needed
     if args.resid_handling == "input":
         for molecule in system.molecules:
             old_resids = nx.get_node_attributes(molecule, "_old_resid")
             nx.set_node_attributes(molecule, old_resids, "resid")
 
-    LOGGER.info('Writing output.', type='step')
+    # The Martini Go model assumes that we do not mess with the order of
+    # particles in any way especially the virtual sites needed for the Go
+    # model, thus we skip the sorting here altogether.
+    if not args.govs_includes:
+        LOGGER.info("Sorting atomids", type="step")
+        vermouth.SortMoleculeAtoms().run_system(system)
+
+    LOGGER.info("Writing output.", type="step")
     for molecule in system.molecules:
-        LOGGER.debug("Writing molecule {}.", molecule, type='step')
+        LOGGER.debug("Writing molecule {}.", molecule, type="step")
         for loglevel, entries in molecule.log_entries.items():
             for entry, fmt_args in entries.items():
                 for fmt_arg in fmt_args:
                     fmt_arg = {str(k): molecule.nodes[v] for k, v in fmt_arg.items()}
-                    LOGGER.log(loglevel, entry, **fmt_arg, type='model')
+                    LOGGER.log(loglevel, entry, **fmt_arg, type="model")
 
     # Write the topology if requested
     # grompp has a limit in the number of character it can read per line
     # (due to the size limit of a buffer somewhere in its implementation).
     # The command line can be longer than this limit and therefore
     # prevent grompp from reading the topology.
     gromacs_char_limit = 4000  # the limit is actually 4095, but I play safe
-    command = ' '.join(sys.argv)
+    command = " ".join(sys.argv)
     if len(command) > gromacs_char_limit:
-        command = command[:gromacs_char_limit] + ' ...'
+        command = command[:gromacs_char_limit] + " ..."
     header = [
-        'This file was generated using the following command:',
+        "This file was generated using the following command:",
         command,
         VERSION,
     ]
     if None not in ss_sequence:
         header += [
-            'The following sequence of secondary structure ',
-            'was used for the full system:',
-            ''.join(ss_sequence),
+            "The following sequence of secondary structure ",
+            "was used for the full system:",
+            "".join(ss_sequence),
         ]
 
     if args.top_path is not None:
         write_gmx_topology(system, args.top_path, defines=defines, header=header)
 
     # Write a PDB file.
     vermouth.pdb.write_pdb(system, str(args.outpath), omit_charges=True)
 
     # TODO: allow ignoring warnings per class/amount (i.e. ignore 2
     #       inconsistent-data warnings)
 
     leftover_warnings = ignore_warnings_and_count(COUNTER, args.maxwarn)
     if leftover_warnings:
-        LOGGER.error('{} warnings were encountered after accounting for the '
-                     '-maxwarn flag. No output files will be '
-                     'written. Consider fixing the warnings, or if you are sure'
-                     ' they are harmless, use the -maxwarn flag.', leftover_warnings)
+        LOGGER.error(
+            "{} warnings were encountered after accounting for the "
+            "-maxwarn flag. No output files will be "
+            "written. Consider fixing the warnings, or if you are sure"
+            " they are harmless, use the -maxwarn flag.",
+            leftover_warnings,
+        )
         sys.exit(2)
     else:
         DeferredFileWriter().write()
         vermouth.Quoter().run_system(system)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     entry()
```

### Comparing `vermouth-0.9.1/bin/run_martinize2.py` & `vermouth-0.9.3/bin/run_martinize2.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/doc/Makefile` & `vermouth-0.9.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/doc/source/conf.py` & `vermouth-0.9.3/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/doc/source/data.rst` & `vermouth-0.9.3/doc/source/data.rst`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/doc/source/file_formats.rst` & `vermouth-0.9.3/doc/source/file_formats.rst`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/doc/source/general_overview.rst` & `vermouth-0.9.3/doc/source/general_overview.rst`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/doc/source/graph_algorithms.rst` & `vermouth-0.9.3/doc/source/graph_algorithms.rst`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/doc/source/index.rst` & `vermouth-0.9.3/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/doc/source/martinize2_workflow.rst` & `vermouth-0.9.3/doc/source/martinize2_workflow.rst`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/maintainers/head_template_data` & `vermouth-0.9.3/maintainers/head_template_data`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/maintainers/head_template_py` & `vermouth-0.9.3/maintainers/head_template_py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/maintainers/releasing.md` & `vermouth-0.9.3/maintainers/releasing.md`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/maintainers/vim/syntax/ff.vim` & `vermouth-0.9.3/maintainers/vim/syntax/ff.vim`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/setup.cfg` & `vermouth-0.9.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/setup.py` & `vermouth-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/__init__.py` & `vermouth-0.9.3/vermouth/__init__.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/citation_parser.py` & `vermouth-0.9.3/vermouth/citation_parser.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/amber/aminoacids.rtp` & `vermouth-0.9.3/vermouth/data/force_fields/amber/aminoacids.rtp`

 * *Files 1% similar despite different names*

```diff
@@ -510,45 +510,36 @@
    HB1    HC           0.054608    6
    HB2    HC           0.054608    7
     CG    CC           0.278406    8
    ND1    NB          -0.423316    9
    CE1    CR           0.025960   10
    HE1    H5           0.126832   11
    NE2    NA          -0.097984   12
-   HE2    H            0.266865   13
-   CD2    CW          -0.297563   14
-   HD2    H4           0.160413   15
-     C    C            0.662405   16
-     O    O           -0.528966   17
+   CD2    CW          -0.297563   13
+   HD2    H4           0.160413   14
+     C    C            0.662405   15
+     O    O           -0.528966   16
  [ bonds ]
      N     H
      N    CA
     CA    HA
     CA    CB
     CA     C
     CB   HB2
     CB   HB1
     CB    CG
     CG   ND1
     CG   CD2
    ND1   CE1
    CE1   HE1
    CE1   NE2
-   NE2   HE2
    NE2   CD2
    CD2   HD2
      C     O
     -C     N
- [ impropers ]
-    -C    CA     N     H
-    CA    +N     C     O
-   CE1   CD2   NE2   HE2
-    CG   NE2   CD2   HD2
-   ND1   NE2   CE1   HE1
-   ND1   CD2    CG    CB
 
 [ HIP ]
  [ atoms ]
      N    N           -0.424967    1
      H    H            0.285872    2
     CA    CT           0.375022    3
     HA    H1          -0.014621    4
```

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/amber/modifications.ff` & `vermouth-0.9.3/vermouth/data/force_fields/amber/modifications.ff`

 * *Files 26% similar despite different names*

```diff
@@ -42,32 +42,100 @@
 CA {"element": "C"}
 N {"element": "N"}
 HN2 {"element": "H", "PTM_atom": true, "replace": {"atomname": "HN2"}}
 [ edges ]
 N CA
 N HN2
 
+; ;;;;;;;;;;;;;;;;;;;;;;;;;
+;  GLU/ASP MODIFICATIONS
+; ;;;;;;;;;;;;;;;;;;;;;;;;;
+
 [ modification ]
-GLU-H
+GLU-HE1
 [ atoms ]
-CD {"element": "C"}
 OE1 {"element": "O"}
-OE2 {"element": "O"}
 HE1 {"element": "H", "PTM_atom": true}
 [ edges ]
-CD OE1
-CD OE2
 OE1 HE1
 
 [ modification ]
-HIS_PROT
+GLU-HE2
+[ atoms ]
+OE2 {"element": "O"}
+HE2 {"element": "H", "PTM_atom": true}
+[ edges ]
+OE2 HE2
+
+[ modification ]
+ASP-HD2
+[ atoms ]
+HD2 {"resname": "ASP", "element": "H", "PTM_atom": true}
+OD2 {"resname": "ASP"}
+[ edges ]
+OD2 HD2
+
+[ modification ]
+ASP-HD1
+[ atoms ]
+HD1 {"resname": "ASP", "element": "H", "PTM_atom": true}
+OD1 {"resname": "ASP"}
+[ edges ]
+OD1 HD1
+
+; ;;;;;;;;;;;;;;;;;;;;;;;;;
+;  LYS MODIFICATIONS
+; ;;;;;;;;;;;;;;;;;;;;;;;;;
+
+[ modification ]
+LYS-LSN
+[ atoms ]
+NZ  {"resname": "LYS", "element": "N"}
+HZ1 {"resname": "LYS", "element": "H"}
+HZ2 {"resname": "LYS", "element": "H"}
+HZ3 {"resnmae": "LYS", "element": "H", "PTM_atom": true, "replace": {"atomname": null}}
+[ edges ]
+NZ HZ1
+NZ HZ2
+NZ HZ3
+
+; ;;;;;;;;;;;;;;;;;;;;;;;;;
+;  HIS MODIFICATIONS
+; ;;;;;;;;;;;;;;;;;;;;;;;;;
+
+[ modification ]
+HIS-HP
 [ atoms ]
 NE2 {"resname": "HIS", "element": "N"}
-HE2 {"resname": "HIS", "element": "H"}
 ND1 {"resname": "HIS", "element": "N"}
 HD1 {"resname": "HIS", "element": "H", "PTM_atom": true}
+HE2 {"resname": "HIS", "element": "H", "PTM_atom": true}
 CE1 {"resname": "HIS", "element": "C"}
 [ edges ]
 NE2 HE2
 ND1 HD1
 CE1 NE2
 CE1 ND1
+
+[ modification ]
+HIS-HD
+[ atoms ]
+NE2 {"resname": "HIS", "element": "N"}
+ND1 {"resname": "HIS", "element": "N"}
+HD1 {"resname": "HIS", "element": "H", "PTM_atom": true}
+CE1 {"resname": "HIS", "element": "C"}
+[ edges ]
+ND1 HD1
+CE1 NE2
+CE1 ND1
+
+[ modification ]
+HIS-HE
+[ atoms ]
+NE2 {"resname": "HIS", "element": "N"}
+HE2 {"resname": "HIS", "element": "H", "PTM_atom": true}
+ND1 {"resname": "HIS", "element": "N"}
+CE1 {"resname": "HIS", "element": "C"}
+[ edges ]
+NE2 HE2
+CE1 NE2
+CE1 ND1
```

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/charmm/aminoacids.rtp` & `vermouth-0.9.3/vermouth/data/force_fields/charmm/aminoacids.rtp`

 * *Files 0% similar despite different names*

```diff
@@ -755,17 +755,14 @@
 	CD	CT2	-0.18	10
 	HD1	HA	0.09	11
 	HD2	HA	0.09	12
 	CE	CT2	0.21	13
 	HE1	HA	0.05	14
 	HE2	HA	0.05	15
 	NZ	NH3	-0.30	16
-	HZ1	HC	0.33	17
-	HZ2	HC	0.33	18
-	HZ3	HC	0.33	19
 	C	C	0.51	20
 	O	O	-0.51	21
  [ bonds ]
 	CB	CA
 	CG	CB
 	CD	CG
 	CE	CD
@@ -780,17 +777,14 @@
 	CG	HG1
 	CG	HG2
 	CD	HD1
 	CD	HD2
 	CE	HE1
 	CE	HE2
 	O	C
-	NZ	HZ1
-	NZ	HZ2
-	NZ	HZ3
  [ impropers ]
 	N	-C	CA	HN
 	C	CA	+N	O
  [ cmap ]
 	-C	N	CA	C	+N
 
 [ LSN ] ; neutral lysine residue
```

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/charmm/small_molecule_charmm.ff` & `vermouth-0.9.3/vermouth/data/force_fields/charmm/small_molecule_charmm.ff`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/elnedyn21/aminoacids.ff` & `vermouth-0.9.3/vermouth/data/force_fields/elnedyn21/aminoacids.ff`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/elnedyn21/citations.bib` & `vermouth-0.9.3/vermouth/data/force_fields/elnedyn21/citations.bib`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/elnedyn21/general.ff` & `vermouth-0.9.3/vermouth/data/force_fields/elnedyn21/general.ff`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/elnedyn22/aminoacids.ff` & `vermouth-0.9.3/vermouth/data/force_fields/elnedyn22/aminoacids.ff`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/elnedyn22/citations.bib` & `vermouth-0.9.3/vermouth/data/force_fields/elnedyn22/citations.bib`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/elnedyn22/general.ff` & `vermouth-0.9.3/vermouth/data/force_fields/elnedyn22/general.ff`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/elnedyn22p/aminoacids.ff` & `vermouth-0.9.3/vermouth/data/force_fields/elnedyn22p/aminoacids.ff`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/elnedyn22p/citations.bib` & `vermouth-0.9.3/vermouth/data/force_fields/elnedyn22p/citations.bib`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/elnedyn22p/general.ff` & `vermouth-0.9.3/vermouth/data/force_fields/elnedyn22p/general.ff`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/gromos/aminoacids.rtp` & `vermouth-0.9.3/vermouth/data/force_fields/gromos/aminoacids.rtp`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/gromos/cofactors.ff` & `vermouth-0.9.3/vermouth/data/force_fields/gromos/cofactors.ff`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/martini22/aminoacids.ff` & `vermouth-0.9.3/vermouth/data/force_fields/martini22/aminoacids.ff`

 * *Files 0% similar despite different names*

```diff
@@ -305,21 +305,21 @@
     1     2    3       2   180.000    25.0      
 
 
 ;;; LYSINE - NEUTRAL FORM
 
 [ moleculetype ]
 ; molname       nrexcl
-LYS0               1
+LSN               1
 
 [ atoms ]
 ;id type resnr residu atom cgnr   charge
- 1   P5    1     LYS     BB     1      0    
- 2   C3    1     LYS     SC1    2      0    
- 3   P1    1     LYS     SC2    3      0    
+ 1   P5    1     LSN     BB     1      0    
+ 2   C3    1     LSN     SC1    2      0    
+ 3   P1    1     LSN     SC2    3      0    
 
 [bonds]
 #meta {"group": "Side chain bonds"}
 ;  i     j   funct   length  force.c.
    1     2    1       0.33     5000      
    2     3    1       0.28     5000
```

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/martini22/citations.bib` & `vermouth-0.9.3/vermouth/data/force_fields/martini22/citations.bib`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/martini22/general.ff` & `vermouth-0.9.3/vermouth/data/force_fields/martini22/general.ff`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/martini22/modifications.ff` & `vermouth-0.9.3/vermouth/data/force_fields/elnedyn21/modifications.ff`

 * *Files 16% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 [ modification ]
 NH2-ter
 [ atoms ]
 BB {"replace": {"atype": "P5", "charge": 0}}
 
 [ modification ]
-TYRPHOS
+LYS-LSN
 [ atoms ]
-SC3 {"replace": {"atype": "SNda"}}
-PO4 {"atype": "Qa", "charge": "-1", "PTM_atom": true}
-[ bonds ]
-SC3 PO4 1 0.47 1250 {"comment": "phospho"}
-[ edges ]
-SC3 PO4
+SC2 {"resname": "LYS", "replace": {"atype": "P1", "charge": 0}}
+
+[ modification ]
+LYS-HZ3
+[ atoms ]
+SC2 {"replace": {"resname": "LYS"}}
```

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/martini22/nucleotides.ff` & `vermouth-0.9.3/vermouth/data/force_fields/martini22/nucleotides.ff`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/martini22p/aminoacids.ff` & `vermouth-0.9.3/vermouth/data/force_fields/martini22p/aminoacids.ff`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/martini22p/citations.bib` & `vermouth-0.9.3/vermouth/data/force_fields/martini22p/citations.bib`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/martini22p/general.ff` & `vermouth-0.9.3/vermouth/data/force_fields/martini22p/general.ff`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/martini3001/aminoacids.ff` & `vermouth-0.9.3/vermouth/data/force_fields/martini3001/aminoacids.ff`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/martini3001/citations.bib` & `vermouth-0.9.3/vermouth/data/force_fields/martini3001/citations.bib`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/martini3001/general.ff` & `vermouth-0.9.3/vermouth/data/force_fields/martini3001/general.ff`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/martini3001/modifications.ff` & `vermouth-0.9.3/vermouth/data/force_fields/martini3001/modifications.ff`

 * *Files 22% similar despite different names*

```diff
@@ -33,18 +33,74 @@
 
 [ modification ]
 NCAP-ter
 [ atoms ]
 BB {"replace": {"atype": "P2", "charge": 0}}
 
 [ modification ]
-HIS_PROT
+GLU-HE1
 [ atoms ]
-BB  {"resname": "HIS", "replace": {"resname": "HIP"}}
-SC1 {"resname": "HIS", "replace": {"resname": "HIP"}}
-SC2 {"resname": "HIS", "replace": {"atype": "TP1dq", "charge": "0.5", "resname": "HIP"}}
-SC3 {"resname": "HIS", "replace": {"atype": "TP1dq", "charge": "0.5", "resname": "HIP"}}
+SC1 {"replace": {"atype": "P2", "charge": 0}}
+
+[ modification ]
+GLU-HE2
+[ atoms ]
+SC1 {"replace": {"atype": "P2", "charge": 0}}
+
+[ modification ]
+ASP-HD1
+[ atoms ]
+SC1 {"replace": {"atype": "P2", "charge": 0}}
+
+[ modification ]
+ASP-HD2
+[ atoms ]
+SC1 {"replace": {"atype": "P2", "charge": 0}}
+
+[ modification ]
+LYS-LSN
+[ atoms ]
+SC2 {"resname": "LYS", "replace": {"atype": "SN6d", "charge": 0}}
+
+[ modification ]
+LYS-HZ3
+[ atoms ]
+SC2 {"replace": {"resname": "LYS"}}
+
+[ modification ]
+HIS-HP
+[ atoms ]
+BB  {"resname": "HIS", "replace": {"resname": "HIS"}}
+SC1 {"resname": "HIS", "replace": {"resname": "HIS"}}
+SC2 {"resname": "HIS", "replace": {"atype": "TP1dq", "charge": "0.5", "resname": "HIS"}}
+SC3 {"resname": "HIS", "replace": {"atype": "TP1dq", "charge": "0.5", "resname": "HIS"}}
+[ edges ]
+BB SC1 
+SC1 SC2
+SC1 SC3
+SC2 SC3
+
+[ modification ]
+HIS-HE
+[ atoms ]
+BB  {"resname": "HIS", "replace": {"resname": "HIS"}}
+SC1 {"resname": "HIS", "replace": {"resname": "HIS"}}
+SC2 {"resname": "HIS", "replace": {"resname": "HIS"}}
+SC3 {"resname": "HIS", "replace": {"resname": "HIS"}}
+[ edges ]
+BB SC1 
+SC1 SC2
+SC1 SC3
+SC2 SC3
+
+[ modification ]
+HIS-HD
+[ atoms ]
+BB  {"resname": "HIS", "replace": {"resname": "HIS"}}
+SC1 {"resname": "HIS", "replace": {"resname": "HIS"}}
+SC2 {"resname": "HIS", "replace": {"resname": "HIS", "atype": "TN5a"}}
+SC3 {"resname": "HIS", "replace": {"resname": "HIS", "atype": "TN6a"}}
 [ edges ]
 BB SC1 
 SC1 SC2
 SC1 SC3
 SC2 SC3
```

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/martini3001/small_molecule_martini3.ff` & `vermouth-0.9.3/vermouth/data/force_fields/martini3001/small_molecule_martini3.ff`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/martini30b32/aminoacids.ff` & `vermouth-0.9.3/vermouth/data/force_fields/martini30b32/aminoacids.ff`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/force_fields/martini30dev/aminoacids.ff` & `vermouth-0.9.3/vermouth/data/force_fields/martini30dev/aminoacids.ff`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/ala.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/ala.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/arg.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/arg.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/arg.charmm36.martini22p.map` & `vermouth-0.9.3/vermouth/data/mappings/arg.charmm36.martini22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/asn.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/asn.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/asn.charmm36.martini22p.map` & `vermouth-0.9.3/vermouth/data/mappings/asn.charmm36.martini22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/asp.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/asp.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/asp.charmm36.martini22p.map` & `vermouth-0.9.3/vermouth/data/mappings/asp.charmm36.martini22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/chol.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/chol.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/cys.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/cys.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/dmpc.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/dmpc.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/dopc.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/dopc.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/dppc.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/dppc.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/dppg.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/dppg.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/ala.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/ala.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/arg.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/arg.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/asn.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/asn.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/asp.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/asp.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/chol.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/chol.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/cys.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/cys.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/dmpc.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/dmpc.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/dopc.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/dopc.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/dppc.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/dppc.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/dppg.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/dppg.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/elnedyn22p/arg.charmm36.elnedyn22p.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/elnedyn22p/arg.charmm36.elnedyn22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/elnedyn22p/asn.charmm36.elnedyn22p.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/elnedyn22p/asn.charmm36.elnedyn22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/elnedyn22p/asp.charmm36.elnedyn22p.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/elnedyn22p/asp.charmm36.elnedyn22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/elnedyn22p/gln.charmm36.elnedyn22p.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/elnedyn22p/gln.charmm36.elnedyn22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/elnedyn22p/glu.charmm36.elnedyn22p.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/elnedyn22p/glu.charmm36.elnedyn22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/elnedyn22p/lys.charmm36.elnedyn22p.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/elnedyn22p/lys.charmm36.elnedyn22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/elnedyn22p/ser.charmm36.elnedyn22p.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/elnedyn22p/ser.charmm36.elnedyn22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/elnedyn22p/thr.charmm36.elnedyn22p.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/elnedyn22p/thr.charmm36.elnedyn22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/gln.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/gln.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/glu.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/glu.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/gly.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/gly.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/his.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/his.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/ile.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/ile.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/leu.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/leu.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/lys.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/lys.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/met.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/met.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/modifications.elnedyn21.mapping` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/modifications.mapping`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/modifications.elnedyn22.mapping` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/modifications.elnedyn22p.mapping`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [ modification ]
 [ from ]
 charmm
 [ to ]
-elnedyn22
+elnedyn22p
 
 [ from blocks ]
 C-ter
 [ to blocks ]
 C-ter
 
 [ from nodes ]
@@ -24,15 +24,15 @@
 OXT BB 0
 
 
 [modification]
 [ from ]
 charmm
 [ to ]
-elnedyn22
+elnedyn22p
 [ from blocks ]
 N-ter
 [ to blocks ]
 N-ter
 
 [ from nodes ]
 C
@@ -50,15 +50,15 @@
 C   BB 0
 O   BB 0
 
 [ modification ]
 [ from ]
 charmm
 [ to ]
-elnedyn22
+elnedyn22p
 
 [ from blocks ]
 COOH-ter
 [ to blocks ]
 COOH-ter
 
 [ from nodes ]
@@ -79,15 +79,15 @@
 OXT BB 0
 
 
 [modification]
 [ from ]
 charmm
 [ to ]
-elnedyn22
+elnedyn22p
 [ from blocks ]
 NH2-ter
 [ to blocks ]
 NH2-ter
 
 [ from nodes ]
 C
@@ -99,31 +99,7 @@
 
 [ mapping ]
 HN2 BB 0
 N   BB 0
 CA  BB
 C   BB 0
 O   BB 0
-
-[modification]
-[ from ]
-charmm
-[ to ]
-elnedyn22
-[ from blocks ]
-ASP0
-[ to blocks ]
-ASP0
-[ from nodes ]
-CB
-CG
-OD1
-[ from edges ]
-CB CG
-CG OD1
-CG OD2
-[ mapping ]
-CB SC1
-CG SC1
-OD1 SC1
-OD2 SC1
-HD2 SC1
```

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/phe.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/phe.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/popc.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/popc.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/pope.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/pope.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/popg.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/popg.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/pops.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/pops.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/pro.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/pro.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/ser.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/ser.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/thr.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/thr.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/trp.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/trp.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/tyr.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/tyr.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn/val.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/val.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/ala.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/ala.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/arg.charmm36.elnedyn22p.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/arg.charmm36.elnedyn22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/arg.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/arg.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/asn.charmm36.elnedyn22p.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/asn.charmm36.elnedyn22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/asn.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/asn.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/asp.charmm36.elnedyn22p.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/asp.charmm36.elnedyn22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/asp.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/asp.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/cys.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/cys.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/gln.charmm36.elnedyn22p.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/gln.charmm36.elnedyn22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/gln.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/gln.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/glu.charmm36.elnedyn22p.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/glu.charmm36.elnedyn22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/glu.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/glu.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/gly.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/gly.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/his.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/his.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/ile.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/ile.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/leu.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/leu.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/lys.charmm36.elnedyn22p.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/lys.charmm36.elnedyn22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/lys.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/lys.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/met.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/met.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/phe.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/phe.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/pro.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/pro.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/ser.charmm36.elnedyn22p.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/ser.charmm36.elnedyn22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/ser.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/ser.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/thr.charmm36.elnedyn22p.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/thr.charmm36.elnedyn22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/thr.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/thr.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/trp.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/trp.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/tyr.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/tyr.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/elnedyn21/val.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn21/val.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/fmn.gromos.map` & `vermouth-0.9.3/vermouth/data/mappings/fmn.gromos.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/gln.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/gln.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/gln.charmm36.martini22p.map` & `vermouth-0.9.3/vermouth/data/mappings/gln.charmm36.martini22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/glu.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/glu.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/glu.charmm36.martini22p.map` & `vermouth-0.9.3/vermouth/data/mappings/glu.charmm36.martini22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/gly.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/gly.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/his.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/his.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/hsd.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/hsd.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/hse.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/hse.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/hsp.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/hsp.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/ile.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/ile.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/leu.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/leu.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/lys.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/lys.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/lys.charmm36.martini22p.map` & `vermouth-0.9.3/vermouth/data/mappings/lys.charmm36.martini22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/ala.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/ala.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/ala.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/ala.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/arg.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/arg.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/arg.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/arg.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/ash.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/ash.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/asn.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/asn.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/asn.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/asn.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/asp.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/asp.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/asp.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/asp.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/aspp.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/aspp.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/cys.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/cys.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/cys.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/cys.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/glh.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/glh.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/gln.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/gln.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/gln.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/gln.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/glu.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/glu.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/glu.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/glu.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/glup.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/glup.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/gly.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/gly.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/gly.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/gly.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/hid.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/hid.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/hie.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/hie.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/hip.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/hip.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/his.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/his.amber.map`

 * *Files 6% similar despite different names*

```diff
@@ -38,10 +38,9 @@
     8   CD2   SC2
     9   HD2   SC2
    10    CG   SC1
    11   NE2   SC2
    12   HE2   SC2
    13   ND1   SC3
    14   CE1   SC3
-   15   HE1   SC3
-   16     C    BB
-   17     O    BB
+   15     C    BB
+   16     O    BB
```

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/his.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/his.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/hsd.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/hsd.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/hse.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/hse.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/hsp.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/hsp.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/ile.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/ile.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/ile.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/ile.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/leu.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/leu.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/leu.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/leu.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/lsn.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/lsn.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/lyn.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/lyn.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/lys.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/lys.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/lys.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini30b32/lys.charmm36.map`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [ molecule ]
 LYS
 
 [from]
 charmm
 
 [to]
-martini3001
+martini30b32
 
 [ martini ]
 BB SC1 SC2
 
 [ mapping ]
 charmm27 charmm36
```

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/met.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/met.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/met.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/met.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/phe.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/phe.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/phe.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/phe.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/pro.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/pro.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/pro.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/pro.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/ser.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/ser.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/ser.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/ser.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/thr.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/thr.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/thr.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/thr.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/trp.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/trp.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/trp.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/trp.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/tyr.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/tyr.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/tyr.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/tyr.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/val.amber.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/val.amber.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini3001/val.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/val.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini30b32/ala.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini30b32/ala.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini30b32/arg.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini30b32/arg.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini30b32/asn.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini30b32/asn.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini30b32/asp.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini30b32/asp.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini30b32/cys.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini30b32/cys.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini30b32/gln.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini30b32/gln.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini30b32/glu.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini30b32/glu.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini30b32/gly.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini30b32/gly.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini30b32/his.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini30b32/his.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini30b32/hsd.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini30b32/hsd.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini30b32/ile.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini30b32/ile.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini30b32/leu.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini30b32/leu.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini30b32/lys.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini3001/lys.charmm36.map`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [ molecule ]
 LYS
 
 [from]
 charmm
 
 [to]
-martini30b32
+martini3001
 
 [ martini ]
 BB SC1 SC2
 
 [ mapping ]
 charmm27 charmm36
 
@@ -41,19 +41,16 @@
    11    CD   SC1
    12   HD1   !SC1
    13   HD2   !SC1
    14    CE   SC2
    15   HE1   !SC2
    16   HE2   !SC2
    17    NZ   SC2
-   18   HZ1   SC2
-   19   HZ2   SC2
-   20   HZ3   SC2
-   21     C    BB
-   22     O    BB
+   18     C    BB
+   19     O    BB
 
 [ chiral ]
   CB     CA    N    C
   HB1    CA    N    C
   HB2    CA    N    C
 
 [ chiral ]
```

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini30b32/met.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini30b32/met.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini30b32/phe.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini30b32/phe.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini30b32/pro.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini30b32/pro.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini30b32/ser.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini30b32/ser.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini30b32/thr.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini30b32/thr.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini30b32/trp.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini30b32/trp.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini30b32/tyr.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini30b32/tyr.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/martini30b32/val.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/martini30b32/val.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/met.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/met.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/modifications.mapping` & `vermouth-0.9.3/vermouth/data/mappings/elnedyn/modifications.elnedyn22.mapping`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [ modification ]
 [ from ]
 charmm
 [ to ]
-martini22
+elnedyn22
 
 [ from blocks ]
 C-ter
 [ to blocks ]
 C-ter
 
 [ from nodes ]
@@ -15,50 +15,50 @@
 
 [ from edges ]
 HN N
 N CA
 
 [ mapping ]
 CA BB
-C  BB
-O  BB
-OXT BB
+C  BB 0
+O  BB 0
+OXT BB 0
 
 
 [modification]
 [ from ]
 charmm
 [ to ]
-martini22
+elnedyn22
 [ from blocks ]
 N-ter
 [ to blocks ]
 N-ter
 
 [ from nodes ]
 C
 O
 
 [ from edges ]
 C O
 CA C
 
 [ mapping ]
-HN2 BB
-HN3 BB
-N   BB
+HN2 BB 0
+HN3 BB 0
+N   BB 0
 CA  BB
-C   BB
-O   BB
+C   BB 0
+O   BB 0
 
 [ modification ]
 [ from ]
 charmm
 [ to ]
-martini22
+elnedyn22
 
 [ from blocks ]
 COOH-ter
 [ to blocks ]
 COOH-ter
 
 [ from nodes ]
@@ -66,165 +66,149 @@
 HN
 
 [ from edges ]
 HN N
 N CA
 
 [ mapping ]
-HN BB
-N BB
+HN BB 0
+N BB 0
 CA BB
-C  BB
-O  BB
-HO BB
-OXT BB
+C  BB 0
+O  BB 0
+HO BB 0
+OXT BB 0
 
 
 [modification]
 [ from ]
 charmm
 [ to ]
-martini22
+elnedyn22
 [ from blocks ]
 NH2-ter
 [ to blocks ]
 NH2-ter
 
 [ from nodes ]
 C
 O
 
 [ from edges ]
 C O
 CA C
 
 [ mapping ]
-HN2 BB
-N   BB
+HN2 BB 0
+N   BB 0
 CA  BB
-C   BB
-O   BB
+C   BB 0
+O   BB 0
 
-;################
-;# Martini 2.2p #
-;################
 
 [ modification ]
 [ from ]
 charmm
 [ to ]
-martini22p
+elnedyn22
 [ from blocks ]
-C-ter
+ASP-HD2
 [ to blocks ]
-C-ter
+ASP-HD2
 [ from nodes ]
-N
-HN
-[ from edges ]
-HN N
-N CA
-[ mapping ]
-CA BB
-C  BB
-O  BB
-OXT BB
-
-
-[modification]
-[ from ]
-charmm
-[ to ]
-martini22p
-[ from blocks ]
-N-ter
-[ to blocks ]
-N-ter
-[ from nodes ]
-C
-O
-[ from edges ]
-C O
-CA C
-[ mapping ]
-HN2 BB
-HN3 BB
-N   BB
-CA  BB
-C   BB
-O   BB
+    CB
+   HB1
+   HB2
+    CG
+   OD1
+[ from edges ]
+CG CB
+CB HB1
+CB HB2
+CG OD1
+CG OD2
+[ mapping ]
+CG   SC1
+OD1  SC1
+OD2  SC1
+HD2  SC1
+CB   SC1
 
 [ modification ]
 [ from ]
 charmm
 [ to ]
-martini22p
+elnedyn22
 [ from blocks ]
-COOH-ter
+ASP-HD1
 [ to blocks ]
-COOH-ter
+ASP-HD1
 [ from nodes ]
-N
-HN
-[ from edges ]
-HN N
-N CA
-[ mapping ]
-HN BB
-N BB
-CA BB
-C  BB
-O  BB
-HO BB
-OXT BB
+    CB
+   HB1
+   HB2
+    CG
+   OD2
+[ from edges ]
+CG CB
+CB HB1
+CB HB2
+CG OD1
+CG OD2
+[ mapping ]
+CG   SC1
+OD1  SC1
+OD2  SC1
+HD1  SC1
+CB   SC1
 
 
-[modification]
+[ modification ]
 [ from ]
 charmm
 [ to ]
-martini22p
+elnedyn22
 [ from blocks ]
-NH2-ter
+LYS-LSN
 [ to blocks ]
-NH2-ter
+LYS-LSN
 [ from nodes ]
-C
-O
+CE
+HE1
+HE2
 [ from edges ]
-C O
-CA C
-[ mapping ]
-HN2 BB
-N   BB
-CA  BB
-C   BB
-O   BB
+CE NZ
+CE HE1
+CE HE2
+[ mapping ]
+CE  SC2
+HE1 SC2
+HE2 SC2
+NZ  SC2
+HZ1 SC2
+HZ2 SC2
 
 [ modification ]
 [ from ]
 charmm
 [ to ]
-martini22
-
+elnedyn22
 [ from blocks ]
-TYRPHOS
+LYS-HZ3
 [ to blocks ]
-TYRPHOS
-
+LYS-HZ3
 [ from nodes ]
-CE1
+CE
 HE1
+HE2
 [ from edges ]
-CE1	HE1
-CE1	CZ
-[ mapping ]
-P1   PO4
-O3   PO4
-O4   PO4
-O2   PO4
-H2   PO4
-CE1  SC3
-HE1  SC3
-CZ   SC3
-OH   SC3
-HH   SC3
+CE NZ
+CE HE1
+CE HE2
+[ mapping ]
+CE  SC2
+HE1 SC2
+HE2 SC2
+NZ  SC2
+HZ1 SC2
+HZ2 SC2
+HZ3 SC2
```

### Comparing `vermouth-0.9.1/vermouth/data/mappings/nad.gromos.map` & `vermouth-0.9.3/vermouth/data/mappings/nad.gromos.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/phe.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/phe.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/popc.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/popc.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/pope.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/pope.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/popg.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/popg.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/pops.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/pops.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/pro.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/pro.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/ser.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/ser.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/ser.charmm36.martini22p.map` & `vermouth-0.9.3/vermouth/data/mappings/ser.charmm36.martini22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/thr.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/thr.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/thr.charmm36.martini22p.map` & `vermouth-0.9.3/vermouth/data/mappings/thr.charmm36.martini22p.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/tpp.gromos.map` & `vermouth-0.9.3/vermouth/data/mappings/tpp.gromos.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/trp.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/trp.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/trp.gromos.map` & `vermouth-0.9.3/vermouth/data/mappings/trp.gromos.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/tyr.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/tyr.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/tyr.gromos.map` & `vermouth-0.9.3/vermouth/data/mappings/tyr.gromos.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/mappings/val.charmm36.map` & `vermouth-0.9.3/vermouth/data/mappings/val.charmm36.map`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/data/quotes.txt` & `vermouth-0.9.3/vermouth/data/quotes.txt`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/dssp/__init__.py` & `vermouth-0.9.3/vermouth/dssp/__init__.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/dssp/dssp.py` & `vermouth-0.9.3/vermouth/dssp/dssp.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,24 +17,26 @@
 """
 
 import collections
 import logging
 import os
 import subprocess
 import tempfile
+import re
 
 from ..file_writer import deferred_open
 from ..pdb import pdb
 from ..system import System
 from ..processors.processor import Processor
 from ..selectors import is_protein, selector_has_position, filter_minimal, select_all
 from .. import utils
 from ..log_helpers import StyleAdapter, get_logger
 
 LOGGER = StyleAdapter(get_logger(__name__))
+SUPPORTED_DSSP_VERSIONS = ("2.2.1", "3.0.0")
 
 
 class DSSPError(Exception):
     """
     Exception raised if DSSP fails.
     """
 
@@ -139,15 +141,15 @@
             secstructs.append(secondary_structure)
         else:
             raise IOError('Line {} is too short: "{}".'.format(line_num, line))
 
     return secstructs
 
 
-def run_dssp(system, executable='dssp', savefile=None, defer_writing=True, version="3.0.0"):
+def run_dssp(system, executable='dssp', savefile=None, defer_writing=True):
     """
     Run DSSP on a system and return the assigned secondary structures.
 
     Run DSSP using the path (or name in the research PATH) given by
     "executable". Return the secondary structure parsed from the output of the
     program.
 
@@ -168,16 +170,14 @@
     system: System
     executable: str
         Where to find the DSSP executable.
     savefile: None or str or pathlib.Path
         If set to a path, the output of DSSP is written in that file.
     defer_writing: bool
         Whether to use :meth:`~vermouth.file_writer.DeferredFileWriter.write` for writing data
-    version: str
-        Supported versions for running dssp
 
     Returns
     list[str]
         The assigned secondary structures as a list of one-letter codes.
         The secondary structure sequences of all the molecules are combined
         in a single list without delimitation.
 
@@ -190,18 +190,27 @@
 
     See Also
     --------
     read_dssp2
         Parse a DSSP output.
     """
     # check version
-    process = subprocess.run(["dssp", "--version"], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-    version_found = process.stdout.decode('UTF8')
-    if version not in version_found:
-        raise DSSPError('Vermouth currently only supports DSSP version 3.0.0.')
+    process = subprocess.run([executable, "--version"], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    match = re.search('\d+\.\d+\.\d+', process.stdout.decode('UTF8'))
+    version = match[0] if match else None
+    if not version:
+        raise DSSPError('Failed to get DSSP version information.')
+    if not version in SUPPORTED_DSSP_VERSIONS:
+        LOGGER.warning("Vermouth is tested only with DSSP versions {}. "
+                       "The provided DSSP (version {}) may result in inaccurate "
+                       "secondary structure assignments. As alternative you can "
+                       "provide a secondary structure assignment string using "
+                       "the `-ss` option.",
+                       SUPPORTED_DSSP_VERSIONS, version,
+                       type='DSSP-version')
 
     tmpfile_handle, tmpfile_name = tempfile.mkstemp(suffix='.pdb', text=True,
                                                     dir='.', prefix='dssp_in_')
     tmpfile_handle = os.fdopen(tmpfile_handle, mode='w')
     tmpfile_handle.write(pdb.write_pdb_string(system, conect=False))
     tmpfile_handle.close()
```

### Comparing `vermouth-0.9.1/vermouth/edge_tuning.py` & `vermouth-0.9.3/vermouth/edge_tuning.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/ffinput.py` & `vermouth-0.9.3/vermouth/ffinput.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,14 +218,52 @@
         self.current_block.name = name
         self.current_block.nrexcl = int(nrexcl)
 
     @SectionLineParser.section_parser('moleculetype', 'atoms')
     def _block_atoms(self, line, lineno=0):
         tokens = collections.deque(_tokenize(line))
         _parse_block_atom(tokens, self.current_block)
+        
+    @SectionLineParser.section_parser('moleculetype', 'meta')
+    def _parse_block_meta(self, line, lineno=0):
+        """
+        Parse the meta section and update the object current_block with meta information. 
+        Allow the dictionnary value to be None (in case of flag), string, int or float. 
+        
+        Example :
+            [meta]
+            flag1
+            key value
+            key2 value1 0.37 
+        
+            will give :
+                {   
+                    'flag1' : None, 
+                    'key': 'value', 
+                    'key2': ['value1' , '0.37']
+                }
+        
+        Parameters
+        ----------
+        line: str
+        lineno: str
+        """
+        
+        split_line = line.split()
+        key = split_line[0]
+        
+        # depend of the number of value(s) 
+        if len(split_line[1:]) == 0 : 
+            value = None
+        elif len(split_line[1:]) == 1 : 
+            value = split_line[1]
+        else: 
+            value = split_line[1:]
+        
+        self.current_block.meta[key] = value
 
     @SectionLineParser.section_parser('moleculetype', 'edges',
                                       negate=False, context_type='block')
     @SectionLineParser.section_parser('moleculetype', 'non-edges',
                                       negate=True, context_type='block')
     @SectionLineParser.section_parser('link', 'edges',
                                       negate=False, context_type='link')
```

### Comparing `vermouth-0.9.1/vermouth/file_writer.py` & `vermouth-0.9.3/vermouth/file_writer.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/forcefield.py` & `vermouth-0.9.3/vermouth/forcefield.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/geometry.py` & `vermouth-0.9.3/vermouth/geometry.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/gmx/__init__.py` & `vermouth-0.9.3/vermouth/gmx/__init__.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/gmx/gro.py` & `vermouth-0.9.3/vermouth/gmx/gro.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,14 +103,19 @@
 
             if has_vel:
                 vel = (properties.pop('vx'), properties.pop('vy'), properties.pop('vz'))
                 properties['velocity'] = np.array(vel, dtype=float)
 
             molecule.add_node(idx, **properties)
             idx += 1
+        box = np.array(line.strip().split(), dtype=float)
+        # not pretty but the parser is out of touch with the rest of the parsing
+        # infrastructure already
+        molecule.box = box
+
     return molecule
 
 
 def write_gro(system, file_name, precision=7, title='Martinized!', box=(0, 0, 0), defer_writing=True):
     """
     Write `system` to `file_name`, which will be a GRO96 file.
```

### Comparing `vermouth-0.9.1/vermouth/gmx/itp.py` & `vermouth-0.9.3/vermouth/gmx/itp.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,17 @@
     # left as the user responsibility. Make sure residues and charge groups are
     # correctly numbered.
     correspondence = {}
     outfile.write('[ atoms ]\n')
     seen_sections.add('atoms')
     for line in pre_section_lines.get('atoms', []):
         outfile.write(line + '\n')
-    for idx, (original_idx, atom) in enumerate(molecule.atoms, start=1):
+    # for idx, (original_idx, atom) in enumerate(molecule.atoms, start=1):
+    for idx, original_idx in enumerate(molecule.sorted_nodes, start=1):
+        atom = molecule.nodes[original_idx]
         correspondence[original_idx] = idx
         new_atom = copy.copy(atom)
         # The charge and the mass can be blank and read from the [atomtypes]
         # section of the ITP file.
         new_atom['charge'] = new_atom.get('charge', '')
         new_atom['mass'] = new_atom.get('mass', '')
```

### Comparing `vermouth-0.9.1/vermouth/gmx/itp_read.py` & `vermouth-0.9.3/vermouth/gmx/itp_read.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/gmx/rtp.py` & `vermouth-0.9.3/vermouth/gmx/rtp.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/graph_utils.py` & `vermouth-0.9.3/vermouth/graph_utils.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/graphing/grappa.py` & `vermouth-0.9.3/vermouth/graphing/grappa.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/ismags.py` & `vermouth-0.9.3/vermouth/ismags.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/log_helpers.py` & `vermouth-0.9.3/vermouth/log_helpers.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/map_input.py` & `vermouth-0.9.3/vermouth/map_input.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/map_parser.py` & `vermouth-0.9.3/vermouth/map_parser.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/molecule.py` & `vermouth-0.9.3/vermouth/molecule.py`

 * *Files 0% similar despite different names*

```diff
@@ -426,14 +426,18 @@
         """
         # TODO: should just be an alias for nodes. If you need the attributes,
         #       do g.nodes(data=<attr>) or g.nodes(data=True)
         for node in self.nodes():
             node_attr = self.nodes[node]
             yield node, node_attr
 
+    @property
+    def sorted_nodes(self):
+        yield from sorted(self.nodes, key=lambda n_idx: self.nodes[n_idx].get('atomid', np.inf))
+
     def copy(self):
         """
         Creates a copy of the molecule.
 
         Returns
         -------
         Molecule
```

### Comparing `vermouth-0.9.1/vermouth/parser_utils.py` & `vermouth-0.9.3/vermouth/parser_utils.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/pdb/__init__.py` & `vermouth-0.9.3/vermouth/pdb/__init__.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/pdb/pdb.py` & `vermouth-0.9.3/vermouth/pdb/pdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         self.active_molecule = Molecule()
         self.molecules = []
         self._conects = []
         self.exclude = exclude
         self.ignh = ignh
         self.modelidx = modelidx
         self._skipahead = False
+        self.cryst = {}
 
     def dispatch(self, line):
         """
         Returns the appropriate method for parsing `line`. This is determined
         based on the first 6 characters of `line`.
 
         Parameters
@@ -147,15 +148,14 @@
     link   = _skip
     cispep = _skip
 
     # MISCELLANEOUS FEATURES SECTION
     site   = _skip
 
     # CRYSTALLOGRAPHIC AND COORDINATE TRANSFORMATION SECTION
-    cryst1 = _skip
     origx1 = _skip
     origx2 = _skip
     origx3 = _skip
     scale1 = _skip
     scale2 = _skip
     scale3 = _skip
     mtrix1 = _skip
@@ -261,14 +261,45 @@
             return
         idx = max(self.active_molecule) + 1 if self.active_molecule else 0
         self.active_molecule.add_node(idx, **properties)
 
     atom = _atom
     hetatm = _atom
 
+    def cryst1(self, line, lineno=0):
+        """
+        Parse the CRYST1 record. Crystal structure information are stored with
+        the parser object and may be extracted later.
+        """
+        fields = [
+            ('', str, 6),
+            ('a', float, 9),
+            ('b', float, 9),
+            ('c', float, 9),
+            ('alpha', float, 7),
+            ('beta', float, 7),
+            ('gamma', float, 7),
+            ('space_group', str, 11),
+            ('', str, 1),
+            ('z_value', int, 4),
+            ]
+        start = 0
+        field_slices = []
+        for name, type_, width in fields:
+            if name:
+                field_slices.append((name, type_, slice(start, start + width)))
+            start += width
+
+        for name, type_, slice_ in field_slices:
+            value = line[slice_].strip()
+            if value:
+                self.cryst[name] = type_(value)
+            else:
+                LOGGER.warning(f"CRYST1 directive incomplete. Missing entry for {name}.")
+
     def model(self, line, lineno=0):
         """
         Parse a MODEL record. If the model is not the same as :attr:`modelidx`,
         this model will not be parsed.
 
         Parameters
         ----------
@@ -494,25 +525,25 @@
     formatter = TruncFormatter()
 #    format_string = 'ATOM  {: >5.5d} {:4.4s}{:1.1s}{:3.3s} {:1.1s}{:4.4d}{:1.1s}   {:8.3f}{:8.3f}{:8.3f}{:6.2f}{:6.2f}          {:2.2s}{:2.2s}'
     format_string = 'ATOM  {: >5dt} {:4st}{:1st}{:3st} {:1st}{:>4dt}{:1st}   {:8.3ft}{:8.3ft}{:8.3ft}{:6.2ft}{:6.2ft}          {:2st}{:2st}'
 
     nodeidx2atomid = {}
     atomid = 1
     for mol_idx, molecule in enumerate(system.molecules):
-        for node_idx in molecule:
+        for node_idx in molecule.sorted_nodes:
             # Node indices do not have to be unique across molecules. So store
             # them as (mol_idx, node_idx)
             nodeidx2atomid[(mol_idx, node_idx)] = atomid
             node = molecule.nodes[node_idx]
             atomname = get_not_none(node, 'atomname', '')
             altloc = get_not_none(node, 'altloc', '')
             resname = get_not_none(node, 'resname', '')
             chain = get_not_none(node, 'chain', '')
             resid = get_not_none(node, 'resid', 1)
-            insertion_code = get_not_none(node, 'insertioncode', '')
+            insertion_code = get_not_none(node, 'insertion_code', '')
             try:
                 # converting from nm to A
                 x, y, z = node['position'] * 10  # pylint: disable=invalid-name
             except KeyError:
                 if nan_missing_pos:
                     x = y = z = float('nan')  # pylint: disable=invalid-name
                 else:
```

### Comparing `vermouth-0.9.1/vermouth/processors/__init__.py` & `vermouth-0.9.3/vermouth/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/processors/add_molecule_edges.py` & `vermouth-0.9.3/vermouth/processors/add_molecule_edges.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/processors/annotate_mut_mod.py` & `vermouth-0.9.3/vermouth/processors/annotate_mut_mod.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/processors/apply_posres.py` & `vermouth-0.9.3/vermouth/processors/apply_posres.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/processors/apply_rubber_band.py` & `vermouth-0.9.3/vermouth/processors/apply_rubber_band.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/processors/attach_mass.py` & `vermouth-0.9.3/vermouth/processors/attach_mass.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/processors/average_beads.py` & `vermouth-0.9.3/vermouth/processors/average_beads.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/processors/canonicalize_modifications.py` & `vermouth-0.9.3/vermouth/processors/canonicalize_modifications.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/processors/do_links.py` & `vermouth-0.9.3/vermouth/processors/do_links.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/processors/do_mapping.py` & `vermouth-0.9.3/vermouth/processors/do_mapping.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/processors/go_vs_includes.py` & `vermouth-0.9.3/vermouth/processors/go_vs_includes.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,15 @@
     new_charge_group = max(charge_groups) if charge_groups else 0
     for node_id, atom in molecule.nodes(data=True):
         if atom.get('atomname') == backbone:
             new_node_id += 1
             new_charge_group += 1
             virtual_site_nodes.append((new_node_id, {
                 'resid': atom['resid'],
+                '_old_resid': atom['_old_resid'],
                 'resname': atom['resname'],
                 'atype': '{}_{}'.format(prefix, atom['resid']),
                 'charge_group': new_charge_group,
                 'chain': atom['chain'],
                 'position': atom['position'],
                 'atomname': atomname,
                 'charge': charge,
```

### Comparing `vermouth-0.9.1/vermouth/processors/gro_reader.py` & `vermouth-0.9.3/vermouth/processors/gro_reader.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/processors/locate_charge_dummies.py` & `vermouth-0.9.3/vermouth/processors/locate_charge_dummies.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/processors/make_bonds.py` & `vermouth-0.9.3/vermouth/processors/make_bonds.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/processors/merge_all_molecules.py` & `vermouth-0.9.3/vermouth/processors/merge_all_molecules.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/processors/merge_chains.py` & `vermouth-0.9.3/vermouth/processors/merge_chains.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/processors/name_moltype.py` & `vermouth-0.9.3/vermouth/processors/name_moltype.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/processors/pdb_reader.py` & `vermouth-0.9.3/vermouth/processors/pdb_reader.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/processors/processor.py` & `vermouth-0.9.3/vermouth/processors/processor.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/processors/quote.py` & `vermouth-0.9.3/vermouth/processors/quote.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/processors/rename_modified_residues.py` & `vermouth-0.9.3/vermouth/processors/rename_modified_residues.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/processors/repair_graph.py` & `vermouth-0.9.3/vermouth/processors/repair_graph.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/processors/set_molecule_meta.py` & `vermouth-0.9.3/vermouth/processors/set_molecule_meta.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/processors/tune_cystein_bridges.py` & `vermouth-0.9.3/vermouth/processors/tune_cystein_bridges.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/selectors.py` & `vermouth-0.9.3/vermouth/selectors.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/system.py` & `vermouth-0.9.3/vermouth/system.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/__init__.py` & `vermouth-0.9.3/vermouth/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/1bta.pdb` & `vermouth-0.9.3/vermouth/tests/data/1bta.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/1bta_mutated.pdb` & `vermouth-0.9.3/vermouth/tests/data/1bta_mutated.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/2QWO.pdb` & `vermouth-0.9.3/vermouth/tests/data/2QWO.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/2dn2.pdb` & `vermouth-0.9.3/vermouth/tests/data/2dn2.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/6E8W.pdb` & `vermouth-0.9.3/vermouth/tests/data/6E8W.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/ala5.pdb` & `vermouth-0.9.3/vermouth/tests/data/ala5.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/ala5_cg.pdb` & `vermouth-0.9.3/vermouth/tests/data/ala5_cg.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/dna-short.pdb` & `vermouth-0.9.3/vermouth/tests/data/dna-short.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/dssp_1bta.ssd` & `vermouth-0.9.3/vermouth/tests/data/dssp_tests/dssp_1bta.ssd`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/force_fields/martini-test/aminoacids.ff` & `vermouth-0.9.3/vermouth/tests/data/force_fields/martini-test/aminoacids.ff`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/force_fields/pepplane/ala.ff` & `vermouth-0.9.3/vermouth/tests/data/force_fields/pepplane/ala.ff`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/force_fields/pepplane/general.ff` & `vermouth-0.9.3/vermouth/tests/data/force_fields/pepplane/general.ff`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/force_fields/universal-test/aminoacids.rtp` & `vermouth-0.9.3/vermouth/tests/data/force_fields/universal-test/aminoacids.rtp`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/force_fields/universal-test/modifications.ff` & `vermouth-0.9.3/vermouth/tests/data/force_fields/universal-test/modifications.ff`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/heme.pdb` & `vermouth-0.9.3/vermouth/tests/data/heme.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/dipro-termini/aa.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/dipro-termini/aa.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/dipro-termini/martinize2/molecule_0.itp` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/dipro-termini/martinize2/molecule_0.itp`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/aa.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/aa.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/cg.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/cg.pdb`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ATOM      1 BB   SER A   1      27.102  10.017 -17.685  1.00  0.00              
 ATOM      2 SC1  SER A   1      25.399   9.738 -15.572  1.00  0.00              
 ATOM      3 BB   LYS A   2      28.269  13.652 -18.042  1.00  0.00              
 ATOM      4 SC1  LYS A   2      28.657  13.278 -21.110  1.00  0.00              
-ATOM      5 SC2  LYS A   2      27.891  13.949 -24.259  1.00  0.00              
+ATOM      5 SC2  LYS A   2      27.835  13.973 -24.194  1.00  0.00              
 ATOM      6 BB   TYR A   3      30.697  16.103 -17.294  1.00  0.00              
 ATOM      7 SC1  TYR A   3      32.250  15.410 -15.448  1.00  0.00              
 ATOM      8 SC2  TYR A   3      34.135  16.705 -14.750  1.00  0.00              
 ATOM      9 SC3  TYR A   3      35.645  15.049 -15.657  1.00  0.00              
 ATOM     10 BB   GLU A   4      30.218  19.770 -17.376  1.00  0.00              
 ATOM     11 SC1  GLU A   4      28.724  20.998 -20.948  1.00  0.00              
 ATOM     12 BB   TYR A   5      33.057  21.627 -16.377  1.00  0.00              
@@ -44,15 +44,15 @@
 ATOM     44 SC1  PRO A  18      32.394  15.019 -10.054  1.00  0.00              
 ATOM     45 BB   THR A  19      30.735  18.242  -7.150  1.00  0.00              
 ATOM     46 SC1  THR A  19      28.525  18.825  -5.619  1.00  0.00              
 ATOM     47 BB   VAL A  20      31.085  21.964  -6.778  1.00  0.00              
 ATOM     48 SC1  VAL A  20      31.560  21.907  -9.600  1.00  0.00              
 ATOM     49 BB   LYS A  21      32.547  25.021  -6.400  1.00  0.00              
 ATOM     50 SC1  LYS A  21      35.238  25.373  -6.115  1.00  0.00              
-ATOM     51 SC2  LYS A  21      36.880  27.341  -8.234  1.00  0.00              
+ATOM     51 SC2  LYS A  21      36.918  27.266  -8.205  1.00  0.00              
 ATOM     52 BB   PRO A  22      32.459  28.481  -6.262  1.00  0.00              
 ATOM     53 SC1  PRO A  22      31.485  28.354  -4.069  1.00  0.00              
 ATOM     54 BB   ALA A  23      32.163  29.554  -9.931  1.00  0.00              
 ATOM     55 BB   VAL A  24      31.840  26.324 -10.532  1.00  0.00              
 ATOM     56 SC1  VAL A  24      34.204  24.880 -11.322  1.00  0.00              
 ATOM     57 BB   THR A  25      29.402  24.619 -12.989  1.00  0.00              
 ATOM     58 SC1  THR A  25      28.066  26.700 -12.505  1.00  0.00
```

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/chain_A.ssd` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/chain_A.ssd`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/molecule_0.itp` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/molecule_0.itp`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/screen.output` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein1_betasheet/martinize2/screen.output`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/aa.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/aa.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/cg.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/cg.pdb`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ATOM      1 BB   ARG A   1       3.483  -1.063  -1.716  1.00  0.00              
 ATOM      2 SC1  ARG A   1       5.890   0.035  -1.481  1.00  0.00              
 ATOM      3 SC2  ARG A   1       7.255   2.074  -3.427  1.00  0.00              
 ATOM      4 BB   LYS A   2       1.573  -2.205  -4.856  1.00  0.00              
 ATOM      5 SC1  LYS A   2      -0.692  -2.977  -3.657  1.00  0.00              
-ATOM      6 SC2  LYS A   2      -2.937  -4.274  -4.219  1.00  0.00              
+ATOM      6 SC2  LYS A   2      -2.884  -4.331  -4.179  1.00  0.00              
 ATOM      7 BB   TRP A   3       1.238  -0.541  -8.337  1.00  0.00              
 ATOM      8 SC1  TRP A   3       3.576  -0.344  -9.006  1.00  0.00              
 ATOM      9 SC2  TRP A   3       5.433  -1.209  -8.441  1.00  0.00              
 ATOM     10 SC3  TRP A   3       4.900   2.256  -8.475  1.00  0.00              
 ATOM     11 SC4  TRP A   3       6.885   1.420  -7.880  1.00  0.00              
 ATOM     12 BB   GLU A   4      -2.256  -2.095  -8.732  1.00  0.00              
 ATOM     13 SC1  GLU A   4      -4.041  -4.886  -7.524  1.00  0.00              
@@ -55,15 +55,15 @@
 ATOM     55 BB   ALA A  24       2.713   4.228 -16.541  1.00  0.00              
 ATOM     56 BB   VAL A  25       2.411   3.816 -12.744  1.00  0.00              
 ATOM     57 SC1  VAL A  25       1.515   2.386 -11.646  1.00  0.00              
 ATOM     58 BB   GLU A  26       5.983   2.377 -12.109  1.00  0.00              
 ATOM     59 SC1  GLU A  26       7.283  -0.339 -13.984  1.00  0.00              
 ATOM     60 BB   LYS A  27       7.725   5.087 -14.252  1.00  0.00              
 ATOM     61 SC1  LYS A  27       8.425   4.133 -16.164  1.00  0.00              
-ATOM     62 SC2  LYS A  27       9.787   1.846 -17.502  1.00  0.00              
+ATOM     62 SC2  LYS A  27       9.803   1.825 -17.418  1.00  0.00              
 ATOM     63 BB   ALA A  28       5.635   7.780 -12.457  1.00  0.00              
 ATOM     64 BB   GLY A  29       6.649   6.143  -9.116  1.00  0.00              
 ATOM     65 BB   GLY A  30       3.018   5.812  -7.950  1.00  0.00              
 ATOM     66 BB   ASN A  31       2.056   9.361  -9.099  1.00  0.00              
 ATOM     67 SC1  ASN A  31       2.534  11.900  -9.369  1.00  0.00              
 ATOM     68 BB   GLU A  32      -1.388   9.140 -10.850  1.00  0.00              
 ATOM     69 SC1  GLU A  32      -4.067   8.014  -8.854  1.00  0.00              
@@ -80,30 +80,30 @@
 ATOM     80 SC2  ARG A  37       3.834  16.055 -18.960  1.00  0.00              
 ATOM     81 BB   ILE A  38       2.827   8.131 -19.529  1.00  0.00              
 ATOM     82 SC1  ILE A  38       4.607   7.850 -17.842  1.00  0.00              
 ATOM     83 BB   VAL A  39      -0.241   5.806 -20.027  1.00  0.00              
 ATOM     84 SC1  VAL A  39      -2.094   5.808 -19.237  1.00  0.00              
 ATOM     85 BB   LYS A  40      -1.029   7.633 -23.317  1.00  0.00              
 ATOM     86 SC1  LYS A  40      -2.820   9.577 -22.980  1.00  0.00              
-ATOM     87 SC2  LYS A  40      -5.512  11.416 -22.446  1.00  0.00              
+ATOM     87 SC2  LYS A  40      -5.496  11.344 -22.399  1.00  0.00              
 ATOM     88 BB   LYS A  41       1.415   6.438 -25.971  1.00  0.00              
 ATOM     89 SC1  LYS A  41       3.020   4.403 -25.416  1.00  0.00              
-ATOM     90 SC2  LYS A  41       4.222   2.876 -23.258  1.00  0.00              
+ATOM     90 SC2  LYS A  41       4.296   2.883 -23.306  1.00  0.00              
 ATOM     91 BB   ARG A  42       0.336   8.506 -29.035  1.00  0.00              
 ATOM     92 SC1  ARG A  42       0.158  10.449 -30.246  1.00  0.00              
 ATOM     93 SC2  ARG A  42      -1.135  13.331 -29.650  1.00  0.00              
 ATOM     94 BB   LEU A  43       2.007   6.140 -31.572  1.00  0.00              
 ATOM     95 SC1  LEU A  43       2.190   3.938 -30.056  1.00  0.00              
 TER      96      LEU A  43 
 CONECT    1    2    4
 CONECT    2    3
 CONECT    4    5    7
 CONECT    5    6
 CONECT    7    8   12
-CONECT    8   11   10    9
+CONECT    8    9   10   11
 CONECT    9   11
 CONECT   10   11
 CONECT   12   13   14
 CONECT   14   15   16
 CONECT   16   17   18
 CONECT   18   19
 CONECT   19   20   21
```

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/chain_A.ssd` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/chain_A.ssd`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/molecule_0.itp` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/molecule_0.itp`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/screen.output` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein2_helix/martinize2/screen.output`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/aa.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/aa.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/cg.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/cg.pdb`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ATOM     15 SC2  TRP A   6       2.923   0.581   0.477  1.00  0.00              
 ATOM     16 SC3  TRP A   6       1.045   0.479   3.466  1.00  0.00              
 ATOM     17 SC4  TRP A   6       3.281   0.423   3.567  1.00  0.00              
 ATOM     18 BB   LEU A   7      -1.641  -2.932   1.963  1.00  0.00              
 ATOM     19 SC1  LEU A   7      -2.395  -1.889   4.258  1.00  0.00              
 ATOM     20 BB   LYS A   8      -3.024  -5.791  -0.269  1.00  0.00              
 ATOM     21 SC1  LYS A   8      -3.945  -5.564  -2.515  1.00  0.00              
-ATOM     22 SC2  LYS A   8      -4.147  -5.370  -5.639  1.00  0.00              
+ATOM     22 SC2  LYS A   8      -4.073  -5.333  -5.607  1.00  0.00              
 ATOM     23 BB   ASP A   9       0.466  -6.016  -1.905  1.00  0.00              
 ATOM     24 SC1  ASP A   9       0.678  -4.907  -4.211  1.00  0.00              
 ATOM     25 BB   GLY A  10       2.060  -6.618   1.593  1.00  0.00              
 ATOM     26 BB   GLY A  11       2.626  -2.967   2.723  1.00  0.00              
 ATOM     27 BB   PRO A  12       6.333  -2.533   3.806  1.00  0.00              
 ATOM     28 SC1  PRO A  12       5.521  -2.318   5.475  1.00  0.00              
 ATOM     29 BB   SER A  13       7.049  -6.179   2.704  1.00  0.00              
@@ -41,15 +41,15 @@
 ATOM     41 BB   PRO A  19       1.185   6.543  -0.353  1.00  0.00              
 ATOM     42 SC1  PRO A  19       0.082   5.047  -0.456  1.00  0.00              
 ATOM     43 BB   SER A  20       0.852  10.027   1.285  1.00  0.00              
 ATOM     44 SC1  SER A  20       2.635  10.743   1.678  1.00  0.00              
 TER      45      SER A  20 
 CONECT    1    2    3
 CONECT    3    4    5
-CONECT    5    7    6    9
+CONECT    5    6    7    9
 CONECT    6    7    8
 CONECT    7    8
 CONECT    9   10   11
 CONECT   11   12   13
 CONECT   13   14   18
 CONECT   14   15   16   17
 CONECT   15   17
```

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/chain_A.ssd` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/chain_A.ssd`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/citation` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/citation`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/molecule_0.itp` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/molecule_0.itp`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/screen.output` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-0/mini-protein3_trp-cage/martinize2/screen.output`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5/aa.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5/aa.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/cg.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/cg.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/chain_.ssd` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/chain_.ssd`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/molecule_0.itp` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/molecule_0.itp`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/screen.output` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5/martinize2/screen.output`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/aa.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/aa.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/cg.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/cg.pdb`

 * *Files 0% similar despite different names*

```diff
@@ -3,43 +3,43 @@
 ATOM      3 BB   LEU     2       3.472  22.892  -7.373  1.00  0.00              
 ATOM      4 SC1  LEU     2       6.873  24.160  -7.387  1.00  0.00              
 ATOM      5 BB   GLY     3       2.005  26.171  -6.771  1.00  0.00              
 ATOM      6 BB   ALA     4      -0.188  29.158  -6.044  1.00  0.00              
 ATOM      7 SC1  ALA     4       0.134  30.121  -7.770  1.00  0.00              
 ATOM      8 BB   LYS     5      -1.926  28.105  -3.988  1.00  0.00              
 ATOM      9 SC1  LYS     5      -4.594  27.166  -3.877  1.00  0.00              
-ATOM     10 SC2  LYS     5      -6.389  27.128  -0.981  1.00  0.00              
+ATOM     10 SC2  LYS     5      -6.414  27.164  -1.059  1.00  0.00              
 ATOM     11 BB   PRO     6      -3.187  28.114  -1.068  1.00  0.00              
 ATOM     12 SC1  PRO     6      -3.898  30.287  -1.251  1.00  0.00              
 ATOM     13 BB   PHE     7      -3.680  26.087   1.748  1.00  0.00              
 ATOM     14 SC1  PHE     7      -1.880  24.735   2.991  1.00  0.00              
 ATOM     15 SC2  PHE     7      -2.278  22.245   3.230  1.00  0.00              
 ATOM     16 SC3  PHE     7      -2.249  23.126   4.910  1.00  0.00              
 ATOM     17 BB   GLY     8      -5.497  28.225   3.164  1.00  0.00              
 ATOM     18 BB   GLU     9      -7.365  29.952   5.283  1.00  0.00              
 ATOM     19 SC1  GLU     9     -11.026  30.715   3.096  1.00  0.00              
 ATOM     20 BB   LYS    10      -7.469  32.516   7.352  1.00  0.00              
 ATOM     21 SC1  LYS    10      -4.748  33.904   6.404  1.00  0.00              
-ATOM     22 SC2  LYS    10      -2.161  34.367   5.047  1.00  0.00              
+ATOM     22 SC2  LYS    10      -2.182  34.283   5.026  1.00  0.00              
 ATOM     23 BB   LYS    11      -6.908  33.077  10.677  1.00  0.00              
 ATOM     24 SC1  LYS    11      -8.271  29.981  11.504  1.00  0.00              
-ATOM     25 SC2  LYS    11      -9.077  27.539  10.096  1.00  0.00              
+ATOM     25 SC2  LYS    11      -9.112  27.520  10.174  1.00  0.00              
 ATOM     26 BB   PHE    12      -7.884  34.796  13.901  1.00  0.00              
 ATOM     27 SC1  PHE    12      -8.096  36.697  11.519  1.00  0.00              
 ATOM     28 SC2  PHE    12      -8.672  36.356   9.080  1.00  0.00              
 ATOM     29 SC3  PHE    12      -6.995  37.375   9.412  1.00  0.00              
 ATOM     30 BB   ILE    13      -5.906  36.634  16.471  1.00  0.00              
 ATOM     31 SC1  ILE    13      -5.640  33.823  18.059  1.00  0.00              
 ATOM     32 BB   GLU    14      -5.890  38.467  19.366  1.00  0.00              
 ATOM     33 SC1  GLU    14      -8.282  40.927  17.834  1.00  0.00              
 ATOM     34 BB   ILE    15      -2.892  40.652  19.850  1.00  0.00              
 ATOM     35 SC1  ILE    15      -1.630  38.002  19.874  1.00  0.00              
 ATOM     36 BB   LYS    16      -2.323  43.417  21.667  1.00  0.00              
 ATOM     37 SC1  LYS    16       0.439  42.144  22.572  1.00  0.00              
-ATOM     38 SC2  LYS    16       2.469  40.912  24.457  1.00  0.00              
+ATOM     38 SC2  LYS    16       2.461  40.854  24.390  1.00  0.00              
 ATOM     39 BB   GLY    17      -4.608  44.693  19.398  1.00  0.00              
 ATOM     40 BB   ARG    18      -3.854  42.577  17.142  1.00  0.00              
 ATOM     41 SC1  ARG    18      -1.913  44.889  16.381  1.00  0.00              
 ATOM     42 SC2  ARG    18      -1.766  48.578  15.853  1.00  0.00              
 ATOM     43 BB   ARG    19      -4.307  41.037  14.227  1.00  0.00              
 ATOM     44 SC1  ARG    19      -7.360  40.535  13.380  1.00  0.00              
 ATOM     45 SC2  ARG    19      -8.823  40.418  10.303  1.00  0.00              
@@ -152,15 +152,15 @@
 ATOM    152 SC1  ASP    67      -3.574  38.265   4.828  1.00  0.00              
 ATOM    153 BB   SER    68      -1.064  40.922   9.648  1.00  0.00              
 ATOM    154 SC1  SER    68      -0.177  38.761  11.269  1.00  0.00              
 ATOM    155 BB   ASP    69      -0.924  43.526  11.456  1.00  0.00              
 ATOM    156 SC1  ASP    69      -4.279  43.991  12.292  1.00  0.00              
 ATOM    157 BB   LYS    70      -0.043  46.746  11.705  1.00  0.00              
 ATOM    158 SC1  LYS    70       0.857  47.028   8.713  1.00  0.00              
-ATOM    159 SC2  LYS    70       2.229  45.462   6.189  1.00  0.00              
+ATOM    159 SC2  LYS    70       2.148  45.497   6.183  1.00  0.00              
 ATOM    160 BB   LEU    71       2.078  48.915  13.139  1.00  0.00              
 ATOM    161 SC1  LEU    71       3.341  46.642  15.386  1.00  0.00              
 ATOM    162 BB   ASP    72       1.021  51.888  15.194  1.00  0.00              
 ATOM    163 SC1  ASP    72      -0.082  53.843  12.974  1.00  0.00              
 ATOM    164 BB   PRO    73       3.639  53.040  15.326  1.00  0.00              
 ATOM    165 SC1  PRO    73       3.343  54.472  17.029  1.00  0.00              
 ATOM    166 BB   SER    74       6.261  53.680  12.830  1.00  0.00              
@@ -552,15 +552,15 @@
 ATOM    552 SC1  PRO   234      18.886  16.059  24.233  1.00  0.00              
 ATOM    553 BB   ILE   235      16.775  16.868  19.958  1.00  0.00              
 ATOM    554 SC1  ILE   235      14.710  18.902  21.161  1.00  0.00              
 ATOM    555 BB   PRO   236      15.315  16.219  17.158  1.00  0.00              
 ATOM    556 SC1  PRO   236      14.293  14.327  18.192  1.00  0.00              
 ATOM    557 BB   LYS   237      16.750  16.588  13.814  1.00  0.00              
 ATOM    558 SC1  LYS   237      18.382  18.890  15.638  1.00  0.00              
-ATOM    559 SC2  LYS   237      19.558  18.900  18.211  1.00  0.00              
+ATOM    559 SC2  LYS   237      19.555  18.989  18.203  1.00  0.00              
 ATOM    560 BB   LEU   238      16.289  18.547  10.661  1.00  0.00              
 ATOM    561 SC1  LEU   238      14.671  16.836   8.572  1.00  0.00              
 ATOM    562 BB   PHE   239      18.480  19.043   7.949  1.00  0.00              
 ATOM    563 SC1  PHE   239      20.800  20.312   8.453  1.00  0.00              
 ATOM    564 SC2  PHE   239      21.398  22.405   7.183  1.00  0.00              
 ATOM    565 SC3  PHE   239      22.873  21.099   7.323  1.00  0.00              
 ATOM    566 BB   ILE   240      17.888  21.381   5.336  1.00  0.00
```

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/chain_.ssd` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/chain_.ssd`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/molecule_0.itp` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/molecule_0.itp`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/screen.output` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/1mj5-charmm/martinize2/screen.output`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/3i40/3i40.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/3i40/3i40.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/cg.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/cg.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/chain_A.ssd` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/chain_A.ssd`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/chain_C.ssd` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/chain_C.ssd`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/insulin_dimer.itp` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/insulin_dimer.itp`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/molecule_0.itp` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/molecule_0.itp`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/screen.output` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/3i40/martinize2/screen.output`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/6LFO_gap.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/6LFO_gap.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/cg.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/cg.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/chain_R.ssd` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/chain_R.ssd`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/molecule_0.itp` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/molecule_0.itp`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/screen.output` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/6LFO_gap/martinize2/screen.output`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_chain/aa.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_chain/aa.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/cg.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/cg.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/chain_A.ssd` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/chain_A.ssd`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/molecule_0.itp` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/molecule_0.itp`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/screen.output` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_chain/martinize2/screen.output`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_region/aa.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_region/aa.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/cg.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/cg.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/chain_A.ssd` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/chain_A.ssd`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/molecule_0.itp` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/molecule_0.itp`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/screen.output` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/EN_region/martinize2/screen.output`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/bpti/aa.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/bpti/aa.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/cg.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/cg.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/chain_A.ssd` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/chain_A.ssd`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/citation` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/citation`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/molecule_0.itp` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/molecule_0.itp`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/screen.output` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/bpti/martinize2/screen.output`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme/aa.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme/aa.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/cg.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/cg.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/chain_A.ssd` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/chain_A.ssd`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/molecule_0.itp` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/molecule_0.itp`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/screen.output` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/screen.output`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/test.itp` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/test.itp`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/aa.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/aa.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/cg.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/cg.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/chain_A.ssd` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/chain_A.ssd`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/molecule_0.itp` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/molecule_0.itp`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/screen.output` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/screen.output`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/test.itp` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/test.itp`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/villin/aa.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/villin/aa.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/villin/martinize2/cg.pdb` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/villin/martinize2/cg.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/villin/martinize2/molecule_0.itp` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/villin/martinize2/molecule_0.itp`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/integration_tests/tier-1/villin/martinize2/screen.output` & `vermouth-0.9.3/vermouth/tests/data/integration_tests/tier-1/villin/martinize2/screen.output`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/mappings/universal-test/pepplane/ala.mapping` & `vermouth-0.9.3/vermouth/tests/data/mappings/universal-test/pepplane/ala.mapping`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/mappings/universal-test/pepplane/modifications.mapping` & `vermouth-0.9.3/vermouth/tests/data/mappings/universal-test/pepplane/modifications.mapping`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/data/tri_alanine.pdb` & `vermouth-0.9.3/vermouth/tests/data/tri_alanine.pdb`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/datafiles.py` & `vermouth-0.9.3/vermouth/tests/datafiles.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 PDB_CYS = TEST_DATA / '2QWO.pdb'  # Contains cystein bridges
 PDB_HB = TEST_DATA / '2dn2.pdb'  # Hemoglobin with heme and 2*2 protein chains
 PDB_MULTIMODEL = TEST_DATA / '6E8W.pdb'  # HIV-1, 15 models
 
 # DNA
 SHORT_DNA = TEST_DATA / 'dna-short.pdb'
 
-DSSP_OUTPUT = TEST_DATA / 'dssp_1bta.ssd'
+DSSP_OUTPUT = TEST_DATA / 'dssp_tests' / 'dssp_1bta.ssd'
+DSSP_SS_OUTPUT = TEST_DATA / 'dssp_tests'
 
 # Test force fields
 FF_UNIVERSAL_TEST = TEST_DATA / 'force_fields' / 'universal-test'
 FF_PEPPLANE = TEST_DATA / 'force_fields' / 'pepplane'
 FF_MARTINI_TEST = TEST_DATA / 'force_fields' / 'martini-test'
 
 # Mappings
```

### Comparing `vermouth-0.9.1/vermouth/tests/gmx/test_gro.py` & `vermouth-0.9.3/vermouth/tests/gmx/test_gro.py`

 * *Files 1% similar despite different names*

```diff
@@ -536,15 +536,15 @@
     Test the GRO reader.
     """
     filename, reference = gro_reference
     filter_molecule(reference, exclude=exclude, ignh=ignh)
     molecule = gro.read_gro(filename, exclude=exclude, ignh=ignh)
     pprint(list(molecule.nodes.items()))
     assert_molecule_equal(molecule, reference)
-
+    assert all(molecule.box == np.array([10.0, 11.1, 12.2]))
 
 def test_read_gro_wrong_atom_number(gro_wrong_length):  # pylint: disable=redefined-outer-name
     """
     Test that the GRO reader raises an exception if the number of atoms is not
     consistent.
     """
     with pytest.raises(ValueError):
```

### Comparing `vermouth-0.9.1/vermouth/tests/gmx/test_itp.py` & `vermouth-0.9.3/vermouth/tests/gmx/test_itp.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/helper_functions.py` & `vermouth-0.9.3/vermouth/tests/helper_functions.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/integration_tests/__init__.py` & `vermouth-0.9.3/vermouth/tests/integration_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/integration_tests/test_integration.py` & `vermouth-0.9.3/vermouth/tests/integration_tests/test_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,17 +135,17 @@
     ['tier-1', 'villin'],
     ['tier-1', '3i40'],
     ['tier-1', '6LFO_gap'],
     ['tier-1', '1mj5'],
     ['tier-1', '1mj5-charmm'],
     ['tier-1', 'EN_chain'],
     ['tier-1', 'EN_region'],
-    # ['tier-2', 'barnase_barstar'],
-    # ['tier-2', 'dna'],
-   # ['tier-2', 'gpa_dimer'],
+#   ['tier-2', 'barnase_barstar'],
+#   ['tier-2', 'dna'],
+#   ['tier-2', 'gpa_dimer'],
 ])
 def test_integration_protein(tmp_path, monkeypatch, tier, protein):
     """
     Runs integration tests by executing the contents of the file `command` in
     the folder tier/protein, and tests whether the contents of the produced
     files are the same as the reference files. The comparison of the files is
     governed by `COMPARERS`.
```

### Comparing `vermouth-0.9.1/vermouth/tests/molecule_strategies.py` & `vermouth-0.9.3/vermouth/tests/molecule_strategies.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/pdb/test_read_pdb.py` & `vermouth-0.9.3/vermouth/tests/pdb/test_read_pdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -151,15 +151,14 @@
     mols = list(parser.parse(pdbstr.splitlines()))
     assert len(mols) == len(nnodesnedges)
     for mol, nnodes_edges in zip(mols, nnodesnedges):
         nnodes, nedges = nnodes_edges
         assert len(mol.nodes) == nnodes
         assert len(mol.edges) == nedges
 
-
 @pytest.mark.parametrize('ignh', [True, False])
 @pytest.mark.parametrize('modelidx', range(1, 16))
 def test_integrative(ignh, modelidx):
     parser = PDBParser(ignh=ignh, modelidx=modelidx)
     with open(str(PDB_MULTIMODEL)) as pdb_file:
         mols = list(parser.parse(pdb_file))
     assert len(mols) == 3  # 3 chains
@@ -229,7 +228,38 @@
             assert set(n_attrs[n_idx].keys()) == set(mol.nodes[n_idx].keys())
             for attr in mol.nodes[n_idx]:
                 assert attr in n_attrs[n_idx]
                 if attr == 'position':
                     assert np.allclose(n_attrs[n_idx][attr], mol.nodes[n_idx][attr])
                 else:
                     assert n_attrs[n_idx][attr] == mol.nodes[n_idx][attr]
+
+
+@pytest.mark.parametrize('pdbstr, cryst_dict', (
+    # complete directive
+    ('''CRYST1   77.987   77.987   77.987  90.00  90.00  90.00 P 1           1
+    MODEL        1
+    ATOM      1  EO  PEO     0      74.550  37.470  22.790  1.00  0.00
+    ATOM      2  EO  PEO     1      77.020  38.150  25.000  1.00  0.00
+    ATOM      3  EO  PEO     2      76.390  37.180  28.130  1.00  0.00
+    ATOM      4  EO  PEO     3      75.430  37.920  31.450  1.00  0.00
+    ''',
+    {"a": 77.987, "b": 77.987, "c": 77.987,
+     "alpha": 90.0, "beta": 90.0, "gamma": 90,
+    "space_group": "P 1", "z_value": 1}
+    ),
+    # incomplete directive
+    ('''CRYST1   77.987   77.987   77.987
+    MODEL        1
+    ATOM      1  EO  PEO     0      74.550  37.470  22.790  1.00  0.00
+    ATOM      2  EO  PEO     1      77.020  38.150  25.000  1.00  0.00
+    ATOM      3  EO  PEO     2      76.390  37.180  28.130  1.00  0.00
+    ATOM      4  EO  PEO     3      75.430  37.920  31.450  1.00  0.00
+    ''',
+    {"a": 77.987, "b": 77.987, "c": 77.987,}
+    )))
+def test_cryst1(caplog, pdbstr, cryst_dict):
+    parser = PDBParser()
+    mols = list(parser.parse(pdbstr.splitlines()))
+    assert parser.cryst == cryst_dict
+    if len(cryst_dict) < 8:
+        assert any(rec.levelname == 'WARNING' for rec in caplog.records)
```

### Comparing `vermouth-0.9.1/vermouth/tests/pdb/test_write_pdb.py` & `vermouth-0.9.3/vermouth/tests/pdb/test_write_pdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         {'atomname': 'A', 'resname': 'A', 'resid': 1, },
         {'atomname': 'B', 'resname': 'A', 'resid': 1, 'charge': -1},
         {'atomname': 'C', 'resname': 'A', 'resid': 2, 'charge': 1},
         {'atomname': 'D', 'resname': 'A', 'resid': 3, },
         {'atomname': 'E', 'resname': 'A', 'resid': 4, },
         {'atomname': 'F', 'resname': 'B', 'resid': 4, },
         {'atomname': 'G', 'resname': 'B', 'resid': 4, },
-        {'atomname': 'H', 'resname': 'B', 'resid': 4, },
+        {'atomname': 'H', 'resname': 'B', 'resid': 4, 'insertion_code': 'A'},
     )
     edges = [(0, 1), (2, 3), (4, 5), (5, 6), (5, 7)]
     graph = nx.Graph()
     for idx, node in enumerate(nodes):
         node['chain'] = ''
         node['element'] = node['atomname']
         node['position'] = np.array([1, 2, -3])
@@ -96,16 +96,16 @@
 TER       3      A       1 
 ATOM      4 C    A       2      10.000  20.000 -30.000  1.00  0.00          C 1+
 ATOM      5 D    A       3      10.000  20.000 -30.000  1.00  0.00          D   
 TER       6      A       3 
 ATOM      7 E    A       4      10.000  20.000 -30.000  1.00  0.00          E   
 ATOM      8 F    B       4      10.000  20.000 -30.000  1.00  0.00          F   
 ATOM      9 G    B       4      10.000  20.000 -30.000  1.00  0.00          G   
-ATOM     10 H    B       4      10.000  20.000 -30.000  1.00  0.00          H   
-TER      11      B       4 
+ATOM     10 H    B       4A     10.000  20.000 -30.000  1.00  0.00          H   
+TER      11      B       4A
 CONECT    1    2
 CONECT    4    5
 CONECT    7    8
 CONECT    8    9   10
 END
 '''
     assert pdb_found.strip() == expected.strip()
@@ -137,12 +137,12 @@
 TER       3      A       1 
 ATOM      4 C    A       2         nan     nan     nan  1.00  0.00          C 1+
 ATOM      5 D    A       3         nan     nan     nan  1.00  0.00          D   
 TER       6      A       3 
 ATOM      7 E    A       4      10.000  20.000 -30.000  1.00  0.00          E   
 ATOM      8 F    B       4      10.000  20.000 -30.000  1.00  0.00          F   
 ATOM      9 G    B       4      10.000  20.000 -30.000  1.00  0.00          G   
-ATOM     10 H    B       4      10.000  20.000 -30.000  1.00  0.00          H   
-TER      11      B       4 
+ATOM     10 H    B       4A     10.000  20.000 -30.000  1.00  0.00          H   
+TER      11      B       4A
 END
 '''
     assert pdb_found.strip() == expected.strip()
```

### Comparing `vermouth-0.9.1/vermouth/tests/test_add_molecule_edges.py` & `vermouth-0.9.3/vermouth/tests/test_add_molecule_edges.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_annotate_mut_mod.py` & `vermouth-0.9.3/vermouth/tests/test_annotate_mut_mod.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_apply_rubber_band.py` & `vermouth-0.9.3/vermouth/tests/test_apply_rubber_band.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_average_beads.py` & `vermouth-0.9.3/vermouth/tests/test_average_beads.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_do_mapping.py` & `vermouth-0.9.3/vermouth/tests/test_do_mapping.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_dssp.py` & `vermouth-0.9.3/vermouth/tests/test_dssp.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,38 +28,42 @@
 from vermouth.forcefield import get_native_force_field
 from vermouth.dssp import dssp
 from vermouth.dssp.dssp import DSSPError
 from vermouth.pdb.pdb import read_pdb
 from vermouth.tests.datafiles import (
     PDB_PROTEIN,
     DSSP_OUTPUT,
+    DSSP_SS_OUTPUT,
     PDB_ALA5_CG,
 )
 
-DSSP_EXECUTABLE = os.environ.get('VERMOUTH_TEST_DSSP', 'dssp')
-SECSTRUCT_1BTA = list('CEEEEETTTCCSHHHHHHHHHHHHTCCTTCCCSHHHHHHHHTTT'
-                      'SCSSEEEEEESTTHHHHTTTSSHHHHHHHHHHHHHTTCCEEEEEC')
+DSSP_EXECUTABLE = os.environ.get("VERMOUTH_TEST_DSSP", "dssp")
+SECSTRUCT_1BTA = list(
+    "CEEEEETTTCCSHHHHHHHHHHHHTCCTTCCCSHHHHHHHHTTT"
+    "SCSSEEEEEESTTHHHHTTTSSHHHHHHHHHHHHHTTCCEEEEEC"
+)
 
 
 # TODO: The code is very repetitive. There may be a way to refactor it with
 # clever use of parametrize and fixtures.
 class TestAnnotateResidues:
     """
     Tests for the :class:`dssp.AnnotateResidues` processor.
     """
+
     @staticmethod
     def build_molecule(nresidues):
         """
         Build a dummy molecule with the requested number of residues and 3
         atoms per residue.
         """
         molecule = vermouth.molecule.Molecule()
         residue_template = vermouth.molecule.Molecule()
         residue_template.add_nodes_from(
-            (idx, {'chain':'', 'atomname':str(idx), 'resname': 'DUMMY', 'resid': 1})
+            (idx, {"chain": "", "atomname": str(idx), "resname": "DUMMY", "resid": 1})
             for idx in range(3)
         )
         for _ in range(nresidues):
             molecule.merge_molecule(residue_template)
         return molecule
 
     @staticmethod
@@ -69,35 +73,37 @@
         """
         return [node.get(attribute, default) for node in molecule.nodes.values()]
 
     def sequence_from_system(self, system, attribute, default=None):
         """
         Extract the content of an attribute for each node of a system.
         """
-        return list(itertools.chain(*(
-            self.sequence_from_mol(molecule, attribute, default)
-            for molecule in system.molecules
-        )))
+        return list(
+            itertools.chain(
+                *(
+                    self.sequence_from_mol(molecule, attribute, default)
+                    for molecule in system.molecules
+                )
+            )
+        )
 
-    @pytest.mark.parametrize('nres', (0, 1, 3, 10))
+    @pytest.mark.parametrize("nres", (0, 1, 3, 10))
     def test_build_molecule(self, nres):
         """
         :meth:`build_molecule` and :meth:`sequence_from_mol` work as excpected.
         """
-        expected_resid = list(itertools.chain(
-            *([idx + 1] * 3 for idx in range(nres))
-        ))
-        expected_atomname = ['0', '1', '2'] * nres
-        expected_chain = [''] * (nres * 3)
-        expected_resname = ['DUMMY'] * (nres * 3)
+        expected_resid = list(itertools.chain(*([idx + 1] * 3 for idx in range(nres))))
+        expected_atomname = ["0", "1", "2"] * nres
+        expected_chain = [""] * (nres * 3)
+        expected_resname = ["DUMMY"] * (nres * 3)
         molecule = self.build_molecule(nres)
-        assert self.sequence_from_mol(molecule, 'resid') == expected_resid
-        assert self.sequence_from_mol(molecule, 'resname') == expected_resname
-        assert self.sequence_from_mol(molecule, 'chain') == expected_chain
-        assert self.sequence_from_mol(molecule, 'atomname') == expected_atomname
+        assert self.sequence_from_mol(molecule, "resid") == expected_resid
+        assert self.sequence_from_mol(molecule, "resname") == expected_resname
+        assert self.sequence_from_mol(molecule, "chain") == expected_chain
+        assert self.sequence_from_mol(molecule, "atomname") == expected_atomname
 
     @pytest.fixture
     def single_mol_system(self):
         """
         Build a system with a single molecule that count 5 residues of 3 atoms
         each.
         """
@@ -121,262 +127,306 @@
         """
         Build a system with 3 molecules having each 4 residues.
         """
         system = vermouth.system.System()
         system.molecules = [self.build_molecule(4) for _ in range(3)]
         return system
 
-    @pytest.mark.parametrize('sequence', (
-        'ABCDE',
-        ['A', 'B', 'C', 'D', 'E'],
-        range(5),
-    ))
+    @pytest.mark.parametrize(
+        "sequence",
+        (
+            "ABCDE",
+            ["A", "B", "C", "D", "E"],
+            range(5),
+        ),
+    )
     def test_single_molecule(self, single_mol_system, sequence):
         """
         The simple case with a single molecule and a sequence of the right size
         works as expected.
         """
-        expected = list(itertools.chain(
-            *([element] * 3 for element in sequence)
-        ))
-        processor = dssp.AnnotateResidues('test', sequence)
+        expected = list(itertools.chain(*([element] * 3 for element in sequence)))
+        processor = dssp.AnnotateResidues("test", sequence)
         processor.run_system(single_mol_system)
-        found = self.sequence_from_system(single_mol_system, 'test')
+        found = self.sequence_from_system(single_mol_system, "test")
         assert found == expected
 
-    @pytest.mark.parametrize('sequence', (
-        'ABCDEFGHIJKLMNO',
-        list('ABCDEFGHIJKLMNO'),
-        range(15),
-    ))
+    @pytest.mark.parametrize(
+        "sequence",
+        (
+            "ABCDEFGHIJKLMNO",
+            list("ABCDEFGHIJKLMNO"),
+            range(15),
+        ),
+    )
     def test_multi_molecules_diff_sizes(self, multi_mol_system_irregular, sequence):
         """
         The case of many protein of various sizes and a sequence of the right
         size works as expected.
         """
-        expected = list(itertools.chain(
-            *([element] * 3 for element in sequence)
-        ))
-        processor = dssp.AnnotateResidues('test', sequence)
+        expected = list(itertools.chain(*([element] * 3 for element in sequence)))
+        processor = dssp.AnnotateResidues("test", sequence)
         processor.run_system(multi_mol_system_irregular)
-        found = self.sequence_from_system(multi_mol_system_irregular, 'test')
+        found = self.sequence_from_system(multi_mol_system_irregular, "test")
         assert found == expected
 
-    @pytest.mark.parametrize('sequence', (
-        'ABCD',
-        ['A', 'B', 'C', 'D'],
-        range(4),
-    ))
+    @pytest.mark.parametrize(
+        "sequence",
+        (
+            "ABCD",
+            ["A", "B", "C", "D"],
+            range(4),
+        ),
+    )
     def test_multi_molecules_cycle(self, multi_mol_system_regular, sequence):
         """
         The case with multiple molecules with all the same size and one
         sequence to repeat for each molecule works as expected.
         """
-        expected = list(itertools.chain(
-            *([element] * 3 for element in sequence)
-        ))
+        expected = list(itertools.chain(*([element] * 3 for element in sequence)))
         expected = expected * 3
-        processor = dssp.AnnotateResidues('test', sequence)
+        processor = dssp.AnnotateResidues("test", sequence)
         processor.run_system(multi_mol_system_regular)
-        found = self.sequence_from_system(multi_mol_system_regular, 'test')
+        found = self.sequence_from_system(multi_mol_system_regular, "test")
         assert found == expected
 
     def test_single_molecules_cycle_one(self, single_mol_system):
         """
         One molecule and a one element sequence to repeat over all residues of
         the molecule.
         """
-        sequence = 'A'
+        sequence = "A"
         expected = [sequence] * (5 * 3)
-        processor = dssp.AnnotateResidues('test', sequence)
+        processor = dssp.AnnotateResidues("test", sequence)
         processor.run_system(single_mol_system)
-        found = self.sequence_from_system(single_mol_system, 'test')
+        found = self.sequence_from_system(single_mol_system, "test")
         assert found == expected
 
-
     def test_multi_molecules_cycle_one(self, multi_mol_system_irregular):
         """
         Many molecules and a one element sequence to repeat.
         """
-        sequence = 'A'
+        sequence = "A"
         expected = [sequence] * (15 * 3)
-        processor = dssp.AnnotateResidues('test', sequence)
+        processor = dssp.AnnotateResidues("test", sequence)
         processor.run_system(multi_mol_system_irregular)
-        found = self.sequence_from_system(multi_mol_system_irregular, 'test')
+        found = self.sequence_from_system(multi_mol_system_irregular, "test")
         assert found == expected
 
     @staticmethod
-    @pytest.mark.parametrize('sequence', (
-        'ABC',  # Too short
-        'ABCD',  # Too short, match the length of the first molecule
-        'ABCDEFGHIFKLMNOPQRSTU',  # Too long
-        '',  # Empty
-    ))
+    @pytest.mark.parametrize(
+        "sequence",
+        (
+            "ABC",  # Too short
+            "ABCD",  # Too short, match the length of the first molecule
+            "ABCDEFGHIFKLMNOPQRSTU",  # Too long
+            "",  # Empty
+        ),
+    )
     def test_wrong_length(multi_mol_system_irregular, sequence):
         """
         Many molecule and a sequence that has the wrong length raises an error.
         """
-        processor = dssp.AnnotateResidues('test', sequence)
+        processor = dssp.AnnotateResidues("test", sequence)
         with pytest.raises(ValueError):
             processor.run_system(multi_mol_system_irregular)
 
     @staticmethod
-    @pytest.mark.parametrize('sequence', (
-        'ABC',  # Too short
-        'ABCD',  # Too short, match the length of the first molecule
-        'ABCDEFGHIFKLMNOPQRSTU',  # Too long
-        '',  # Empty
-        'ABCDEFGHIJKLMNO',  # Length of all the molecules, without filter
-    ))
+    @pytest.mark.parametrize(
+        "sequence",
+        (
+            "ABC",  # Too short
+            "ABCD",  # Too short, match the length of the first molecule
+            "ABCDEFGHIFKLMNOPQRSTU",  # Too long
+            "",  # Empty
+            "ABCDEFGHIJKLMNO",  # Length of all the molecules, without filter
+        ),
+    )
     def test_wrong_length_with_filter(multi_mol_system_irregular, sequence):
         """
         Many molecules and a sequence that has the wrong length because of a
         molecule selector.
         """
         # We exclude the second molecule. The filter excludes it based on the
         # number of nodes, which is 15 because it has 5 residues with 3 nodes
         # each.
         processor = dssp.AnnotateResidues(
-            'test', sequence,
+            "test",
+            sequence,
             molecule_selector=lambda mol: len(mol.nodes) != (5 * 3),
         )
         with pytest.raises(ValueError):
             processor.run_system(multi_mol_system_irregular)
 
     @staticmethod
     def test_empty_system_empty_sequence():
         """
         There are no molecules, but the sequence is empty.
         """
         system = vermouth.system.System()
-        sequence = ''
-        processor = dssp.AnnotateResidues('test', sequence)
+        sequence = ""
+        processor = dssp.AnnotateResidues("test", sequence)
         try:
             processor.run_system(system)
         except ValueError:
-            pytest.fail('Should not have raised a ValueError.')
+            pytest.fail("Should not have raised a ValueError.")
 
     @staticmethod
     def test_empty_system_error():
         """
         There are no molecules, but there is a sequence. Should raise an error.
         """
         system = vermouth.system.System()
-        sequence = 'not empty'
-        processor = dssp.AnnotateResidues('test', sequence)
+        sequence = "not empty"
+        processor = dssp.AnnotateResidues("test", sequence)
         with pytest.raises(ValueError):
             processor.run_system(system)
 
     @staticmethod
     def test_empty_with_filter(multi_mol_system_irregular):
         """
         There is a sequence, but no molecule are accepted by the molecule
         selector. Should raise an error.
         """
-        sequence = 'not empty'
+        sequence = "not empty"
         processor = dssp.AnnotateResidues(
-            'test', sequence, molecule_selector=lambda mol: False
+            "test", sequence, molecule_selector=lambda mol: False
         )
         with pytest.raises(ValueError):
             processor.run_system(multi_mol_system_irregular)
 
     def test_run_molecule(self, single_mol_system):
         """
         The `run_molecule` method works.
         """
-        sequence = 'ABCDE'
-        expected = list(itertools.chain(
-            *([element] * 3 for element in sequence)
-        ))
-        processor = dssp.AnnotateResidues('test', sequence)
+        sequence = "ABCDE"
+        expected = list(itertools.chain(*([element] * 3 for element in sequence)))
+        processor = dssp.AnnotateResidues("test", sequence)
         processor.run_molecule(single_mol_system.molecules[0])
-        found = self.sequence_from_system(single_mol_system, 'test')
+        found = self.sequence_from_system(single_mol_system, "test")
         assert found == expected
 
     def test_run_molecule_not_selected(self, single_mol_system):
         """
         The molecule selector works with `run_molecule`.
         """
-        sequence = 'ABCDE'
+        sequence = "ABCDE"
         processor = dssp.AnnotateResidues(
-            'test', sequence, molecule_selector=lambda mol: False
+            "test", sequence, molecule_selector=lambda mol: False
         )
         processor.run_molecule(single_mol_system.molecules[0])
-        found = self.sequence_from_system(single_mol_system, 'test')
+        found = self.sequence_from_system(single_mol_system, "test")
         assert vermouth.utils.are_all_equal(found)
         assert found[0] is None
 
 
-def test_read_dssp2():
+@pytest.mark.parametrize(
+    "input_file, expected",
+    [
+        (str(DSSP_OUTPUT), "".join(SECSTRUCT_1BTA)),
+        (
+            str(DSSP_SS_OUTPUT / "mini-protein1_betasheet.pdb.v2.2.1-3b2-deb_cv1.ssd"),
+            "CEEEEEETTEEEEEECCCCCCTTCEEEEC",
+        ),
+        (
+            str(DSSP_SS_OUTPUT / "mini-protein1_betasheet.pdb.v3.0.0-3b1-deb_cv1.ssd"),
+            "CEEEEEETTEEEEEECCCCCCTTCEEEEC",
+        ),
+        (
+            str(DSSP_SS_OUTPUT / "mini-protein2_helix.pdb.v2.2.1-3b2-deb_cv1.ssd"),
+            "CCSHHHHHHHHHHCCCCHHHHHHHHHHHTSCHHHHHHHTCCC",
+        ),
+        (
+            str(DSSP_SS_OUTPUT / "mini-protein2_helix.pdb.v3.0.0-3b1-deb_cv1.ssd"),
+            "CCSHHHHHHHHHHCCCCHHHHHHHHHHHTSCHHHHHHHTCCC",
+        ),
+        (
+            str(DSSP_SS_OUTPUT / "mini-protein3_trp-cage.pdb.v2.2.1-3b2-deb_cv1.ssd"),
+            "CHHHHHHHTTGGGGTCCCCC",
+        ),
+        (
+            str(DSSP_SS_OUTPUT / "mini-protein3_trp-cage.pdb.v3.0.0-3b1-deb_cv1.ssd"),
+            "CHHHHHHHTTGGGGTCCCCC",
+        ),
+    ],
+)
+def test_read_dssp2(input_file, expected):
     """
     Test that :func:`vermouth.dssp.dssp.read_dssp2` returns the expected
     secondary structure sequence.
     """
-    with open(str(DSSP_OUTPUT)) as infile:
+    with open(input_file, encoding="utf-8") as infile:
         secondary_structure = dssp.read_dssp2(infile)
-    assert secondary_structure == SECSTRUCT_1BTA
+    assert "".join(secondary_structure) == expected
 
 
-@pytest.mark.parametrize('savefile', [True, False])
+@pytest.mark.parametrize("savefile", [True, False])
 def test_run_dssp(savefile, tmpdir):
     """
     Test that :func:`vermouth.molecule.dssp.dssp.run_dssp` runs as expected and
     generate a save file only if requested.
     """
     # The test runs twice, once with the savefile set to True so we test with
     # saving the DSSP output to file, and once with savefile set t False so we
     # do not generate the file. The "savefile" argument is set by
     # pytest.mark.parametrize.
     # The "tmpdir" argument is set by pytest and is the path to a temporary
     # directory that exists only for one iteration of the test.
     if savefile:
-        path = tmpdir.join('dssp_output')
+        path = tmpdir.join("dssp_output")
     else:
         path = None
     system = vermouth.System()
     for molecule in read_pdb(str(PDB_PROTEIN)):
         system.add_molecule(molecule)
-    secondary_structure = dssp.run_dssp(system,
-                                        executable=DSSP_EXECUTABLE,
-                                        savefile=path)
+    secondary_structure = dssp.run_dssp(
+        system, executable=DSSP_EXECUTABLE, savefile=path
+    )
 
     # Make sure we produced the expected sequence of secondary structures
     assert secondary_structure == SECSTRUCT_1BTA
 
     # If we test with savefile, then we need to make sure the file is created
     # and its content corresponds to the reference (excluding the first lines
     # that are variable or contain non-essencial data read from the PDB file).
     # If we test without savefile, then we need to make sure the file is not
     # created.
     if savefile:
         DeferredFileWriter().write()
         assert path.exists()
-        with open(str(path)) as genfile, open(str(DSSP_OUTPUT)) as reffile:
+        with open(str(path), encoding="utf-8") as genfile, open(
+            str(DSSP_OUTPUT), encoding="utf-8"
+        ) as reffile:
             # DSSP 3 is outputs mostly the same thing as DSSP2, though there
             # are some differences in non significant whitespaces, and an extra
             # field header. We need to normalize these differences to be able
             # to compare.
-            gen = '\n'.join([
-                line.strip().replace('            CHAIN', '')
-                for line in genfile.readlines()[6:]
-            ])
-            ref = '\n'.join([line.strip() for line in reffile.readlines()[6:]])
+            gen = "\n".join(
+                [
+                    line.strip().replace("            CHAIN", "")
+                    for line in genfile.readlines()[6:]
+                ]
+            )
+            ref = "\n".join([line.strip() for line in reffile.readlines()[6:]])
             assert gen == ref
     else:
         # Is the directory empty?
         assert not os.listdir(str(tmpdir))
 
 
-@pytest.mark.parametrize('pdb, loglevel,expected', [
-    (PDB_PROTEIN, 10, True),  # DEBUG
-    (PDB_PROTEIN, 30, False),  # WARNING
-    # Using a CG pdb will cause a DSSP error, which should preserve the input
-    (PDB_ALA5_CG, 10, True),  # DEBUG
-    (PDB_ALA5_CG, 30, True),  # WARNING
-])
+@pytest.mark.parametrize(
+    "pdb, loglevel,expected",
+    [
+        (PDB_PROTEIN, 10, True),  # DEBUG
+        (PDB_PROTEIN, 30, False),  # WARNING
+        # Using a CG pdb will cause a DSSP error, which should preserve the input
+        (PDB_ALA5_CG, 10, True),  # DEBUG
+        (PDB_ALA5_CG, 30, True),  # WARNING
+    ],
+)
 def test_run_dssp_input_file(tmpdir, caplog, pdb, loglevel, expected):
     """
     Test that the DSSP input file is preserved (only) in the right conditions
     """
     caplog.set_level(loglevel)
     system = vermouth.System()
     for molecule in read_pdb(str(pdb)):
@@ -386,61 +436,217 @@
             dssp.run_dssp(system, executable=DSSP_EXECUTABLE)
         except DSSPError:
             pass
         if expected:
             target = 1
         else:
             target = 0
-        matches = glob.glob('dssp_in*.pdb')
+        matches = glob.glob("dssp_in*.pdb")
         assert len(matches) == target, matches
         if matches:
             # Make sure it's a valid PDB file. Mostly anyway.
             list(read_pdb(matches[0]))
 
 
 def test_cterm_atomnames():
     nodes = [
-        dict(resname="ALA", atomname="N", element='N', resid=1, chain="", position=np.array([9.534, 5.359, 0.000])),
-        dict(resname="ALA", atomname="CA", element='C', resid=1, chain="", position=np.array([10.190, 6.661, -0.000])),
-        dict(resname="ALA", atomname="C", element='C', resid=1, chain="", position=np.array([11.706, 6.515, 0.000])),
-        dict(resname="ALA", atomname="O", element='O', resid=1, chain="", position=np.array([12.232, 5.403, 0.000])),
-        dict(resname="ALA", atomname="CB", element='C', resid=1, chain="", position=np.array([9.733, 7.484, 1.196])),
-        dict(resname="ALA", atomname="H", element='H', resid=1, chain="", position=np.array([10.101, 4.523, 0.000])),
-        dict(resname="ALA", atomname="HA", element='H', resid=1, chain="", position=np.array([9.914, 7.191, -0.912])),
-        dict(resname="ALA", atomname="1HB", element='H', resid=1, chain="", position=np.array([10.231, 8.454, 1.181])),
-        dict(resname="ALA", atomname="2HB", element='H', resid=1, chain="", position=np.array([8.654, 7.630, 1.147])),
-        dict(resname="ALA", atomname="3HB", element='H', resid=1, chain="", position=np.array([9.987, 6.960, 2.116])),
-
-        dict(resname="ALA", atomname="N", element='N', resid=2, chain="", position=np.array([12.404, 7.646, 0.000])),
-        dict(resname="ALA", atomname="CA", element='C', resid=2, chain="", position=np.array([13.862, 7.646, 0.000])),
-        dict(resname="ALA", atomname="C", element='C', resid=2, chain="", position=np.array([14.413, 9.066, 0.000])),
-        dict(resname="ALA", atomname="O1", element='O', resid=2, chain="", position=np.array([14.462, 9.691, 1.023])),
-        dict(resname="ALA", atomname="O2", element='O', resid=2, chain="", position=np.array([14.798, 9.560, -1.023])),
-        dict(resname="ALA", atomname="CB", element='C', resid=2, chain="", position=np.array([14.392, 6.868, -1.196])),
-        dict(resname="ALA", atomname="H", element='H', resid=2, chain="", position=np.array([11.912, 8.528, -0.000])),
-        dict(resname="ALA", atomname="HA", element='H', resid=2, chain="", position=np.array([14.212, 7.162, 0.912])),
-        dict(resname="ALA", atomname="1HB", element='H', resid=2, chain="", position=np.array([15.482, 6.878, -1.181])),
-        dict(resname="ALA", atomname="2HB", element='H', resid=2, chain="", position=np.array([14.038, 5.839, -1.147])),
-        dict(resname="ALA", atomname="3HB", element='H', resid=2, chain="", position=np.array([14.038, 7.331, -2.116])),
-
+        dict(
+            resname="ALA",
+            atomname="N",
+            element="N",
+            resid=1,
+            chain="",
+            position=np.array([9.534, 5.359, 0.000]),
+        ),
+        dict(
+            resname="ALA",
+            atomname="CA",
+            element="C",
+            resid=1,
+            chain="",
+            position=np.array([10.190, 6.661, -0.000]),
+        ),
+        dict(
+            resname="ALA",
+            atomname="C",
+            element="C",
+            resid=1,
+            chain="",
+            position=np.array([11.706, 6.515, 0.000]),
+        ),
+        dict(
+            resname="ALA",
+            atomname="O",
+            element="O",
+            resid=1,
+            chain="",
+            position=np.array([12.232, 5.403, 0.000]),
+        ),
+        dict(
+            resname="ALA",
+            atomname="CB",
+            element="C",
+            resid=1,
+            chain="",
+            position=np.array([9.733, 7.484, 1.196]),
+        ),
+        dict(
+            resname="ALA",
+            atomname="H",
+            element="H",
+            resid=1,
+            chain="",
+            position=np.array([10.101, 4.523, 0.000]),
+        ),
+        dict(
+            resname="ALA",
+            atomname="HA",
+            element="H",
+            resid=1,
+            chain="",
+            position=np.array([9.914, 7.191, -0.912]),
+        ),
+        dict(
+            resname="ALA",
+            atomname="1HB",
+            element="H",
+            resid=1,
+            chain="",
+            position=np.array([10.231, 8.454, 1.181]),
+        ),
+        dict(
+            resname="ALA",
+            atomname="2HB",
+            element="H",
+            resid=1,
+            chain="",
+            position=np.array([8.654, 7.630, 1.147]),
+        ),
+        dict(
+            resname="ALA",
+            atomname="3HB",
+            element="H",
+            resid=1,
+            chain="",
+            position=np.array([9.987, 6.960, 2.116]),
+        ),
+        dict(
+            resname="ALA",
+            atomname="N",
+            element="N",
+            resid=2,
+            chain="",
+            position=np.array([12.404, 7.646, 0.000]),
+        ),
+        dict(
+            resname="ALA",
+            atomname="CA",
+            element="C",
+            resid=2,
+            chain="",
+            position=np.array([13.862, 7.646, 0.000]),
+        ),
+        dict(
+            resname="ALA",
+            atomname="C",
+            element="C",
+            resid=2,
+            chain="",
+            position=np.array([14.413, 9.066, 0.000]),
+        ),
+        dict(
+            resname="ALA",
+            atomname="O1",
+            element="O",
+            resid=2,
+            chain="",
+            position=np.array([14.462, 9.691, 1.023]),
+        ),
+        dict(
+            resname="ALA",
+            atomname="O2",
+            element="O",
+            resid=2,
+            chain="",
+            position=np.array([14.798, 9.560, -1.023]),
+        ),
+        dict(
+            resname="ALA",
+            atomname="CB",
+            element="C",
+            resid=2,
+            chain="",
+            position=np.array([14.392, 6.868, -1.196]),
+        ),
+        dict(
+            resname="ALA",
+            atomname="H",
+            element="H",
+            resid=2,
+            chain="",
+            position=np.array([11.912, 8.528, -0.000]),
+        ),
+        dict(
+            resname="ALA",
+            atomname="HA",
+            element="H",
+            resid=2,
+            chain="",
+            position=np.array([14.212, 7.162, 0.912]),
+        ),
+        dict(
+            resname="ALA",
+            atomname="1HB",
+            element="H",
+            resid=2,
+            chain="",
+            position=np.array([15.482, 6.878, -1.181]),
+        ),
+        dict(
+            resname="ALA",
+            atomname="2HB",
+            element="H",
+            resid=2,
+            chain="",
+            position=np.array([14.038, 5.839, -1.147]),
+        ),
+        dict(
+            resname="ALA",
+            atomname="3HB",
+            element="H",
+            resid=2,
+            chain="",
+            position=np.array([14.038, 7.331, -2.116]),
+        ),
     ]
     edges = [
-        (0, 1), (0, 5),
-        (1, 2), (1, 4), (1, 6),
+        (0, 1),
+        (0, 5),
+        (1, 2),
+        (1, 4),
+        (1, 6),
         (2, 3),
-        (4, 7), (4, 8), (4, 9),
+        (4, 7),
+        (4, 8),
+        (4, 9),
         (2, 10),
-        (10, 11), (10, 16),
-        (11, 12), (11, 15), (11, 17),
-        (12, 13), (12, 14),
-        (15, 18), (15, 19), (15, 20),
+        (10, 11),
+        (10, 16),
+        (11, 12),
+        (11, 15),
+        (11, 17),
+        (12, 13),
+        (12, 14),
+        (15, 18),
+        (15, 19),
+        (15, 20),
     ]
-    ff = get_native_force_field('charmm')
+    ff = get_native_force_field("charmm")
     mol = vermouth.molecule.Molecule(force_field=ff)
     mol.add_nodes_from(enumerate(nodes))
     mol.add_edges_from(edges)
     system = vermouth.system.System(force_field=ff)
     system.add_molecule(mol)
     vermouth.processors.RepairGraph().run_system(system)
     vermouth.processors.CanonicalizeModifications().run_system(system)
     dssp_out = dssp.run_dssp(system, executable=DSSP_EXECUTABLE)
-    assert dssp_out == list('CC')
+    assert dssp_out == list("CC")
```

### Comparing `vermouth-0.9.1/vermouth/tests/test_edge_tuning.py` & `vermouth-0.9.3/vermouth/tests/test_edge_tuning.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_ff_files.py` & `vermouth-0.9.3/vermouth/tests/test_ff_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,34 @@
                                       'mass': 7.0}
         assert block.nodes['SC2'] == {'atomname': 'SC2', 'atype': 'P2',
                                       'resname': 'ALA', 'resid': 1,
                                       'charge_group': 3, 'custom': 4,
                                       'other': 'plop'}
 
     @staticmethod
+    def test_meta():
+        lines = """
+        [ moleculetype ]
+        XXX 1
+        [ meta ]
+        flag
+        key1 0.15 ;test
+        key2 value1 value2
+        """
+        lines = textwrap.dedent(lines).splitlines()
+        ff = vermouth.forcefield.ForceField(name='test_ff')
+        vermouth.ffinput.read_ff(lines, ff)
+        block = ff.blocks['XXX']
+        assert len(block.meta) == 3
+        assert block.meta['flag'] == None 
+        assert block.meta['key1'] == '0.15' 
+        assert block.meta['key2'] ==  ['value1', 'value2']
+        
+        
+    @staticmethod
     def test_fixed_number_interaction():
         """
         Define an interaction for which the number of atoms required is known.
         """
         lines = """
         [ moleculetype ]
         GLY 1
```

### Comparing `vermouth-0.9.1/vermouth/tests/test_ffinput.py` & `vermouth-0.9.3/vermouth/tests/test_ffinput.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_file_writer.py` & `vermouth-0.9.3/vermouth/tests/test_file_writer.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_forcefield.py` & `vermouth-0.9.3/vermouth/tests/test_forcefield.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_geometry.py` & `vermouth-0.9.3/vermouth/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_go_vs_includes.py` & `vermouth-0.9.3/vermouth/tests/test_go_vs_includes.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     molecule = Molecule()
     for residue_idx in range(n_residues):
         base_atom_idx = residue_idx * 2
         for relative_atom_idx, atomname in enumerate(('BB', 'SC1')):
             molecule.add_node(
                 base_atom_idx + relative_atom_idx,
                 resid=residue_idx,
+                _old_resid=residue_idx,
                 resname='XX',
                 atomname=atomname,
                 charge_group=base_atom_idx,
                 chain='A',
                 # Should be an array, but it is not relevant for the test
                 position=[0, 0, 0],
             )
```

### Comparing `vermouth-0.9.1/vermouth/tests/test_graph_utils.py` & `vermouth-0.9.3/vermouth/tests/test_graph_utils.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_grappa.py` & `vermouth-0.9.3/vermouth/tests/test_grappa.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_ismags.py` & `vermouth-0.9.3/vermouth/tests/test_ismags.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_itp_files.py` & `vermouth-0.9.3/vermouth/tests/test_itp_files.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_links.py` & `vermouth-0.9.3/vermouth/tests/test_links.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_logging.py` & `vermouth-0.9.3/vermouth/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_make_bonds.py` & `vermouth-0.9.3/vermouth/tests/test_make_bonds.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_map_input.py` & `vermouth-0.9.3/vermouth/tests/test_map_input.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_map_parser.py` & `vermouth-0.9.3/vermouth/tests/test_map_parser.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_mapping_integrative.py` & `vermouth-0.9.3/vermouth/tests/test_mapping_integrative.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_molecule.py` & `vermouth-0.9.3/vermouth/tests/test_molecule.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_name_moltype.py` & `vermouth-0.9.3/vermouth/tests/test_name_moltype.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_native_forcefield.py` & `vermouth-0.9.3/vermouth/tests/test_native_forcefield.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_ptm_detection.py` & `vermouth-0.9.3/vermouth/tests/test_ptm_detection.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_repair_graph.py` & `vermouth-0.9.3/vermouth/tests/test_repair_graph.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_section_parser.py` & `vermouth-0.9.3/vermouth/tests/test_section_parser.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_selectors.py` & `vermouth-0.9.3/vermouth/tests/test_selectors.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_set_molecule_meta.py` & `vermouth-0.9.3/vermouth/tests/test_set_molecule_meta.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_sort_molecule_atoms.py` & `vermouth-0.9.3/vermouth/tests/test_sort_molecule_atoms.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,19 +14,23 @@
 
 """
 Tests for the:class:`vermouth.processors.sort_molecule_atoms.SortMoleculeAtoms`
 processor.
 """
 
 import copy
+import pytest
 from vermouth import Molecule, SortMoleculeAtoms
 from vermouth.molecule import Interaction
 
-
-def test_sort_molecule_atoms():
+@pytest.mark.parametrize("target_attr", [
+    None,
+    "atomid",
+ ])
+def test_sort_molecule_atoms(target_attr):
     """
     Test the :class:`vermouth.processors.sort_molecule_atoms.SortMoleculeAtoms`
     processor in normal conditions.
     """
     molecule = Molecule()
     nodes = [
         (6, {'chain': 'C', 'resid': 2, 'resname': 'AA0', 'atomname': 'A5'}),
@@ -50,14 +54,17 @@
             Interaction(atoms=[0, 1, 2], parameters=['b', 'c'], meta={'a': 0}),
         ],
     }
 
     molecule.add_nodes_from(nodes)
     molecule.add_edges_from(edges)
     molecule.interactions = copy.copy(interactions)
+    edges = {frozenset((i, j)): data for i, j, data in edges}
 
-    processor = SortMoleculeAtoms()
+    processor = SortMoleculeAtoms(target_attr=target_attr)
     processor.run_molecule(molecule)
 
     assert list(molecule.nodes) == [5, 1, 4, 0, 3, 6, 2]
-    assert sorted(molecule.edges(data=True)) == edges
+    if target_attr:
+        [molecule.nodes[nidx][target_attr] for nidx in molecule] == list(range(len(molecule)))
+    assert {frozenset((i, j)): data for i, j, data in molecule.edges(data=True)} == edges
     assert molecule.interactions == interactions
```

### Comparing `vermouth-0.9.1/vermouth/tests/test_tune_cystein_bridges.py` & `vermouth-0.9.3/vermouth/tests/test_tune_cystein_bridges.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_utils.py` & `vermouth-0.9.3/vermouth/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/tests/test_version.py` & `vermouth-0.9.3/vermouth/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/truncating_formatter.py` & `vermouth-0.9.3/vermouth/truncating_formatter.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth/utils.py` & `vermouth-0.9.3/vermouth/utils.py`

 * *Files identical despite different names*

### Comparing `vermouth-0.9.1/vermouth.egg-info/PKG-INFO` & `vermouth-0.9.3/vermouth.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vermouth
-Version: 0.9.1
+Version: 0.9.3
 Home-page: https://github.com/marrink-lab/vermouth-martinize
 Author: P C Kroon
 Author-email: p.c.kroon@rug.nl
 License: Apache 2.0
 Keywords: martini MD martinize
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -81,14 +81,24 @@
 At the moment, martinize2 tries to reproduce the interface of the original
 Martinize. You can find explanations on how to use Martinize on the [Martini
 tutorials]; in most cases, replacing calls to `martinize.py` by calls to
 `martinize2` should produce similar results.
 
 The documentation of the vermouth python library will come soon.
 
+## Citation
+```
+@article{kroon2022martinize2,
+  title={Martinize2 and Vermouth: Unified Framework for Topology Generation},
+  author={Kroon, Peter C and Gr{\"u}newald, Fabian and Barnoud, Jonathan and van Tilburg, Marco 
+          and Souza, Paulo CT and Wassenaar, Tsjerk A and Marrink, Siewert-Jan},
+  journal={arXiv preprint arXiv:2212.01191},
+  year={2022}}
+```
+
 ## License
 
 Martinize2 and vermouth are distributed under the Apache 2.0 license.
 
     Copyright 2018 University of Groningen
 
 	Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `vermouth-0.9.1/vermouth.egg-info/SOURCES.txt` & `vermouth-0.9.3/vermouth.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -440,17 +440,23 @@
 vermouth/tests/data/1bta_mutated.pdb
 vermouth/tests/data/2QWO.pdb
 vermouth/tests/data/2dn2.pdb
 vermouth/tests/data/6E8W.pdb
 vermouth/tests/data/ala5.pdb
 vermouth/tests/data/ala5_cg.pdb
 vermouth/tests/data/dna-short.pdb
-vermouth/tests/data/dssp_1bta.ssd
 vermouth/tests/data/heme.pdb
 vermouth/tests/data/tri_alanine.pdb
+vermouth/tests/data/dssp_tests/dssp_1bta.ssd
+vermouth/tests/data/dssp_tests/mini-protein1_betasheet.pdb.v2.2.1-3b2-deb_cv1.ssd
+vermouth/tests/data/dssp_tests/mini-protein1_betasheet.pdb.v3.0.0-3b1-deb_cv1.ssd
+vermouth/tests/data/dssp_tests/mini-protein2_helix.pdb.v2.2.1-3b2-deb_cv1.ssd
+vermouth/tests/data/dssp_tests/mini-protein2_helix.pdb.v3.0.0-3b1-deb_cv1.ssd
+vermouth/tests/data/dssp_tests/mini-protein3_trp-cage.pdb.v2.2.1-3b2-deb_cv1.ssd
+vermouth/tests/data/dssp_tests/mini-protein3_trp-cage.pdb.v3.0.0-3b1-deb_cv1.ssd
 vermouth/tests/data/force_fields/martini-test/aminoacids.ff
 vermouth/tests/data/force_fields/pepplane/ala.ff
 vermouth/tests/data/force_fields/pepplane/general.ff
 vermouth/tests/data/force_fields/pepplane/modifications.ff
 vermouth/tests/data/force_fields/universal-test/aminoacids.rtp
 vermouth/tests/data/force_fields/universal-test/modifications.ff
 vermouth/tests/data/integration_tests/tier-0/dipro-termini/README
@@ -560,22 +566,36 @@
 vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/command
 vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/molecule_0.itp
 vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/screen.output
 vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/test.itp
 vermouth/tests/data/integration_tests/tier-1/lysozyme/martinize2/topol.top
 vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/README
 vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/aa.pdb
+vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/cg.pdb
+vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/chain_A.ssd
+vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/molecule_0.itp
+vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/topol.top
 vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/cg.pdb
 vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/chain_A.ssd
 vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/citation
 vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/command
 vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/molecule_0.itp
 vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/screen.output
 vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/test.itp
 vermouth/tests/data/integration_tests/tier-1/lysozyme_prot/martinize2/topol.top
+vermouth/tests/data/integration_tests/tier-1/prot_modf_charmm/README
+vermouth/tests/data/integration_tests/tier-1/prot_modf_charmm/input.pdb
+vermouth/tests/data/integration_tests/tier-1/prot_modf_charmm/martinize2/cg.pdb
+vermouth/tests/data/integration_tests/tier-1/prot_modf_charmm/martinize2/cg.top
+vermouth/tests/data/integration_tests/tier-1/prot_modf_charmm/martinize2/chain_.ssd
+vermouth/tests/data/integration_tests/tier-1/prot_modf_charmm/martinize2/citation
+vermouth/tests/data/integration_tests/tier-1/prot_modf_charmm/martinize2/command
+vermouth/tests/data/integration_tests/tier-1/prot_modf_charmm/martinize2/molecule_0.itp
+vermouth/tests/data/integration_tests/tier-1/prot_modf_charmm/martinize2/screen.output
+vermouth/tests/data/integration_tests/tier-1/prot_modf_charmm/martinize2/sys.top
 vermouth/tests/data/integration_tests/tier-1/villin/README
 vermouth/tests/data/integration_tests/tier-1/villin/aa.pdb
 vermouth/tests/data/integration_tests/tier-1/villin/martinize2/cg.pdb
 vermouth/tests/data/integration_tests/tier-1/villin/martinize2/citation
 vermouth/tests/data/integration_tests/tier-1/villin/martinize2/command
 vermouth/tests/data/integration_tests/tier-1/villin/martinize2/molecule_0.itp
 vermouth/tests/data/integration_tests/tier-1/villin/martinize2/screen.output
```

