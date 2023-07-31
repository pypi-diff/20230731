# Comparing `tmp/oneutil-0.0.3.tar.gz` & `tmp/oneutil-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oneutil-0.0.3.tar", last modified: Sun Jul 30 17:44:39 2023, max compression
+gzip compressed data, was "oneutil-0.0.4.tar", last modified: Mon Jul 31 02:11:53 2023, max compression
```

## Comparing `oneutil-0.0.3.tar` & `oneutil-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:44:39.101060 oneutil-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-30 17:44:29.000000 oneutil-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-30 17:44:39.101060 oneutil-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-30 17:44:29.000000 oneutil-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:44:39.101060 oneutil-0.0.3/oneutil/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 17:44:29.000000 oneutil-0.0.3/oneutil/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:44:39.101060 oneutil-0.0.3/oneutil/etl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 17:44:29.000000 oneutil-0.0.3/oneutil/etl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-30 17:44:29.000000 oneutil-0.0.3/oneutil/etl/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-30 17:44:29.000000 oneutil-0.0.3/oneutil/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 17:44:39.101060 oneutil-0.0.3/oneutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-30 17:44:39.000000 oneutil-0.0.3/oneutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-30 17:44:39.000000 oneutil-0.0.3/oneutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 17:44:39.000000 oneutil-0.0.3/oneutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-30 17:44:39.000000 oneutil-0.0.3/oneutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-30 17:44:39.000000 oneutil-0.0.3/oneutil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 17:44:39.101060 oneutil-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-30 17:44:29.000000 oneutil-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:11:53.401859 oneutil-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-31 02:11:41.000000 oneutil-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-31 02:11:53.401859 oneutil-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-31 02:11:41.000000 oneutil-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:11:53.397859 oneutil-0.0.4/oneutil/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 02:11:41.000000 oneutil-0.0.4/oneutil/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:11:53.397859 oneutil-0.0.4/oneutil/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 02:11:41.000000 oneutil-0.0.4/oneutil/etl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-07-31 02:11:41.000000 oneutil-0.0.4/oneutil/etl/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-31 02:11:41.000000 oneutil-0.0.4/oneutil/etl/databento.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-31 02:11:41.000000 oneutil-0.0.4/oneutil/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:11:53.397859 oneutil-0.0.4/oneutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-31 02:11:53.000000 oneutil-0.0.4/oneutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-31 02:11:53.000000 oneutil-0.0.4/oneutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 02:11:53.000000 oneutil-0.0.4/oneutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-31 02:11:53.000000 oneutil-0.0.4/oneutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 02:11:53.000000 oneutil-0.0.4/oneutil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 02:11:53.401859 oneutil-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-31 02:11:41.000000 oneutil-0.0.4/setup.py
```

### Comparing `oneutil-0.0.3/LICENSE` & `oneutil-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `oneutil-0.0.3/PKG-INFO` & `oneutil-0.0.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,11 @@
-Metadata-Version: 2.1
-Name: oneutil
-Version: 0.0.3
-Summary: OneSquared Utilities
-Author: Shawn Lin
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # One Squared Utilities
 
+[![PyPI version](https://badge.fury.io/py/oneutil.svg)](https://badge.fury.io/py/oneutil)
+
 oneutil is a Python package that provides useful utilities for work we do at One Squared.
 
 ## Installation
 
 To install oneutil, you can get it from PYPI:
 
 ```bash
@@ -27,20 +20,24 @@
 pip install -e . 
 ```
 
 ## Usage
 
 ```python
 from oneutil.etl.aws import get_s3_bucket_files, get_s3_buckets
+from oneutil.etl.databento import get_df_from_s3
 
 # List files in the default S3 bucket in 'us-east-1' region
 files = get_s3_bucket_files()
 
 # List all available S3 buckets in 'us-east-1' region
 buckets = get_s3_buckets()
