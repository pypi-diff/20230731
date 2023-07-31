# Comparing `tmp/datarails-0.3.2.tar.gz` & `tmp/datarails-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datarails-0.3.2.tar", last modified: Mon Jul 31 13:52:43 2023, max compression
+gzip compressed data, was "datarails-0.3.3.tar", last modified: Mon Jul 31 19:43:14 2023, max compression
```

## Comparing `datarails-0.3.2.tar` & `datarails-0.3.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:52:43.645198 datarails-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-31 13:52:20.000000 datarails-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-31 13:52:43.645198 datarails-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-31 13:52:33.000000 datarails-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:52:43.645198 datarails-0.3.2/datarails/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 13:52:33.000000 datarails-0.3.2/datarails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-31 13:52:20.000000 datarails-0.3.2/datarails/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-31 13:52:20.000000 datarails-0.3.2/datarails/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-31 13:52:20.000000 datarails-0.3.2/datarails/step.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 13:52:20.000000 datarails-0.3.2/datarails/type_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:52:43.645198 datarails-0.3.2/datarails.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-31 13:52:43.000000 datarails-0.3.2/datarails.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-31 13:52:43.000000 datarails-0.3.2/datarails.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 13:52:43.000000 datarails-0.3.2/datarails.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-31 13:52:43.000000 datarails-0.3.2/datarails.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-31 13:52:43.000000 datarails-0.3.2/datarails.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-31 13:52:33.000000 datarails-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 13:52:43.645198 datarails-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-31 13:52:20.000000 datarails-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:52:43.645198 datarails-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-31 13:52:20.000000 datarails-0.3.2/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-31 13:52:20.000000 datarails-0.3.2/tests/test_databox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-31 13:52:20.000000 datarails-0.3.2/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-31 13:52:20.000000 datarails-0.3.2/tests/test_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:43:14.165879 datarails-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-31 19:42:48.000000 datarails-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-07-31 19:43:14.165879 datarails-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-07-31 19:43:02.000000 datarails-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:43:14.165879 datarails-0.3.3/datarails/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 19:43:02.000000 datarails-0.3.3/datarails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-31 19:42:48.000000 datarails-0.3.3/datarails/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-31 19:42:48.000000 datarails-0.3.3/datarails/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-31 19:42:48.000000 datarails-0.3.3/datarails/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 19:42:48.000000 datarails-0.3.3/datarails/type_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:43:14.165879 datarails-0.3.3/datarails.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-07-31 19:43:14.000000 datarails-0.3.3/datarails.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-31 19:43:14.000000 datarails-0.3.3/datarails.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:43:14.000000 datarails-0.3.3/datarails.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-31 19:43:14.000000 datarails-0.3.3/datarails.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-31 19:43:14.000000 datarails-0.3.3/datarails.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-31 19:43:02.000000 datarails-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:43:14.165879 datarails-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-31 19:42:48.000000 datarails-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:43:14.165879 datarails-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-31 19:42:48.000000 datarails-0.3.3/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-31 19:42:48.000000 datarails-0.3.3/tests/test_databox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-31 19:42:48.000000 datarails-0.3.3/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-31 19:42:48.000000 datarails-0.3.3/tests/test_step.py
```

### Comparing `datarails-0.3.2/LICENSE` & `datarails-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datarails-0.3.2/PKG-INFO` & `datarails-0.3.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,99 @@
 Metadata-Version: 2.1
 Name: datarails
