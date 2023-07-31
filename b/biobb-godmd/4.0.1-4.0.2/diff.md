# Comparing `tmp/biobb_godmd-4.0.1.tar.gz` & `tmp/biobb_godmd-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biobb_godmd-4.0.1.tar", last modified: Thu Jul 27 11:11:51 2023, max compression
+gzip compressed data, was "dist/biobb_godmd-4.0.2.tar", last modified: Mon Jul 31 11:53:02 2023, max compression
```

## Comparing `biobb_godmd-4.0.1.tar` & `biobb_godmd-4.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/
--rw-r--r--   0 gbayarri (1147421021) 1791188573    11357 2023-04-11 11:37:10.000000 biobb_godmd-4.0.1/LICENSE
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1011 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573     5295 2023-07-27 11:10:07.000000 biobb_godmd-4.0.1/README.md
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/biobb_godmd/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       63 2023-07-27 11:09:06.000000 biobb_godmd-4.0.1/biobb_godmd/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/biobb_godmd/godmd/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       53 2023-04-11 11:37:10.000000 biobb_godmd-4.0.1/biobb_godmd/godmd/__init__.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     2281 2023-07-27 10:53:24.000000 biobb_godmd-4.0.1/biobb_godmd/godmd/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    16873 2023-04-12 10:26:31.000000 biobb_godmd-4.0.1/biobb_godmd/godmd/godmd_prep.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    16069 2023-07-27 10:53:24.000000 biobb_godmd-4.0.1/biobb_godmd/godmd/godmd_run.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/biobb_godmd.egg-info/
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1011 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/biobb_godmd.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573      383 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/biobb_godmd.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/biobb_godmd.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573      110 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/biobb_godmd.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       20 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/biobb_godmd.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       12 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/biobb_godmd.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2023-07-27 11:11:51.000000 biobb_godmd-4.0.1/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1495 2023-07-27 11:08:46.000000 biobb_godmd-4.0.1/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-07-31 11:53:02.000000 biobb_godmd-4.0.2/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11357 2023-04-11 11:37:10.000000 biobb_godmd-4.0.2/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1011 2023-07-31 11:53:02.000000 biobb_godmd-4.0.2/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5295 2023-07-31 11:48:04.000000 biobb_godmd-4.0.2/README.md
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-07-31 11:53:02.000000 biobb_godmd-4.0.2/biobb_godmd/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       63 2023-07-31 11:47:41.000000 biobb_godmd-4.0.2/biobb_godmd/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-07-31 11:53:02.000000 biobb_godmd-4.0.2/biobb_godmd/godmd/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       53 2023-04-11 11:37:10.000000 biobb_godmd-4.0.2/biobb_godmd/godmd/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2281 2023-07-27 10:53:24.000000 biobb_godmd-4.0.2/biobb_godmd/godmd/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    16841 2023-07-31 11:32:52.000000 biobb_godmd-4.0.2/biobb_godmd/godmd/godmd_prep.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    16003 2023-07-31 11:32:52.000000 biobb_godmd-4.0.2/biobb_godmd/godmd/godmd_run.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-07-31 11:53:02.000000 biobb_godmd-4.0.2/biobb_godmd.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1011 2023-07-31 11:53:02.000000 biobb_godmd-4.0.2/biobb_godmd.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      383 2023-07-31 11:53:02.000000 biobb_godmd-4.0.2/biobb_godmd.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-07-31 11:53:02.000000 biobb_godmd-4.0.2/biobb_godmd.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      110 2023-07-31 11:53:02.000000 biobb_godmd-4.0.2/biobb_godmd.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2023-07-31 11:53:02.000000 biobb_godmd-4.0.2/biobb_godmd.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       12 2023-07-31 11:53:02.000000 biobb_godmd-4.0.2/biobb_godmd.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-07-31 11:53:02.000000 biobb_godmd-4.0.2/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1495 2023-07-31 11:47:27.000000 biobb_godmd-4.0.2/setup.py
```

### Comparing `biobb_godmd-4.0.1/LICENSE` & `biobb_godmd-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_godmd-4.0.1/PKG-INFO` & `biobb_godmd-4.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobb_godmd
-Version: 4.0.1
+Version: 4.0.2
 Summary: Biobb_godmd is a BioBB category for GOdMD tool (protein conformational transitions).
 Home-page: https://github.com/bioexcel/biobb_godmd
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
 Project-URL: Documentation, http://biobb_godmd.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility Ensemble Protein Transitions GOdMD