+
+# Read a databento file
+df = get_df_from_s3(get_s3_bucket_files()[-1])
 ```
 
 oneutil relies on the AWS SDK (boto3) for interacting with AWS S3. To use the package, make sure you have valid AWS access credentials (access key ID and secret access key) set as environment variables or provide them explicitly when calling the functions.
 
 - `s3_public_key`: The AWS access key ID.
 - `s3_private_key`: The AWS secret access key.
```

### Comparing `oneutil-0.0.3/README.md` & `oneutil-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,20 @@
+Metadata-Version: 2.1
+Name: oneutil
+Version: 0.0.4
+Summary: OneSquared Utilities
+Author: Shawn Lin
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # One Squared Utilities
 
+[![PyPI version](https://badge.fury.io/py/oneutil.svg)](https://badge.fury.io/py/oneutil)
+
 oneutil is a Python package that provides useful utilities for work we do at One Squared.
 
 ## Installation
 
 To install oneutil, you can get it from PYPI:
 
 ```bash
@@ -18,20 +29,24 @@
 pip install -e . 
 ```
 
 ## Usage
 
 ```python
 from oneutil.etl.aws import get_s3_bucket_files, get_s3_buckets
+from oneutil.etl.databento import get_df_from_s3
 
 # List files in the default S3 bucket in 'us-east-1' region
 files = get_s3_bucket_files()
 
 # List all available S3 buckets in 'us-east-1' region
 buckets = get_s3_buckets()
+
+# Read a databento file
+df = get_df_from_s3(get_s3_bucket_files()[-1])
 ```
 
 oneutil relies on the AWS SDK (boto3) for interacting with AWS S3. To use the package, make sure you have valid AWS access credentials (access key ID and secret access key) set as environment variables or provide them explicitly when calling the functions.
 
 - `s3_public_key`: The AWS access key ID.
 - `s3_private_key`: The AWS secret access key.
```

### Comparing `oneutil-0.0.3/oneutil/etl/aws.py` & `oneutil-0.0.4/oneutil/etl/databento.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,84 +1,56 @@
-import boto3
 import os
-
+import databento
 from oneutil.logging import logger
+from oneutil.etl.aws import read_s3_bucket_file
+
 
-def get_s3_bucket_files(
+def get_df_from_s3(
+    filename: str,
     bucket: str = "onesquared-databento",
     region: str = "us-east-1",
     public_key: str = os.environ.get("s3_public_key"),
     private_key: str = os.environ.get("s3_private_key"),
 ):
     """
-    Get a list of file keys from a specified AWS S3 bucket.
+    Fetches data from an S3 bucket, converts it to a DataFrame, and returns the DataFrame.
 
     Parameters:
+        filename (str): The name of the file to read from the S3 bucket.
         bucket (str): The name of the S3 bucket. Default is 'onesquared-databento'.
         region (str): The AWS region where the bucket is located. Default is 'us-east-1'.
-        public_key (str): AWS access key ID. It can be provided as an argument or read from environment variables.
-        private_key (str): AWS secret access key. It can be provided as an argument or read from environment variables.
+        public_key (str): The AWS access key ID for authenticating with S3. If not provided,
+            it will be fetched from the environment variable "s3_public_key".
+        private_key (str): The AWS secret access key for authenticating with S3. If not provided,
+            it will be fetched from the environment variable "s3_private_key".
 
     Returns:
-        list: A list of file keys present in the specified S3 bucket.
-    """
-
-    # Log the function call with provided arguments
-    logger.debug(f"get_s3_bucket_files called with bucket={bucket}, region={region}")
-
-    # Create an S3 resource object using the provided credentials and region.
-    s3 = boto3.resource(
-        service_name="s3",
-        region_name=region,
-        aws_access_key_id=public_key,
-        aws_secret_access_key=private_key,
-    )
-
-    # Get the S3 bucket object.
-    bucket_obj = s3.Bucket(bucket)
-
-    # List all objects (files) in the bucket and store their keys in a list.
-    files = [file.key for file in bucket_obj.objects.all()]
-
-    # Log the number of files retrieved
-    logger.debug(f"Number of files retrieved: {len(files)}")
-
-    # Return the list of file keys.
-    return files
-
+        pandas.DataFrame: The DataFrame containing the data from the specified file.
 
-def get_s3_buckets(
-    region: str = "us-east-1",
-    public_key: str = os.environ.get("s3_public_key"),
-    private_key: str = os.environ.get("s3_private_key"),
-):
+    Raises:
+        FileNotFoundError: If the specified file is not found in the S3 bucket.
+        Exception: If there are any errors during the conversion to DataFrame.
+
+    Note:
+        The function assumes that the required AWS credentials (public_key and private_key)
+        are available as environment variables: "s3_public_key" and "s3_private_key".
+
+    Example:
+        # Fetch data from the file "data.csv" in the S3 bucket "my-data-bucket"
+        df = get_df_from_s3(filename="data.csv", bucket="my-data-bucket", region="us-west-2")
     """
-    Get a list of AWS S3 bucket names available in the specified AWS region.
-
-    Parameters:
-        region (str): The AWS region to list the S3 buckets from. Default is 'us-east-1'.
-        public_key (str): AWS access key ID. It can be provided as an argument or read from environment variables.
-        private_key (str): AWS secret access key. It can be provided as an argument or read from environment variables.
 
-    Returns:
-        list: A list of AWS S3 bucket names available in the specified region.
-    """
-
-    # Log the function call with provided arguments
-    logger.debug(f"get_s3_buckets called with region={region}")
-
-    # Create an S3 resource object using the provided credentials and region.
-    s3 = boto3.resource(
-        service_name="s3",
-        region_name=region,
-        aws_access_key_id=public_key,
-        aws_secret_access_key=private_key,
+    logger.debug(
+        f"get_df_from_s3 called with filename={filename}, bucket={bucket}, region={region}"
     )
 
-    # List all buckets in the specified region and store their names in a list.
-    buckets = [bucket.name for bucket in s3.buckets.all()]
+    # Read the file content from the S3 bucket using the provided filename
+    body = read_s3_bucket_file(filename, bucket, region, public_key, private_key)
+
+    # Create a Databento store from the bytes read from the S3 bucket
+    dbn = databento.DBNStore.from_bytes(body)
 
-    # Log the number of buckets retrieved
-    logger.debug(f"Number of buckets retrieved: {len(buckets)}")
+    # Convert the Databento store to a DataFrame
+    df = dbn.to_df()
 
-    # Return the list of bucket names.
-    return buckets
+    # Return the DataFrame
+    return df
```

### Comparing `oneutil-0.0.3/oneutil.egg-info/PKG-INFO` & `oneutil-0.0.4/oneutil.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: oneutil
-Version: 0.0.3
+Version: 0.0.4
 Summary: OneSquared Utilities
 Author: Shawn Lin
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # One Squared Utilities
 
+[![PyPI version](https://badge.fury.io/py/oneutil.svg)](https://badge.fury.io/py/oneutil)
+
 oneutil is a Python package that provides useful utilities for work we do at One Squared.
 
 ## Installation
 
 To install oneutil, you can get it from PYPI:
 
 ```bash
@@ -27,20 +29,24 @@
 pip install -e . 
 ```
 
 ## Usage
 
 ```python
 from oneutil.etl.aws import get_s3_bucket_files, get_s3_buckets
+from oneutil.etl.databento import get_df_from_s3
 
 # List files in the default S3 bucket in 'us-east-1' region
 files = get_s3_bucket_files()
 
 # List all available S3 buckets in 'us-east-1' region
 buckets = get_s3_buckets()
+
+# Read a databento file
+df = get_df_from_s3(get_s3_bucket_files()[-1])
 ```
 
 oneutil relies on the AWS SDK (boto3) for interacting with AWS S3. To use the package, make sure you have valid AWS access credentials (access key ID and secret access key) set as environment variables or provide them explicitly when calling the functions.
 
 - `s3_public_key`: The AWS access key ID.
 - `s3_private_key`: The AWS secret access key.
```

