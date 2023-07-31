# Comparing `tmp/wormcat_batch-1.0.9.tar.gz` & `tmp/wormcat_batch-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wormcat_batch-1.0.9.tar", last modified: Mon Jul 31 12:07:09 2023, max compression
+gzip compressed data, was "wormcat_batch-1.1.0.tar", last modified: Mon Jul 31 21:03:05 2023, max compression
```

## Comparing `wormcat_batch-1.0.9.tar` & `wormcat_batch-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-31 12:07:09.574432 wormcat_batch-1.0.9/
--rw-r--r--   0 dan        (501) staff       (20)       95 2022-08-16 12:41:26.000000 wormcat_batch-1.0.9/MANIFEST.in
--rw-r--r--   0 dan        (501) staff       (20)      226 2023-07-31 12:07:09.574281 wormcat_batch-1.0.9/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)     2346 2023-06-28 11:53:36.000000 wormcat_batch-1.0.9/README.md
--rw-r--r--   0 dan        (501) staff       (20)       38 2023-07-31 12:07:09.574518 wormcat_batch-1.0.9/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)      691 2023-07-31 12:06:10.000000 wormcat_batch-1.0.9/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-31 12:07:09.573091 wormcat_batch-1.0.9/wormcat_batch/
--rw-r--r--   0 dan        (501) staff       (20)     2024 2022-08-16 12:41:26.000000 wormcat_batch-1.0.9/wormcat_batch/create_wormcat_xlsx.py
--rw-r--r--   0 dan        (501) staff       (20)     2486 2023-06-27 18:05:20.000000 wormcat_batch-1.0.9/wormcat_batch/execute_r.py
--rwxr-xr-x   0 dan        (501) staff       (20)       46 2022-08-16 12:41:26.000000 wormcat_batch-1.0.9/wormcat_batch/is_wormcat_installed.R
--rwxr-xr-x   0 dan        (501) staff       (20)     8365 2023-07-31 11:42:52.000000 wormcat_batch-1.0.9/wormcat_batch/run_wormcat_batch.py
--rwxr-xr-x   0 dan        (501) staff       (20)     1446 2022-08-16 12:41:26.000000 wormcat_batch-1.0.9/wormcat_batch/worm_cat.R
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-31 12:07:09.574113 wormcat_batch-1.0.9/wormcat_batch.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)      226 2023-07-31 12:07:09.000000 wormcat_batch-1.0.9/wormcat_batch.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      451 2023-07-31 12:07:09.000000 wormcat_batch-1.0.9/wormcat_batch.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-07-31 12:07:09.000000 wormcat_batch-1.0.9/wormcat_batch.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)       69 2023-07-31 12:07:09.000000 wormcat_batch-1.0.9/wormcat_batch.egg-info/entry_points.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-07-31 12:07:09.000000 wormcat_batch-1.0.9/wormcat_batch.egg-info/not-zip-safe
--rw-r--r--   0 dan        (501) staff       (20)       23 2023-07-31 12:07:09.000000 wormcat_batch-1.0.9/wormcat_batch.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)       14 2023-07-31 12:07:09.000000 wormcat_batch-1.0.9/wormcat_batch.egg-info/top_level.txt
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-31 21:03:05.353602 wormcat_batch-1.1.0/
+-rw-r--r--   0 dan        (501) staff       (20)       95 2022-08-16 12:41:26.000000 wormcat_batch-1.1.0/MANIFEST.in
+-rw-r--r--   0 dan        (501) staff       (20)      226 2023-07-31 21:03:05.353464 wormcat_batch-1.1.0/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)     2382 2023-07-31 16:03:44.000000 wormcat_batch-1.1.0/README.md
+-rw-r--r--   0 dan        (501) staff       (20)       38 2023-07-31 21:03:05.353643 wormcat_batch-1.1.0/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)      702 2023-07-31 21:01:44.000000 wormcat_batch-1.1.0/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-31 21:03:05.352328 wormcat_batch-1.1.0/wormcat_batch/
+-rw-r--r--   0 dan        (501) staff       (20)     2109 2023-07-31 17:33:31.000000 wormcat_batch-1.1.0/wormcat_batch/create_wormcat_xlsx.py
+-rw-r--r--   0 dan        (501) staff       (20)     2443 2023-07-31 16:16:50.000000 wormcat_batch-1.1.0/wormcat_batch/execute_r.py
+-rwxr-xr-x   0 dan        (501) staff       (20)       46 2022-08-16 12:41:26.000000 wormcat_batch-1.1.0/wormcat_batch/is_wormcat_installed.R
+-rwxr-xr-x   0 dan        (501) staff       (20)     8566 2023-07-31 20:54:46.000000 wormcat_batch-1.1.0/wormcat_batch/run_wormcat_batch.py
+-rwxr-xr-x   0 dan        (501) staff       (20)     1484 2023-07-31 16:25:55.000000 wormcat_batch-1.1.0/wormcat_batch/worm_cat.R
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-31 21:03:05.353299 wormcat_batch-1.1.0/wormcat_batch.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)      226 2023-07-31 21:03:05.000000 wormcat_batch-1.1.0/wormcat_batch.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      451 2023-07-31 21:03:05.000000 wormcat_batch-1.1.0/wormcat_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-07-31 21:03:05.000000 wormcat_batch-1.1.0/wormcat_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)       69 2023-07-31 21:03:05.000000 wormcat_batch-1.1.0/wormcat_batch.egg-info/entry_points.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-07-31 21:03:05.000000 wormcat_batch-1.1.0/wormcat_batch.egg-info/not-zip-safe
+-rw-r--r--   0 dan        (501) staff       (20)       32 2023-07-31 21:03:05.000000 wormcat_batch-1.1.0/wormcat_batch.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)       14 2023-07-31 21:03:05.000000 wormcat_batch-1.1.0/wormcat_batch.egg-info/top_level.txt
```

### Comparing `wormcat_batch-1.0.9/README.md` & `wormcat_batch-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 pip install .
 
 #### Test
 cd /Users/dan/delme #some working directory
 wormcat_cli --input-excel /Users/dan/Code/Python/Wormcat_batch/Example/Murphy_TS.xlsx --output-path ./output  
 
 #### Deploy