```

### Comparing `biobb_godmd-4.0.1/README.md` & `biobb_godmd-4.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_godmd?label=Version)](https://GitHub.com/bioexcel/biobb_godmd/tags/)
 [![](https://img.shields.io/pypi/v/biobb-godmd.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-godmd/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_godmd?label=Conda)](https://anaconda.org/bioconda/biobb_godmd)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_godmd?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_godmd)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_godmd?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_godmd:4.0.1--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_godmd:4.0.2--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_godmd)
 [![](https://img.shields.io/pypi/pyversions/biobb-godmd.svg?label=Python%20Versions)](https://pypi.org/project/biobb-godmd/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_godmd)
 
 [![](https://readthedocs.org/projects/biobb-godmd/badge/?version=latest&label=Docs)](https://biobb-godmd.readthedocs.io/en/latest/?badge=latest)
@@ -30,61 +30,61 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb_godmd.readthedocs.io/en/latest/).
 
 ### Version
-v4.0.1 2023.2
+v4.0.2 2023.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
 
-        pip install "biobb_godmd>=4.0.1"
+        pip install "biobb_godmd>=4.0.2"
 
 
 * Usage: [Python API documentation](https://biobb-godmd.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_godmd>=4.0.1"
+        conda install -c bioconda "biobb_godmd>=4.0.2"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-godmd.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-godmd.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_godmd:4.0.1--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_godmd:4.0.2--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_godmd:4.0.1--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_godmd:4.0.2--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_godmd.sif https://depot.galaxyproject.org/singularity/biobb_godmd:4.0.1--pyhdfd78af_0
+        singularity pull --name biobb_godmd.sif https://depot.galaxyproject.org/singularity/biobb_godmd:4.0.2--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_godmd.sif <command>
```

### Comparing `biobb_godmd-4.0.1/biobb_godmd/godmd/common.py` & `biobb_godmd-4.0.2/biobb_godmd/godmd/common.py`

 * *Files identical despite different names*

### Comparing `biobb_godmd-4.0.1/biobb_godmd/godmd/godmd_prep.py` & `biobb_godmd-4.0.2/biobb_godmd/godmd/godmd_prep.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 """Module containing the GOdMDPrep class and the command line interface."""
 import argparse
-from pathlib import PurePath
+from pathlib import Path
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
 from biobb_godmd.godmd.common import check_input_path, check_output_path
 
 
@@ -21,14 +21,15 @@
         input_pdb_target_path (str): Input PDB file to be used as target in the conformational transition. File type: input. `Sample file <https://github.com/bioexcel/biobb_godmd/raw/master/biobb_godmd/test/data/godmd/4ake_A.pdb>`_. Accepted formats: pdb (edam:format_1476).
         output_aln_orig_path (str): Output GOdMD alignment file corresponding to the origin structure of the conformational transition. File type: output. `Sample file <https://github.com/bioexcel/biobb_godmd/raw/master/biobb_godmd/test/data/godmd/1ake_A.aln>`_. Accepted formats: aln (edam:format_2330), txt (edam:format_2330).
         output_aln_target_path (str): Output GOdMD alignment file corresponding to the target structure of the conformational transition. File type: output. `Sample file <https://github.com/bioexcel/biobb_godmd/raw/master/biobb_godmd/test/data/godmd/4ake_A.aln>`_. Accepted formats: aln (edam:format_2330), txt (edam:format_2330).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
             * **gapopen** (*float*) - (12.0) Standard gap penalty: score taken away when a gap is created.
             * **gapextend** (*float*) - (2.0) Penalty added to the standard gap penalty for each base or residue in the gap.
             * **datafile** (*str*) - ("EPAM250") Scoring matrix file used when comparing sequences.
+            * **binary_path** (*str*) - ("water") Binary path.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
             from biobb_godmd.godmd.godmd_prep import godmd_prep
@@ -98,17 +99,18 @@
                    'input_pdb_target_path': input_pdb_target_path},
             'out': {'output_aln_orig_path': output_aln_orig_path,
                     'output_aln_target_path': output_aln_target_path}
         }
 
         # Properties specific for BB
         self.properties = properties
-        self.gapopen = properties.get('gapopen', "12.0")
-        self.gapextend = properties.get('gapextend', "2.0")
+        self.gapopen = properties.get('gapopen', 12.0)
+        self.gapextend = properties.get('gapextend', 2.0)
         self.datafile = properties.get('datafile', "EPAM250")
+        self.binary_path = properties.get('binary_path', "water")
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     def check_data_params(self, out_log, out_err):
         """ Checks input/output paths correctness """
@@ -216,15 +218,15 @@
             if sseq[i] != '-':
                 idx2 += 1
             if qseq[i] == '-' or sseq[i] == '-':
                 continue
             resid_pairs += [(resids1[idx1], resids2[idx2])]
         # Check contents of the residues of the alignment
         if len(resid_pairs) == 0:  # Alignment file was empty or there was no possible matching residues between the PDBs
-            fu.log('Alignment file was empty or there was no possible matching residues between the PDBs' % self.tmp_folder, self.out_log)
+            fu.log('Alignment file was empty or there was no possible matching residues between the PDBs' % self.stage_io_dict["unique_dir"], self.out_log)
             return False, False
         else:
             return seq_id, resid_pairs
 
     @launchlogger
     def launch(self):
         """Launches the execution of the GOdMDPrep module."""
@@ -245,48 +247,44 @@
         # Generate sequence of first PDB
         seq1, resids1 = self.extract_sequence(pdb1)
 
         # Generate sequence of second PDB
         seq2, resids2 = self.extract_sequence(pdb2)
 
         if len(seq1) < 50:
-            fu.log('WARNING: Short sequence (ORIGIN)' % self.tmp_folder, self.out_log)
-            # print("short_sequence ORIGIN",len(seq1))
+            fu.log('WARNING: Short sequence (ORIGIN)' % self.stage_io_dict["unique_dir"], self.out_log)
         if len(seq2) < 50:
-            fu.log('WARNING: Short sequence (TARGET)' % self.tmp_folder, self.out_log)
-            # print("short_sequence TARGET",len(seq2))
-
-        # Creating temporary folder
-        self.tmp_folder = fu.create_unique_dir()
-        fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
+            fu.log('WARNING: Short sequence (TARGET)' % self.stage_io_dict["unique_dir"], self.out_log)
 
         # Produce FASTA files
-        fasta1Filename = str(PurePath(self.tmp_folder).joinpath(pdb1 + ".fa"))
+        name1 = "fasta1.fa"
+        name2 = "fasta2.fa"
+        fasta1Filename = str(Path(self.stage_io_dict["unique_dir"]).joinpath(name1))
         fasta1File = open(fasta1Filename, "w")
         fasta1File.write(">"+pdb1+"\n"+seq1)
         fasta1File.close()
-        fasta2Filename = str(PurePath(self.tmp_folder).joinpath(pdb2 + ".fa"))
+        fasta2Filename = str(Path(self.stage_io_dict["unique_dir"]).joinpath(name2))
         fasta2File = open(fasta2Filename, "w")
         fasta2File.write(">"+pdb2+"\n"+seq2)
         fasta2File.close()
 
-        waterFilename = str(PurePath(self.tmp_folder).joinpath("water_align.out"))
+        waterFilename = str(Path(self.stage_io_dict["unique_dir"]).joinpath("water_align.out"))
 
         # water -auto -outfile=water_align.out -asequence=1ake.chains.nolig.pdb.fa
         # -bsequence=4ake.chains.pdb.fa -gapopen=12 -gapextend=2
         # -datafile=EPAM250 -aformat=markx10
 
         # Command line
-        self.cmd = ["water",
+        self.cmd = [self.binary_path,
                     '-auto',
                     '-outfile', waterFilename,
                     '-asequence', fasta1Filename,
                     '-bsequence', fasta2Filename,
-                    '-gapopen', self.gapopen,
-                    '-gapextend', self.gapextend,
+                    '-gapopen', str(self.gapopen),
+                    '-gapextend', str(self.gapextend),
                     '-datafile', self.datafile,
                     '-aformat', "markx10"
                     ]
 
         # Run Biobb block
         self.run_biobb()
 
@@ -310,16 +308,15 @@
         aln2File.close()
 
         # Copy files to host
         self.copy_to_host()
 
         # remove temporary folder(s)
         self.tmp_files.extend([
-            self.stage_io_dict.get("unique_dir"),
-            self.tmp_folder
+            self.stage_io_dict.get("unique_dir")
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
```

### Comparing `biobb_godmd-4.0.1/biobb_godmd/godmd/godmd_run.py` & `biobb_godmd-4.0.2/biobb_godmd/godmd/godmd_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """Module containing the GOdMDRun class and the command line interface."""
 import argparse
 import shutil
 from pathlib import Path
 from pathlib import PurePath
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
-from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
 from biobb_godmd.godmd.common import check_input_path, check_output_path
 
 
 class GOdMDRun(BiobbObject):
     """
     | biobb_godmd GOdMDRun
@@ -165,48 +164,42 @@
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
         if self.check_restart():
             return 0
         self.stage_files()
 
-        # Creating temporary folder
-        self.tmp_folder = fu.create_unique_dir()
-        fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
-
         # Creating GOdMD input file
-        self.output_godmdin_path = self.create_godmdin(path=str(Path(self.tmp_folder).joinpath("godmd.in")))
+        self.output_godmdin_path = self.create_godmdin(path=str(Path(self.stage_io_dict["unique_dir"]).joinpath("godmd.in")))
 
         # Command line
         # discrete -i $fileName.in -pdbin $pdbch1 -pdbtarg $pdbch2 -ener $fileName.ene -trj $fileName.crd -p1 $alignFile1 -p2 $alignFile2 -o $fileName.log >& $fileName.out
-        self.cmd = [self.binary_path,
-                    # '-i', self.io_dict["in"]["input_config_path"],
-                    '-i', self.output_godmdin_path,
-                    '-pdbin', self.io_dict["in"]["input_pdb_orig_path"],
-                    '-pdbtarg', self.io_dict["in"]["input_pdb_target_path"],
-                    '-p1', self.io_dict["in"]["input_aln_orig_path"],
-                    '-p2', self.io_dict["in"]["input_aln_target_path"],
-                    '-o', self.io_dict["out"]["output_log_path"],
-                    '-ener', self.io_dict["out"]["output_ene_path"],
-                    '-trj', self.io_dict["out"]["output_trj_path"]
+        self.cmd = ['cd', self.stage_io_dict["unique_dir"], ';', self.binary_path,
+                    '-i', "godmd.in",
+                    '-pdbin', PurePath(self.stage_io_dict["in"]["input_pdb_orig_path"]).name,
+                    '-pdbtarg', PurePath(self.stage_io_dict["in"]["input_pdb_target_path"]).name,
+                    '-p1', PurePath(self.stage_io_dict["in"]["input_aln_orig_path"]).name,
+                    '-p2', PurePath(self.stage_io_dict["in"]["input_aln_target_path"]).name,
+                    '-o', PurePath(self.stage_io_dict["out"]["output_log_path"]).name,
+                    '-ener', PurePath(self.stage_io_dict["out"]["output_ene_path"]).name,
+                    '-trj', PurePath(self.stage_io_dict["out"]["output_trj_path"]).name
                     ]
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy outputs from temporary folder to output path
-        shutil.copy2("reference.pdb", PurePath(self.io_dict["out"]["output_pdb_path"]).name)
+        shutil.copy2(str(Path(self.stage_io_dict["unique_dir"]).joinpath("reference.pdb")), PurePath(self.io_dict["out"]["output_pdb_path"]))
 
         # Copy files to host
         self.copy_to_host()
 
         # remove temporary folder(s)
         self.tmp_files.extend([
             self.stage_io_dict.get("unique_dir"),
-            self.tmp_folder
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
```

### Comparing `biobb_godmd-4.0.1/biobb_godmd.egg-info/PKG-INFO` & `biobb_godmd-4.0.2/biobb_godmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobb-godmd
-Version: 4.0.1
+Version: 4.0.2
 Summary: Biobb_godmd is a BioBB category for GOdMD tool (protein conformational transitions).
 Home-page: https://github.com/bioexcel/biobb_godmd
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
 Project-URL: Documentation, http://biobb_godmd.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility Ensemble Protein Transitions GOdMD
```

### Comparing `biobb_godmd-4.0.1/setup.py` & `biobb_godmd-4.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_godmd",
-    version="4.0.1",
+    version="4.0.2",
     author="Biobb developers",
     author_email="adam.hospital@irbbarcelona.org",
     description="Biobb_godmd is a BioBB category for GOdMD tool (protein conformational transitions).",
     long_description="Biobb_godmd allows the calculation of protein conformational transitions using the GOdMD tool.",
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility Ensemble Protein Transitions GOdMD",
     url="https://github.com/bioexcel/biobb_godmd",
```

