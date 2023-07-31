# Comparing `tmp/FastaTransformer-0.0.13.tar.gz` & `tmp/FastaTransformer-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastaTransformer-0.0.13.tar", last modified: Tue Jul 18 21:41:29 2023, max compression
+gzip compressed data, was "FastaTransformer-0.0.14.tar", last modified: Mon Jul 31 17:52:49 2023, max compression
```

## Comparing `FastaTransformer-0.0.13.tar` & `FastaTransformer-0.0.14.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 21:41:29.380398 FastaTransformer-0.0.13/
--rw-rw-rw-   0        0        0     4272 2023-07-18 21:41:29.381415 FastaTransformer-0.0.13/PKG-INFO
--rw-rw-rw-   0        0        0     3703 2023-06-15 18:18:59.000000 FastaTransformer-0.0.13/README.md
--rw-rw-rw-   0        0        0      150 2023-05-30 20:49:19.000000 FastaTransformer-0.0.13/pyproject.toml
--rw-rw-rw-   0        0        0      729 2023-07-18 21:41:29.389429 FastaTransformer-0.0.13/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-18 21:41:29.336400 FastaTransformer-0.0.13/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 21:41:29.347400 FastaTransformer-0.0.13/src/CigarBreaker/
--rw-rw-rw-   0        0        0     7061 2023-06-15 17:45:36.000000 FastaTransformer-0.0.13/src/CigarBreaker/CigarBreaker.py
--rw-rw-rw-   0        0        0       39 2023-06-15 16:53:41.000000 FastaTransformer-0.0.13/src/CigarBreaker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 21:41:29.352396 FastaTransformer-0.0.13/src/FastaTransformer/
--rw-rw-rw-   0        0        0    50118 2023-07-18 21:36:59.000000 FastaTransformer-0.0.13/src/FastaTransformer/FastaTransformer.py
--rw-rw-rw-   0        0        0       99 2023-06-15 16:54:04.000000 FastaTransformer-0.0.13/src/FastaTransformer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 21:41:29.378397 FastaTransformer-0.0.13/src/FastaTransformer.egg-info/
--rw-rw-rw-   0        0        0     4272 2023-07-18 21:41:29.000000 FastaTransformer-0.0.13/src/FastaTransformer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-07-18 21:41:29.000000 FastaTransformer-0.0.13/src/FastaTransformer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 21:41:29.000000 FastaTransformer-0.0.13/src/FastaTransformer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-07-18 21:41:29.000000 FastaTransformer-0.0.13/src/FastaTransformer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 17:52:49.394036 FastaTransformer-0.0.14/
+-rw-rw-rw-   0        0        0     4218 2023-07-31 17:52:49.395037 FastaTransformer-0.0.14/PKG-INFO
+-rw-rw-rw-   0        0        0     3649 2023-07-28 16:36:50.000000 FastaTransformer-0.0.14/README.md
+-rw-rw-rw-   0        0        0      150 2023-05-30 20:49:19.000000 FastaTransformer-0.0.14/pyproject.toml
+-rw-rw-rw-   0        0        0      729 2023-07-31 17:52:49.400037 FastaTransformer-0.0.14/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 17:52:49.335035 FastaTransformer-0.0.14/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 17:52:49.347036 FastaTransformer-0.0.14/src/CigarBreaker/
+-rw-rw-rw-   0        0        0     7061 2023-06-15 17:45:36.000000 FastaTransformer-0.0.14/src/CigarBreaker/CigarBreaker.py
+-rw-rw-rw-   0        0        0       39 2023-06-15 16:53:41.000000 FastaTransformer-0.0.14/src/CigarBreaker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 17:52:49.352039 FastaTransformer-0.0.14/src/FastaTransformer/
+-rw-rw-rw-   0        0        0    52178 2023-07-28 21:28:07.000000 FastaTransformer-0.0.14/src/FastaTransformer/FastaTransformer.py
+-rw-rw-rw-   0        0        0      188 2023-07-18 21:50:42.000000 FastaTransformer-0.0.14/src/FastaTransformer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 17:52:49.392037 FastaTransformer-0.0.14/src/FastaTransformer.egg-info/
+-rw-rw-rw-   0        0        0     4218 2023-07-31 17:52:49.000000 FastaTransformer-0.0.14/src/FastaTransformer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-07-31 17:52:49.000000 FastaTransformer-0.0.14/src/FastaTransformer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 17:52:49.000000 FastaTransformer-0.0.14/src/FastaTransformer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-07-31 17:52:49.000000 FastaTransformer-0.0.14/src/FastaTransformer.egg-info/top_level.txt
```

### Comparing `FastaTransformer-0.0.13/PKG-INFO` & `FastaTransformer-0.0.14/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FastaTransformer
-Version: 0.0.13
+Version: 0.0.14
 Summary: This package helps resolve bioprogramming problems
 Home-page: https://github.com/Global-ASFV-Research-Alliance/FastaTransformer
 Author: MDinhobl
 Author-email: markdinhobl@gmail.com
 Project-URL: Bug Tracker, https://github.com/Global-ASFV-Research-Alliance/FastaTransformer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,14 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # FastaTransformer
 FastaTransformer is a python toolset containing fucntions to simplify the usage of .fasta files in analysis as well as transform them into useful states for other tools.
 
 ### Authors