+advance version='1.0.9' in setup.py
 conda deactivate # twine is installed in base env
 cd in project directory
 rm -rf ./dist
 rm -rf ./wormcat_batch.egg-info
 python setup.py sdist
 twine check dist/*
 twine upload --repository pypi dist/*
```

### Comparing `wormcat_batch-1.0.9/setup.py` & `wormcat_batch-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 # rm -rf dist
 # python setup.py sdist
 #pip install dist/wormcat_batch-1.0.1.tar.gz
 # twine check dist/*
 # twine upload --repository pypi dist/*
 
 setup(name='wormcat_batch',
-      version='1.0.9',
+      version='1.1.0',
       description='Batch processing for Wormcat data',
       url='https://github.com/dphiggs01/Wormcat_batch',
       author='Dan Higgins',
       author_email='daniel.higgins@yahoo.com',
       license='MIT',
 
       packages=['wormcat_batch'],
-      install_requires=['pandas','xlrd','xlsxwriter'],
+      install_requires=['pandas','xlrd','xlsxwriter','openpyxl'],
       entry_points={
           'console_scripts': ['wormcat_cli=wormcat_batch.run_wormcat_batch:main'],
       },
       include_package_data=True,
       zip_safe=False)
```

### Comparing `wormcat_batch-1.0.9/wormcat_batch/create_wormcat_xlsx.py` & `wormcat_batch-1.1.0/wormcat_batch/create_wormcat_xlsx.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,24 +33,26 @@
     elif x >= 0.05:
         ret_val = 'NS'
     return ret_val
 
 
 def process_category_files(files_to_process, annotation_file, out_data_xlsx):
     data = pd.read_csv(annotation_file)
+    #writer = pd.ExcelWriter("{}".format(out_data_xlsx), engine='openpyxl')
     writer = pd.ExcelWriter("{}".format(out_data_xlsx), engine='xlsxwriter')
 
     #files_to_process = pd.read_csv("{}/files_to_process.csv".format(base_dir))
 
     sheets = files_to_process['sheet'].unique()
 
     for sheet_label in sheets:
         cat_files = files_to_process[files_to_process['sheet'] == sheet_label]
         label_category = "Category {}".format(cat_files['category'].iloc[0])
         category_sheet = create_category_summary(data, label_category)
         for index, row in cat_files.iterrows():
             category_sheet = process_category_file_row(row, category_sheet)
 
         category_sheet.to_excel(writer, sheet_name=sheet_label, index=False)
+        
 
     writer.save()
```

### Comparing `wormcat_batch-1.0.9/wormcat_batch/execute_r.py` & `wormcat_batch-1.1.0/wormcat_batch/execute_r.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,45 +4,45 @@
 import platform
 import logging
 
 logger = logging.getLogger()
 logger.setLevel(logging.DEBUG)
 
 class ExecuteR(object):
-    wormcat_r = '{}{}worm_cat.R'.format(os.path.dirname(__file__),os.path.sep)
+    wormcat_r = f'{os.path.dirname(__file__)}{os.path.sep}worm_cat.R'
 
     worm_cat_function = [wormcat_r,
                                '--file', 0,
                                '--title', 1,
                                '--out_dir', 2,
                                '--rm_dir', 3,
                                '--annotation_file',4,
-                               '--input_type', 5
+                               '--input_type', 5,
+                               '--zip_files', 6
                                ]
 
-    is_wormcat_installed = '{}{}is_wormcat_installed.R'.format(os.path.dirname(__file__),os.path.sep)
+    is_wormcat_installed = f'{os.path.dirname(__file__)}{os.path.sep}is_wormcat_installed.R'
     wormcat_library_path = [is_wormcat_installed, '--no-save', 0, '--quiet', 1]
 
     if platform.system() == 'Windows':
         wormcat_library_path.insert(0,'rscript.exe')
         worm_cat_function.insert(0,'rscript.exe')
 
 
     def wormcat_library_path_fun(self):
         ret_val = self.run(self.wormcat_library_path,"")
         return ret_val
 
-    def worm_cat_fun(self, file_name, out_dir, title="rgs", annotation_file="straight", input_type="Sequence ID"):
-        ret_val = self.run(self.worm_cat_function, file_name, title, out_dir, "False", annotation_file, input_type)
+    def worm_cat_fun(self, file_name, out_dir, title, annotation_file, input_type):
+        ret_val = self.run(self.worm_cat_function, file_name, title, out_dir, "False", annotation_file, input_type, "False")
         return ret_val
 
     def run(self, arg_list, *args):
         try:
             processed_args = self.process_args(arg_list, *args)
-            #print(f"R function: {processed_args}")
             process = Popen(processed_args, stdout=PIPE)
             out, err = process.communicate()
             out = str(out, 'utf-8')
             if not out:
                 out = None
             #sys.stderr.write("run: out={} err={}\n".format(out,err))
             return out
```

### Comparing `wormcat_batch-1.0.9/wormcat_batch/run_wormcat_batch.py` & `wormcat_batch-1.1.0/wormcat_batch/run_wormcat_batch.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,59 @@
 from wormcat_batch.execute_r import ExecuteR
 from wormcat_batch.create_wormcat_xlsx import process_category_files
 
 import warnings
 warnings.filterwarnings('ignore', category=UserWarning, module='openpyxl')
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
+# Create CSV Files from the given Excelsheet
+def extract_csv_files(input_excel_nm, csv_file_path):
+    input_excel = pd.ExcelFile(input_excel_nm)
+    for sheet in input_excel.sheet_names:
+        sheet_df = input_excel.parse(sheet)
+        sheet_df.to_csv(f'{csv_file_path}{os.path.sep}{sheet}.csv', index=False)
+
+        
+# Read CSV Files and call worm cat for each file
+def process_csv_files(csv_file_path, wormcat_out_path, annotation_file):
+    '''
+    Read the Excel file and process each sheet individually through Wormcat
+    '''
+    for dir_content in os.listdir(csv_file_path):
+        conetnt_full_path = os.path.join(csv_file_path, dir_content)
+        if os.path.isfile(conetnt_full_path):
+            with open(conetnt_full_path, 'r') as file:
+                header_line = file.readline().strip()
+            wormcat_input_type = header_line.replace(' ', '.')
+            csv_file_nm = os.path.basename(conetnt_full_path)
+            file_nm_wo_ext = csv_file_nm[:-4] # Remove .csv from file name
+            title = file_nm_wo_ext.replace('_', ' ')
+            wormcat_output_dir = f'{wormcat_out_path}{os.path.sep}{file_nm_wo_ext}'
+            executeR = ExecuteR()
+            executeR.worm_cat_fun(conetnt_full_path, wormcat_output_dir, title, annotation_file, wormcat_input_type)
+    return wormcat_out_path
+
+def create_summary_spreadsheet(wormcat_out_path, annotation_file, out_xsl_file_nm):
+    '''
+    After all the sheets on the Excel have been executed create a dataframe that can be used to summarize the results
+    this dataframe is used to create the output Excel
+    '''
+    process_lst = []
+    for dir_nm in os.listdir(wormcat_out_path):
+        for cat_num in [1,2,3]:
+            rgs_fisher = f"{wormcat_out_path}{os.path.sep}{dir_nm}{os.path.sep}rgs_fisher_cat{cat_num}.csv"
+            cat_nm = f"Cat{cat_num}"
+            row = {'sheet': cat_nm, 'category': cat_num, 'file': rgs_fisher,'label': dir_nm}
+            process_lst.append(row)
+
+    df_process = pd.DataFrame(process_lst, columns=['sheet', 'category', 'file','label'])
+    process_category_files(df_process, annotation_file, out_xsl_file_nm)
+
+## Wormcat Utility functions
+
 def get_wormcat_lib():
     '''
     Find the location where the R Wormcat program is installed
     '''
     executeR = ExecuteR()
     path = executeR.wormcat_library_path_fun()
     if path:
@@ -39,182 +84,122 @@
     index=1
     path = "{}{}extdata".format(path, os.path.sep)
     for root, dirs, files in os.walk(path):
         for filename in files:
             category_files.append(filename)
             index +=1
 
-    return category_files, path
-
-def call_wormcat(name, gene_ids, output_dir, annotation_file, input_type):
-    '''
-    Call the R Wormcat program.
-    The input "gene_ids" is provided as a csv file.
-    The output of the Wormcat R program is a directory containing the results and a zip of the directory.
-    The clean-up process moves the results output to an aggregation directory and deletes the input csv and the zip file.
-    '''
-    # input_type = 'Wormbase.ID'
-    file_nm = f"{name}.csv"
-    dir_nm = f"{name}"
-    title = dir_nm.replace('_', ' ')
-
-    gene_ids = gene_ids.to_frame(name=input_type)
-    # gene_ids.to_csv(file_nm, encoding='utf-8', index=False)
-    gene_ids.to_csv(file_nm, index=False)
-
-    executeR = ExecuteR()
-    executeR.worm_cat_fun(file_nm, dir_nm, title, annotation_file, input_type)
-
-    # Clean up
-    mv_dir = file_nm.replace(".csv", "")
-    os.rename(mv_dir, f"{output_dir}{os.path.sep}{mv_dir}")
-    if os.path.exists(file_nm):
-        os.remove(file_nm)
-    if os.path.exists(f"{dir_nm}.zip"):
-        os.remove(f"{dir_nm}.zip")
-    
-
-def process_spreadsheet(xsl_file_nm, output_dir, annotation_file):
-    '''
-    Read the Excel file and process each sheet individually through Wormcat
-    '''
-    xl = pd.ExcelFile(xsl_file_nm)
-    for sheet in xl.sheet_names:
-        print(f"Processing sheet {sheet}")
-        df = xl.parse(sheet)
-        if 'Wormbase ID' in df.columns:
-            gene_id_all = df['Wormbase ID']
-            input_type = 'Wormbase.ID'
-        elif 'Sequence ID' in df.columns:
-            gene_id_all = df['Sequence ID']
-            input_type = 'Sequence.ID'
-        else:
-            print("ERROR: You must provide column names with either 'Sequence ID' or 'Wormbase ID")
-            exit(-1)
-
-        call_wormcat(sheet, gene_id_all, output_dir, annotation_file, input_type)
-
-def files_to_process(output_dir):
-    '''
-    After all the sheets on the Excel have been executed create a dataframe that can be used to summarize the results
-    this dataframe is used to create the output Excel
-    '''
-    process_lst = []
-    for dir_nm in os.listdir(output_dir):
-        for cat_num in [1,2,3]:
-            rgs_fisher = f"{output_dir}{os.path.sep}{dir_nm}{os.path.sep}rgs_fisher_cat{cat_num}.csv"
-            cat_nm = f"Cat{cat_num}"
-            row = {'sheet': cat_nm, 'category': cat_num, 'file': rgs_fisher,'label': dir_nm}
-            process_lst.append(row)
-
-    df_process = pd.DataFrame(process_lst, columns=['sheet', 'category', 'file','label'])
-    return df_process
+    return category_files
 
-##########################################################
 ## Utility functions
 
-def move_file_to_output_directory(file_path, output_directory,copy=False):
-    '''
-    Utility function to move or copy a file to a different directory
-    '''
-    file_name = os.path.basename(file_path)
-    destination_path = os.path.join(output_directory, file_name)
-    if copy:
-        shutil.copy(file_path, destination_path)
-    else:
-        shutil.move(file_path, destination_path)
-
-
-
-def create_directory_with_backup(directory):
+def create_directory(directory, with_backup=False):
     '''
-    Utility function to create a directory and backuo the original if it exists
+    Utility function to create a directory and backup the original if it exists and has content
     '''
-    if os.path.exists(directory):
-        print(f"directory Exists [{directory}]")
+    if with_backup and os.path.exists(directory) and os.listdir(directory):
+        print(f"Directory exists with content [{directory}]")
         # Create backup directory name with a unique timestamp suffix
         timestamp = datetime.now().strftime("%Y%m%d-%H%M%S")
         backup_dir = f"{directory}_{timestamp}.bk"
         # Create a backup of the existing directory
-        shutil.copytree(directory, backup_dir)
+        shutil.move(directory, backup_dir)
 
     # Create a new empty directory
     os.makedirs(directory, exist_ok=True)
 
-def zip_directory(directory_path, zip_name):
-    '''
-    Utility function to recursivley compress a directory and it subdirectories
-    '''
-    parent_dir = os.path.dirname(directory_path)
-    zip_path = os.path.join(parent_dir, zip_name)
-    os.rename(directory_path, zip_path)
-
-    output_path = zip_path.rstrip(os.sep) + '.zip'  # Output zip file path
-    with zipfile.ZipFile(output_path, 'w', compression=zipfile.ZIP_DEFLATED) as zipf:
-        for root, dirs, files in os.walk(zip_path):
+def zip_directory(directory_path, zip_file_name):
+    with zipfile.ZipFile(zip_file_name, 'w') as zipf:
+        for root, _, files in os.walk(directory_path):
             for file in files:
                 file_path = os.path.join(root, file)
-                rel_path = os.path.relpath(file_path, zip_path)  # Get relative path
-                zipf.write(file_path, arcname=rel_path)
-    return output_path
+                zipf.write(file_path, os.path.relpath(file_path, directory_path))
+
 
 ##########################################################
 
 def main():
     print("Wormcat Batch")
     parser = argparse.ArgumentParser()
-    help_statement="wormcat_cli --input-excel <full_path_to_excel> --output-path <full_path_to_out_dir> --backup-output-path True --annotation-file-nm 'whole_genome_v2_nov-11-2021.csv' "
-    parser.add_argument('-i', '--input-excel', help='Inputfile in Excel format')
+    help_statement="wormcat_cli --input-excel <path_to_excel> | --input-csv-path <path_to_csv> --output-path <path_to_out_dir> --annotation-file 'whole_genome_v2_nov-11-2021.csv' --clean-temp False"
+    parser.add_argument('-i', '--input-excel', help='Input file in Excel/Wormcat format')
+    parser.add_argument('-c', '--input-csv-path', help='Input path to a collection of CSV files in Wormcat format')
     parser.add_argument('-o', '--output-path', help='Output path')
-    parser.add_argument('-b', '--backup-output-path', default=True, help='Backup or create outpath path if it does not exists')
-    parser.add_argument('-a', '--annotation-file-nm', default='whole_genome_v2_nov-11-2021.csv', help='Annotation file name')
+    parser.add_argument('-a', '--annotation-file', default='whole_genome_v2_nov-11-2021.csv', help='Annotation file name or path default=whole_genome_v2_nov-11-2021.csv')
+    parser.add_argument('-t', '--clean-temp', default=False, help='Remove files created while processing default=False')
 
     parser.add_argument('-v', '--version', action='version', version=f'%(prog)s v{importlib.metadata.version("wormcat_batch")}')
     args = parser.parse_args()
 
-    if not args.input_excel:
+    if not args.input_excel and not args.input_csv_path:
         print(help_statement)
-        print("Inputfile in Excel format is missing.")
+        print("An Excel Input file or a path to CSV files is required.")
         return
 
     if not args.output_path:
         print(help_statement)
-        print("Output path is missing")
+        print("Output path is required.")
         return
 
-    wormcat_path = get_wormcat_lib()
-    annotation_files, path = get_category_files(wormcat_path)
-
-    if not args.annotation_file_nm or not args.annotation_file_nm in annotation_files:
-        print(help_statement)
-        print("Missing or incorrect annotation-file-nm.")
-        print("Available names: {}".format(annotation_files))
-        return
- 
-    # Rest of your program logic goes here
+    if os.path.sep in args.annotation_file:
+        # Assume we are given a path to an external Annotation file
+        annotation_file_path = args.annotation_file
+    else:
+        wormcat_path = get_wormcat_lib()
+        annotation_files = get_category_files(wormcat_path)
+         
+        if not args.annotation_file or not args.annotation_file in annotation_files:
+            print(help_statement)
+            print("Missing or incorrect annotation-file-nm.")
+            print("Available names: {}".format(annotation_files))
+            return
+        annotation_file_path = f"{wormcat_path}{os.path.sep}extdata{os.path.sep}{args.annotation_file}"
+    
     print("Input Excel:", args.input_excel)
+    print("Input CSV Path:", args.input_csv_path)
     print("Output Path:", args.output_path)
-    print("Backup Path:", args.backup_output_path)
-    print("Annotation File Nm:", args.annotation_file_nm)
-    
-    # Add output to a temp_output director
-    temp_output_path= f".{os.path.sep}temp_output"
-    create_directory_with_backup(temp_output_path)
-
-    process_spreadsheet(args.input_excel, temp_output_path, args.annotation_file_nm)
-    base_input_excel = os.path.basename(args.input_excel)
-    input_excel_no_ext = os.path.splitext(base_input_excel)[0]
-
-    out_xsl_file_nm=f"{temp_output_path}{os.path.sep}Out_{base_input_excel}"
+    print("Annotation File:", args.annotation_file)
 
-    annotation_file =f"{path}{os.path.sep}{args.annotation_file_nm}"
-    df_process = files_to_process(temp_output_path)
-    process_category_files(df_process, annotation_file, out_xsl_file_nm)
-    move_file_to_output_directory(args.input_excel, temp_output_path,copy=True)
-    
+    # Create the output directory if it does not exsist
+    # Create a backup of the directory if it does exist and has content
+    create_directory(args.output_path, with_backup=True)
+
+    # If needed Extract the sreadsheet data
+    if args.input_csv_path:
+        csv_file_path = args.input_csv_path
+    else:
+        # Create a directory to extrat the Spreadsheet data into CSV
+        csv_file_path = f"{args.output_path}{os.path.sep}csv_files"
+        create_directory(csv_file_path)
+        extract_csv_files(args.input_excel, csv_file_path)
+
+    # Create a directory based on the Excel file name or CSV directory and a timestamp
+    # Wormcat processing will write to this directory
+    if args.input_excel:
+        base_input_excel = os.path.basename(args.input_excel)
+        input_data_nm = os.path.splitext(base_input_excel)[0]
+    else:
+        input_data_nm = os.path.basename(args.input_csv_path)
     timestamp = datetime.now().strftime("%Y%m%d-%H%M%S")
-    zip_dir_nm = f"{input_excel_no_ext}_{timestamp}"
-    output_zip = zip_directory(temp_output_path, zip_dir_nm)
-    move_file_to_output_directory(output_zip, args.output_path)
+    output_base_dir =f"{input_data_nm}_{timestamp}"
+    wormcat_out_path = f"{args.output_path}{os.path.sep}{output_base_dir}"
+    create_directory(wormcat_out_path)
+
+    # Call wormcat on each CSV file
+    process_csv_files(csv_file_path, wormcat_out_path, args.annotation_file)
+
+    # Create a summary spreadsheet of all CSV runs
+    out_xsl_file_nm = f"{wormcat_out_path}{os.path.sep}Out_{input_data_nm}.xlsx"
+    create_summary_spreadsheet(wormcat_out_path, annotation_file_path, out_xsl_file_nm)
+    
+    # Zip the results
+    zip_dir_nm = f"{args.output_path}{os.path.sep}{output_base_dir}.zip"
+    zip_directory(wormcat_out_path, zip_dir_nm)
+    
+    # If set Remove files created while processing
+    if args.clean_temp:
+        shutil.rmtree(wormcat_out_path)
+        if args.input_excel:
+            shutil.rmtree(csv_file_path)
 
 if __name__ == '__main__':
     main()
```

### Comparing `wormcat_batch-1.0.9/wormcat_batch/worm_cat.R` & `wormcat_batch-1.1.0/wormcat_batch/worm_cat.R`

 * *Files 24% similar despite different names*

```diff
@@ -2,43 +2,39 @@
 
 suppressPackageStartupMessages(library("wormcat"))
 suppressPackageStartupMessages(library("argparse"))
 
 # create parser object
 parser <- ArgumentParser()
 
-parser$add_argument("-f", "--file", help="File to be processed")
+parser$add_argument("-f", "--file", help = "File to be processed")
 
-parser$add_argument("-t", "--title", default="rgs",
-    help="Title for the graph")
+parser$add_argument("-t", "--title", default = "rgs", help = "Title for the graph")
 
-parser$add_argument("-o", "--out_dir", default="./worm_cat_output",
-    help="The output directory")
+parser$add_argument("-o", "--out_dir", default = "./worm_cat_output", help = "The output directory")
 
-parser$add_argument("-a", "--annotation_file", default="physiology_nov-24-2018.csv",
-    help="Provide the Annotation file {'straight_mmm-DD-YYYY.csv', 'physiology_mmm-DD-YYYY.csv'} [default]")
+parser$add_argument("-a", "--annotation_file", default="physiology_nov-24-2018.csv", help="Provide the Annotation file {'straight_mmm-DD-YYYY.csv', 'physiology_mmm-DD-YYYY.csv'} [default]")
 
-parser$add_argument("-i", "--input_type", default="Sequence ID",
-    help="Provide the Input type {'Sequence.ID', 'Wormbase.ID'} [default]")
+parser$add_argument("-i", "--input_type", default="Sequence ID", help = "Provide the Input type {'Sequence.ID', 'Wormbase.ID'} [default]")
 
-parser$add_argument("-r", "--rm_dir", default=TRUE,
-    help="Remove temp directory [default]")
+parser$add_argument("-r", "--rm_dir", default=TRUE, help="Remove temp directory [default]")
+
+parser$add_argument("-z", "--zip_files", default=TRUE, help="Create a zip file of the results directory [default]")
 
 args <- parser$parse_args()
 
 if (is.null(args$file)){
   stop("At least one argument must be supplied (input file).n", call.=FALSE)
 }
 
-print(paste("worm_cat_fun", args$file, args$title, args$out_dir, args$rm_dir, args$annotation_file, args$input_type))
+print(paste("worm_cat_fun", args$file, args$title, args$out_dir, args$rm_dir, args$annotation_file, args$input_type, args$zip_files))
+
 worm_cat_fun(
-    file_to_process=args$file,
-    title=args$title,
-    output_dir=args$out_dir,
-    rm_dir=args$rm_dir,
-    annotation_file=args$annotation_file,
-    input_type=args$input_type
+    file_to_process = args$file,
+    title = args$title,
+    output_dir = args$out_dir,
+    rm_dir = args$rm_dir,
+    annotation_file = args$annotation_file,
+    input_type = args$input_type,
+    zip_files = args$zip_files
 )
 
-# After processing move file to web accessable directory
-#file.rename(args$out_dir, paste("../gruber_data/",args$out_dir, sep=""))
-
```