-Version: 0.3.2
-Requires-Python: >=3.9
+Version: 0.3.3
+Summary: A simple lightweight library for Dataframe based ETL pipelines
+Project-URL: homepage, https://github.com/JesseMaitland/datarails
+Project-URL: documentation, https://jessemaitland.github.io/datarails/
+Project-URL: changelog, https://github.com/JesseMaitland/datarails/blob/main/CHANGELOG.md
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 [![Release python package](https://github.com/JesseMaitland/datarails/actions/workflows/release.yml/badge.svg)](https://github.com/JesseMaitland/datarails/actions/workflows/release.yml)
-# datarails -- A Simple Framework for Dataframe ETL
-####  -- VERSION 0.3.2 --
 
+# datarails -- A Simple, Lightweight Framework for Dataframe ETL
+####  -- VERSION 0.3.3 --
+
+Datarails is a simple framework for organizing your in memory Dataframe based ETL jobs. It doesn't matter of you are using `pandas`, `spark`, `glue` or anything else
+this library serves as a simple way to structure your ETL jobs. It is not a replacement for `airflow`, `luigi`, `dagster` or any other workflow management tool, but rather
+can serve as the "entry point" for your workflow management tool to execute your ETL job.
 
 ## Official Documentation
 The official documentation is hosted on github pages at [jesse.maitland.github.io](https://jessemaitland.github.io/datarails/)
 
-## Example Project
-There is an example repo containing some simple ETL jobs, notebooks and commands for building documentation at [jessemaitland/datarails-example](https://github.com/JesseMaitland/datarails_examples)
+## Installation
+Datarails is available on PyPI and can be installed with pip. It has no dependencies and is written in pure python.
+```bash
+pip install datarails
+```
 
-Datarails is a simple framework for organizing your in memory Dataframe based ETL jobs. It doesn't matter of you are using `pandas`, `spark`, `glue` or anything else
-this library serves as a simple way to structure your ETL jobs so that others don't come along and have to debug your 300 line script by copy / pasting sections of it into
-a jupyter notebook.
+## Features
 
-## Basic Usage
+Datarails consists of 4 main classes:
 
-Steps are defined as classes and then passed to a step runner. All methods in the class that start with `step_` will be run in the order they are defined.
+**DataBox:** A dynamic data store for DataFrame objects. It can handle any DataFrame type, and offers methods for adding, retrieving, and removing data. It's a bit like a dictionary for DataFrames.
+
+**DataRailsContext:** A companion to DataBox, this class is designed for storing and retrieving additional data that you may need alongside your DataFrame objects. It allows you to associate metadata, configuration details, and other supplementary information with your data.
+
+**DataRailsStepRunner:** This class is responsible for running a sequence of DataRailsStep objects. It takes a DataBox as input and manages the execution of each step, tracking the state of the DataBox as it goes.
+
+**DataRailsStep:** A base class for defining steps in your data pipeline. By inheriting from this class, you can create custom steps that fit your specific needs.
+
+## Simple Example
+
+ETL steps are defined as classes and then passed to a step runner. All methods in the class that start with `step_` will be run in the order they are defined.
 Each step has access to a `DataBox` object that can be used to store dataframes and access them by name in downstream steps.
 
 In addition to the `DataBox` object, each step has access to a `DataRailsContext` object that can be used to store and access variables that are not dataframes.
 
+In this below example we are doing some simple procssing using pandas, however any other dataframe library could be used.
+
 ```python
 import pandas as pd
 from datarails.step import DataRailsStep
 from datarails.runner import DataRailsStepRunner
 
 
 class LoadDataFromCSV(DataRailsStep):
-
+    """Loads data from a CSV file into a DataBox."""
+    
     def step_load_csv(self) -> None:
+        """Loads a DataFrame from a CSV file and stores it in the DataBox under 'data'."""
         print('loading data from csv')
         df = pd.read_csv('data.csv')
-        self.dbx.put_df('data', df)  # dbx now has an attribute called data that is a dataframe
+        self.dbx.put_df('data', df)
 
 
 class TransformData(DataRailsStep):
-
+    """Applies transformation operations to a DataFrame stored in a DataBox."""
+    
     def step_add_new_column(self) -> None:
+        """Adds a new column to the DataFrame which is double the values of the 'old_column'."""
         print('adding new column')
         self.dbx.data['new_column'] = self.dbx.data['old_column'] * 2
 
     def step_drop_all_null_rows(self) -> None:
+        """Removes all rows from the DataFrame that contain any null values."""
         print('dropping null rows')
         self.dbx.data = self.dbx.data.dropna()
 
-    def rename_columns(self) -> None:
+    def step_rename_columns(self) -> None:
+        """Renames the 'new_column' in the DataFrame to 'blue_column'."""
         print('renaming columns')
         self.dbx.data = self.dbx.data.rename(columns={'new_column': 'blue_column'})
 
 
 class SaveData(DataRailsStep):
-
+    """Saves the DataFrame from a DataBox to a CSV file."""
+    
     def step_save_data(self) -> None:
+        """Saves the DataFrame to a CSV file named 'new_data.csv'."""
         print('saving data')
         self.dbx.data.to_csv('new_data.csv')
 
 
 # gather your steps in a list of class definitions. The class instances will be created by the step runner
 # while the jobs is being executed.
 steps = [
@@ -80,46 +109,43 @@
 # executed in the order they are defined in the class.
 
 if __name__ == '__main__':
     runner.run()
 
 ```
 
+## Example Project
+There is an example repo containing some simple ETL jobs, notebooks and commands for building documentation at [jessemaitland/datarails-example](https://github.com/JesseMaitland/datarails_examples)
+
 ## Why Use DataRails?
 
-`datarails` is intended to solve a few simple problems that I have encountered while working with small to medium sized etl scripts in python. It is a very
-simple framework for ETL job execution and nothing more. It is not a replacement for `airflow`, `luigi`, `dagster` or any other workflow management tool, but rather
-can serve as the "entry point" for your workflow management tool to execute your ETL job.
+`datarails` addresses several critical issues commonly encountered during the execution of small to medium scale ETL (Extract, Transform, Load) scripts in Python. While simple, it is an effective framework that streamlines ETL tasks, and serves as a robust "entry point" for other workflow management tools, like `airflow`, `luigi`, or `dagster`, to execute your ETL job.
+
+### 1. Segmenting Your ETL Job into Manageable Steps
+ETL tasks of small or medium complexity can often transform into a single, monolithic script. While functional, this approach could be challenging to debug when data-related errors occur. `datarails` allows the segmentation of ETL tasks into distinct, manageable steps, enhancing clarity and error-handling.
 
-### 1. Break your ETL Job into Smaller Steps
-Quite often what happens with "small" or "medium" sized etl jobs is that they are thrown together as a single script that does everything.
-This works ok until the first time your script throws an error. As during the ETL process, your error is likely due to a problem with the data,
-and the single script approach makes it difficult to debug.
-
-### 2. Step Through Your ETL Job
-In the event you do encounter a problem with your ETL job, with `datarails` you can simply import your runner into a python shell or a jupyter notebook
-like this:
+### 2. Navigating Your ETL Job Step by Step
+With `datarails`, it's possible to debug ETL jobs step-by-step. You can import your runner into a Python shell or a Jupyter notebook, advancing through each step individually. This method is particularly beneficial when working with schema-less source data formats like JSON or CSV, enabling precise data inspection at every stage.
 
 ```python
 from my_etl_job import runner
 runner.advance() # run the next step and stop execution
-```
 
-This allows you to step through your job and inspect the data at each step. This is especially useful when you are working with a format such a json or csv as
-your source data that does not have a schema.
+step_to_debug = runner.get_current_step() # get the current step
+
+step_to_debug.dbx.data # inspect the data in the DataBox
+step_to_debug.dbx.context # inspect the context in the DataRailsContext
+
+step_to_debug.advance() # run the next step and stop execution. Repeat as needed.
+```
 
+### 3. A Practical Solution for Typical Data Sizes
+Most often, external processes fetch data and upload it into S3 (or similar cloud storage) on a daily basis. The data, typically in the size range of 20MB to 100MB and in diverse formats like `json`, `json lines`, or `csv`, needs transformation and cleaning before it can be utilized by other teams in your data lake or warehouse. `datarails` is an ideal library for managing and transforming these types of data.
 
-### 3. You Probably Don't Have Big Data
-In all likelihood you have some external process fetching data and dumping it into S3 (or some other cloud storage) on a daily bases. The files entering your landing zone 
-are in the order of 20MB to 100MB and are stored in some horrible format like `json`, or `json lines` or even `csv`. You need to transform this data into a format that is more useful and 
-do a bit of clean up so that the data is available for other teams in your datalake, or data warehouse. You probably have 10s or even 100s of jobs that are similar to this. `datarails` is
-a perfect library for these types of jobs.
+### 4. Simplified Documentation
+`datarails` encourages the practice of dividing ETL jobs into smaller methods, thus facilitating the process of documentation. This feature works well with Python's native tools for generating documentation from docstrings, and such documentation can be published through your CI job. This way, it is readily available for business users or other technical users, significantly reducing the time you spend responding to queries about your ETL jobs.
 
+### 5. Facilitating Standardization Across the Organization
 
-### 4. Documentation
-How often you you get a request from someone non-technical in the company who asks a question about an ETL job that was written 6 months ago? You get a question like,
-"Hey, I noticed that the data in the `blue_column` is different than the data in the `red_column`. Can you tell me why that is?" You of course have no idea why that is, and you have to go
-back to the code to figure it out. 
+In many organizations, ETL processes and data pipelines can be constructed in vastly different ways depending on the preferences and experience of individual developers. This can lead to considerable confusion, difficulty in maintaining code, and barriers to effective collaboration. `datarails` can help overcome these challenges by offering a standard framework for developing ETL jobs.
 
-`datarails` forces you to break up your ETL job into smaller steps or methods. Since python provides many tools for building documentation from docstrings, you can easily
-incorporate documentation using standard python docstrings, which can be published in your CI job. The documentation can then be available to business users, or other technical users
-which will save you time from having to answer questions about your ETL jobs.
+The use of `datarails` ensures that all ETL scripts follow the same structure and approach, creating a uniform coding style across the organization. This not only makes the codebase easier to understand and maintain, but also encourages effective collaboration between team members. Moreover, the standardized structure can expedite the onboarding process for new team members, as they only need to familiarize themselves with one framework, rather than a multitude of disparate coding styles.
```

### Comparing `datarails-0.3.2/README.md` & `datarails-0.3.3/datarails.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,99 @@
+Metadata-Version: 2.1
+Name: datarails
+Version: 0.3.3
+Summary: A simple lightweight library for Dataframe based ETL pipelines
+Project-URL: homepage, https://github.com/JesseMaitland/datarails
+Project-URL: documentation, https://jessemaitland.github.io/datarails/
+Project-URL: changelog, https://github.com/JesseMaitland/datarails/blob/main/CHANGELOG.md
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: docs
+License-File: LICENSE
+
 [![Release python package](https://github.com/JesseMaitland/datarails/actions/workflows/release.yml/badge.svg)](https://github.com/JesseMaitland/datarails/actions/workflows/release.yml)
-# datarails -- A Simple Framework for Dataframe ETL
-####  -- VERSION 0.3.2 --
 
+# datarails -- A Simple, Lightweight Framework for Dataframe ETL
+####  -- VERSION 0.3.3 --
+
+Datarails is a simple framework for organizing your in memory Dataframe based ETL jobs. It doesn't matter of you are using `pandas`, `spark`, `glue` or anything else
+this library serves as a simple way to structure your ETL jobs. It is not a replacement for `airflow`, `luigi`, `dagster` or any other workflow management tool, but rather
+can serve as the "entry point" for your workflow management tool to execute your ETL job.
 
 ## Official Documentation
 The official documentation is hosted on github pages at [jesse.maitland.github.io](https://jessemaitland.github.io/datarails/)
 
-## Example Project
-There is an example repo containing some simple ETL jobs, notebooks and commands for building documentation at [jessemaitland/datarails-example](https://github.com/JesseMaitland/datarails_examples)
+## Installation
+Datarails is available on PyPI and can be installed with pip. It has no dependencies and is written in pure python.
+```bash
+pip install datarails
+```
 
-Datarails is a simple framework for organizing your in memory Dataframe based ETL jobs. It doesn't matter of you are using `pandas`, `spark`, `glue` or anything else
-this library serves as a simple way to structure your ETL jobs so that others don't come along and have to debug your 300 line script by copy / pasting sections of it into
-a jupyter notebook.
+## Features
+
+Datarails consists of 4 main classes:
+
+**DataBox:** A dynamic data store for DataFrame objects. It can handle any DataFrame type, and offers methods for adding, retrieving, and removing data. It's a bit like a dictionary for DataFrames.
+
+**DataRailsContext:** A companion to DataBox, this class is designed for storing and retrieving additional data that you may need alongside your DataFrame objects. It allows you to associate metadata, configuration details, and other supplementary information with your data.
+
+**DataRailsStepRunner:** This class is responsible for running a sequence of DataRailsStep objects. It takes a DataBox as input and manages the execution of each step, tracking the state of the DataBox as it goes.
+
+**DataRailsStep:** A base class for defining steps in your data pipeline. By inheriting from this class, you can create custom steps that fit your specific needs.
 
-## Basic Usage
+## Simple Example
 
-Steps are defined as classes and then passed to a step runner. All methods in the class that start with `step_` will be run in the order they are defined.
+ETL steps are defined as classes and then passed to a step runner. All methods in the class that start with `step_` will be run in the order they are defined.
 Each step has access to a `DataBox` object that can be used to store dataframes and access them by name in downstream steps.
 
 In addition to the `DataBox` object, each step has access to a `DataRailsContext` object that can be used to store and access variables that are not dataframes.
 
+In this below example we are doing some simple procssing using pandas, however any other dataframe library could be used.
+
 ```python
 import pandas as pd
 from datarails.step import DataRailsStep
 from datarails.runner import DataRailsStepRunner
 
 
 class LoadDataFromCSV(DataRailsStep):
-
+    """Loads data from a CSV file into a DataBox."""
+    
     def step_load_csv(self) -> None:
+        """Loads a DataFrame from a CSV file and stores it in the DataBox under 'data'."""
         print('loading data from csv')
         df = pd.read_csv('data.csv')
-        self.dbx.put_df('data', df)  # dbx now has an attribute called data that is a dataframe
+        self.dbx.put_df('data', df)
 
 
 class TransformData(DataRailsStep):
-
+    """Applies transformation operations to a DataFrame stored in a DataBox."""
+    
     def step_add_new_column(self) -> None:
+        """Adds a new column to the DataFrame which is double the values of the 'old_column'."""
         print('adding new column')
         self.dbx.data['new_column'] = self.dbx.data['old_column'] * 2
 
     def step_drop_all_null_rows(self) -> None:
+        """Removes all rows from the DataFrame that contain any null values."""
         print('dropping null rows')
         self.dbx.data = self.dbx.data.dropna()
 
-    def rename_columns(self) -> None:
+    def step_rename_columns(self) -> None:
+        """Renames the 'new_column' in the DataFrame to 'blue_column'."""
         print('renaming columns')
         self.dbx.data = self.dbx.data.rename(columns={'new_column': 'blue_column'})
 
 
 class SaveData(DataRailsStep):
-
+    """Saves the DataFrame from a DataBox to a CSV file."""
+    
     def step_save_data(self) -> None:
+        """Saves the DataFrame to a CSV file named 'new_data.csv'."""
         print('saving data')
         self.dbx.data.to_csv('new_data.csv')
 
 
 # gather your steps in a list of class definitions. The class instances will be created by the step runner
 # while the jobs is being executed.
 steps = [
@@ -71,46 +109,43 @@
 # executed in the order they are defined in the class.
 
 if __name__ == '__main__':
     runner.run()
 
 ```
 
+## Example Project
+There is an example repo containing some simple ETL jobs, notebooks and commands for building documentation at [jessemaitland/datarails-example](https://github.com/JesseMaitland/datarails_examples)
+
 ## Why Use DataRails?
 
-`datarails` is intended to solve a few simple problems that I have encountered while working with small to medium sized etl scripts in python. It is a very
-simple framework for ETL job execution and nothing more. It is not a replacement for `airflow`, `luigi`, `dagster` or any other workflow management tool, but rather
-can serve as the "entry point" for your workflow management tool to execute your ETL job.
+`datarails` addresses several critical issues commonly encountered during the execution of small to medium scale ETL (Extract, Transform, Load) scripts in Python. While simple, it is an effective framework that streamlines ETL tasks, and serves as a robust "entry point" for other workflow management tools, like `airflow`, `luigi`, or `dagster`, to execute your ETL job.
+
+### 1. Segmenting Your ETL Job into Manageable Steps
+ETL tasks of small or medium complexity can often transform into a single, monolithic script. While functional, this approach could be challenging to debug when data-related errors occur. `datarails` allows the segmentation of ETL tasks into distinct, manageable steps, enhancing clarity and error-handling.
 
-### 1. Break your ETL Job into Smaller Steps
-Quite often what happens with "small" or "medium" sized etl jobs is that they are thrown together as a single script that does everything.
-This works ok until the first time your script throws an error. As during the ETL process, your error is likely due to a problem with the data,
-and the single script approach makes it difficult to debug.
-
-### 2. Step Through Your ETL Job
-In the event you do encounter a problem with your ETL job, with `datarails` you can simply import your runner into a python shell or a jupyter notebook
-like this:
+### 2. Navigating Your ETL Job Step by Step
+With `datarails`, it's possible to debug ETL jobs step-by-step. You can import your runner into a Python shell or a Jupyter notebook, advancing through each step individually. This method is particularly beneficial when working with schema-less source data formats like JSON or CSV, enabling precise data inspection at every stage.
 
 ```python
 from my_etl_job import runner
 runner.advance() # run the next step and stop execution
-```
 
-This allows you to step through your job and inspect the data at each step. This is especially useful when you are working with a format such a json or csv as
-your source data that does not have a schema.
+step_to_debug = runner.get_current_step() # get the current step
+
+step_to_debug.dbx.data # inspect the data in the DataBox
+step_to_debug.dbx.context # inspect the context in the DataRailsContext
+
+step_to_debug.advance() # run the next step and stop execution. Repeat as needed.
+```
 
+### 3. A Practical Solution for Typical Data Sizes
+Most often, external processes fetch data and upload it into S3 (or similar cloud storage) on a daily basis. The data, typically in the size range of 20MB to 100MB and in diverse formats like `json`, `json lines`, or `csv`, needs transformation and cleaning before it can be utilized by other teams in your data lake or warehouse. `datarails` is an ideal library for managing and transforming these types of data.
 
-### 3. You Probably Don't Have Big Data
-In all likelihood you have some external process fetching data and dumping it into S3 (or some other cloud storage) on a daily bases. The files entering your landing zone 
-are in the order of 20MB to 100MB and are stored in some horrible format like `json`, or `json lines` or even `csv`. You need to transform this data into a format that is more useful and 
-do a bit of clean up so that the data is available for other teams in your datalake, or data warehouse. You probably have 10s or even 100s of jobs that are similar to this. `datarails` is
-a perfect library for these types of jobs.
+### 4. Simplified Documentation
+`datarails` encourages the practice of dividing ETL jobs into smaller methods, thus facilitating the process of documentation. This feature works well with Python's native tools for generating documentation from docstrings, and such documentation can be published through your CI job. This way, it is readily available for business users or other technical users, significantly reducing the time you spend responding to queries about your ETL jobs.
 
+### 5. Facilitating Standardization Across the Organization
 
-### 4. Documentation
-How often you you get a request from someone non-technical in the company who asks a question about an ETL job that was written 6 months ago? You get a question like,
-"Hey, I noticed that the data in the `blue_column` is different than the data in the `red_column`. Can you tell me why that is?" You of course have no idea why that is, and you have to go
-back to the code to figure it out. 
+In many organizations, ETL processes and data pipelines can be constructed in vastly different ways depending on the preferences and experience of individual developers. This can lead to considerable confusion, difficulty in maintaining code, and barriers to effective collaboration. `datarails` can help overcome these challenges by offering a standard framework for developing ETL jobs.
 
-`datarails` forces you to break up your ETL job into smaller steps or methods. Since python provides many tools for building documentation from docstrings, you can easily
-incorporate documentation using standard python docstrings, which can be published in your CI job. The documentation can then be available to business users, or other technical users
-which will save you time from having to answer questions about your ETL jobs.
+The use of `datarails` ensures that all ETL scripts follow the same structure and approach, creating a uniform coding style across the organization. This not only makes the codebase easier to understand and maintain, but also encourages effective collaboration between team members. Moreover, the standardized structure can expedite the onboarding process for new team members, as they only need to familiarize themselves with one framework, rather than a multitude of disparate coding styles.
```

### Comparing `datarails-0.3.2/datarails/contexts.py` & `datarails-0.3.3/datarails/contexts.py`

 * *Files identical despite different names*

### Comparing `datarails-0.3.2/datarails/runner.py` & `datarails-0.3.3/datarails/runner.py`

 * *Files identical despite different names*

### Comparing `datarails-0.3.2/datarails/step.py` & `datarails-0.3.3/datarails/step.py`

 * *Files identical despite different names*

### Comparing `datarails-0.3.2/datarails.egg-info/PKG-INFO` & `datarails-0.3.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,86 @@
-Metadata-Version: 2.1
-Name: datarails
-Version: 0.3.2
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE
-
 [![Release python package](https://github.com/JesseMaitland/datarails/actions/workflows/release.yml/badge.svg)](https://github.com/JesseMaitland/datarails/actions/workflows/release.yml)
-# datarails -- A Simple Framework for Dataframe ETL
-####  -- VERSION 0.3.2 --
 
+# datarails -- A Simple, Lightweight Framework for Dataframe ETL
+####  -- VERSION 0.3.3 --
+
+Datarails is a simple framework for organizing your in memory Dataframe based ETL jobs. It doesn't matter of you are using `pandas`, `spark`, `glue` or anything else
+this library serves as a simple way to structure your ETL jobs. It is not a replacement for `airflow`, `luigi`, `dagster` or any other workflow management tool, but rather
+can serve as the "entry point" for your workflow management tool to execute your ETL job.
 
 ## Official Documentation
 The official documentation is hosted on github pages at [jesse.maitland.github.io](https://jessemaitland.github.io/datarails/)
 
-## Example Project
-There is an example repo containing some simple ETL jobs, notebooks and commands for building documentation at [jessemaitland/datarails-example](https://github.com/JesseMaitland/datarails_examples)
+## Installation
+Datarails is available on PyPI and can be installed with pip. It has no dependencies and is written in pure python.
+```bash
+pip install datarails
+```
 
-Datarails is a simple framework for organizing your in memory Dataframe based ETL jobs. It doesn't matter of you are using `pandas`, `spark`, `glue` or anything else
-this library serves as a simple way to structure your ETL jobs so that others don't come along and have to debug your 300 line script by copy / pasting sections of it into
-a jupyter notebook.
+## Features
+
+Datarails consists of 4 main classes:
+
+**DataBox:** A dynamic data store for DataFrame objects. It can handle any DataFrame type, and offers methods for adding, retrieving, and removing data. It's a bit like a dictionary for DataFrames.
+
+**DataRailsContext:** A companion to DataBox, this class is designed for storing and retrieving additional data that you may need alongside your DataFrame objects. It allows you to associate metadata, configuration details, and other supplementary information with your data.
+
+**DataRailsStepRunner:** This class is responsible for running a sequence of DataRailsStep objects. It takes a DataBox as input and manages the execution of each step, tracking the state of the DataBox as it goes.
+
+**DataRailsStep:** A base class for defining steps in your data pipeline. By inheriting from this class, you can create custom steps that fit your specific needs.
 
-## Basic Usage
+## Simple Example
 
-Steps are defined as classes and then passed to a step runner. All methods in the class that start with `step_` will be run in the order they are defined.
+ETL steps are defined as classes and then passed to a step runner. All methods in the class that start with `step_` will be run in the order they are defined.
 Each step has access to a `DataBox` object that can be used to store dataframes and access them by name in downstream steps.
 
 In addition to the `DataBox` object, each step has access to a `DataRailsContext` object that can be used to store and access variables that are not dataframes.
 
+In this below example we are doing some simple procssing using pandas, however any other dataframe library could be used.
+
 ```python
 import pandas as pd
 from datarails.step import DataRailsStep
 from datarails.runner import DataRailsStepRunner
 
 
 class LoadDataFromCSV(DataRailsStep):
-
+    """Loads data from a CSV file into a DataBox."""
+    
     def step_load_csv(self) -> None:
+        """Loads a DataFrame from a CSV file and stores it in the DataBox under 'data'."""
         print('loading data from csv')
         df = pd.read_csv('data.csv')
-        self.dbx.put_df('data', df)  # dbx now has an attribute called data that is a dataframe
+        self.dbx.put_df('data', df)
 
 
 class TransformData(DataRailsStep):
-
+    """Applies transformation operations to a DataFrame stored in a DataBox."""
+    
     def step_add_new_column(self) -> None:
+        """Adds a new column to the DataFrame which is double the values of the 'old_column'."""
         print('adding new column')
         self.dbx.data['new_column'] = self.dbx.data['old_column'] * 2
 
     def step_drop_all_null_rows(self) -> None:
+        """Removes all rows from the DataFrame that contain any null values."""
         print('dropping null rows')
         self.dbx.data = self.dbx.data.dropna()
 
-    def rename_columns(self) -> None:
+    def step_rename_columns(self) -> None:
+        """Renames the 'new_column' in the DataFrame to 'blue_column'."""
         print('renaming columns')
         self.dbx.data = self.dbx.data.rename(columns={'new_column': 'blue_column'})
 
 
 class SaveData(DataRailsStep):
-
+    """Saves the DataFrame from a DataBox to a CSV file."""
+    
     def step_save_data(self) -> None:
+        """Saves the DataFrame to a CSV file named 'new_data.csv'."""
         print('saving data')
         self.dbx.data.to_csv('new_data.csv')
 
 
 # gather your steps in a list of class definitions. The class instances will be created by the step runner
 # while the jobs is being executed.
 steps = [
@@ -80,46 +96,43 @@
 # executed in the order they are defined in the class.
 
 if __name__ == '__main__':
     runner.run()
 
 ```
 
+## Example Project
+There is an example repo containing some simple ETL jobs, notebooks and commands for building documentation at [jessemaitland/datarails-example](https://github.com/JesseMaitland/datarails_examples)
+
 ## Why Use DataRails?
 
-`datarails` is intended to solve a few simple problems that I have encountered while working with small to medium sized etl scripts in python. It is a very
-simple framework for ETL job execution and nothing more. It is not a replacement for `airflow`, `luigi`, `dagster` or any other workflow management tool, but rather
-can serve as the "entry point" for your workflow management tool to execute your ETL job.
+`datarails` addresses several critical issues commonly encountered during the execution of small to medium scale ETL (Extract, Transform, Load) scripts in Python. While simple, it is an effective framework that streamlines ETL tasks, and serves as a robust "entry point" for other workflow management tools, like `airflow`, `luigi`, or `dagster`, to execute your ETL job.
+
+### 1. Segmenting Your ETL Job into Manageable Steps
+ETL tasks of small or medium complexity can often transform into a single, monolithic script. While functional, this approach could be challenging to debug when data-related errors occur. `datarails` allows the segmentation of ETL tasks into distinct, manageable steps, enhancing clarity and error-handling.
 
-### 1. Break your ETL Job into Smaller Steps
-Quite often what happens with "small" or "medium" sized etl jobs is that they are thrown together as a single script that does everything.
-This works ok until the first time your script throws an error. As during the ETL process, your error is likely due to a problem with the data,
-and the single script approach makes it difficult to debug.
-
-### 2. Step Through Your ETL Job
-In the event you do encounter a problem with your ETL job, with `datarails` you can simply import your runner into a python shell or a jupyter notebook
-like this:
+### 2. Navigating Your ETL Job Step by Step
+With `datarails`, it's possible to debug ETL jobs step-by-step. You can import your runner into a Python shell or a Jupyter notebook, advancing through each step individually. This method is particularly beneficial when working with schema-less source data formats like JSON or CSV, enabling precise data inspection at every stage.
 
 ```python
 from my_etl_job import runner
 runner.advance() # run the next step and stop execution
-```
 
-This allows you to step through your job and inspect the data at each step. This is especially useful when you are working with a format such a json or csv as
-your source data that does not have a schema.
+step_to_debug = runner.get_current_step() # get the current step
+
+step_to_debug.dbx.data # inspect the data in the DataBox
+step_to_debug.dbx.context # inspect the context in the DataRailsContext
+
+step_to_debug.advance() # run the next step and stop execution. Repeat as needed.
+```
 
+### 3. A Practical Solution for Typical Data Sizes
+Most often, external processes fetch data and upload it into S3 (or similar cloud storage) on a daily basis. The data, typically in the size range of 20MB to 100MB and in diverse formats like `json`, `json lines`, or `csv`, needs transformation and cleaning before it can be utilized by other teams in your data lake or warehouse. `datarails` is an ideal library for managing and transforming these types of data.
 
-### 3. You Probably Don't Have Big Data
-In all likelihood you have some external process fetching data and dumping it into S3 (or some other cloud storage) on a daily bases. The files entering your landing zone 
-are in the order of 20MB to 100MB and are stored in some horrible format like `json`, or `json lines` or even `csv`. You need to transform this data into a format that is more useful and 
-do a bit of clean up so that the data is available for other teams in your datalake, or data warehouse. You probably have 10s or even 100s of jobs that are similar to this. `datarails` is
-a perfect library for these types of jobs.
+### 4. Simplified Documentation
+`datarails` encourages the practice of dividing ETL jobs into smaller methods, thus facilitating the process of documentation. This feature works well with Python's native tools for generating documentation from docstrings, and such documentation can be published through your CI job. This way, it is readily available for business users or other technical users, significantly reducing the time you spend responding to queries about your ETL jobs.
 
+### 5. Facilitating Standardization Across the Organization
 
-### 4. Documentation
-How often you you get a request from someone non-technical in the company who asks a question about an ETL job that was written 6 months ago? You get a question like,
-"Hey, I noticed that the data in the `blue_column` is different than the data in the `red_column`. Can you tell me why that is?" You of course have no idea why that is, and you have to go
-back to the code to figure it out. 
+In many organizations, ETL processes and data pipelines can be constructed in vastly different ways depending on the preferences and experience of individual developers. This can lead to considerable confusion, difficulty in maintaining code, and barriers to effective collaboration. `datarails` can help overcome these challenges by offering a standard framework for developing ETL jobs.
 
-`datarails` forces you to break up your ETL job into smaller steps or methods. Since python provides many tools for building documentation from docstrings, you can easily
-incorporate documentation using standard python docstrings, which can be published in your CI job. The documentation can then be available to business users, or other technical users
-which will save you time from having to answer questions about your ETL jobs.
+The use of `datarails` ensures that all ETL scripts follow the same structure and approach, creating a uniform coding style across the organization. This not only makes the codebase easier to understand and maintain, but also encourages effective collaboration between team members. Moreover, the standardized structure can expedite the onboarding process for new team members, as they only need to familiarize themselves with one framework, rather than a multitude of disparate coding styles.
```

### Comparing `datarails-0.3.2/pyproject.toml` & `datarails-0.3.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datarails"
-version = "0.3.2"
-description = ""
+version = "0.3.3"
+description = "A simple lightweight library for Dataframe based ETL pipelines"
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 
 
+[project.urls]
+homepage = "https://github.com/JesseMaitland/datarails"
+documentation = "https://jessemaitland.github.io/datarails/"
+changelog = "https://github.com/JesseMaitland/datarails/blob/main/CHANGELOG.md"
+
 [project.optional-dependencies]
 dev = [
     "setuptools==68.0.0",
     "build==0.10.0",
     "python-semantic-release==7.34.6",
     "pytest==7.2.2",
     "black==22.6.0",
     "isort==5.12.0",
 ]
 
 docs = [
     "mkdocs==1.4.2",
     "mkdocstrings[python]==0.20.0",
     "mkdocs-material==9.1.3",
+    "markdown-include==0.8.1"
 ]
 
 [tool.semantic_release]
 version_variable = "datarails/__init__.py:__version__"
 version_toml = "pyproject.toml:project.version"
 version_pattern = "README.md:VERSION {version}"
 upload_to_pypi = false
```

### Comparing `datarails-0.3.2/tests/test_context.py` & `datarails-0.3.3/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `datarails-0.3.2/tests/test_databox.py` & `datarails-0.3.3/tests/test_databox.py`

 * *Files identical despite different names*

### Comparing `datarails-0.3.2/tests/test_runner.py` & `datarails-0.3.3/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `datarails-0.3.2/tests/test_step.py` & `datarails-0.3.3/tests/test_step.py`

 * *Files identical despite different names*