-
 The primary author of the FastaTransformer package is [MDinhobl](https://github.com/MDinhobl).
 
 ## Major Functions
 The following list contains the most useful functions of FastaTransformer.
 
 ### Creating Data Folders
 
@@ -29,20 +28,19 @@
 1. **AlignmentBankToMatrixBank** - Take a folder of .fasta alignment files (such as one produced by **GeneBankToAlignmentBank**) and produce a folder of distance matricies using the [BioPython](https://biopython.org/docs/1.76/api/Bio.Phylo.TreeConstruction.html) package.
 1. **MatrixBankToClusterBank** - Take a folder of distance matricies and create a folder of clusters using [DBSCAN](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.DBSCAN.html).
 
 The functionality of the above tools are combined in  **CSVToAllBanks** - A tool that combines the functionality of **MakeGeneBank**, **GeneBankToAlignmentBank**, **AlignmentBankToMatrixBank**, and **MatrixBankToClusterBank** into one script.
 
 ### Other Tools
 
-1. **AlignmentChangeFinder** - Searches a folder of .fasta alignment files an searches for novel changes in several designated ('new') genomes compared to reference ('old') genomes. These results can be further refined by **AlignmentChangeFinderSelector** and **AlignmentChangeFinderCleanup**.
+1. **AlignmentChangeFinder** - Searches a folder of .fasta alignment files for novel changes in several designated ('new') genomes compared to reference ('old') genomes. These results can be further refined by **AlignmentChangeFinderCleanup**.
 1. **MatrixBankToAverageMatrix** - Take a folder of distance matricices and produce an 'average' distance matrix with weights.
 1. **MatrixBankStats** - Find the statistics of each gene in a folder of distance matricies, such as one produced by **AlignmentBankToMatrixBank**.
 1. **FastaDescriptionHunter** - A tool used to search the descriptions of fasta entries (everything following the ">") downloaded from the [NCBI Genbank](https://www.ncbi.nlm.nih.gov/genbank/) for information in specific categories. This is especially useful when trying to search for speicfic sequences after gathering a large number of accession sequences, such as when using [NCBI Batch Entrez](https://www.ncbi.nlm.nih.gov/sites/batchentrez). 
 
-
 ## Installation
 To install the latest version of FastaTransformer, use pip install:
 
     pip install FastaTransformer
 
 ## What is a .fasta file?
 A .fasta file is a text file format commonly used for storing sequence information for genomic analysis. Each .fasta file can contain information on multiple sequences. Each sequence includes the following information:
```

### Comparing `FastaTransformer-0.0.13/README.md` & `FastaTransformer-0.0.14/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # FastaTransformer
 FastaTransformer is a python toolset containing fucntions to simplify the usage of .fasta files in analysis as well as transform them into useful states for other tools.
 
 ### Authors
-
 The primary author of the FastaTransformer package is [MDinhobl](https://github.com/MDinhobl).
 
 ## Major Functions
 The following list contains the most useful functions of FastaTransformer.
 
 ### Creating Data Folders
 
@@ -15,20 +14,19 @@
 1. **AlignmentBankToMatrixBank** - Take a folder of .fasta alignment files (such as one produced by **GeneBankToAlignmentBank**) and produce a folder of distance matricies using the [BioPython](https://biopython.org/docs/1.76/api/Bio.Phylo.TreeConstruction.html) package.
 1. **MatrixBankToClusterBank** - Take a folder of distance matricies and create a folder of clusters using [DBSCAN](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.DBSCAN.html).
 
 The functionality of the above tools are combined in  **CSVToAllBanks** - A tool that combines the functionality of **MakeGeneBank**, **GeneBankToAlignmentBank**, **AlignmentBankToMatrixBank**, and **MatrixBankToClusterBank** into one script.
 
 ### Other Tools
 
-1. **AlignmentChangeFinder** - Searches a folder of .fasta alignment files an searches for novel changes in several designated ('new') genomes compared to reference ('old') genomes. These results can be further refined by **AlignmentChangeFinderSelector** and **AlignmentChangeFinderCleanup**.
+1. **AlignmentChangeFinder** - Searches a folder of .fasta alignment files for novel changes in several designated ('new') genomes compared to reference ('old') genomes. These results can be further refined by **AlignmentChangeFinderCleanup**.
 1. **MatrixBankToAverageMatrix** - Take a folder of distance matricices and produce an 'average' distance matrix with weights.
 1. **MatrixBankStats** - Find the statistics of each gene in a folder of distance matricies, such as one produced by **AlignmentBankToMatrixBank**.
 1. **FastaDescriptionHunter** - A tool used to search the descriptions of fasta entries (everything following the ">") downloaded from the [NCBI Genbank](https://www.ncbi.nlm.nih.gov/genbank/) for information in specific categories. This is especially useful when trying to search for speicfic sequences after gathering a large number of accession sequences, such as when using [NCBI Batch Entrez](https://www.ncbi.nlm.nih.gov/sites/batchentrez). 
 
-
 ## Installation
 To install the latest version of FastaTransformer, use pip install:
 
     pip install FastaTransformer
 
 ## What is a .fasta file?
 A .fasta file is a text file format commonly used for storing sequence information for genomic analysis. Each .fasta file can contain information on multiple sequences. Each sequence includes the following information:
```

### Comparing `FastaTransformer-0.0.13/setup.cfg` & `FastaTransformer-0.0.14/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2046 6173 7461 5472 616e 7366 6f72   = FastaTransfor
 00000020: 6d65 720d 0a76 6572 7369 6f6e 203d 2030  mer..version = 0
-00000030: 2e30 2e31 330d 0a61 7574 686f 7220 3d20  .0.13..author = 
+00000030: 2e30 2e31 340d 0a61 7574 686f 7220 3d20  .0.14..author = 
 00000040: 4d44 696e 686f 626c 0d0a 6175 7468 6f72  MDinhobl..author
 00000050: 5f65 6d61 696c 203d 206d 6172 6b64 696e  _email = markdin
 00000060: 686f 626c 4067 6d61 696c 2e63 6f6d 0d0a  hobl@gmail.com..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 5468  description = Th
 00000080: 6973 2070 6163 6b61 6765 2068 656c 7073  is package helps
 00000090: 2072 6573 6f6c 7665 2062 696f 7072 6f67   resolve bioprog
 000000a0: 7261 6d6d 696e 6720 7072 6f62 6c65 6d73  ramming problems
```

### Comparing `FastaTransformer-0.0.13/src/CigarBreaker/CigarBreaker.py` & `FastaTransformer-0.0.14/src/CigarBreaker/CigarBreaker.py`

 * *Files identical despite different names*

### Comparing `FastaTransformer-0.0.13/src/FastaTransformer/FastaTransformer.py` & `FastaTransformer-0.0.14/src/FastaTransformer/FastaTransformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -336,38 +336,46 @@
     
     if SpecialReference != None:
         if SpecialReference not in OldGenomeNames:
             print("SpecialReference Must be in OldGenomeNames, To Avoid Error SpecialReference set to None")
 
     my_files = glob.glob(AlignmentBank + '*')
     FinalFrame = pd.DataFrame(NewGenomeNames, columns=['id']).set_index('id')
+    NoHistoricGenes = []
+    NoNewGenes = []
     for fasta in my_files:
 
         #fasta = AlignmentBank+'B962L.fasta'
         gene = fasta.replace(AlignmentBank, "").replace(".fasta", "").replace(".fa", "")
 
         df = pd.DataFrame(columns=['id', 'sequence'])
         for Genome in SeqIO.parse(fasta,format='fasta'):
             df.loc[len(df.index)] = [Genome.description, str(Genome.seq)]
-
+        
         Old_df = df[df['id'].isin(OldGenomeNames)].set_index('id')
-
+        if len(Old_df) == 0:
+            NoHistoricGenes.append(gene)
+            continue
+        
         if SpecialReference != None:
             try:
                 Spec_Seq = df[df['id'] == SpecialReference].set_index('id').iloc[0]['sequence']
             except:
                 Spec_Seq = None
         else:
             Spec_Seq = None
 
         New_df = df[df['id'].isin(NewGenomeNames)].set_index('id')
-
-        #Checking for a destructive bug
-        if len(New_df) > len(FinalFrame):
-            print(str(gene) + "likely has duplicate genes. Results ommitted to prevent crash.")
+        if len(New_df) == 0:
+            NoNewGenes.append(gene)
+        
+        #Duplicate Entires Check
+        if len(df[df.duplicated(['id'], keep=False)]) > 0:
+            print("Gene " + gene + " contains duplicate entries, gene skipped to avoid crash.")
+            print(df[df.duplicated(['id'], keep=False)])
             continue
 
         AllSequences = []
         for sequence in list(map(''.join, zip(*Old_df['sequence']))):
             AllSequences.append('.'.join([i + "#" + str(sequence.count(i)) for i in set(sequence)]))
         
         def FindFlaw(Sequence, CompareSequences, Spec_Seq = None):
@@ -394,41 +402,23 @@
         try:
             results = pd.DataFrame()
             results[str(gene)] = New_df['sequence'].map(lambda x: FindFlaw(x, AllSequences, Spec_Seq))
             FinalFrame = pd.concat([FinalFrame,results], axis=1)
         except:
             print("Failed at Final Frame Concatonation at " + fasta)
             continue
-
-    return FinalFrame
-
-def AlignmentChangeFinderSelector(df, GeneList = None, DropNA = True):
     
-    """
-    A function that selects the specific outputs of the :func:`AlignmentChangeFinder` that are desired.
-
-    Parameters
-    ---
-    df : A dataframe constructed by :func:`AlignmentChangeFinder`.
-
-    Genelist : A list, or pd.Series object with a list of Genes to be kept. All other genes will be removed.
-
-    DropNa : Drop all genes only containing NaN entries. Does not include Genes that are empty because there were no genes missing in the Genomes and differences were not found.
-
-    Returns
-    ---
-    Returns a dataframe modified to remove values the user is not interested in.
-    """
-
-    if GeneList != None:
-        GeneList = InputToList(GeneList, 'Gene')
-        df = df[GeneList]
-    if DropNA == True:
-        df = df.dropna(how='all', axis=1)
-    return df
+    if len(NoHistoricGenes) > 0:
+        print("The following genes did not have a historic entry and were skipped: ")
+        print(NoHistoricGenes)
+    if len(NoNewGenes) > 0:
+        print("The following genes did not have a new entry, they were not skipped but their rows will have na. These can be removed in AlignmentChangeFinderCleanup by setting DropNA = True: ")
+        print(NoNewGenes)
+    
+    return FinalFrame
 
 def Rangemaker(info, FirstAA, FirstPositions):
         
         """
         A function for cleaning up a list object within a pd.DataFrame produced by :func:`AlignmentChangeFinder` into a more interpretable form. This function primarily exists for development purposes. To convert an entire pd.DataFrame, use its wrapper, :func:`AlignmentChangeFinderCleanup`.
 
         Parameters
@@ -491,39 +481,45 @@
                 OldCount = []
                 for OldEntry in Old:
                     OldAA.append(OldEntry.split('#')[0])
                     OldCount.append(int(OldEntry.split('#')[1]))
                 AAFirst.append(OldAA[OldCount.index(max(OldCount))])
         
         #Identify Ranges
-        from itertools import groupby
-        from operator import itemgetter
-        listdf = pd.DataFrame(list(zip(AAFirst, Positions, AALast)), columns=['AAFirst','Positions','AALast']).sort_values('Positions', ascending=True)    
-        data = sorted(set(Positions))
-        Ranges = []
-        for k, g in groupby(enumerate(data), lambda ix : ix[0] - ix[1]):
-            Rangedf = listdf.loc[listdf['Positions'].isin(list(map(itemgetter(1), g)))]
-
-            AAFirstRange = ''.join(list(Rangedf['AAFirst']))
-            if len(set(AAFirstRange)) == 1:
-                AAFirstRange = ''.join(set(AAFirstRange))
-            AALastRange = ''.join(list(Rangedf['AALast']))
-            if len(set(AALastRange)) == 1:
-                AALastRange = ''.join(set(AALastRange))
-            if AAFirstRange == "-":
-                AAFirstRange = "Ins"
-            if AALastRange == "-":
-                AALastRange = "Del"
-            if len(Rangedf) > 1:
-                Ranges.append(AAFirstRange + str(int(Rangedf['Positions'][0:1])) + "-" + str(int(Rangedf['Positions'][-1:])) + AALastRange)
-            else:
-                Ranges.append(AAFirstRange + str(int(Rangedf['Positions'][0:1])) + AALastRange)
-        return Ranges
+        
+        def RangeMakerInside(AAFirst, Positions, AALast):
+            from itertools import groupby
+            from operator import itemgetter
+            import pandas as pd
+            listdf = pd.DataFrame(list(zip(AAFirst, Positions, AALast)), columns=['AAFirst','Positions','AALast']).sort_values('Positions', ascending=True)    
+            data = sorted(set(Positions))
+            Ranges = []
+            for k, g in groupby(enumerate(data), lambda ix : ix[0] - ix[1]):
+                Rangedf = listdf.loc[listdf['Positions'].isin(list(map(itemgetter(1), g)))]
+
+                AAFirstRange = ''.join(list(Rangedf['AAFirst']))
+                if len(set(AAFirstRange)) == 1:
+                    AAFirstRange = ''.join(set(AAFirstRange))
+                AALastRange = ''.join(list(Rangedf['AALast']))
+                if len(set(AALastRange)) == 1:
+                    AALastRange = ''.join(set(AALastRange))
+                if AAFirstRange == "-":
+                    AAFirstRange = "Ins"
+                if AALastRange == "-":
+                    AALastRange = "Del"
+                
+                if len(Rangedf) > 1:
+                    Ranges.append(AAFirstRange + str(Rangedf['Positions'].iloc[0]) + "-" + str(Rangedf['Positions'].iloc[-1]) + AALastRange)
+                else:
+                    Ranges.append(AAFirstRange + str(Rangedf['Positions'].iloc[0]) + AALastRange)
+            return Ranges
+
+        return RangeMakerInside(AAFirst, Positions, AALast)
 
-def AlignmentChangeFinderCleanup(df, FirstAA = 'Ref', FirstPositions = 'Ref'):
+def AlignmentChangeFinderCleanup(df, FirstAA = 'Ref', FirstPositions = 'Ref', GeneList = None, DropNA = True):
     
     """
     A function for cleaning up a pd.DataFrame produced by :func:`AlignmentChangeFinder`. It is a wrapper for the :func:`Rangemaker` function, which should be viewed for further explanation.
 
     Parameters
     ---
     df : A pd.DataFrame constructed by :func:`AlignmentChangeFinder`.
@@ -537,19 +533,29 @@
     FirstPositions : Indicates which positional marker should be shown for the result. Options include:
 
         'Ref' : Use the position from the (RefPos) substring. Does not include gaps. Default option.
 
         'Self' : Use the data in the (SelfPos) substring. Does not include gaps.
 
         'Align' : Use the data in the (AlignPos) substring.
+        
+    Genelist : A list, or pd.Series object with a list of Genes to be kept. All other genes will be removed.
+
+    DropNa : Drop all genes only containing NaN entries. Does not include Genes that are empty because there were no genes missing in the Genomes and differences were not found.
 
     """
 
     import numpy as np
     import pandas as pd
+    
+    if GeneList != None:
+        GeneList = InputToList(GeneList, 'Gene')
+        df = df[GeneList]
+    if DropNA == True:
+        df = df.dropna(how='all', axis=1)
 
     def list2Str(lst, FirstAA, FirstPositions):
         if type(lst) is list: # apply conversion to list columns
             return ", ".join(map(str, Rangemaker(lst, FirstAA, FirstPositions)))
         else:
             return lst
     
@@ -722,36 +728,37 @@
 def MatrixBankAverageMaker(dfnumber, dflength, dflist, OutputFolder, CriticalGeneList, NonCriticalWeightList, PenaltyList, MinGenomesList, CounterEnd = 15, CounterInterval = 0.1):
     
     """
     A wrapper for the :func:`MatrixDataToAverageMatrix` and :func:`MatrixToCluster` specifications to perform analysis on a wide variety of samples.
     
     Parameters
     ---
-    dfnumber : returns a matrix, where each cell contains a list of the distances between two genomes across a number of genes.
+    dfnumber : returns a matrix, where each cell contains a list of the distances between two genomes across a number of genes. An output of :func:'MatrixBankToMatrixData'.
     
-    dflength : returns a matrix, where each cell contains a list of the number of genomes for each gene.
+    dflength : returns a matrix, where each cell contains a list of the number of genomes for each gene. An output of :func:'MatrixBankToMatrixData'.
     
-    dflist : returns a matrix, where each cell contains a list of the name of genes.
+    dflist : returns a matrix, where each cell contains a list of the name of genes. An output of :func:'MatrixBankToMatrixData'.
     
-    OutputFolder : 
+    OutputFolder : A string indicating the folder where the outputs should be placed.
     
     CriticalGeneList : A list of a list of Strings, Default None. Use the name as defined by the name used in the .csv file. Items indicated here will not be modified by NonCriticalWeight.
     
     NonCriticalWeightList : A list of numbers, Default 1. Genes not in the CriticalGene list will have thier weight equal to this number. A weight of 0 means genes not in the CriticalGene will not be weighted.
     
     PenaltyList : A list of numbers, Default 0. This number modifies the weight of a gne by the number of genomes present in it by an exponent equal to the number. For instance, a value of 0.5 would multiply the weight of each gene by the square root of how many genomes it has.
     
     MinGenomesList : A list of numbers, Default 0. This number is the minimum number of genomes a gene must appear in before being considered.
     
-    CounterEnd : 
-    
-    CounterInterval :
+    CounterEnd : Integer, default 15. How high the eps from DBSCAN should be calculated.
+
+    CounterInterval : Float, default 0.1. At what intervals the DBSCAN eps should be calculated.
     
     Returns
     ---
+    The folder will be filled with alignment and cluster files after running through all iterations.
     
     """
     
     import pandas as pd
 
     OutputFolder = FolderPathFixer(OutputFolder)
 
@@ -880,17 +887,16 @@
     
     dflist : returns a matrix, where each cell contains a list of the name of genes.
     
     """
 
     import pandas as pd
     import glob
-    import Programs.FastaTransformer.src.FastaTransformer.FastaTransformer as FastaTranformer
 
-    MatrixBank = FastaTranformer.FolderPathFixer(MatrixBank)
+    MatrixBank = FolderPathFixer(MatrixBank)
     my_files = glob.glob(MatrixBank + '*')
     
     GenomeList = []
     for file in my_files:
         dfactive = pd.read_csv(file, index_col=0)
         GenomeList.extend(list(dfactive.index))
     GenomeList = pd.unique(GenomeList)
@@ -916,46 +922,14 @@
                 dfnumber[item][name].append(float(row.values))
                 dflength[item][name].append(len(dfactive))
                 dflist[item][name].append(file.replace(MatrixBank, "").replace(".csv",""))
 
 
     return dfnumber, dflength, dflist
 
-def MatrixBankToAverageMatrix(MatrixBank, CriticalGene = None, NonCriticalWeight = 1, Penalty = 0, MinGenomes = 0):
-    """
-    A wrapper of :func:`MatrixBankToMatrixData` and :func:`MatrixDataToAverageMatrix`.
-    
-    Parameters
-    ---
-    
-    MatrixBank : String. A path to a folder, where the distance matricies for each gene will be contained as .csv files.
-    >>> Example
-    'Project_AD-Unique Protein Sequences in new Genomes\MatrixBank'
-    
-    CriticalGene : List of Strings, Default None. Use the name as defined by the name used in the .csv file. Items indicated here will not be modified by NonCriticalWeight.
-    >>> Example
-    ['285L','B646L']
-
-    NonCriticalWeight : A number, Default 1. Genes not in the CriticalGene list will have thier weight equal to this number. A weight of 0 means genes not in the CriticalGene will not be weighted.
-
-    Penalty : A number, Default 0. This number modifies the weight of a gne by the number of genomes present in it by an exponent equal to the number. For instance, a value of 0.5 would multiply the weight of each gene by the square root of how many genomes it has.
-
-    MinGenomes : A number, Default 0. This number is the minimum number of genomes a gene must appear in before being considered.
-    
-    Returns
-    ---
-    A pd.DataFrame of a distance matrix, with the distances being the weighted average of the matricies.
-    
-    """
-    
-    
-    dfnumber, dflength, dflist = MatrixBankToMatrixData(MatrixBank)
-    dfaverage = MatrixDataToAverageMatrix(dfnumber, dflength, dflist, CriticalGene, NonCriticalWeight, Penalty, MinGenomes)
-    return dfaverage
-
 def MatrixDataToAverageMatrix(MatrixNumbers, MatrixLengths, MatrixLists, CriticalGene = None, NonCriticalWeight = 1, Penalty = 0, MinGenomes = 0):
 
     """
     A function for generating an average matrix from a folder containing .csv matrix files such as one created by :func:`AlignmentBankToMatrixBank`. Returns a pandas DataFrame.
 
     Parameters
     ---
@@ -1007,14 +981,45 @@
         Weights = dfall.apply(lambda x: list(a*b for a,b in zip(x['a'], x['b'])), axis=1)
         dfall2 = pd.DataFrame(pd.concat([MatrixNumbers[item],Weights],axis=1))
         dfall2.columns = ['a', 'b']
         dfaverage[item] = dfall2.apply(lambda x: np.average(ast.literal_eval(x['a']), weights = x['b']), axis = 1) #np.average(x[0], weights = x[1])
 
     return dfaverage
 
+def MatrixBankToAverageMatrix(MatrixBank, CriticalGene = None, NonCriticalWeight = 1, Penalty = 0, MinGenomes = 0):
+    """
+    A wrapper of :func:`MatrixBankToMatrixData` and :func:`MatrixDataToAverageMatrix`.
+    
+    Parameters
+    ---
+    
+    MatrixBank : String. A path to a folder, where the distance matricies for each gene will be contained as .csv files.
+    >>> Example
+    'Project_AD-Unique Protein Sequences in new Genomes\MatrixBank'
+    
+    CriticalGene : List of Strings, Default None. Use the name as defined by the name used in the .csv file. Items indicated here will not be modified by NonCriticalWeight.
+    >>> Example
+    ['285L','B646L']
+
+    NonCriticalWeight : A number, Default 1. Genes not in the CriticalGene list will have thier weight equal to this number. A weight of 0 means genes not in the CriticalGene will not be weighted.
+
+    Penalty : A number, Default 0. This number modifies the weight of a gne by the number of genomes present in it by an exponent equal to the number. For instance, a value of 0.5 would multiply the weight of each gene by the square root of how many genomes it has.
+
+    MinGenomes : A number, Default 0. This number is the minimum number of genomes a gene must appear in before being considered.
+    
+    Returns
+    ---
+    A pd.DataFrame of a distance matrix, with the distances being the weighted average of the matricies.
+    
+    """
+    
+    dfnumber, dflength, dflist = MatrixBankToMatrixData(MatrixBank)
+    dfaverage = MatrixDataToAverageMatrix(dfnumber, dflength, dflist, CriticalGene, NonCriticalWeight, Penalty, MinGenomes)
+    return dfaverage
+
 def AlignmentToMatrix(fasta):
 
     """
     A wrapper of the :func:`Bio.Phylo.TreeConstruction.DistanceCalculator('identity').get_distance` function to take a .fasta alignment file and change it into a distance matrix. 
 
     Parameters
     ---
@@ -1046,14 +1051,16 @@
         df = df.apply(lambda x: 1-x)
     
     return df
 
 def MatrixToCluster(Matrix, CounterEnd = 15, CounterInterval = 0.1):
 
     """
+    A function that uses sklearn.clusters DBSCAN many times to create a series of increasingly large clusters.
+    
     Parameters
     ---
 
     Matrix : String of Path to a .csv file containing a distance matrix, or a pd.DataFrame of the matrix.
 
     CounterEnd : Integer, default 15. How high the eps from DBSCAN should be calculated.
 
@@ -1101,23 +1108,55 @@
     ---
     MatrixBank : A path to a folder, where the distance matricies for each gene are contained as .csv files.
     >>> Example
     'Project_AD-Unique Protein Sequences in new Genomes\MatrixBank'
     
     Returns
     ---
-    A pd.DataFrame consisting of the mean, median, standard deviation and number of genomes in each genes difference matrix.
+    A pd.DataFrame consisting of the mean, median, standard deviation and number of genomes in each genes distance matrix.
     """
     import pandas as pd
     import glob
     import numpy as np
     DF_Stats = pd.DataFrame(columns=['Mean', 'Median', 'StdDev', 'Count'])
     MatrixBank = FolderPathFixer(MatrixBank)
     my_files = glob.glob(MatrixBank + '*')
     for file in my_files:
         Numbers = []
         dfactive = pd.read_csv(file, index_col=0)
         for item in dfactive.index:
             Numbers.extend(list(dfactive[str(item)].values))
             Numbers.remove(1)
         DF_Stats.loc[str(file.replace(MatrixBank, "").replace(".csv",""))] = [np.mean(Numbers), np.median(Numbers), np.std(Numbers), int(len(dfactive))]
-    return DF_Stats
+    return DF_Stats
+
+### Deprecated Functions
+
+def AlignmentChangeFinderSelector(df, GeneList = None, DropNA = True):
+    
+    """
+    DEPRECATED
+    
+    A function that selects the specific outputs of the :func:`AlignmentChangeFinder` that are desired.
+
+    Parameters
+    ---
+    df : A dataframe constructed by :func:`AlignmentChangeFinder`.
+
+    Genelist : A list, or pd.Series object with a list of Genes to be kept. All other genes will be removed.
+
+    DropNa : Drop all genes only containing NaN entries. Does not include Genes that are empty because there were no genes missing in the Genomes and differences were not found.
+
+    Returns
+    ---
+    Returns a dataframe modified to remove values the user is not interested in.
+    """
+
+    print("Depreceated, please use AlignmentChangeFinderCleanup")
+    
+    if GeneList != None:
+        GeneList = InputToList(GeneList, 'Gene')
+        df = df[GeneList]
+    if DropNA == True:
+        df = df.dropna(how='all', axis=1)
+    return df
+
```

### Comparing `FastaTransformer-0.0.13/src/FastaTransformer.egg-info/PKG-INFO` & `FastaTransformer-0.0.14/src/FastaTransformer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FastaTransformer
-Version: 0.0.13
+Version: 0.0.14
 Summary: This package helps resolve bioprogramming problems
 Home-page: https://github.com/Global-ASFV-Research-Alliance/FastaTransformer
 Author: MDinhobl
 Author-email: markdinhobl@gmail.com
 Project-URL: Bug Tracker, https://github.com/Global-ASFV-Research-Alliance/FastaTransformer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,14 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # FastaTransformer
 FastaTransformer is a python toolset containing fucntions to simplify the usage of .fasta files in analysis as well as transform them into useful states for other tools.
 
 ### Authors
-
 The primary author of the FastaTransformer package is [MDinhobl](https://github.com/MDinhobl).
 
 ## Major Functions
 The following list contains the most useful functions of FastaTransformer.
 
 ### Creating Data Folders
 
@@ -29,20 +28,19 @@
 1. **AlignmentBankToMatrixBank** - Take a folder of .fasta alignment files (such as one produced by **GeneBankToAlignmentBank**) and produce a folder of distance matricies using the [BioPython](https://biopython.org/docs/1.76/api/Bio.Phylo.TreeConstruction.html) package.
 1. **MatrixBankToClusterBank** - Take a folder of distance matricies and create a folder of clusters using [DBSCAN](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.DBSCAN.html).
 
 The functionality of the above tools are combined in  **CSVToAllBanks** - A tool that combines the functionality of **MakeGeneBank**, **GeneBankToAlignmentBank**, **AlignmentBankToMatrixBank**, and **MatrixBankToClusterBank** into one script.
 
 ### Other Tools
 
-1. **AlignmentChangeFinder** - Searches a folder of .fasta alignment files an searches for novel changes in several designated ('new') genomes compared to reference ('old') genomes. These results can be further refined by **AlignmentChangeFinderSelector** and **AlignmentChangeFinderCleanup**.
+1. **AlignmentChangeFinder** - Searches a folder of .fasta alignment files for novel changes in several designated ('new') genomes compared to reference ('old') genomes. These results can be further refined by **AlignmentChangeFinderCleanup**.
 1. **MatrixBankToAverageMatrix** - Take a folder of distance matricices and produce an 'average' distance matrix with weights.
 1. **MatrixBankStats** - Find the statistics of each gene in a folder of distance matricies, such as one produced by **AlignmentBankToMatrixBank**.
 1. **FastaDescriptionHunter** - A tool used to search the descriptions of fasta entries (everything following the ">") downloaded from the [NCBI Genbank](https://www.ncbi.nlm.nih.gov/genbank/) for information in specific categories. This is especially useful when trying to search for speicfic sequences after gathering a large number of accession sequences, such as when using [NCBI Batch Entrez](https://www.ncbi.nlm.nih.gov/sites/batchentrez). 
 
-
 ## Installation
 To install the latest version of FastaTransformer, use pip install:
 
     pip install FastaTransformer
 
 ## What is a .fasta file?
 A .fasta file is a text file format commonly used for storing sequence information for genomic analysis. Each .fasta file can contain information on multiple sequences. Each sequence includes the following information:
```

