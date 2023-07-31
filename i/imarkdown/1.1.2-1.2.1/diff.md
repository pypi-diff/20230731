# Comparing `tmp/imarkdown-1.1.2.tar.gz` & `tmp/imarkdown-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imarkdown-1.1.2.tar", last modified: Sun Jul 30 15:17:20 2023, max compression
+gzip compressed data, was "imarkdown-1.2.1.tar", last modified: Mon Jul 31 04:51:56 2023, max compression
```

## Comparing `imarkdown-1.1.2.tar` & `imarkdown-1.2.1.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 15:17:20.819378 imarkdown-1.1.2/
--rw-rw-rw-   0        0        0    17228 2023-07-30 15:17:20.818376 imarkdown-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    16366 2023-07-13 10:10:10.000000 imarkdown-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 15:17:20.790769 imarkdown-1.1.2/imarkdown/
--rw-rw-rw-   0        0        0      464 2023-07-13 10:10:10.000000 imarkdown-1.1.2/imarkdown/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 15:17:20.803769 imarkdown-1.1.2/imarkdown/adapter/
--rw-rw-rw-   0        0        0      476 2023-07-13 10:10:10.000000 imarkdown-1.1.2/imarkdown/adapter/__init__.py
--rw-rw-rw-   0        0        0     2939 2023-07-13 10:10:10.000000 imarkdown-1.1.2/imarkdown/adapter/aliyun_adapter.py
--rw-rw-rw-   0        0        0      835 2023-07-13 10:10:10.000000 imarkdown-1.1.2/imarkdown/adapter/base.py
--rw-rw-rw-   0        0        0      755 2023-07-13 10:10:10.000000 imarkdown-1.1.2/imarkdown/adapter/local_adapter.py
-drwxrwxrwx   0        0        0        0 2023-07-30 15:17:20.805773 imarkdown-1.1.2/imarkdown/client/
--rw-rw-rw-   0        0        0        0 2023-07-13 10:10:10.000000 imarkdown-1.1.2/imarkdown/client/__init__.py
--rw-rw-rw-   0        0        0     1371 2023-07-13 10:10:10.000000 imarkdown-1.1.2/imarkdown/config.py
--rw-rw-rw-   0        0        0      267 2023-07-13 10:10:10.000000 imarkdown-1.1.2/imarkdown/constant.py
--rw-rw-rw-   0        0        0    13230 2023-07-30 15:11:33.000000 imarkdown-1.1.2/imarkdown/converter.py
--rw-rw-rw-   0        0        0    10130 2023-07-30 14:13:57.000000 imarkdown-1.1.2/imarkdown/schema.py
-drwxrwxrwx   0        0        0        0 2023-07-30 15:17:20.809770 imarkdown-1.1.2/imarkdown/utils/
--rw-rw-rw-   0        0        0     2784 2023-07-30 13:02:07.000000 imarkdown-1.1.2/imarkdown/utils/__init__.py
--rw-rw-rw-   0        0        0      282 2023-07-13 10:10:10.000000 imarkdown-1.1.2/imarkdown/utils/cache.py
--rw-rw-rw-   0        0        0     1403 2023-07-13 10:10:10.000000 imarkdown-1.1.2/imarkdown/utils/singleton.py
-drwxrwxrwx   0        0        0        0 2023-07-30 15:17:20.797773 imarkdown-1.1.2/imarkdown.egg-info/
--rw-rw-rw-   0        0        0    17228 2023-07-30 15:17:20.000000 imarkdown-1.1.2/imarkdown.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      629 2023-07-30 15:17:20.000000 imarkdown-1.1.2/imarkdown.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 15:17:20.000000 imarkdown-1.1.2/imarkdown.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-07-30 15:17:20.000000 imarkdown-1.1.2/imarkdown.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-30 15:17:20.000000 imarkdown-1.1.2/imarkdown.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2022-12-18 07:47:47.000000 imarkdown-1.1.2/license
--rw-rw-rw-   0        0        0       42 2023-07-30 15:17:20.819378 imarkdown-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1940 2023-07-30 15:13:01.000000 imarkdown-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 15:17:20.816479 imarkdown-1.1.2/tests/
--rw-rw-rw-   0        0        0     2379 2023-07-13 10:10:10.000000 imarkdown-1.1.2/tests/test_adapter.py
--rw-rw-rw-   0        0        0     2273 2023-07-13 10:10:10.000000 imarkdown-1.1.2/tests/test_image_converter.py
--rw-rw-rw-   0        0        0     2235 2023-07-13 10:10:10.000000 imarkdown-1.1.2/tests/test_md_file.py
--rw-rw-rw-   0        0        0     2957 2023-07-13 10:10:10.000000 imarkdown-1.1.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:51:56.436812 imarkdown-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-07-31 04:51:56.436812 imarkdown-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16937 2023-07-31 04:51:45.000000 imarkdown-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:51:56.432812 imarkdown-1.2.1/imarkdown/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-31 04:51:45.000000 imarkdown-1.2.1/imarkdown/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:51:56.432812 imarkdown-1.2.1/imarkdown/adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-31 04:51:45.000000 imarkdown-1.2.1/imarkdown/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-31 04:51:45.000000 imarkdown-1.2.1/imarkdown/adapter/aliyun_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-31 04:51:45.000000 imarkdown-1.2.1/imarkdown/adapter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-31 04:51:45.000000 imarkdown-1.2.1/imarkdown/adapter/local_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:51:56.432812 imarkdown-1.2.1/imarkdown/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 04:51:45.000000 imarkdown-1.2.1/imarkdown/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-31 04:51:45.000000 imarkdown-1.2.1/imarkdown/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-31 04:51:45.000000 imarkdown-1.2.1/imarkdown/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13796 2023-07-31 04:51:45.000000 imarkdown-1.2.1/imarkdown/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-07-31 04:51:45.000000 imarkdown-1.2.1/imarkdown/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:51:56.432812 imarkdown-1.2.1/imarkdown/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-31 04:51:45.000000 imarkdown-1.2.1/imarkdown/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-31 04:51:45.000000 imarkdown-1.2.1/imarkdown/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-31 04:51:45.000000 imarkdown-1.2.1/imarkdown/utils/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:51:56.432812 imarkdown-1.2.1/imarkdown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-07-31 04:51:56.000000 imarkdown-1.2.1/imarkdown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-31 04:51:56.000000 imarkdown-1.2.1/imarkdown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 04:51:56.000000 imarkdown-1.2.1/imarkdown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-31 04:51:56.000000 imarkdown-1.2.1/imarkdown.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-31 04:51:56.000000 imarkdown-1.2.1/imarkdown.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 04:51:56.436812 imarkdown-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-31 04:51:45.000000 imarkdown-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:51:56.436812 imarkdown-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-31 04:51:45.000000 imarkdown-1.2.1/tests/test_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-31 04:51:45.000000 imarkdown-1.2.1/tests/test_image_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-31 04:51:45.000000 imarkdown-1.2.1/tests/test_md_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-31 04:51:45.000000 imarkdown-1.2.1/tests/test_utils.py
```

### Comparing `imarkdown-1.1.2/PKG-INFO` & `imarkdown-1.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,337 +1,358 @@
-Metadata-Version: 2.1
-Name: imarkdown
-Version: 1.1.2
-Summary: A practical Markdown image url converter
-Home-page: https://github.com/Undertone0809/imarkdown
-Author: Zeeland
-Author-email: zeeland@foxmail.com
-License: Apache 2.0
-Keywords: Markdown,markdown,imarkdown,markdown converter
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: license
-
-<h1 align="center">
-    imarkdown
-</h1>
-<p align="center">
-  <strong>imarkdown is a lightweight markdown image link converter that allows you to easily convert image links between local and image server, as well as between different image servers.</strong>
-</p>
-
-[English](/README.md) [中文](/README_zh.md)
-
-> When converting markdown from Yuque, the images are protected against external linking. If you want to publish the converted markdown on other platforms, you need to change all the image addresses in the markdown to local image addresses or custom image server addresses, so that others can view them correctly. This project aims to solve this problem by providing a converter that can batch convert image links in markdown and supports customized conversion in complex scenarios.
-
-## Features
-
-- Batch Download: imarkdown can batch download all the images in the markdown that are referenced using image links.
-- Multiple Conversion Methods: imarkdown supports various conversion methods for image links in markdown, such as converting to local image, converting web URL to local image, and converting web URL to image server URL.
-- Batch Conversion: It supports batch conversion of single or multiple files, as well as formatting and renaming of generated files.
-- Highly Customizable: By inheriting the `MdAdapter` class, you can easily implement custom URL conversion for different image servers.
-- Image Server Adapters: Currently, only Aliyun OSS is supported as an image server. Contributions are welcome to add support for more types of image servers.
-
-## Target Audience
-
-- People who need to batch convert image links in markdown.
-- Users who export markdown from Yuque and need to convert image links.
-- People who need to develop third-party extensions.
-
-## Technical Architecture
-
-`imarkdown` is designed with a modular architecture, allowing easy extension of each component. The following diagram provides a simplified overview of the technical architecture of imarkdown, which consists of the following components:
-
-- `MdImageConverter`: The image converter responsible for converting the image addresses in markdown and generating new markdown files.
-- `MdAdapter`: The adapter for converting `Image` objects to different types, such as `LocalFileAdapter` for local conversion, `AliyunAdapter` for Aliyun OSS conversion, and `CustomAdapter` for custom conversion. By injecting the adapter into `MdImageConverter`, you can define the type of address to convert `Image` objects to.
-- `MdMedium`: Includes `MdFile` and `MdFolder`, encapsulating some features used for data conversion in `MdImageConverter`.
-
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230713154424.png"/>
-
-The execution process of `imarkdown` is roughly as follows: after the `convert` method is called on `MdImageConverter`, `imarkdown` builds a virtual `MdTree` based on the provided `MdMedium`, and performs batch image URL conversion on the files according to this tree.
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230713155912.png"/>
-
-## Quick Start
-
-This project is developed in Python and distributed on PyPI. Users can easily use imarkdown by installing it with pip. The following sections will explain several usage scenarios and methods of imarkdown.
-
-- Third-Party Package Installation: Open a terminal or command prompt and run the following command.
-
-```sh
-pip install -U imarkdown
-```
-
-**Examples**
-- [Convert Web URLs to Local Addresses](#converting-web-urls-to-local-file-paths)
-- [Convert Web URLs to Image Server URLs](#converting-web-urls-to-image-hosting-service-urls)
-- [Batch Conversion: Web URLs to Local](#batch-conversion-of-multiple-files-web-url-to-local)
-- [Batch Conversion: Local to Image Server](#batch-conversion-of-multiple-files-local-to-image-hosting-service)
-- [Custom Image Hosting Service](#custom-image-hosting-service)
-
-
-### Converting Web URLs to Local File Paths
-
-If you have web URL links for images in your Markdown file and you want to download them in bulk to your local machine while converting the image addresses in Markdown to local file paths, the following example will solve your problem.
-
-Assuming the file you want to convert is `test.md` with the following content:
-
-> The examples below will be based on the initial Markdown file if it is a web URL. They are not repeated here.
-
-```text
-## 6.3 Converting MD Image Addresses
-Only supports uploading to a local image hosting service.
-
-- [https://github.com/JyHu/useful_script.git](https://github.com/JyHu/useful_script.git)
-- [https://github.com/JyHu/useful_script/blob/](https://github.com/JyHu/useful_script/blob/master/Scripts/md%E6%96%87%E4%BB%B6%E5%9B%BE%E7%89%87%E5%9B%BE%E5%BA%8A%E8%BD%AC%E6%8D%A2/%E8%87%AA%E5%8A%A8%E8%BD%AC%E6%8D%A2markdown%E6%96%87%E4%BB%B6%E4%B8%AD%E5%9B%BE%E7%89%87%E5%88%B0%E5%9B%BE%E5%BA%8A.md/)
-
-After all the hassle and trying this, I found it doesn't work either.
-![image.png](https://cdn.nlark.com/yuque/0/2022/png/26910220/1670091709979-52f8c3c4-a00f-4668-a236-29ad2c09d0da.png#averageHue=%23272c34&clientId=ubb991e0d-3414-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=928&id=u4a7a8376&margin=%5Bobject%20Object%5D&name=image.png&originHeight=928&originWidth=1050&originalType=binary&ratio=1&rotation=0&showTitle=false&size=201083&status=done&style=none&taskId=u27493dc0-9d78-4c07-929c-cc946d41409&title=&width=1050)
-
-In the end, PigGo is still the best. It provides a shortcut for uploading, and after uploading, you can directly xxxTODO.
-
-## 6.4 Pycasbin
-
-In pycasbin, I saw a colleague who frequently contributes to pycasbin. You can refer to some of his contributions:
-
-- [https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md](https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md)
-
-
-![image.png](https://cdn.nlark.com/yuque/0/2022/png/26910220/1670150012015-3a93ec6b-bb27-4ed3-b42f-252a0f70b65c.png#averageHue=%23fcfbf5&clientId=u86ce0a81-ec80-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=936&id=ube9c482c&margin=%5Bobject%20Object%5D&name=image.png&originHeight=936&originWidth=1920&originalType=binary&ratio=1&rotation=0&showTitle=false&size=205691&status=done&style=none&taskId=u6a6825da-aaf4-471c-ad0e-2280c325c66&title=&width=1920)
-```
-
-This content is the exported Markdown file from Yuque, and its image links are protected against external access. They need to be downloaded and replaced with local file paths in the Markdown.
-
-```python
-from imarkdown import MdFile, LocalFileAdapter, MdImageConverter
-
-def main():
-    adapter = LocalFileAdapter()
-    converter = MdImageConverter(adapter=adapter)
-    
-    md_file = MdFile(name="test.md")
-    converter.convert(md_file)
-
-if __name__ == '__main__':
-    main()
-```
-
-> In imarkdown, there are many places where you need to provide paths. You can use relative paths or absolute paths. It is recommended to use `/` as the path separator instead of `\\`.
-
-The converted result will generate a new Markdown file named `test_converted.md`, with the following content:
-
-```text
-## 6.3 Converting MD Image Addresses
-Only supports uploading to a local image hosting service.
-
-- [https://github.com/JyHu/useful_script.git](https://github.com/JyHu/useful_script.git)
-- [https://github.com/JyHu/useful_script/blob/](https://github.com/JyHu/useful_script/blob/master/Scripts/md%E6%96%87%E4%BB%B6%E5%9B%BE%E7%89%87%E5%9B%BE%E5%BA%8A%E8%BD%AC%E6%8D%A2/%E8%87%AA%E5%8A%A8%E8%BD%AC%E6%8D%A2markdown%E6%96%87%E4%BB%B6%E4%B8%AD%E5%9B%BE%E7%89%87%E5%88%B0%E5%9B%BE%E5%BA%8A.md/)
-
-After all the hassle and trying this, I found it doesn't work either.
-![image.png](./images/20230713_1356451324.png)
-
-In the end, PigGo is still the best. It provides a shortcut for uploading, and after uploading, you can directly xxxTODO.
-
-## 6.4 Pycasbin
-
-In pycasbin, I saw a colleague who frequently contributes to pycasbin. You can refer to some of his contributions:
-
-- [https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md](https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md)
-
-
-![image.png](./images/20230713_1356469646.png)
-```
-
-- Customizing the Output File Name
-When using imarkdown for conversion, the default name for the converted Markdown file is `{markdown_file_name}_converted.md`. If you want to customize the output file name, you can use the following configuration:
-
-```python
-md_converter.convert(md_file, name_prefix="new_", name_suffix="_converted")
-```
-
-Using this method of conversion will result in a file named `new_test_converted.md`. If you want to completely customize the converted name, you can use the following method:
-
-```python
-md_converter.convert(md_file, new_name="A new markdown.md")
-```
-
-With the above method, a file named `A new markdown.md` will be generated.
-
-### Converting Web URLs to Image Hosting Service URLs
-
-In the following example, we will use the `test.md` file provided earlier to demonstrate the conversion of image addresses from web URLs to URLs on the Alibaba Cloud OSS server, showcasing the functionality of converting web URLs to image hosting service URLs.
-
-```python
-from imarkdown import MdImageConverter, AliyunAdapter, MdFile
-
-
-def main():
-    aliyun_config = {
-        "access_key_id": "key_id",
-        "access_key_secret": "key_secret",
-        "bucket_name": "bucket_name",
-        "place": "bucket_place",
-        "storage_path_prefix": "prefix",
-    }
-    adapter = AliyunAdapter(**aliyun_config)
-    md_converter = MdImageConverter(adapter=adapter)
-    md_file = MdFile(name="markdown.md")
-    md_converter.convert(md_file)
-
-
-if __name__ == "__main__":
-    main()
-```
-
-In the example above, `storage_path_prefix` represents the file prefix in the bucket where the image is uploaded to OSS. If you want to store the image in the `/imarkdown` directory, you need to set `storage_path_prefix="/imarkdown"`. The remaining configuration details are specific to Alibaba Cloud OSS, so please fill them in accordingly.
-
-
-### Batch Conversion of Multiple Files: Web URL to Local
-
-The following example demonstrates a solution for batch conversion of multiple Markdown files, converting web image URLs to local image addresses.
-
-```python
-from imarkdown import LocalFileAdapter, MdFolder, MdImageConverter
-
-def main():
-    adapter = LocalFileAdapter()
-    converter = MdImageConverter(adapter=adapter)
-    
-    # Folder name is "mds"
-    md_folder = MdFolder(name="mds")
-    # Output files to "converted_mds"
-    converter.convert(md_folder, output_directory="converted_mds")
-```
-
-Using the above code snippet will create a folder named "converted_mds" where the converted files will be saved. The images will be saved in the `converted_mds/images` directory. If you want to output the images to a specific folder, you can set it as follows:
-
-```python
-md_folder = MdFolder(name="mds", image_directory="mds/my_images")
-```
-
-### Batch Conversion of Multiple Files: Local to Image Hosting Service
-
-The following example demonstrates a solution for batch conversion of multiple Markdown files, converting local image addresses to image hosting service URLs.
-
-```python
-from imarkdown import LocalFileAdapter, MdFolder, MdImageConverter
-
-def main():
-    adapter = LocalFileAdapter()
-    converter = MdImageConverter(adapter=adapter)
-    
-    # Folder name is "local_mds", images are of local type, and image URLs are saved in "local_mds/images"
-    md_folder = MdFolder(name="local_mds", image_type="local", image_directory="local_mds/images")
-    # Output files to "converted_mds"
-    converter.convert(md_folder, output_directory="converted_mds")
-```
-
-### Custom Image Hosting Service
-
-The following example demonstrates how to use imarkdown to upload images to a custom file server and retrieve the URL.
-
-First, you need to create a custom adapter by inheriting from `BaseMdAdapter` and implementing the `upload` and `get_replaced_url` methods. Then, you can inject the custom adapter into `MdImageConverter`.
-
-```python
-import os
-import json
-
-import requests
-from imarkdown import BaseMdAdapter, MdImageConverter, MdFolder
-
-class CustomMdAdapter(BaseMdAdapter):
-    name = "custom"
-    url = "https://server/upload/file/batch"
-    headers = {
-        "X-Upload-Token": "my_token"
-    }
-    cur_key = ""
-
-    def upload(self, key: str, file):
-        files = {"file": file}
-        response = requests.post(self.url, headers=self.headers, files=files)
-        if response.status_code == 200:
-            res_data = json.loads(response.content.decode("utf-8"))
-            self.cur_key = res_data["data"]["images"]["url"]
-        else:
-            raise Exception(response.content)
-
-    def get_replaced_url(self, key):
-        return self.cur_key
-
-def get_all_folder_names():
-    return os.listdir("my-blog")
-
-    
-def main():
-    adapter = CustomMdAdapter()
-    md_converter = MdImageConverter(adapter=adapter)
-
-    md_folders = []
-    for folder_name in get_all_folder_names():
-        md_folders.append(
-            MdFolder(
-                name=f"my-blog/{folder_name}",
-                image_directory=f"my-blog/{folder_name}/images",
-                image_type="local",
-            )
-        )
-    md_converter.convert(md_folders, output_directory="converted")
-
-
-if __name__ == "__main__":
-    main()
-```
-
-## Roadmap
-
-- [ ] Add client-side support
-- [ ] Support Tencent Cloud, Qiniu Cloud, and other image hosting services
-- [x] Support batch file modification
-- [x] Custom adapters
-- [ ] Support compression of large images
-- [ ] Support command-line interface
-- [x] Support PyPI for simplified operations
-- [ ] Provide file custom naming
-- [ ] Provide custom formatting for image names
-
-## FAQ
-
-**1. How can I extend to other image hosting services?**
-
-If you want to develop support for other image hosting services, all you need to do is implement an adapter similar to `AliyunAdapter` and inject it into `MdImageConverter` when using it. Refer to [Custom Image Hosting Service](#custom-image-hosting-service). That's all you need to do. In fact, I've wrapped it up nicely, so extending it is straightforward.
-
-**2. Usage of file addresses**
-
-In Python, both `/` and `\\` can be used as file path separators. However, there are some differences in their usage.
-
-- `/` (forward slash): In most operating systems, including Windows, Linux, and Mac, `/` is used as the file path separator. Using `/` as the separator can make your code portable across different operating systems. For example:
-
-```python
-path = "folder/file.txt"
-```
-
-- `\\` (backslash): In the Windows operating system, `\\` is used as the file path separator. This is because `\` is used as an escape character in Windows, so to represent a plain backslash, you need to use two consecutive backslashes. For example:
-
-```python
-path = "folder\\file.txt"
-```
-
-When using `\\` as the separator, keep the following points in mind:
-
-- When using `\\` in a string, you need to escape it as `\\\\` because the first `\` will be interpreted as an escape character.
-- You can use raw strings to avoid the hassle of escaping. In a raw string, `\` is not interpreted as an escape character. For example: `path = r"folder\file.txt"`
-
-In summary, if your code needs to run on different operating systems, it is recommended to use `/` as the file path separator to maintain code portability. If you are only running the code on Windows, using `\\` is also acceptable. However, in `imarkdown`, all `\\` paths will be converted to `/`. In this project, all `\\` paths will be converted to `/`.
-
-## Contribution
-
-Contributions are welcome! If you would like to contribute to this project, you can submit a pull request or an issue. There are some extensible features listed in the [Development Roadmap](#development-roadmap), and there are still many third-party image hosting services that need to be adapted. If you are working on these aspects, feel free to submit a pull request! I'm excited to see more people involved in improving and optimizing it.
+Metadata-Version: 2.1
+Name: imarkdown
+Version: 1.2.1
+Summary: A practical Markdown image url converter
+Home-page: https://github.com/Undertone0809/imarkdown
+Author: Zeeland
+Author-email: zeeland@foxmail.com
+License: Apache 2.0
+Keywords: Markdown,markdown,imarkdown,markdown converter
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+
+<h1 align="center">
+    imarkdown
+</h1>
+<p align="center">
+  <strong>imarkdown is a lightweight markdown image link converter that allows you to easily convert image links between local and image server, as well as between different image servers.</strong>
+</p>
+
+[English](/README.md) [中文](/README_zh.md)
+
+> When converting markdown from Yuque, the images are protected against external linking. If you want to publish the converted markdown on other platforms, you need to change all the image addresses in the markdown to local image addresses or custom image server addresses, so that others can view them correctly. This project aims to solve this problem by providing a converter that can batch convert image links in markdown and supports customized conversion in complex scenarios.
+
+## Features
+
+- Batch Download: imarkdown can batch download all the images in the markdown that are referenced using image links.
+- Multiple Conversion Methods: imarkdown supports various conversion methods for image links in markdown, such as converting to local image, converting web URL to local image, and converting web URL to image server URL.
+- Batch Conversion: It supports batch conversion of single or multiple files, as well as formatting and renaming of generated files.
+- Highly Customizable: By inheriting the `MdAdapter` class, you can easily implement custom URL conversion for different image servers.
+- Image Server Adapters: Currently, only Aliyun OSS is supported as an image server. Contributions are welcome to add support for more types of image servers.
+
+## Target Audience
+
+- People who need to batch convert image links in markdown.
+- Users who export markdown from Yuque and need to convert image links.
+- People who need to develop third-party extensions.
+
+## Technical Architecture
+
+`imarkdown` is designed with a modular architecture, allowing easy extension of each component. The following diagram provides a simplified overview of the technical architecture of imarkdown, which consists of the following components:
+
+- `MdImageConverter`: The image converter responsible for converting the image addresses in markdown and generating new markdown files.
+- `MdAdapter`: The adapter for converting `Image` objects to different types, such as `LocalFileAdapter` for local conversion, `AliyunAdapter` for Aliyun OSS conversion, and `CustomAdapter` for custom conversion. By injecting the adapter into `MdImageConverter`, you can define the type of address to convert `Image` objects to.
+- `MdMedium`: Includes `MdFile` and `MdFolder`, encapsulating some features used for data conversion in `MdImageConverter`.
+
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230713154424.png"/>
+
+The execution process of `imarkdown` is roughly as follows: after the `convert` method is called on `MdImageConverter`, `imarkdown` builds a virtual `MdTree` based on the provided `MdMedium`, and performs batch image URL conversion on the files according to this tree.
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230713155912.png"/>
+
+## Quick Start
+
+This project is developed in Python and distributed on PyPI. Users can easily use imarkdown by installing it with pip. The following sections will explain several usage scenarios and methods of imarkdown.
+
+- Third-Party Package Installation: Open a terminal or command prompt and run the following command.
+
+```sh
+pip install -U imarkdown
+```
+
+**Examples**
+- [Convert Web URLs to Local Addresses](#converting-web-urls-to-local-file-paths)
+- [Convert Web URLs to Image Server URLs](#converting-web-urls-to-image-hosting-service-urls)
+- [Batch Conversion: Web URLs to Local](#batch-conversion-of-multiple-files-web-url-to-local)
+- [Batch Conversion: Local to Image Server](#batch-conversion-of-multiple-files-local-to-image-hosting-service)
+- [Custom Image Hosting Service](#custom-image-hosting-service)
+
+
+### Converting Web URLs to Local File Paths
+
+If you have web URL links for images in your Markdown file and you want to download them in bulk to your local machine while converting the image addresses in Markdown to local file paths, the following example will solve your problem.
+
+Assuming the file you want to convert is `test.md` with the following content:
+
+> The examples below will be based on the initial Markdown file if it is a web URL. They are not repeated here.
+
+```text
+## 6.3 Converting MD Image Addresses
+Only supports uploading to a local image hosting service.
+
+- [https://github.com/JyHu/useful_script.git](https://github.com/JyHu/useful_script.git)
+- [https://github.com/JyHu/useful_script/blob/](https://github.com/JyHu/useful_script/blob/master/Scripts/md%E6%96%87%E4%BB%B6%E5%9B%BE%E7%89%87%E5%9B%BE%E5%BA%8A%E8%BD%AC%E6%8D%A2/%E8%87%AA%E5%8A%A8%E8%BD%AC%E6%8D%A2markdown%E6%96%87%E4%BB%B6%E4%B8%AD%E5%9B%BE%E7%89%87%E5%88%B0%E5%9B%BE%E5%BA%8A.md/)
+
+After all the hassle and trying this, I found it doesn't work either.
+![image.png](https://cdn.nlark.com/yuque/0/2022/png/26910220/1670091709979-52f8c3c4-a00f-4668-a236-29ad2c09d0da.png#averageHue=%23272c34&clientId=ubb991e0d-3414-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=928&id=u4a7a8376&margin=%5Bobject%20Object%5D&name=image.png&originHeight=928&originWidth=1050&originalType=binary&ratio=1&rotation=0&showTitle=false&size=201083&status=done&style=none&taskId=u27493dc0-9d78-4c07-929c-cc946d41409&title=&width=1050)
+
+In the end, PigGo is still the best. It provides a shortcut for uploading, and after uploading, you can directly xxxTODO.
+
+## 6.4 Pycasbin
+
+In pycasbin, I saw a colleague who frequently contributes to pycasbin. You can refer to some of his contributions:
+
+- [https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md](https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md)
+
+
+![image.png](https://cdn.nlark.com/yuque/0/2022/png/26910220/1670150012015-3a93ec6b-bb27-4ed3-b42f-252a0f70b65c.png#averageHue=%23fcfbf5&clientId=u86ce0a81-ec80-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=936&id=ube9c482c&margin=%5Bobject%20Object%5D&name=image.png&originHeight=936&originWidth=1920&originalType=binary&ratio=1&rotation=0&showTitle=false&size=205691&status=done&style=none&taskId=u6a6825da-aaf4-471c-ad0e-2280c325c66&title=&width=1920)
+```
+
+This content is the exported Markdown file from Yuque, and its image links are protected against external access. They need to be downloaded and replaced with local file paths in the Markdown.
+
+```python
+from imarkdown import MdFile, LocalFileAdapter, MdImageConverter
+
+def main():
+    adapter = LocalFileAdapter()
+    converter = MdImageConverter(adapter=adapter)
+    
+    md_file = MdFile(name="test.md")
+    converter.convert(md_file)
+
+if __name__ == '__main__':
+    main()
+```
+
+> In imarkdown, there are many places where you need to provide paths. You can use relative paths or absolute paths. It is recommended to use `/` as the path separator instead of `\\`.
+
+The converted result will generate a new Markdown file named `test_converted.md`, with the following content:
+
+```text
+## 6.3 Converting MD Image Addresses
+Only supports uploading to a local image hosting service.
+
+- [https://github.com/JyHu/useful_script.git](https://github.com/JyHu/useful_script.git)
+- [https://github.com/JyHu/useful_script/blob/](https://github.com/JyHu/useful_script/blob/master/Scripts/md%E6%96%87%E4%BB%B6%E5%9B%BE%E7%89%87%E5%9B%BE%E5%BA%8A%E8%BD%AC%E6%8D%A2/%E8%87%AA%E5%8A%A8%E8%BD%AC%E6%8D%A2markdown%E6%96%87%E4%BB%B6%E4%B8%AD%E5%9B%BE%E7%89%87%E5%88%B0%E5%9B%BE%E5%BA%8A.md/)
+
+After all the hassle and trying this, I found it doesn't work either.
+![image.png](./images/20230713_1356451324.png)
+
+In the end, PigGo is still the best. It provides a shortcut for uploading, and after uploading, you can directly xxxTODO.
+
+## 6.4 Pycasbin
+
+In pycasbin, I saw a colleague who frequently contributes to pycasbin. You can refer to some of his contributions:
+
+- [https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md](https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md)
+
+
+![image.png](./images/20230713_1356469646.png)
+```
+
+- Customizing the Output File Name
+When using imarkdown for conversion, the default name for the converted Markdown file is `{markdown_file_name}_converted.md`. If you want to customize the output file name, you can use the following configuration:
+
+```python
+md_converter.convert(md_file, name_prefix="new_", name_suffix="_converted")
+```
+
+Using this method of conversion will result in a file named `new_test_converted.md`. If you want to completely customize the converted name, you can use the following method:
+
+```python
+md_converter.convert(md_file, new_name="A new markdown.md")
+```
+
+With the above method, a file named `A new markdown.md` will be generated.
+
+### Converting Web URLs to Image Hosting Service URLs
+
+In the following example, we will use the `test.md` file provided earlier to demonstrate the conversion of image addresses from web URLs to URLs on the Alibaba Cloud OSS server, showcasing the functionality of converting web URLs to image hosting service URLs.
+
+```python
+from imarkdown import MdImageConverter, AliyunAdapter, MdFile
+
+
+def main():
+    aliyun_config = {
+        "access_key_id": "key_id",
+        "access_key_secret": "key_secret",
+        "bucket_name": "bucket_name",
+        "place": "bucket_place",
+        "storage_path_prefix": "prefix",
+    }
+    adapter = AliyunAdapter(**aliyun_config)
+    md_converter = MdImageConverter(adapter=adapter)
+    md_file = MdFile(name="markdown.md")
+    md_converter.convert(md_file)
+
+
+if __name__ == "__main__":
+    main()
+```
+
+In the example above, `storage_path_prefix` represents the file prefix in the bucket where the image is uploaded to OSS. If you want to store the image in the `/imarkdown` directory, you need to set `storage_path_prefix="/imarkdown"`. The remaining configuration details are specific to Alibaba Cloud OSS, so please fill them in accordingly.
+
+
+### Batch Conversion of Multiple Files: Web URL to Local
+
+The following example demonstrates a solution for batch conversion of multiple Markdown files, converting web image URLs to local image addresses.
+
+```python
+from imarkdown import LocalFileAdapter, MdFolder, MdImageConverter
+
+def main():
+    adapter = LocalFileAdapter()
+    converter = MdImageConverter(adapter=adapter)
+    
+    # Folder name is "mds"
+    md_folder = MdFolder(name="mds")
+    # Output files to "converted_mds"
+    converter.convert(md_folder, output_directory="converted_mds")
+```
+
+Using the above code snippet will create a folder named "converted_mds" where the converted files will be saved. The images will be saved in the `converted_mds/images` directory. If you want to output the images to a specific folder, you can set it as follows:
+
+```python
+md_folder = MdFolder(name="mds", image_directory="mds/my_images")
+```
+
+### Batch Conversion of Multiple Files: Local to Image Hosting Service
+
+The following example demonstrates a solution for batch conversion of multiple Markdown files, converting local image addresses to image hosting service URLs.
+
+```python
+from imarkdown import LocalFileAdapter, MdFolder, MdImageConverter
+
+def main():
+    adapter = LocalFileAdapter()
+    converter = MdImageConverter(adapter=adapter)
+    
+    # Folder name is "local_mds", images are of local type, and image URLs are saved in "local_mds/images"
+    md_folder = MdFolder(name="local_mds", image_type="local", image_directory="local_mds/images")
+    # Output files to "converted_mds"
+    converter.convert(md_folder, output_directory="converted_mds")
+```
+
+### Custom Image Hosting Service
+
+The following example demonstrates how to use imarkdown to upload images to a custom file server and retrieve the URL.
+
+First, you need to create a custom adapter by inheriting from `BaseMdAdapter` and implementing the `upload` and `get_replaced_url` methods. Then, you can inject the custom adapter into `MdImageConverter`.
+
+```python
+import os
+import json
+
+import requests
+from imarkdown import BaseMdAdapter, MdImageConverter, MdFolder
+
+class CustomMdAdapter(BaseMdAdapter):
+    name = "custom"
+    url = "https://server/upload/file/batch"
+    headers = {
+        "X-Upload-Token": "my_token"
+    }
+    cur_key = ""
+
+    def upload(self, key: str, file):
+        files = {"file": file}
+        response = requests.post(self.url, headers=self.headers, files=files)
+        if response.status_code == 200:
+            res_data = json.loads(response.content.decode("utf-8"))
+            self.cur_key = res_data["data"]["images"]["url"]
+        else:
+            raise Exception(response.content)
+
+    def get_replaced_url(self, key):
+        return self.cur_key
+
+def get_all_folder_names():
+    return os.listdir("my-blog")
+
+    
+def main():
+    adapter = CustomMdAdapter()
+    md_converter = MdImageConverter(adapter=adapter)
+
+    md_folders = []
+    for folder_name in get_all_folder_names():
+        md_folders.append(
+            MdFolder(
+                name=f"my-blog/{folder_name}",
+                image_directory=f"my-blog/{folder_name}/images",
+                image_type="local",
+            )
+        )
+    md_converter.convert(md_folders, output_directory="converted")
+
+
+if __name__ == "__main__":
+    main()
+```
+
+### Custom Regular Expression
+`imarkdown` use regular expression to find your images. It supports `![](image_url)` and `<img src="image_url"/>` format, but there are still some other format `imarkdown` can not find it.
+
+At this point, `imarkdown` supports custom regular expression to address this issue. You can customize a regular expression which can find your markdown image url and pass it to MdImageConverter. The following example show how to use it.
+
+```python
+from imarkdown import MdImageConverter, LocalFileAdapter, MdFolder
+
+
+def main():
+    custom_re = r"(?:!\[(.*?)\]\((.*?)\))|<img.*?src=[\'\"](.*?)[\'\"].*?>"
+    adapter = LocalFileAdapter()
+    md_converter = MdImageConverter(adapter=adapter)
+    
+    md_folder = MdFolder(name="mds")
+    md_converter.convert(md_folder, output_directory="output_mds", re_rule=custom_re)
+
+
+if __name__ == "__main__":
+    main()
+```
+
+## Roadmap
+
+- [ ] Add client-side support
+- [ ] Support Tencent Cloud, Qiniu Cloud, and other image hosting services
+- [x] Support batch file modification
+- [x] Custom adapters
+- [ ] Support compression of large images
+- [ ] Support command-line interface
+- [x] Support PyPI for simplified operations
+- [ ] Provide file custom naming
+- [ ] Provide custom formatting for image names
+
+## FAQ
+
+**1. How can I extend to other image hosting services?**
+
+If you want to develop support for other image hosting services, all you need to do is implement an adapter similar to `AliyunAdapter` and inject it into `MdImageConverter` when using it. Refer to [Custom Image Hosting Service](#custom-image-hosting-service). That's all you need to do. In fact, I've wrapped it up nicely, so extending it is straightforward.
+
+**2. Usage of file addresses**
+
+In Python, both `/` and `\\` can be used as file path separators. However, there are some differences in their usage.
+
+- `/` (forward slash): In most operating systems, including Windows, Linux, and Mac, `/` is used as the file path separator. Using `/` as the separator can make your code portable across different operating systems. For example:
+
+```python
+path = "folder/file.txt"
+```
+
+- `\\` (backslash): In the Windows operating system, `\\` is used as the file path separator. This is because `\` is used as an escape character in Windows, so to represent a plain backslash, you need to use two consecutive backslashes. For example:
+
+```python
+path = "folder\\file.txt"
+```
+
+When using `\\` as the separator, keep the following points in mind:
+
+- When using `\\` in a string, you need to escape it as `\\\\` because the first `\` will be interpreted as an escape character.
+- You can use raw strings to avoid the hassle of escaping. In a raw string, `\` is not interpreted as an escape character. For example: `path = r"folder\file.txt"`
+
+In summary, if your code needs to run on different operating systems, it is recommended to use `/` as the file path separator to maintain code portability. If you are only running the code on Windows, using `\\` is also acceptable. However, in `imarkdown`, all `\\` paths will be converted to `/`. In this project, all `\\` paths will be converted to `/`.
+
+## Contribution
+
+Contributions are welcome! If you would like to contribute to this project, you can submit a pull request or an issue. There are some extensible features listed in the [Development Roadmap](#development-roadmap), and there are still many third-party image hosting services that need to be adapted. If you are working on these aspects, feel free to submit a pull request! I'm excited to see more people involved in improving and optimizing it.
```

### Comparing `imarkdown-1.1.2/README.md` & `imarkdown-1.2.1/imarkdown.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,315 +1,358 @@
-<h1 align="center">
-    imarkdown
-</h1>
-<p align="center">
-  <strong>imarkdown is a lightweight markdown image link converter that allows you to easily convert image links between local and image server, as well as between different image servers.</strong>
-</p>
-
-[English](/README.md) [中文](/README_zh.md)
-
-> When converting markdown from Yuque, the images are protected against external linking. If you want to publish the converted markdown on other platforms, you need to change all the image addresses in the markdown to local image addresses or custom image server addresses, so that others can view them correctly. This project aims to solve this problem by providing a converter that can batch convert image links in markdown and supports customized conversion in complex scenarios.
-
-## Features
-
-- Batch Download: imarkdown can batch download all the images in the markdown that are referenced using image links.
-- Multiple Conversion Methods: imarkdown supports various conversion methods for image links in markdown, such as converting to local image, converting web URL to local image, and converting web URL to image server URL.
-- Batch Conversion: It supports batch conversion of single or multiple files, as well as formatting and renaming of generated files.
-- Highly Customizable: By inheriting the `MdAdapter` class, you can easily implement custom URL conversion for different image servers.
-- Image Server Adapters: Currently, only Aliyun OSS is supported as an image server. Contributions are welcome to add support for more types of image servers.
-
-## Target Audience
-
-- People who need to batch convert image links in markdown.
-- Users who export markdown from Yuque and need to convert image links.
-- People who need to develop third-party extensions.
-
-## Technical Architecture
-
-`imarkdown` is designed with a modular architecture, allowing easy extension of each component. The following diagram provides a simplified overview of the technical architecture of imarkdown, which consists of the following components:
-
-- `MdImageConverter`: The image converter responsible for converting the image addresses in markdown and generating new markdown files.
-- `MdAdapter`: The adapter for converting `Image` objects to different types, such as `LocalFileAdapter` for local conversion, `AliyunAdapter` for Aliyun OSS conversion, and `CustomAdapter` for custom conversion. By injecting the adapter into `MdImageConverter`, you can define the type of address to convert `Image` objects to.
-- `MdMedium`: Includes `MdFile` and `MdFolder`, encapsulating some features used for data conversion in `MdImageConverter`.
-
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230713154424.png"/>
-
-The execution process of `imarkdown` is roughly as follows: after the `convert` method is called on `MdImageConverter`, `imarkdown` builds a virtual `MdTree` based on the provided `MdMedium`, and performs batch image URL conversion on the files according to this tree.
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230713155912.png"/>
-
-## Quick Start
-
-This project is developed in Python and distributed on PyPI. Users can easily use imarkdown by installing it with pip. The following sections will explain several usage scenarios and methods of imarkdown.
-
-- Third-Party Package Installation: Open a terminal or command prompt and run the following command.
-
-```sh
-pip install -U imarkdown
-```
-
-**Examples**
-- [Convert Web URLs to Local Addresses](#converting-web-urls-to-local-file-paths)
-- [Convert Web URLs to Image Server URLs](#converting-web-urls-to-image-hosting-service-urls)
-- [Batch Conversion: Web URLs to Local](#batch-conversion-of-multiple-files-web-url-to-local)
-- [Batch Conversion: Local to Image Server](#batch-conversion-of-multiple-files-local-to-image-hosting-service)
-- [Custom Image Hosting Service](#custom-image-hosting-service)
-
-
-### Converting Web URLs to Local File Paths
-
-If you have web URL links for images in your Markdown file and you want to download them in bulk to your local machine while converting the image addresses in Markdown to local file paths, the following example will solve your problem.
-
-Assuming the file you want to convert is `test.md` with the following content:
-
-> The examples below will be based on the initial Markdown file if it is a web URL. They are not repeated here.
-
-```text
-## 6.3 Converting MD Image Addresses
-Only supports uploading to a local image hosting service.
-
-- [https://github.com/JyHu/useful_script.git](https://github.com/JyHu/useful_script.git)
-- [https://github.com/JyHu/useful_script/blob/](https://github.com/JyHu/useful_script/blob/master/Scripts/md%E6%96%87%E4%BB%B6%E5%9B%BE%E7%89%87%E5%9B%BE%E5%BA%8A%E8%BD%AC%E6%8D%A2/%E8%87%AA%E5%8A%A8%E8%BD%AC%E6%8D%A2markdown%E6%96%87%E4%BB%B6%E4%B8%AD%E5%9B%BE%E7%89%87%E5%88%B0%E5%9B%BE%E5%BA%8A.md/)
-
-After all the hassle and trying this, I found it doesn't work either.
-![image.png](https://cdn.nlark.com/yuque/0/2022/png/26910220/1670091709979-52f8c3c4-a00f-4668-a236-29ad2c09d0da.png#averageHue=%23272c34&clientId=ubb991e0d-3414-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=928&id=u4a7a8376&margin=%5Bobject%20Object%5D&name=image.png&originHeight=928&originWidth=1050&originalType=binary&ratio=1&rotation=0&showTitle=false&size=201083&status=done&style=none&taskId=u27493dc0-9d78-4c07-929c-cc946d41409&title=&width=1050)
-
-In the end, PigGo is still the best. It provides a shortcut for uploading, and after uploading, you can directly xxxTODO.
-
-## 6.4 Pycasbin
-
-In pycasbin, I saw a colleague who frequently contributes to pycasbin. You can refer to some of his contributions:
-
-- [https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md](https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md)
-
-
-![image.png](https://cdn.nlark.com/yuque/0/2022/png/26910220/1670150012015-3a93ec6b-bb27-4ed3-b42f-252a0f70b65c.png#averageHue=%23fcfbf5&clientId=u86ce0a81-ec80-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=936&id=ube9c482c&margin=%5Bobject%20Object%5D&name=image.png&originHeight=936&originWidth=1920&originalType=binary&ratio=1&rotation=0&showTitle=false&size=205691&status=done&style=none&taskId=u6a6825da-aaf4-471c-ad0e-2280c325c66&title=&width=1920)
-```
-
-This content is the exported Markdown file from Yuque, and its image links are protected against external access. They need to be downloaded and replaced with local file paths in the Markdown.
-
-```python
-from imarkdown import MdFile, LocalFileAdapter, MdImageConverter
-
-def main():
-    adapter = LocalFileAdapter()
-    converter = MdImageConverter(adapter=adapter)
-    
-    md_file = MdFile(name="test.md")
-    converter.convert(md_file)
-
-if __name__ == '__main__':
-    main()
-```
-
-> In imarkdown, there are many places where you need to provide paths. You can use relative paths or absolute paths. It is recommended to use `/` as the path separator instead of `\\`.
-
-The converted result will generate a new Markdown file named `test_converted.md`, with the following content:
-
-```text
-## 6.3 Converting MD Image Addresses
-Only supports uploading to a local image hosting service.
-
-- [https://github.com/JyHu/useful_script.git](https://github.com/JyHu/useful_script.git)
-- [https://github.com/JyHu/useful_script/blob/](https://github.com/JyHu/useful_script/blob/master/Scripts/md%E6%96%87%E4%BB%B6%E5%9B%BE%E7%89%87%E5%9B%BE%E5%BA%8A%E8%BD%AC%E6%8D%A2/%E8%87%AA%E5%8A%A8%E8%BD%AC%E6%8D%A2markdown%E6%96%87%E4%BB%B6%E4%B8%AD%E5%9B%BE%E7%89%87%E5%88%B0%E5%9B%BE%E5%BA%8A.md/)
-
-After all the hassle and trying this, I found it doesn't work either.
-![image.png](./images/20230713_1356451324.png)
-
-In the end, PigGo is still the best. It provides a shortcut for uploading, and after uploading, you can directly xxxTODO.
-
-## 6.4 Pycasbin
-
-In pycasbin, I saw a colleague who frequently contributes to pycasbin. You can refer to some of his contributions:
-
-- [https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md](https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md)
-
-
-![image.png](./images/20230713_1356469646.png)
-```
-
-- Customizing the Output File Name
-When using imarkdown for conversion, the default name for the converted Markdown file is `{markdown_file_name}_converted.md`. If you want to customize the output file name, you can use the following configuration:
-
-```python
-md_converter.convert(md_file, name_prefix="new_", name_suffix="_converted")
-```
-
-Using this method of conversion will result in a file named `new_test_converted.md`. If you want to completely customize the converted name, you can use the following method:
-
-```python
-md_converter.convert(md_file, new_name="A new markdown.md")
-```
-
-With the above method, a file named `A new markdown.md` will be generated.
-
-### Converting Web URLs to Image Hosting Service URLs
-
-In the following example, we will use the `test.md` file provided earlier to demonstrate the conversion of image addresses from web URLs to URLs on the Alibaba Cloud OSS server, showcasing the functionality of converting web URLs to image hosting service URLs.
-
-```python
-from imarkdown import MdImageConverter, AliyunAdapter, MdFile
-
-
-def main():
-    aliyun_config = {
-        "access_key_id": "key_id",
-        "access_key_secret": "key_secret",
-        "bucket_name": "bucket_name",
-        "place": "bucket_place",
-        "storage_path_prefix": "prefix",
-    }
-    adapter = AliyunAdapter(**aliyun_config)
-    md_converter = MdImageConverter(adapter=adapter)
-    md_file = MdFile(name="markdown.md")
-    md_converter.convert(md_file)
-
-
-if __name__ == "__main__":
-    main()
-```
-
-In the example above, `storage_path_prefix` represents the file prefix in the bucket where the image is uploaded to OSS. If you want to store the image in the `/imarkdown` directory, you need to set `storage_path_prefix="/imarkdown"`. The remaining configuration details are specific to Alibaba Cloud OSS, so please fill them in accordingly.
-
-
-### Batch Conversion of Multiple Files: Web URL to Local
-
-The following example demonstrates a solution for batch conversion of multiple Markdown files, converting web image URLs to local image addresses.
-
-```python
-from imarkdown import LocalFileAdapter, MdFolder, MdImageConverter
-
-def main():
-    adapter = LocalFileAdapter()
-    converter = MdImageConverter(adapter=adapter)
-    
-    # Folder name is "mds"
-    md_folder = MdFolder(name="mds")
-    # Output files to "converted_mds"
-    converter.convert(md_folder, output_directory="converted_mds")
-```
-
-Using the above code snippet will create a folder named "converted_mds" where the converted files will be saved. The images will be saved in the `converted_mds/images` directory. If you want to output the images to a specific folder, you can set it as follows:
-
-```python
-md_folder = MdFolder(name="mds", image_directory="mds/my_images")
-```
-
-### Batch Conversion of Multiple Files: Local to Image Hosting Service
-
-The following example demonstrates a solution for batch conversion of multiple Markdown files, converting local image addresses to image hosting service URLs.
-
-```python
-from imarkdown import LocalFileAdapter, MdFolder, MdImageConverter
-
-def main():
-    adapter = LocalFileAdapter()
-    converter = MdImageConverter(adapter=adapter)
-    
-    # Folder name is "local_mds", images are of local type, and image URLs are saved in "local_mds/images"
-    md_folder = MdFolder(name="local_mds", image_type="local", image_directory="local_mds/images")
-    # Output files to "converted_mds"
-    converter.convert(md_folder, output_directory="converted_mds")
-```
-
-### Custom Image Hosting Service
-
-The following example demonstrates how to use imarkdown to upload images to a custom file server and retrieve the URL.
-
-First, you need to create a custom adapter by inheriting from `BaseMdAdapter` and implementing the `upload` and `get_replaced_url` methods. Then, you can inject the custom adapter into `MdImageConverter`.
-
-```python
-import os
-import json
-
-import requests
-from imarkdown import BaseMdAdapter, MdImageConverter, MdFolder
-
-class CustomMdAdapter(BaseMdAdapter):
-    name = "custom"
-    url = "https://server/upload/file/batch"
-    headers = {
-        "X-Upload-Token": "my_token"
-    }
-    cur_key = ""
-
-    def upload(self, key: str, file):
-        files = {"file": file}
-        response = requests.post(self.url, headers=self.headers, files=files)
-        if response.status_code == 200:
-            res_data = json.loads(response.content.decode("utf-8"))
-            self.cur_key = res_data["data"]["images"]["url"]
-        else:
-            raise Exception(response.content)
-
-    def get_replaced_url(self, key):
-        return self.cur_key
-
-def get_all_folder_names():
-    return os.listdir("my-blog")
-
-    
-def main():
-    adapter = CustomMdAdapter()
-    md_converter = MdImageConverter(adapter=adapter)
-
-    md_folders = []
-    for folder_name in get_all_folder_names():
-        md_folders.append(
-            MdFolder(
-                name=f"my-blog/{folder_name}",
-                image_directory=f"my-blog/{folder_name}/images",
-                image_type="local",
-            )
-        )
-    md_converter.convert(md_folders, output_directory="converted")
-
-
-if __name__ == "__main__":
-    main()
-```
-
-## Roadmap
-
-- [ ] Add client-side support
-- [ ] Support Tencent Cloud, Qiniu Cloud, and other image hosting services
-- [x] Support batch file modification
-- [x] Custom adapters
-- [ ] Support compression of large images
-- [ ] Support command-line interface
-- [x] Support PyPI for simplified operations
-- [ ] Provide file custom naming
-- [ ] Provide custom formatting for image names
-
-## FAQ
-
-**1. How can I extend to other image hosting services?**
-
-If you want to develop support for other image hosting services, all you need to do is implement an adapter similar to `AliyunAdapter` and inject it into `MdImageConverter` when using it. Refer to [Custom Image Hosting Service](#custom-image-hosting-service). That's all you need to do. In fact, I've wrapped it up nicely, so extending it is straightforward.
-
-**2. Usage of file addresses**
-
-In Python, both `/` and `\\` can be used as file path separators. However, there are some differences in their usage.
-
-- `/` (forward slash): In most operating systems, including Windows, Linux, and Mac, `/` is used as the file path separator. Using `/` as the separator can make your code portable across different operating systems. For example:
-
-```python
-path = "folder/file.txt"
-```
-
-- `\\` (backslash): In the Windows operating system, `\\` is used as the file path separator. This is because `\` is used as an escape character in Windows, so to represent a plain backslash, you need to use two consecutive backslashes. For example:
-
-```python
-path = "folder\\file.txt"
-```
-
-When using `\\` as the separator, keep the following points in mind:
-
-- When using `\\` in a string, you need to escape it as `\\\\` because the first `\` will be interpreted as an escape character.
-- You can use raw strings to avoid the hassle of escaping. In a raw string, `\` is not interpreted as an escape character. For example: `path = r"folder\file.txt"`
-
-In summary, if your code needs to run on different operating systems, it is recommended to use `/` as the file path separator to maintain code portability. If you are only running the code on Windows, using `\\` is also acceptable. However, in `imarkdown`, all `\\` paths will be converted to `/`. In this project, all `\\` paths will be converted to `/`.
-
-## Contribution
-
-Contributions are welcome! If you would like to contribute to this project, you can submit a pull request or an issue. There are some extensible features listed in the [Development Roadmap](#development-roadmap), and there are still many third-party image hosting services that need to be adapted. If you are working on these aspects, feel free to submit a pull request! I'm excited to see more people involved in improving and optimizing it.
+Metadata-Version: 2.1
+Name: imarkdown
+Version: 1.2.1
+Summary: A practical Markdown image url converter
+Home-page: https://github.com/Undertone0809/imarkdown
+Author: Zeeland
+Author-email: zeeland@foxmail.com
+License: Apache 2.0
+Keywords: Markdown,markdown,imarkdown,markdown converter
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+
+<h1 align="center">
+    imarkdown
+</h1>
+<p align="center">
+  <strong>imarkdown is a lightweight markdown image link converter that allows you to easily convert image links between local and image server, as well as between different image servers.</strong>
+</p>
+
+[English](/README.md) [中文](/README_zh.md)
+
+> When converting markdown from Yuque, the images are protected against external linking. If you want to publish the converted markdown on other platforms, you need to change all the image addresses in the markdown to local image addresses or custom image server addresses, so that others can view them correctly. This project aims to solve this problem by providing a converter that can batch convert image links in markdown and supports customized conversion in complex scenarios.
+
+## Features
+
+- Batch Download: imarkdown can batch download all the images in the markdown that are referenced using image links.
+- Multiple Conversion Methods: imarkdown supports various conversion methods for image links in markdown, such as converting to local image, converting web URL to local image, and converting web URL to image server URL.
+- Batch Conversion: It supports batch conversion of single or multiple files, as well as formatting and renaming of generated files.
+- Highly Customizable: By inheriting the `MdAdapter` class, you can easily implement custom URL conversion for different image servers.
+- Image Server Adapters: Currently, only Aliyun OSS is supported as an image server. Contributions are welcome to add support for more types of image servers.
+
+## Target Audience
+
+- People who need to batch convert image links in markdown.
+- Users who export markdown from Yuque and need to convert image links.
+- People who need to develop third-party extensions.
+
+## Technical Architecture
+
+`imarkdown` is designed with a modular architecture, allowing easy extension of each component. The following diagram provides a simplified overview of the technical architecture of imarkdown, which consists of the following components:
+
+- `MdImageConverter`: The image converter responsible for converting the image addresses in markdown and generating new markdown files.
+- `MdAdapter`: The adapter for converting `Image` objects to different types, such as `LocalFileAdapter` for local conversion, `AliyunAdapter` for Aliyun OSS conversion, and `CustomAdapter` for custom conversion. By injecting the adapter into `MdImageConverter`, you can define the type of address to convert `Image` objects to.
+- `MdMedium`: Includes `MdFile` and `MdFolder`, encapsulating some features used for data conversion in `MdImageConverter`.
+
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230713154424.png"/>
+
+The execution process of `imarkdown` is roughly as follows: after the `convert` method is called on `MdImageConverter`, `imarkdown` builds a virtual `MdTree` based on the provided `MdMedium`, and performs batch image URL conversion on the files according to this tree.
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230713155912.png"/>
+
+## Quick Start
+
+This project is developed in Python and distributed on PyPI. Users can easily use imarkdown by installing it with pip. The following sections will explain several usage scenarios and methods of imarkdown.
+
+- Third-Party Package Installation: Open a terminal or command prompt and run the following command.
+
+```sh
+pip install -U imarkdown
+```
+
+**Examples**
+- [Convert Web URLs to Local Addresses](#converting-web-urls-to-local-file-paths)
+- [Convert Web URLs to Image Server URLs](#converting-web-urls-to-image-hosting-service-urls)
+- [Batch Conversion: Web URLs to Local](#batch-conversion-of-multiple-files-web-url-to-local)
+- [Batch Conversion: Local to Image Server](#batch-conversion-of-multiple-files-local-to-image-hosting-service)
+- [Custom Image Hosting Service](#custom-image-hosting-service)
+
+
+### Converting Web URLs to Local File Paths
+
+If you have web URL links for images in your Markdown file and you want to download them in bulk to your local machine while converting the image addresses in Markdown to local file paths, the following example will solve your problem.
+
+Assuming the file you want to convert is `test.md` with the following content:
+
+> The examples below will be based on the initial Markdown file if it is a web URL. They are not repeated here.
+
+```text
+## 6.3 Converting MD Image Addresses
+Only supports uploading to a local image hosting service.
+
+- [https://github.com/JyHu/useful_script.git](https://github.com/JyHu/useful_script.git)
+- [https://github.com/JyHu/useful_script/blob/](https://github.com/JyHu/useful_script/blob/master/Scripts/md%E6%96%87%E4%BB%B6%E5%9B%BE%E7%89%87%E5%9B%BE%E5%BA%8A%E8%BD%AC%E6%8D%A2/%E8%87%AA%E5%8A%A8%E8%BD%AC%E6%8D%A2markdown%E6%96%87%E4%BB%B6%E4%B8%AD%E5%9B%BE%E7%89%87%E5%88%B0%E5%9B%BE%E5%BA%8A.md/)
+
+After all the hassle and trying this, I found it doesn't work either.
+![image.png](https://cdn.nlark.com/yuque/0/2022/png/26910220/1670091709979-52f8c3c4-a00f-4668-a236-29ad2c09d0da.png#averageHue=%23272c34&clientId=ubb991e0d-3414-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=928&id=u4a7a8376&margin=%5Bobject%20Object%5D&name=image.png&originHeight=928&originWidth=1050&originalType=binary&ratio=1&rotation=0&showTitle=false&size=201083&status=done&style=none&taskId=u27493dc0-9d78-4c07-929c-cc946d41409&title=&width=1050)
+
+In the end, PigGo is still the best. It provides a shortcut for uploading, and after uploading, you can directly xxxTODO.
+
+## 6.4 Pycasbin
+
+In pycasbin, I saw a colleague who frequently contributes to pycasbin. You can refer to some of his contributions:
+
+- [https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md](https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md)
+
+
+![image.png](https://cdn.nlark.com/yuque/0/2022/png/26910220/1670150012015-3a93ec6b-bb27-4ed3-b42f-252a0f70b65c.png#averageHue=%23fcfbf5&clientId=u86ce0a81-ec80-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=936&id=ube9c482c&margin=%5Bobject%20Object%5D&name=image.png&originHeight=936&originWidth=1920&originalType=binary&ratio=1&rotation=0&showTitle=false&size=205691&status=done&style=none&taskId=u6a6825da-aaf4-471c-ad0e-2280c325c66&title=&width=1920)
+```
+
+This content is the exported Markdown file from Yuque, and its image links are protected against external access. They need to be downloaded and replaced with local file paths in the Markdown.
+
+```python
+from imarkdown import MdFile, LocalFileAdapter, MdImageConverter
+
+def main():
+    adapter = LocalFileAdapter()
+    converter = MdImageConverter(adapter=adapter)
+    
+    md_file = MdFile(name="test.md")
+    converter.convert(md_file)
+
+if __name__ == '__main__':
+    main()
+```
+
+> In imarkdown, there are many places where you need to provide paths. You can use relative paths or absolute paths. It is recommended to use `/` as the path separator instead of `\\`.
+
+The converted result will generate a new Markdown file named `test_converted.md`, with the following content:
+
+```text
+## 6.3 Converting MD Image Addresses
+Only supports uploading to a local image hosting service.
+
+- [https://github.com/JyHu/useful_script.git](https://github.com/JyHu/useful_script.git)
+- [https://github.com/JyHu/useful_script/blob/](https://github.com/JyHu/useful_script/blob/master/Scripts/md%E6%96%87%E4%BB%B6%E5%9B%BE%E7%89%87%E5%9B%BE%E5%BA%8A%E8%BD%AC%E6%8D%A2/%E8%87%AA%E5%8A%A8%E8%BD%AC%E6%8D%A2markdown%E6%96%87%E4%BB%B6%E4%B8%AD%E5%9B%BE%E7%89%87%E5%88%B0%E5%9B%BE%E5%BA%8A.md/)
+
+After all the hassle and trying this, I found it doesn't work either.
+![image.png](./images/20230713_1356451324.png)
+
+In the end, PigGo is still the best. It provides a shortcut for uploading, and after uploading, you can directly xxxTODO.
+
+## 6.4 Pycasbin
+
+In pycasbin, I saw a colleague who frequently contributes to pycasbin. You can refer to some of his contributions:
+
+- [https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md](https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md)
+
+
+![image.png](./images/20230713_1356469646.png)
+```
+
+- Customizing the Output File Name
+When using imarkdown for conversion, the default name for the converted Markdown file is `{markdown_file_name}_converted.md`. If you want to customize the output file name, you can use the following configuration:
+
+```python
+md_converter.convert(md_file, name_prefix="new_", name_suffix="_converted")
+```
+
+Using this method of conversion will result in a file named `new_test_converted.md`. If you want to completely customize the converted name, you can use the following method:
+
+```python
+md_converter.convert(md_file, new_name="A new markdown.md")
+```
+
+With the above method, a file named `A new markdown.md` will be generated.
+
+### Converting Web URLs to Image Hosting Service URLs
+
+In the following example, we will use the `test.md` file provided earlier to demonstrate the conversion of image addresses from web URLs to URLs on the Alibaba Cloud OSS server, showcasing the functionality of converting web URLs to image hosting service URLs.
+
+```python
+from imarkdown import MdImageConverter, AliyunAdapter, MdFile
+
+
+def main():
+    aliyun_config = {
+        "access_key_id": "key_id",
+        "access_key_secret": "key_secret",
+        "bucket_name": "bucket_name",
+        "place": "bucket_place",
+        "storage_path_prefix": "prefix",
+    }
+    adapter = AliyunAdapter(**aliyun_config)
+    md_converter = MdImageConverter(adapter=adapter)
+    md_file = MdFile(name="markdown.md")
+    md_converter.convert(md_file)
+
+
+if __name__ == "__main__":
+    main()
+```
+
+In the example above, `storage_path_prefix` represents the file prefix in the bucket where the image is uploaded to OSS. If you want to store the image in the `/imarkdown` directory, you need to set `storage_path_prefix="/imarkdown"`. The remaining configuration details are specific to Alibaba Cloud OSS, so please fill them in accordingly.
+
+
+### Batch Conversion of Multiple Files: Web URL to Local
+
+The following example demonstrates a solution for batch conversion of multiple Markdown files, converting web image URLs to local image addresses.
+
+```python
+from imarkdown import LocalFileAdapter, MdFolder, MdImageConverter
+
+def main():
+    adapter = LocalFileAdapter()
+    converter = MdImageConverter(adapter=adapter)
+    
+    # Folder name is "mds"
+    md_folder = MdFolder(name="mds")
+    # Output files to "converted_mds"
+    converter.convert(md_folder, output_directory="converted_mds")
+```
+
+Using the above code snippet will create a folder named "converted_mds" where the converted files will be saved. The images will be saved in the `converted_mds/images` directory. If you want to output the images to a specific folder, you can set it as follows:
+
+```python
+md_folder = MdFolder(name="mds", image_directory="mds/my_images")
+```
+
+### Batch Conversion of Multiple Files: Local to Image Hosting Service
+
+The following example demonstrates a solution for batch conversion of multiple Markdown files, converting local image addresses to image hosting service URLs.
+
+```python
+from imarkdown import LocalFileAdapter, MdFolder, MdImageConverter
+
+def main():
+    adapter = LocalFileAdapter()
+    converter = MdImageConverter(adapter=adapter)
+    
+    # Folder name is "local_mds", images are of local type, and image URLs are saved in "local_mds/images"
+    md_folder = MdFolder(name="local_mds", image_type="local", image_directory="local_mds/images")
+    # Output files to "converted_mds"
+    converter.convert(md_folder, output_directory="converted_mds")
+```
+
+### Custom Image Hosting Service
+
+The following example demonstrates how to use imarkdown to upload images to a custom file server and retrieve the URL.
+
+First, you need to create a custom adapter by inheriting from `BaseMdAdapter` and implementing the `upload` and `get_replaced_url` methods. Then, you can inject the custom adapter into `MdImageConverter`.
+
+```python
+import os
+import json
+
+import requests
+from imarkdown import BaseMdAdapter, MdImageConverter, MdFolder
+
+class CustomMdAdapter(BaseMdAdapter):
+    name = "custom"
+    url = "https://server/upload/file/batch"
+    headers = {
+        "X-Upload-Token": "my_token"
+    }
+    cur_key = ""
+
+    def upload(self, key: str, file):
+        files = {"file": file}
+        response = requests.post(self.url, headers=self.headers, files=files)
+        if response.status_code == 200:
+            res_data = json.loads(response.content.decode("utf-8"))
+            self.cur_key = res_data["data"]["images"]["url"]
+        else:
+            raise Exception(response.content)
+
+    def get_replaced_url(self, key):
+        return self.cur_key
+
+def get_all_folder_names():
+    return os.listdir("my-blog")
+
+    
+def main():
+    adapter = CustomMdAdapter()
+    md_converter = MdImageConverter(adapter=adapter)
+
+    md_folders = []
+    for folder_name in get_all_folder_names():
+        md_folders.append(
+            MdFolder(
+                name=f"my-blog/{folder_name}",
+                image_directory=f"my-blog/{folder_name}/images",
+                image_type="local",
+            )
+        )
+    md_converter.convert(md_folders, output_directory="converted")
+
+
+if __name__ == "__main__":
+    main()
+```
+
+### Custom Regular Expression
+`imarkdown` use regular expression to find your images. It supports `![](image_url)` and `<img src="image_url"/>` format, but there are still some other format `imarkdown` can not find it.
+
+At this point, `imarkdown` supports custom regular expression to address this issue. You can customize a regular expression which can find your markdown image url and pass it to MdImageConverter. The following example show how to use it.
+
+```python
+from imarkdown import MdImageConverter, LocalFileAdapter, MdFolder
+
+
+def main():
+    custom_re = r"(?:!\[(.*?)\]\((.*?)\))|<img.*?src=[\'\"](.*?)[\'\"].*?>"
+    adapter = LocalFileAdapter()
+    md_converter = MdImageConverter(adapter=adapter)
+    
+    md_folder = MdFolder(name="mds")
+    md_converter.convert(md_folder, output_directory="output_mds", re_rule=custom_re)
+
+
+if __name__ == "__main__":
+    main()
+```
+
+## Roadmap
+
+- [ ] Add client-side support
+- [ ] Support Tencent Cloud, Qiniu Cloud, and other image hosting services
+- [x] Support batch file modification
+- [x] Custom adapters
+- [ ] Support compression of large images
+- [ ] Support command-line interface
+- [x] Support PyPI for simplified operations
+- [ ] Provide file custom naming
+- [ ] Provide custom formatting for image names
+
+## FAQ
+
+**1. How can I extend to other image hosting services?**
+
+If you want to develop support for other image hosting services, all you need to do is implement an adapter similar to `AliyunAdapter` and inject it into `MdImageConverter` when using it. Refer to [Custom Image Hosting Service](#custom-image-hosting-service). That's all you need to do. In fact, I've wrapped it up nicely, so extending it is straightforward.
+
+**2. Usage of file addresses**
+
+In Python, both `/` and `\\` can be used as file path separators. However, there are some differences in their usage.
+
+- `/` (forward slash): In most operating systems, including Windows, Linux, and Mac, `/` is used as the file path separator. Using `/` as the separator can make your code portable across different operating systems. For example:
+
+```python
+path = "folder/file.txt"
+```
+
+- `\\` (backslash): In the Windows operating system, `\\` is used as the file path separator. This is because `\` is used as an escape character in Windows, so to represent a plain backslash, you need to use two consecutive backslashes. For example:
+
+```python
+path = "folder\\file.txt"
+```
+
+When using `\\` as the separator, keep the following points in mind:
+
+- When using `\\` in a string, you need to escape it as `\\\\` because the first `\` will be interpreted as an escape character.
+- You can use raw strings to avoid the hassle of escaping. In a raw string, `\` is not interpreted as an escape character. For example: `path = r"folder\file.txt"`
+
+In summary, if your code needs to run on different operating systems, it is recommended to use `/` as the file path separator to maintain code portability. If you are only running the code on Windows, using `\\` is also acceptable. However, in `imarkdown`, all `\\` paths will be converted to `/`. In this project, all `\\` paths will be converted to `/`.
+
+## Contribution
+
+Contributions are welcome! If you would like to contribute to this project, you can submit a pull request or an issue. There are some extensible features listed in the [Development Roadmap](#development-roadmap), and there are still many third-party image hosting services that need to be adapted. If you are working on these aspects, feel free to submit a pull request! I'm excited to see more people involved in improving and optimizing it.
```

### Comparing `imarkdown-1.1.2/imarkdown/adapter/base.py` & `imarkdown-1.2.1/imarkdown/adapter/base.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from abc import abstractmethod
-
-from pydantic import BaseModel
-
-
-class BaseMdAdapter(BaseModel):
-    name: str
-    """Adapter name"""
-    storage_path_prefix: str = ""
-    """Image path file prefix. Final image name is `{storage_path_prefix}/{key}`"""
-
-    class Config:
-        arbitrary_types_allowed = True
-
-    @abstractmethod
-    def upload(self, key: str, file):
-        """Upload image to Image Server.
-
-        Args:
-            key: image name
-            file: markdown string data
-        """
-        raise NotImplementedError("Your adapter should implement `upload` method")
-
-    @abstractmethod
-    def get_replaced_url(self, key):
-        """get replaced url or image path"""
-        raise NotImplementedError(
-            "Your adapter should implement `get_replaced_url` method"
-        )
+from abc import abstractmethod
+
+from pydantic import BaseModel
+
+
+class BaseMdAdapter(BaseModel):
+    name: str
+    """Adapter name"""
+    storage_path_prefix: str = ""
+    """Image path file prefix. Final image name is `{storage_path_prefix}/{key}`"""
+
+    class Config:
+        arbitrary_types_allowed = True
+
+    @abstractmethod
+    def upload(self, key: str, file):
+        """Upload image to Image Server.
+
+        Args:
+            key: image name
+            file: markdown string data
+        """
+        raise NotImplementedError("Your adapter should implement `upload` method")
+
+    @abstractmethod
+    def get_replaced_url(self, key):
+        """get replaced url or image path"""
+        raise NotImplementedError(
+            "Your adapter should implement `get_replaced_url` method"
+        )
```

### Comparing `imarkdown-1.1.2/imarkdown/adapter/local_adapter.py` & `imarkdown-1.2.1/imarkdown/adapter/local_adapter.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from pydantic import validator
-
-from imarkdown.adapter.base import BaseMdAdapter
-
-
-class LocalFileAdapter(BaseMdAdapter):
-    name: str = "Local"
-
-    @validator("storage_path_prefix")
-    def show_warnings(cls, v: str):
-        assert v == "", (
-            "LocalFileAdapter can not use storage_path_prefix. You should set image_directory in MdFile or MdFolder "
-            "if you want to set your local image directory."
-        )
-
-    def upload(self, key: str, file):
-        """This adapter does not require upload."""
-        pass
-
-    def get_replaced_url(self, key):
-        path = f"./{self.storage_path_prefix}/{key}"
-        if self.storage_path_prefix == "":
-            path = f"./images/{key}"
-        return path
+from pydantic import validator
+
+from imarkdown.adapter.base import BaseMdAdapter
+
+
+class LocalFileAdapter(BaseMdAdapter):
+    name: str = "Local"
+
+    @validator("storage_path_prefix")
+    def show_warnings(cls, v: str):
+        assert v == "", (
+            "LocalFileAdapter can not use storage_path_prefix. You should set image_directory in MdFile or MdFolder "
+            "if you want to set your local image directory."
+        )
+
+    def upload(self, key: str, file):
+        """This adapter does not require upload."""
+        pass
+
+    def get_replaced_url(self, key):
+        path = f"./{self.storage_path_prefix}/{key}"
+        if self.storage_path_prefix == "":
+            path = f"./images/{key}"
+        return path
```

### Comparing `imarkdown-1.1.2/imarkdown/config.py` & `imarkdown-1.2.1/imarkdown/config.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-import logging
-import os
-from typing import Any
-
-from imarkdown.constant import MdAdapterType, _MdAdapterType
-from imarkdown.utils.cache import Cache
-from imarkdown.utils.singleton import Singleton
-
-logger = logging.getLogger(__name__)
-
-
-class IMarkdownConfig(metaclass=Singleton):
-    def __init__(self):
-        self.cache = Cache()
-        self.root_path = os.path.abspath(os.path.dirname(__file__))
-
-    @property
-    def last_adapter_name(self) -> str:
-        """Obtain the last executed MdAdapter, return LocalFileAdapter if obtain None.
-        Custom MdAdapter currently can not use last adapter name.
-        """
-        adapter_name = self.cache.get("last_adapter", None)
-        logger.debug(f"[imarkdown] get last adapter <{adapter_name}>")
-        if not adapter_name or adapter_name not in _MdAdapterType.keys():
-            return MdAdapterType.Local
-        return _MdAdapterType[str(adapter_name)]
-
-    @last_adapter_name.setter
-    def last_adapter_name(self, value: str):
-        # if value not in _MdAdapterType.keys():
-        #     raise ValueError(f"<{value}> type adapter not exist.")
-        self.cache["last_adapter"] = value
-
-    def load_variable(self, key: str) -> Any:
-        return self.cache.get(key, None)
-
-    def store_variable(self, key: str, value: Any) -> Any:
-        self.cache[key] = value
+import logging
+import os
+from typing import Any
+
+from imarkdown.constant import MdAdapterType, _MdAdapterType
+from imarkdown.utils.cache import Cache
+from imarkdown.utils.singleton import Singleton
+
+logger = logging.getLogger(__name__)
+
+
+class IMarkdownConfig(metaclass=Singleton):
+    def __init__(self):
+        self.cache = Cache()
+        self.root_path = os.path.abspath(os.path.dirname(__file__))
+
+    @property
+    def last_adapter_name(self) -> str:
+        """Obtain the last executed MdAdapter, return LocalFileAdapter if obtain None.
+        Custom MdAdapter currently can not use last adapter name.
+        """
+        adapter_name = self.cache.get("last_adapter", None)
+        logger.debug(f"[imarkdown] get last adapter <{adapter_name}>")
+        if not adapter_name or adapter_name not in _MdAdapterType.keys():
+            return MdAdapterType.Local
+        return _MdAdapterType[str(adapter_name)]
+
+    @last_adapter_name.setter
+    def last_adapter_name(self, value: str):
+        # if value not in _MdAdapterType.keys():
+        #     raise ValueError(f"<{value}> type adapter not exist.")
+        self.cache["last_adapter"] = value
+
+    def load_variable(self, key: str) -> Any:
+        return self.cache.get(key, None)
+
+    def store_variable(self, key: str, value: Any) -> Any:
+        self.cache[key] = value
```

### Comparing `imarkdown-1.1.2/imarkdown/converter.py` & `imarkdown-1.2.1/imarkdown/converter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,330 +1,347 @@
-import logging
-import os
-import random
-import re
-import time
-import traceback
-from typing import List, Optional, Any, Union, Dict
-
-import requests
-from pydantic import BaseModel, Field, root_validator
-
-from imarkdown.adapter import BaseMdAdapter, MdAdapterMapper
-from imarkdown.config import IMarkdownConfig
-from imarkdown.constant import MdAdapterType
-from imarkdown.schema import MdMediumManager, MdFile, MdFolder
-from imarkdown.utils import (
-    polish_path,
-    supplementary_file_path,
-    get_file_name_from_relative_path,
-    calculate_relative_path,
-)
-
-logger = logging.getLogger(__name__)
-cfg = IMarkdownConfig()
-
-
-def _read_md(file_path: str) -> str:
-    """read markdown file and return markdown data"""
-    with open(file_path, "r", encoding="utf-8") as f:
-        res = f.read()
-        logger.info(f"[imarkdown] read file <{file_path}> successfully")
-    return res
-
-
-def _write_data(new_file_path: str, md_str: str):
-    new_file_path = supplementary_file_path(new_file_path)
-
-    with open(f"{new_file_path}", "w", encoding="utf-8") as f:
-        f.write(md_str)
-        logger.info(f"[imarkdown] write successfully to <{new_file_path}>")
-
-
-def _download_img(image_local_storage_directory: str, image_url: str) -> Optional[str]:
-    """Download image from website and stored in image_local_storage_directory
-
-    Args:
-        image_local_storage_directory: image local storage directory
-        image_url: image web url
-
-    Returns:
-        Return converted image absolute path
-    """
-    try:
-        response = requests.get(image_url)
-        now_time = time.strftime("%Y%m%d_%H%M%S", time.localtime(time.time()))
-        image_local_storage_directory = polish_path(image_local_storage_directory)
-        if not os.path.exists(image_local_storage_directory):
-            os.makedirs(image_local_storage_directory, exist_ok=True)
-
-        images_path = f"{image_local_storage_directory}{now_time}{random.randint(1000, 10000)}.png"
-        with open(images_path, "wb") as f:
-            f.write(response.content)
-        logger.info(f"[imarkdown] <{images_path}> has stored in local successfully")
-        return images_path
-    except Exception as e:
-        traceback.print_exc()
-        logger.error(f"[imarkdown] download_img failed, reason: {e}")
-        return None
-
-
-def _load_default_adapter() -> BaseMdAdapter:
-    logger.debug(f"[imarkdown] local default adapter <{cfg.last_adapter_name}>")
-    return MdAdapterMapper[cfg.last_adapter_name]()
-
-
-class BaseMdImageConverter(BaseModel):
-    adapter: BaseMdAdapter = Field(default_factory=_load_default_adapter)
-    """Adapter determines the convert method you choose."""
-    is_local_images: bool = False
-    """You should set True if you want your local images upload to your picture server and you
-    Markdown image url is originally local. Attention, enable_save_images can not be False if
-    is_local_images is True."""
-    enable_save_images: bool = True
-    """It will delete images file after downloading the images if it is False."""
-    image_local_storage_directory: Optional[str] = None
-    """Local storage directory of images"""
-    md_file_original_directory: Optional[str] = None
-    """The storage directory of original markdown file."""
-    md_file_output_directory: Optional[str] = None
-    """The storage directory of converted markdown file."""
-    converted_md_file_name: Optional[str] = None
-
-    @root_validator(pre=True)
-    def variables_check(
-        cls, values: Optional[Dict[str, Any]]
-    ) -> Optional[Dict[str, Any]]:
-        """update IMarkdownConfig last_adapter_name"""
-        logger.debug(
-            f"[imarkdown] BaseMdImageConverter initialization params: {values}"
-        )
-        if "adapter" in values and values["adapter"]:
-            cfg.last_adapter_name = values["adapter"].name
-        return values
-
-    def set_md_file_original_directory(self, md_file_path: str):
-        result = supplementary_file_path(md_file_path)
-        result = "/".join(result.split("/")[:-1])
-        logger.debug(
-            f"[imarkdown] BaseMdImageConverter md_file_original_directory: {result}"
-        )
-        self.md_file_original_directory = result
-
-    def set_md_file_output_directory(self, path: str):
-        result = supplementary_file_path(path)
-        logger.debug(
-            f"[imarkdown] BaseMdImageConverter md_file_output_directory: {result}"
-        )
-        self.md_file_output_directory = result
-
-    def set_image_local_storage_directory(self, path: str):
-        result = supplementary_file_path(path)
-        logger.debug(
-            f"[imarkdown] BaseMdImageConverter set image_local_storage_directory: {result}"
-        )
-        self.image_local_storage_directory = result
-
-    def set_converted_md_file_name(
-        self,
-        md_file_path: str,
-        enable_rename: bool = True,
-        new_name: str = "",
-        name_prefix: str = "",
-        name_suffix: str = "_converted",
-        **kwargs,
-    ):
-        """Set converted markdown file name.
-
-        Args:
-            md_file_path: Original markdown file path.
-            enable_rename: Default is true, it means the generated markdown file will receive a new name.
-            new_name: Custom converted markdown file name. If you pass it, you can not use name_prefix and name_suffix/
-            name_prefix: Prefix name of generated markdown file.
-            name_suffix: Suffix name of generated markdown file.
-        """
-        md_file_path = supplementary_file_path(md_file_path)
-        md_name = md_file_path.split("/")[-1][:-3]
-
-        if enable_rename:
-            if new_name != "":
-                if name_prefix or name_prefix:
-                    raise ValueError(
-                        "You can not set `name_prefix` and `name_prefix` if you set `new_name`."
-                    )
-                self.converted_md_file_name = new_name
-            else:
-                self.converted_md_file_name = f"{name_prefix}{md_name}{name_suffix}.md"
-            logger.debug(
-                f"[imarkdown] BaseMdImageConverter set converted_md_file_name {self.converted_md_file_name}"
-            )
-            return
-        logger.debug(f"[imarkdown] BaseMdImageConverter not rename.")
-        self.converted_md_file_name = f"{md_name}.md"
-
-    def convert(
-        self,
-        md_file_path: str,
-        image_local_storage_directory: Optional[str] = None,
-        output_md_directory: Optional[str] = None,
-        is_local_images: Optional[bool] = None,
-        **kwargs,
-    ):
-        """Convert Markdown image url and generate a new Markdown file.
-
-        Args:
-            md_file_path(str): Markdown file path.
-            image_local_storage_directory(Optional[str]): Specified image storage path. You can pass an absolute or a
-                relative path. Default image directory path is the Markdown directory named `markdown_dir/images`.
-            output_md_directory(Optional[str]): The storage directory of converted markdown file.
-            is_local_images:
-            **kwargs:
-                enable_rename(bool): Default is true, it means the generated markdown file will receive a new name.
-                name_prefix(Optional[str]): Prefix name of generated markdown file.
-                name_suffix(Optional[str]): Suffix name of generated markdown file.
-
-        Returns:
-            A converted markdown file or a list of converted directory.
-        """
-        if not md_file_path.endswith(".md"):
-            return
-        if is_local_images:
-            self.is_local_images = is_local_images
-
-        self.set_converted_md_file_name(md_file_path, **kwargs)
-        self.set_md_file_original_directory(md_file_path)
-        if output_md_directory:
-            self.set_md_file_output_directory(output_md_directory)
-        else:
-            self.set_md_file_output_directory(self.md_file_original_directory)
-        if image_local_storage_directory:
-            self.set_image_local_storage_directory(image_local_storage_directory)
-        else:
-            self.set_image_local_storage_directory(
-                f"{self.md_file_output_directory}/images"
-            )
-
-        original_data: str = _read_md(md_file_path)
-        modified_data: str = self._find_img_and_replace(original_data)
-
-        converted_md_path = (
-            f"{self.md_file_output_directory}/{self.converted_md_file_name}"
-        )
-        _write_data(converted_md_path, modified_data)
-        logger.info(f"[imarkdown] <{md_file_path}> converted task end")
-
-    def _find_img_and_replace(self, md_str: str) -> str:
-        """Input original markdown str and replace images address
-        It can find `[]()` type image url and `<img/>` type image url
-
-        Args:
-            md_str: markdown original data
-
-        Returns:
-            Markdown data for the image url has been changed.
-        """
-        _images = re.findall(
-            r"(?:!\[(.*?)\]\((.*?)\))|<img.*?src=[\'\"](.*?)[\'\"].*?>", md_str
-        )
-
-        images = []
-        for image in _images:
-            if image[1] == "":
-                continue
-            # If current image link is local path URL and you need to web URL to a local path,
-            # the local path url will not be converted.
-            if not self.is_local_images and not image[1].startswith("http"):
-                continue
-            images.append(image[1])
-
-        for image in images:
-            converted_image_url = self._get_converted_image_url(image)
-            md_str = md_str.replace(image, converted_image_url)
-        logger.info(
-            f"[imarkdown] All images conversion for this md file have been completed, ready to save to file."
-        )
-        return md_str
-
-    def _get_converted_image_url(self, original_image_url: str) -> str:
-        """Get converted image url by adapter.
-
-        Args:
-            original_image_url: links to images that needs to be converted
-
-        Returns:
-            converted url
-        """
-        if self.is_local_images:
-            original_image_url = get_file_name_from_relative_path(original_image_url)
-            converted_image_path = (
-                f"{self.image_local_storage_directory}/{original_image_url}"
-            )
-        else:
-            converted_image_path = _download_img(
-                self.image_local_storage_directory, original_image_url
-            )
-
-        if not converted_image_path:
-            raise Exception("get a empty image path")
-
-        logger.debug(f"[imarkdown] local image path: {converted_image_path}")
-        image_name = os.path.basename(converted_image_path)
-        if self.adapter.name == MdAdapterType.Local:
-            return calculate_relative_path(
-                converted_image_path, self.md_file_output_directory
-            )
-
-        # other adapter
-        with open(converted_image_path, "rb") as f:
-            file_data = f.read()
-            self.adapter.upload(image_name, file_data)
-            converted_url = self.adapter.get_replaced_url(image_name)
-            logger.debug(f"[imarkdown] converted image url: {converted_url}")
-        if not self.enable_save_images:
-            os.remove(converted_image_path)
-        if not converted_url:
-            raise Exception(
-                f"<{original_image_url}> try to get new url but return None."
-            )
-        return converted_url
-
-
-class MdImageConverter:
-    def __init__(
-        self, adapter: Optional[BaseMdAdapter] = None, enable_log: bool = True
-    ):
-        self.adapter = _load_default_adapter()
-        if adapter:
-            self.adapter: BaseMdAdapter = adapter
-            cfg.last_adapter_name = adapter.name
-
-        self.converter: BaseMdImageConverter = BaseMdImageConverter(
-            adapter=self.adapter
-        )
-        self.md_medium_manager: Optional[MdMediumManager] = MdMediumManager()
-        if enable_log:
-            logging.basicConfig(level=logging.INFO)
-
-    def convert(
-        self,
-        mediums: Union[MdFile, MdFolder, List[Union[MdFile, MdFolder]]],
-        output_directory: Optional[str] = None,
-        enable_save_images: bool = True,
-        **kwargs,
-    ):
-        def check_warning(medium: Union[MdFile, MdFolder]):
-            if not output_directory and isinstance(medium, MdFolder):
-                raise ValueError(
-                    "Missing argument output_directory. If you pass a MdFolder, you must set output directory."
-                )
-
-        if not isinstance(mediums, List):
-            mediums = [mediums]
-        [check_warning(medium) for medium in mediums]
-
-        self.md_medium_manager.init_md_files(mediums)
-        self.md_medium_manager.update_config(
-            output_directory=output_directory, enable_save_images=enable_save_images
-        )
-        for md_files in self.md_medium_manager.md_files:
-            kwargs.update(**md_files.to_convert_params)
-            self.converter.convert(**kwargs)
+import logging
+import os
+import random
+import re
+import time
+import traceback
+from typing import List, Optional, Any, Union, Dict
+
+import requests
+from pydantic import BaseModel, Field, root_validator
+
+from imarkdown.adapter import BaseMdAdapter, MdAdapterMapper
+from imarkdown.config import IMarkdownConfig
+from imarkdown.constant import MdAdapterType
+from imarkdown.schema import MdMediumManager, MdFile, MdFolder
+from imarkdown.utils import (
+    polish_path,
+    supplementary_file_path,
+    get_file_name_from_relative_path,
+    calculate_relative_path,
+)
+
+logger = logging.getLogger(__name__)
+cfg = IMarkdownConfig()
+
+
+def _read_md(file_path: str) -> str:
+    """read markdown file and return markdown data"""
+    with open(file_path, "r", encoding="utf-8") as f:
+        res = f.read()
+        logger.info(f"[imarkdown] read file <{file_path}> successfully")
+    return res
+
+
+def _write_data(new_file_path: str, md_str: str):
+    new_file_path = supplementary_file_path(new_file_path)
+
+    with open(f"{new_file_path}", "w", encoding="utf-8") as f:
+        f.write(md_str)
+        logger.info(f"[imarkdown] write successfully to <{new_file_path}>")
+
+
+def _download_img(image_local_storage_directory: str, image_url: str) -> Optional[str]:
+    """Download image from website and stored in image_local_storage_directory
+
+    Args:
+        image_local_storage_directory: image local storage directory
+        image_url: image web url
+
+    Returns:
+        Return converted image absolute path
+    """
+    try:
+        response = requests.get(image_url)
+        now_time = time.strftime("%Y%m%d_%H%M%S", time.localtime(time.time()))
+        image_local_storage_directory = polish_path(image_local_storage_directory)
+        if not os.path.exists(image_local_storage_directory):
+            os.makedirs(image_local_storage_directory, exist_ok=True)
+
+        images_path = f"{image_local_storage_directory}{now_time}{random.randint(1000, 10000)}.png"
+        with open(images_path, "wb") as f:
+            f.write(response.content)
+        logger.info(f"[imarkdown] <{images_path}> has stored in local successfully")
+        return images_path
+    except Exception as e:
+        traceback.print_exc()
+        logger.error(f"[imarkdown] download_img failed, reason: {e}")
+        return None
+
+
+def _load_default_adapter() -> BaseMdAdapter:
+    logger.debug(f"[imarkdown] local default adapter <{cfg.last_adapter_name}>")
+    return MdAdapterMapper[cfg.last_adapter_name]()
+
+
+class BaseMdImageConverter(BaseModel):
+    adapter: BaseMdAdapter = Field(default_factory=_load_default_adapter)
+    """Adapter determines the convert method you choose."""
+    is_local_images: bool = False
+    """You should set True if you want your local images upload to your picture server and you
+    Markdown image url is originally local. Attention, enable_save_images can not be False if
+    is_local_images is True."""
+    enable_save_images: bool = True
+    """It will delete images file after downloading the images if it is False."""
+    image_local_storage_directory: Optional[str] = None
+    """Local storage directory of images"""
+    md_file_original_directory: Optional[str] = None
+    """The storage directory of original markdown file."""
+    md_file_output_directory: Optional[str] = None
+    """The storage directory of converted markdown file."""
+    converted_md_file_name: Optional[str] = None
+    """The converted markdown file name."""
+    re_rule: str = r"(?:!\[(.*?)\]\((.*?)\))|<img.*?src=[\'\"](.*?)[\'\"].*?>"
+    """Default regular expression to find images, you can custom re_rule."""
+
+    @root_validator(pre=True)
+    def variables_check(
+        cls, values: Optional[Dict[str, Any]]
+    ) -> Optional[Dict[str, Any]]:
+        """update IMarkdownConfig last_adapter_name"""
+        logger.debug(
+            f"[imarkdown] BaseMdImageConverter initialization params: {values}"
+        )
+        if "adapter" in values and values["adapter"]:
+            cfg.last_adapter_name = values["adapter"].name
+        return values
+
+    def set_md_file_original_directory(self, md_file_path: str):
+        result = supplementary_file_path(md_file_path)
+        result = "/".join(result.split("/")[:-1])
+        logger.debug(
+            f"[imarkdown] BaseMdImageConverter md_file_original_directory: {result}"
+        )
+        self.md_file_original_directory = result
+
+    def set_md_file_output_directory(self, path: str):
+        result = supplementary_file_path(path)
+        logger.debug(
+            f"[imarkdown] BaseMdImageConverter md_file_output_directory: {result}"
+        )
+        self.md_file_output_directory = result
+
+    def set_image_local_storage_directory(self, path: str):
+        result = supplementary_file_path(path)
+        logger.debug(
+            f"[imarkdown] BaseMdImageConverter set image_local_storage_directory: {result}"
+        )
+        self.image_local_storage_directory = result
+
+    def set_converted_md_file_name(
+        self,
+        md_file_path: str,
+        enable_rename: bool = True,
+        new_name: str = "",
+        name_prefix: str = "",
+        name_suffix: str = "_converted",
+        **kwargs,
+    ):
+        """Set converted markdown file name.
+
+        Args:
+            md_file_path: Original markdown file path.
+            enable_rename: Default is true, it means the generated markdown file will receive a new name.
+            new_name: Custom converted markdown file name. If you pass it, you can not use name_prefix and name_suffix/
+            name_prefix: Prefix name of generated markdown file.
+            name_suffix: Suffix name of generated markdown file.
+        """
+        md_file_path = supplementary_file_path(md_file_path)
+        md_name = md_file_path.split("/")[-1][:-3]
+
+        if enable_rename:
+            if new_name != "":
+                if name_prefix or name_prefix:
+                    raise ValueError(
+                        "You can not set `name_prefix` and `name_prefix` if you set `new_name`."
+                    )
+                self.converted_md_file_name = new_name
+            else:
+                self.converted_md_file_name = f"{name_prefix}{md_name}{name_suffix}.md"
+            logger.debug(
+                f"[imarkdown] BaseMdImageConverter set converted_md_file_name {self.converted_md_file_name}"
+            )
+            return
+        logger.debug(f"[imarkdown] BaseMdImageConverter not rename.")
+        self.converted_md_file_name = f"{md_name}.md"
+
+    def convert(
+        self,
+        md_file_path: str,
+        image_local_storage_directory: Optional[str] = None,
+        output_md_directory: Optional[str] = None,
+        is_local_images: Optional[bool] = None,
+        re_rule: Optional[str] = None,
+        **kwargs,
+    ):
+        """Convert Markdown image url and generate a new Markdown file.
+
+        Args:
+            md_file_path(str): Markdown file path.
+            image_local_storage_directory(Optional[str]): Specified image storage path. You can pass an absolute or a
+                relative path. Default image directory path is the Markdown directory named `markdown_dir/images`.
+            output_md_directory(Optional[str]): The storage directory of converted markdown file.
+            re_rule(Optional[str]): Regular expression to find images, you can custom re_rule.
+            is_local_images: It is a local images.
+            **kwargs:
+                enable_rename(bool): Default is true, it means the generated markdown file will receive a new name.
+                name_prefix(Optional[str]): Prefix name of generated markdown file.
+                name_suffix(Optional[str]): Suffix name of generated markdown file.
+
+        Returns:
+            A converted markdown file or a list of converted directory.
+        """
+        if not md_file_path.endswith(".md"):
+            return
+        if is_local_images:
+            self.is_local_images = is_local_images
+        if re_rule:
+            logger.debug(f"[imarkdown] reset regular expression <{re_rule}>")
+            self.re_rule = re_rule
+
+        self.set_converted_md_file_name(md_file_path, **kwargs)
+        self.set_md_file_original_directory(md_file_path)
+        if output_md_directory:
+            self.set_md_file_output_directory(output_md_directory)
+        else:
+            self.set_md_file_output_directory(self.md_file_original_directory)
+        if image_local_storage_directory:
+            self.set_image_local_storage_directory(image_local_storage_directory)
+        else:
+            self.set_image_local_storage_directory(
+                f"{self.md_file_output_directory}/images"
+            )
+
+        original_data: str = _read_md(md_file_path)
+        modified_data: str = self._find_img_and_replace(original_data)
+
+        converted_md_path = (
+            f"{self.md_file_output_directory}/{self.converted_md_file_name}"
+        )
+        _write_data(converted_md_path, modified_data)
+        logger.info(f"[imarkdown] <{md_file_path}> converted task end")
+
+    def _find_img_and_replace(self, md_str: str, re_rule: Optional[str] = None) -> str:
+        """Input original markdown str and replace images address
+        It can find `[]()` type image url and `<img/>` type image url
+
+        Args:
+            md_str: markdown original data
+
+        Returns:
+            Markdown data for the image url has been changed.
+        """
+        _images = re.findall(
+            self.re_rule, md_str
+        )
+
+        images = []
+        for image in _images:
+            if image[1] == "":
+                continue
+            # If current image link is local path URL and you need to web URL to a local path,
+            # the local path url will not be converted.
+            if not self.is_local_images and not image[1].startswith("http"):
+                continue
+            images.append(image[1])
+
+        for image in images:
+            converted_image_url = self._get_converted_image_url(image)
+            md_str = md_str.replace(image, converted_image_url)
+        logger.info(
+            f"[imarkdown] All images conversion for this md file have been completed, ready to save to file."
+        )
+        return md_str
+
+    def _get_converted_image_url(self, original_image_url: str) -> str:
+        """Get converted image url by adapter.
+
+        Args:
+            original_image_url: links to images that needs to be converted
+
+        Returns:
+            converted url
+        """
+        if self.is_local_images:
+            original_image_url = get_file_name_from_relative_path(original_image_url)
+            converted_image_path = (
+                f"{self.image_local_storage_directory}/{original_image_url}"
+            )
+        else:
+            converted_image_path = _download_img(
+                self.image_local_storage_directory, original_image_url
+            )
+
+        if not converted_image_path:
+            raise Exception("get a empty image path")
+
+        logger.debug(f"[imarkdown] local image path: {converted_image_path}")
+        image_name = os.path.basename(converted_image_path)
+        if self.adapter.name == MdAdapterType.Local:
+            return calculate_relative_path(
+                converted_image_path, self.md_file_output_directory
+            )
+
+        # other adapter
+        with open(converted_image_path, "rb") as f:
+            file_data = f.read()
+            self.adapter.upload(image_name, file_data)
+            converted_url = self.adapter.get_replaced_url(image_name)
+            logger.debug(f"[imarkdown] converted image url: {converted_url}")
+        if not self.enable_save_images:
+            os.remove(converted_image_path)
+        if not converted_url:
+            raise Exception(
+                f"<{original_image_url}> try to get new url but return None."
+            )
+        return converted_url
+
+
+class MdImageConverter:
+    def __init__(
+        self, adapter: Optional[BaseMdAdapter] = None, enable_log: bool = True
+    ):
+        self.adapter = _load_default_adapter()
+        if adapter:
+            self.adapter: BaseMdAdapter = adapter
+            cfg.last_adapter_name = adapter.name
+
+        self.converter: BaseMdImageConverter = BaseMdImageConverter(
+            adapter=self.adapter
+        )
+        self.md_medium_manager: Optional[MdMediumManager] = MdMediumManager()
+        if enable_log:
+            logging.basicConfig(level=logging.INFO)
+
+    def convert(
+        self,
+        mediums: Union[MdFile, MdFolder, List[Union[MdFile, MdFolder]]],
+        output_directory: Optional[str] = None,
+        enable_save_images: bool = True,
+        **kwargs,
+    ):
+        """Markdown Image convert.
+
+        Args:
+            mediums(Union[MdFile, MdFolder, List[Union[MdFile, MdFolder]]]): MdFile or MdFolder you need to convert.
+            output_directory(Optional[str]): output directory
+            enable_save_images(bool): It is save image?
+            **kwargs:
+                re_rule(Optional[str]): custom regular expression to find specified element like image.
+        """
+        def check_warning(medium: Union[MdFile, MdFolder]):
+            if not output_directory and isinstance(medium, MdFolder):
+                raise ValueError(
+                    "Missing argument output_directory. If you pass a MdFolder, you must set output directory."
+                )
+
+        if not isinstance(mediums, List):
+            mediums = [mediums]
+        [check_warning(medium) for medium in mediums]
+
+        self.md_medium_manager.init_md_files(mediums)
+        self.md_medium_manager.update_config(
+            output_directory=output_directory, enable_save_images=enable_save_images
+        )
+        for md_files in self.md_medium_manager.md_files:
+            kwargs.update(**md_files.to_convert_params)
+            self.converter.convert(**kwargs)
```

### Comparing `imarkdown-1.1.2/imarkdown/schema.py` & `imarkdown-1.2.1/imarkdown/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,247 +1,247 @@
-import glob
-import logging
-import os
-from typing import List, Optional, Any, Dict, Union
-
-from pydantic import BaseModel, root_validator, validator
-from typing_extensions import Literal
-
-from imarkdown.utils import (
-    supplementary_file_path,
-    convert_backslashes,
-    exist_markdown_file,
-)
-
-logger = logging.getLogger(__name__)
-
-
-class BaseMdMedium(BaseModel):
-    name: str
-    """markdown medium name"""
-    absolute_path_name: str
-    """path + name"""
-    image_directory: Optional[str] = None
-    """image storage path if it exists"""
-    image_type: Literal["local", "remote"] = "remote"
-    is_default_image_directory: bool = True
-    type: Literal["original", "converted"] = "original"
-    output_directory: Optional[str] = None
-    enable_save_images: bool = True
-    enable_rename: bool = True
-    root_directory: Optional[str] = None
-
-
-class MdFile(BaseMdMedium):
-    absolute_path: str
-    """absolute path of markdown file"""
-
-    def update_config(self, **kwargs):
-        if "output_directory" in kwargs and kwargs["output_directory"]:
-            self.output_directory = supplementary_file_path(kwargs["output_directory"])
-            self.output_directory = self.absolute_path.replace(
-                self.root_directory, self.output_directory
-            )
-            if self.is_default_image_directory:
-                self.image_directory = f"{self.output_directory}/images"
-
-        if "image_directory" in kwargs and kwargs["image_directory"]:
-            self.image_directory = supplementary_file_path(kwargs["image_directory"])
-            self.is_default_image_directory = False
-        if "enable_save_images" in kwargs:
-            self.enable_save_images = kwargs["enable_save_images"]
-        if "enable_rename" in kwargs:
-            self.enable_rename = kwargs["enable_rename"]
-
-        os.makedirs(self.output_directory, exist_ok=True)
-        os.makedirs(self.image_directory, exist_ok=True)
-
-    @root_validator(pre=True)
-    def variables_check(cls, values: Dict[str, Any]) -> Optional[Dict[str, Any]]:
-        values["absolute_path_name"] = supplementary_file_path(values["name"])
-        assert os.path.exists(
-            values["absolute_path_name"]
-        ), f'<{values["absolute_path_name"]}> does not exists.'
-        assert (
-            values["name"][-3:] == ".md"
-        ), f'<{values["name"][-3:]}> is not markdown file.'
-
-        values["name"] = values["absolute_path_name"].split("/")[-1]
-        values["absolute_path"] = "/".join(values["absolute_path_name"].split("/")[:-1])
-        if "image_type" in values and values["image_type"] == "local":
-            assert (
-                "image_directory" in values and values["image_directory"]
-            ), "If image_type is local, then image_directory is necessary."
-            values["image_directory"] = supplementary_file_path(
-                values["image_directory"]
-            )
-            values["is_default_image_directory"] = False
-        else:
-            if "image_directory" not in values or not values["image_directory"]:
-                values["image_directory"] = f"{values['absolute_path']}/images"
-                values["is_default_image_directory"] = True
-
-        if "output_directory" not in values:
-            values["output_directory"] = values["absolute_path"]
-        os.makedirs(values["output_directory"], exist_ok=True)
-        return values
-
-    @validator("enable_save_images", always=True)
-    def update_enable_save_images(
-        cls, enable_save_images: bool, values: Dict[str, Any]
-    ) -> bool:
-        if values["image_type"] == "local" and not enable_save_images:
-            raise ValueError(
-                "You can not set enable_save_images = False if you original markdown file image is local url."
-            )
-        return enable_save_images
-
-    @property
-    def to_convert_params(self) -> Dict[str, Any]:
-        params = {
-            "md_file_path": self.absolute_path_name,
-            "enable_rename": self.enable_rename,
-            "output_md_directory": self.output_directory,
-            "image_local_storage_directory": self.image_directory,
-            "is_local_images": True if self.image_type == "local" else False,
-            "enable_save_images": self.enable_save_images,
-        }
-        logger.debug(f"[imarkdown] MdFile convert params {params}")
-        return params
-
-
-class MdFolder(BaseMdMedium):
-    sub_nodes: List[Union[MdFile, "MdFolder"]] = []
-    """Current folder dir or markdown file, it contains list of MdFile and MdFolder instances."""
-    is_root: bool = False
-    enable_keep_original_file_status: bool = False
-    """todo not finish
-    There are a pure markdown folder will be created if MdImageConverter convert MdFolder. But
-    if there are some else files in the folder and you want to keep them. You can set this False."""
-
-    @root_validator(pre=True)
-    def variables_check(cls, values: Dict[str, Any]) -> Optional[Dict[str, Any]]:
-        values["absolute_path_name"] = supplementary_file_path(values["name"])
-        assert os.path.exists(
-            values["absolute_path_name"]
-        ), f'<{values["absolute_path_name"]}> file does not exists.'
-        assert os.path.isdir(
-            values["absolute_path_name"]
-        ), f'<{values["absolute_path_name"]}> file is not dir.'
-
-        md_initialization_params = {
-            "image_type": "remote",
-            "type": "original",
-            "is_root": False,
-        }
-
-        values["name"] = values["absolute_path_name"].split("/")[-1]
-        if "image_type" in values and values["image_type"] == "local":
-            assert (
-                "image_directory" in values and values["image_directory"]
-            ), "If image_type is local, then image_directory is necessary."
-            md_initialization_params["image_type"] = values["image_type"]
-
-        if "type" in values and values["type"]:
-            md_initialization_params["type"] = values["type"]
-
-        if "output_directory" not in values:
-            values["output_directory"] = values["absolute_path_name"]
-        values["output_directory"] = supplementary_file_path(values["output_directory"])
-        md_initialization_params["output_directory"] = values["output_directory"]
-        os.makedirs(values["output_directory"], exist_ok=True)
-
-        if "image_directory" in values and values["image_directory"]:
-            values["image_directory"] = supplementary_file_path(
-                values["image_directory"]
-            )
-        else:
-            values["image_directory"] = f'{values["output_directory"]}/images'
-        md_initialization_params["image_directory"] = values["image_directory"]
-
-        if "root_directory" not in values:
-            values["root_directory"] = values["output_directory"]
-
-        if "is_root" in values and values["is_root"]:
-            md_initialization_params["root_directory"] = values["output_directory"]
-        else:
-            md_initialization_params["root_directory"] = values["root_directory"]
-
-        if "enable_rename" in values and values["enable_rename"]:
-            md_initialization_params["enable_rename"] = values["enable_rename"]
-
-        # build sub nodes
-        values["sub_nodes"] = []
-        sub_files = glob.glob(os.path.join(values["absolute_path_name"], "*"))
-        for sub_file in sub_files:
-            if not exist_markdown_file(sub_file):
-                continue
-            sub_file = convert_backslashes(sub_file)
-            if os.path.isdir(sub_file):
-                values["sub_nodes"].append(
-                    MdFolder(name=sub_file, **md_initialization_params)
-                )
-            if os.path.isfile(sub_file) and sub_file.endswith(".md"):
-                values["sub_nodes"].append(
-                    MdFile(name=sub_file, **md_initialization_params)
-                )
-
-        return values
-
-
-class MdMediumManager(BaseModel):
-    _md_files: List[MdFile] = []
-    output_directory: Optional[str] = None
-    enable_save_images: bool = True
-    additional_kwargs: Optional[Dict[str, Any]] = None
-
-    def update_config(
-        self,
-        output_directory: Optional[str] = None,
-        enable_save_images: bool = True,
-    ):
-        """Update every md_file basic parameters."""
-        if not self._md_files:
-            ValueError("Please run generate_md_files firstly.")
-        for md_file in self._md_files:
-            params = {
-                "output_directory": output_directory,
-                "enable_save_images": enable_save_images,
-            }
-            if output_directory:
-                params.update({"enable_rename": False})
-
-            md_file.update_config(**params)
-
-    def init_md_files(
-        self,
-        md_mediums: List[Union[MdFile, MdFolder]],
-    ) -> List[MdFile]:
-        """MdFolder may contain several MdFile.This method can convert all
-        MdFolders and MdFiles to MdFiles list.
-
-        Args:
-            md_mediums(List[Union[MdFile, MdFolder]]): a list of MdFile and MdFolder
-
-        Returns:
-            A list of all MdFile.
-        """
-        def find_sub_files(md_folder: MdFolder):
-            for sub_node in md_folder.sub_nodes:
-                if isinstance(sub_node, MdFile):
-                    self._md_files.append(sub_node)
-                elif isinstance(sub_node, MdFolder):
-                    find_sub_files(sub_node)
-
-        for medium in md_mediums:
-            if isinstance(medium, MdFile):
-                self._md_files.append(medium)
-            elif isinstance(medium, MdFolder):
-                find_sub_files(medium)
-        return self._md_files
-
-    @property
-    def md_files(self) -> List[MdFile]:
-        """MdFolder may contain several MdFile. This attribute will find all MdFile in mediums."""
-        if self._md_files:
-            return self._md_files
-        raise ValueError("Please run generate_md_files firstly.")
+import glob
+import logging
+import os
+from typing import List, Optional, Any, Dict, Union
+
+from pydantic import BaseModel, root_validator, validator
+from typing_extensions import Literal
+
+from imarkdown.utils import (
+    supplementary_file_path,
+    convert_backslashes,
+    exist_markdown_file,
+)
+
+logger = logging.getLogger(__name__)
+
+
+class BaseMdMedium(BaseModel):
+    name: str
+    """markdown medium name"""
+    absolute_path_name: str = ""
+    """path + name"""
+    image_directory: Optional[str] = None
+    """image storage path if it exists"""
+    image_type: Literal["local", "remote"] = "remote"
+    is_default_image_directory: bool = True
+    type: Literal["original", "converted"] = "original"
+    output_directory: Optional[str] = None
+    enable_save_images: bool = True
+    enable_rename: bool = True
+    root_directory: Optional[str] = None
+
+
+class MdFile(BaseMdMedium):
+    absolute_path: str = ""
+    """absolute path of markdown file"""
+
+    def update_config(self, **kwargs):
+        if "output_directory" in kwargs and kwargs["output_directory"]:
+            self.output_directory = supplementary_file_path(kwargs["output_directory"])
+            self.output_directory = self.absolute_path.replace(
+                self.root_directory, self.output_directory
+            )
+            if self.is_default_image_directory:
+                self.image_directory = f"{self.output_directory}/images"
+
+        if "image_directory" in kwargs and kwargs["image_directory"]:
+            self.image_directory = supplementary_file_path(kwargs["image_directory"])
+            self.is_default_image_directory = False
+        if "enable_save_images" in kwargs:
+            self.enable_save_images = kwargs["enable_save_images"]
+        if "enable_rename" in kwargs:
+            self.enable_rename = kwargs["enable_rename"]
+
+        os.makedirs(self.output_directory, exist_ok=True)
+        os.makedirs(self.image_directory, exist_ok=True)
+
+    @root_validator(pre=True)
+    def variables_check(cls, values: Dict[str, Any]) -> Optional[Dict[str, Any]]:
+        values["absolute_path_name"] = supplementary_file_path(values["name"])
+        assert os.path.exists(
+            values["absolute_path_name"]
+        ), f'<{values["absolute_path_name"]}> does not exists.'
+        assert (
+            values["name"][-3:] == ".md"
+        ), f'<{values["name"][-3:]}> is not markdown file.'
+
+        values["name"] = values["absolute_path_name"].split("/")[-1]
+        values["absolute_path"] = "/".join(values["absolute_path_name"].split("/")[:-1])
+        if "image_type" in values and values["image_type"] == "local":
+            assert (
+                "image_directory" in values and values["image_directory"]
+            ), "If image_type is local, then image_directory is necessary."
+            values["image_directory"] = supplementary_file_path(
+                values["image_directory"]
+            )
+            values["is_default_image_directory"] = False
+        else:
+            if "image_directory" not in values or not values["image_directory"]:
+                values["image_directory"] = f"{values['absolute_path']}/images"
+                values["is_default_image_directory"] = True
+
+        if "output_directory" not in values:
+            values["output_directory"] = values["absolute_path"]
+        os.makedirs(values["output_directory"], exist_ok=True)
+        return values
+
+    @validator("enable_save_images", always=True)
+    def update_enable_save_images(
+        cls, enable_save_images: bool, values: Dict[str, Any]
+    ) -> bool:
+        if values["image_type"] == "local" and not enable_save_images:
+            raise ValueError(
+                "You can not set enable_save_images = False if you original markdown file image is local url."
+            )
+        return enable_save_images
+
+    @property
+    def to_convert_params(self) -> Dict[str, Any]:
+        params = {
+            "md_file_path": self.absolute_path_name,
+            "enable_rename": self.enable_rename,
+            "output_md_directory": self.output_directory,
+            "image_local_storage_directory": self.image_directory,
+            "is_local_images": True if self.image_type == "local" else False,
+            "enable_save_images": self.enable_save_images,
+        }
+        logger.debug(f"[imarkdown] MdFile convert params {params}")
+        return params
+
+
+class MdFolder(BaseMdMedium):
+    sub_nodes: List[Union[MdFile, "MdFolder"]] = []
+    """Current folder dir or markdown file, it contains list of MdFile and MdFolder instances."""
+    is_root: bool = False
+    enable_keep_original_file_status: bool = False
+    """todo not finish
+    There are a pure markdown folder will be created if MdImageConverter convert MdFolder. But
+    if there are some else files in the folder and you want to keep them. You can set this False."""
+
+    @root_validator(pre=True)
+    def variables_check(cls, values: Dict[str, Any]) -> Optional[Dict[str, Any]]:
+        values["absolute_path_name"] = supplementary_file_path(values["name"])
+        assert os.path.exists(
+            values["absolute_path_name"]
+        ), f'<{values["absolute_path_name"]}> file does not exists.'
+        assert os.path.isdir(
+            values["absolute_path_name"]
+        ), f'<{values["absolute_path_name"]}> file is not dir.'
+
+        md_initialization_params = {
+            "image_type": "remote",
+            "type": "original",
+            "is_root": False,
+        }
+
+        values["name"] = values["absolute_path_name"].split("/")[-1]
+        if "image_type" in values and values["image_type"] == "local":
+            assert (
+                "image_directory" in values and values["image_directory"]
+            ), "If image_type is local, then image_directory is necessary."
+            md_initialization_params["image_type"] = values["image_type"]
+
+        if "type" in values and values["type"]:
+            md_initialization_params["type"] = values["type"]
+
+        if "output_directory" not in values:
+            values["output_directory"] = values["absolute_path_name"]
+        values["output_directory"] = supplementary_file_path(values["output_directory"])
+        md_initialization_params["output_directory"] = values["output_directory"]
+        os.makedirs(values["output_directory"], exist_ok=True)
+
+        if "image_directory" in values and values["image_directory"]:
+            values["image_directory"] = supplementary_file_path(
+                values["image_directory"]
+            )
+        else:
+            values["image_directory"] = f'{values["output_directory"]}/images'
+        md_initialization_params["image_directory"] = values["image_directory"]
+
+        if "root_directory" not in values:
+            values["root_directory"] = values["output_directory"]
+
+        if "is_root" in values and values["is_root"]:
+            md_initialization_params["root_directory"] = values["output_directory"]
+        else:
+            md_initialization_params["root_directory"] = values["root_directory"]
+
+        if "enable_rename" in values and values["enable_rename"]:
+            md_initialization_params["enable_rename"] = values["enable_rename"]
+
+        # build sub nodes
+        values["sub_nodes"] = []
+        sub_files = glob.glob(os.path.join(values["absolute_path_name"], "*"))
+        for sub_file in sub_files:
+            if not exist_markdown_file(sub_file):
+                continue
+            sub_file = convert_backslashes(sub_file)
+            if os.path.isdir(sub_file):
+                values["sub_nodes"].append(
+                    MdFolder(name=sub_file, **md_initialization_params)
+                )
+            if os.path.isfile(sub_file) and sub_file.endswith(".md"):
+                values["sub_nodes"].append(
+                    MdFile(name=sub_file, **md_initialization_params)
+                )
+
+        return values
+
+
+class MdMediumManager(BaseModel):
+    _md_files: List[MdFile] = []
+    output_directory: Optional[str] = None
+    enable_save_images: bool = True
+    additional_kwargs: Optional[Dict[str, Any]] = None
+
+    def update_config(
+        self,
+        output_directory: Optional[str] = None,
+        enable_save_images: bool = True,
+    ):
+        """Update every md_file basic parameters."""
+        if not self._md_files:
+            ValueError("Please run generate_md_files firstly.")
+        for md_file in self._md_files:
+            params = {
+                "output_directory": output_directory,
+                "enable_save_images": enable_save_images,
+            }
+            if output_directory:
+                params.update({"enable_rename": False})
+
+            md_file.update_config(**params)
+
+    def init_md_files(
+        self,
+        md_mediums: List[Union[MdFile, MdFolder]],
+    ) -> List[MdFile]:
+        """MdFolder may contain several MdFile.This method can convert all
+        MdFolders and MdFiles to MdFiles list.
+
+        Args:
+            md_mediums(List[Union[MdFile, MdFolder]]): a list of MdFile and MdFolder
+
+        Returns:
+            A list of all MdFile.
+        """
+        def find_sub_files(md_folder: MdFolder):
+            for sub_node in md_folder.sub_nodes:
+                if isinstance(sub_node, MdFile):
+                    self._md_files.append(sub_node)
+                elif isinstance(sub_node, MdFolder):
+                    find_sub_files(sub_node)
+
+        for medium in md_mediums:
+            if isinstance(medium, MdFile):
+                self._md_files.append(medium)
+            elif isinstance(medium, MdFolder):
+                find_sub_files(medium)
+        return self._md_files
+
+    @property
+    def md_files(self) -> List[MdFile]:
+        """MdFolder may contain several MdFile. This attribute will find all MdFile in mediums."""
+        if self._md_files:
+            return self._md_files
+        raise ValueError("Please run generate_md_files firstly.")
```

### Comparing `imarkdown-1.1.2/imarkdown/utils/__init__.py` & `imarkdown-1.2.1/imarkdown/utils/__init__.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-import os
-
-
-def polish_path(path: str, enable_prefix: bool = True, enable_suffix: bool = True):
-    if enable_suffix and (path[-1] != "/" or path[-1] != "\\"):
-        path += "/"
-    if enable_prefix and (path[0] == "/" or path[0] == "\\"):
-        path = path[1:]
-    return path
-
-
-def supplementary_file_path(file_path: str) -> str:
-    """Get absolute file path.
-
-    Args:
-        file_path: absolute file path or relative file path
-
-    Returns:
-        return absolute file path
-    """
-    if os.path.isabs(file_path):
-        return file_path
-    else:
-        current_dir = os.getcwd()
-
-        if file_path.startswith("../"):
-            while file_path.startswith("../"):
-                current_dir = os.path.dirname(current_dir)
-                file_path = file_path[3:]
-        elif file_path.startswith("./"):
-            file_path = file_path[2:]
-
-        absolute_path = os.path.join(current_dir, file_path)
-        return convert_backslashes(absolute_path)
-
-
-def get_file_name_from_relative_path(relative_path: str) -> str:
-    """Get file name, image name, markdown name from relative path."""
-    if relative_path.startswith("../"):
-        while relative_path.startswith("../"):
-            relative_path = relative_path[3:]
-    elif relative_path.startswith("./"):
-        relative_path = relative_path[2:]
-    return relative_path.split("/")[-1]
-
-
-def convert_backslashes(path):
-    """Convert all \\ to / of file path."""
-    return path.replace("\\", "/")
-
-
-def calculate_relative_path(image_path, md_directory):
-    image_path = os.path.abspath(image_path)
-    md_directory = os.path.abspath(md_directory)
-
-    image_parts = image_path.split(os.path.sep)
-    md_parts = md_directory.split(os.path.sep)
-    if not os.path.isdir(md_directory):
-        md_parts = md_parts[:-1]
-
-    common_parts = os.path.commonpath([image_path, md_directory])
-    common_index = len(common_parts.split(os.path.sep))
-
-    relative_parts = []
-    if common_index == len(md_parts):
-        relative_parts.append(".")
-    else:
-        relative_parts.extend([".."] * (len(md_parts) - common_index))
-
-    relative_parts.extend(image_parts[common_index:])
-
-    relative_path = os.path.join(*relative_parts)
-    return convert_backslashes(relative_path)
-
-
-def exist_markdown_file(path: str) -> bool:
-    """Determine whether there are markdown file in the folder directory.
-
-    Args:
-        path: folder absolute path
-
-    Returns:
-        True means existence, False otherwise.
-    """
-    if path.endswith(".md"):
-        return True
-    for root, dirs, files in os.walk(path):
-        for file in files:
-            if file.endswith(".md"):
-                return True
-    return False
+import os
+
+
+def polish_path(path: str, enable_prefix: bool = True, enable_suffix: bool = True):
+    if enable_suffix and (path[-1] != "/" or path[-1] != "\\"):
+        path += "/"
+    if enable_prefix and (path[0] == "/" or path[0] == "\\"):
+        path = path[1:]
+    return path
+
+
+def supplementary_file_path(file_path: str) -> str:
+    """Get absolute file path.
+
+    Args:
+        file_path: absolute file path or relative file path
+
+    Returns:
+        return absolute file path
+    """
+    if os.path.isabs(file_path):
+        return file_path
+    else:
+        current_dir = os.getcwd()
+
+        if file_path.startswith("../"):
+            while file_path.startswith("../"):
+                current_dir = os.path.dirname(current_dir)
+                file_path = file_path[3:]
+        elif file_path.startswith("./"):
+            file_path = file_path[2:]
+
+        absolute_path = os.path.join(current_dir, file_path)
+        return convert_backslashes(absolute_path)
+
+
+def get_file_name_from_relative_path(relative_path: str) -> str:
+    """Get file name, image name, markdown name from relative path."""
+    if relative_path.startswith("../"):
+        while relative_path.startswith("../"):
+            relative_path = relative_path[3:]
+    elif relative_path.startswith("./"):
+        relative_path = relative_path[2:]
+    return relative_path.split("/")[-1]
+
+
+def convert_backslashes(path):
+    """Convert all \\ to / of file path."""
+    return path.replace("\\", "/")
+
+
+def calculate_relative_path(image_path, md_directory):
+    image_path = os.path.abspath(image_path)
+    md_directory = os.path.abspath(md_directory)
+
+    image_parts = image_path.split(os.path.sep)
+    md_parts = md_directory.split(os.path.sep)
+    if not os.path.isdir(md_directory):
+        md_parts = md_parts[:-1]
+
+    common_parts = os.path.commonpath([image_path, md_directory])
+    common_index = len(common_parts.split(os.path.sep))
+
+    relative_parts = []
+    if common_index == len(md_parts):
+        relative_parts.append(".")
+    else:
+        relative_parts.extend([".."] * (len(md_parts) - common_index))
+
+    relative_parts.extend(image_parts[common_index:])
+
+    relative_path = os.path.join(*relative_parts)
+    return convert_backslashes(relative_path)
+
+
+def exist_markdown_file(path: str) -> bool:
+    """Determine whether there are markdown file in the folder directory.
+
+    Args:
+        path: folder absolute path
+
+    Returns:
+        True means existence, False otherwise.
+    """
+    if path.endswith(".md"):
+        return True
+    for root, dirs, files in os.walk(path):
+        for file in files:
+            if file.endswith(".md"):
+                return True
+    return False
```

### Comparing `imarkdown-1.1.2/imarkdown.egg-info/PKG-INFO` & `imarkdown-1.2.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,337 +1,337 @@
-Metadata-Version: 2.1
-Name: imarkdown
-Version: 1.1.2
-Summary: A practical Markdown image url converter
-Home-page: https://github.com/Undertone0809/imarkdown
-Author: Zeeland
-Author-email: zeeland@foxmail.com
-License: Apache 2.0
-Keywords: Markdown,markdown,imarkdown,markdown converter
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: license
-
-<h1 align="center">
-    imarkdown
-</h1>
-<p align="center">
-  <strong>imarkdown is a lightweight markdown image link converter that allows you to easily convert image links between local and image server, as well as between different image servers.</strong>
-</p>
-
-[English](/README.md) [中文](/README_zh.md)
-
-> When converting markdown from Yuque, the images are protected against external linking. If you want to publish the converted markdown on other platforms, you need to change all the image addresses in the markdown to local image addresses or custom image server addresses, so that others can view them correctly. This project aims to solve this problem by providing a converter that can batch convert image links in markdown and supports customized conversion in complex scenarios.
-
-## Features
-
-- Batch Download: imarkdown can batch download all the images in the markdown that are referenced using image links.
-- Multiple Conversion Methods: imarkdown supports various conversion methods for image links in markdown, such as converting to local image, converting web URL to local image, and converting web URL to image server URL.
-- Batch Conversion: It supports batch conversion of single or multiple files, as well as formatting and renaming of generated files.
-- Highly Customizable: By inheriting the `MdAdapter` class, you can easily implement custom URL conversion for different image servers.
-- Image Server Adapters: Currently, only Aliyun OSS is supported as an image server. Contributions are welcome to add support for more types of image servers.
-
-## Target Audience
-
-- People who need to batch convert image links in markdown.
-- Users who export markdown from Yuque and need to convert image links.
-- People who need to develop third-party extensions.
-
-## Technical Architecture
-
-`imarkdown` is designed with a modular architecture, allowing easy extension of each component. The following diagram provides a simplified overview of the technical architecture of imarkdown, which consists of the following components:
-
-- `MdImageConverter`: The image converter responsible for converting the image addresses in markdown and generating new markdown files.
-- `MdAdapter`: The adapter for converting `Image` objects to different types, such as `LocalFileAdapter` for local conversion, `AliyunAdapter` for Aliyun OSS conversion, and `CustomAdapter` for custom conversion. By injecting the adapter into `MdImageConverter`, you can define the type of address to convert `Image` objects to.
-- `MdMedium`: Includes `MdFile` and `MdFolder`, encapsulating some features used for data conversion in `MdImageConverter`.
-
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230713154424.png"/>
-
-The execution process of `imarkdown` is roughly as follows: after the `convert` method is called on `MdImageConverter`, `imarkdown` builds a virtual `MdTree` based on the provided `MdMedium`, and performs batch image URL conversion on the files according to this tree.
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230713155912.png"/>
-
-## Quick Start
-
-This project is developed in Python and distributed on PyPI. Users can easily use imarkdown by installing it with pip. The following sections will explain several usage scenarios and methods of imarkdown.
-
-- Third-Party Package Installation: Open a terminal or command prompt and run the following command.
-
-```sh
-pip install -U imarkdown
-```
-
-**Examples**
-- [Convert Web URLs to Local Addresses](#converting-web-urls-to-local-file-paths)
-- [Convert Web URLs to Image Server URLs](#converting-web-urls-to-image-hosting-service-urls)
-- [Batch Conversion: Web URLs to Local](#batch-conversion-of-multiple-files-web-url-to-local)
-- [Batch Conversion: Local to Image Server](#batch-conversion-of-multiple-files-local-to-image-hosting-service)
-- [Custom Image Hosting Service](#custom-image-hosting-service)
-
-
-### Converting Web URLs to Local File Paths
-
-If you have web URL links for images in your Markdown file and you want to download them in bulk to your local machine while converting the image addresses in Markdown to local file paths, the following example will solve your problem.
-
-Assuming the file you want to convert is `test.md` with the following content:
-
-> The examples below will be based on the initial Markdown file if it is a web URL. They are not repeated here.
-
-```text
-## 6.3 Converting MD Image Addresses
-Only supports uploading to a local image hosting service.
-
-- [https://github.com/JyHu/useful_script.git](https://github.com/JyHu/useful_script.git)
-- [https://github.com/JyHu/useful_script/blob/](https://github.com/JyHu/useful_script/blob/master/Scripts/md%E6%96%87%E4%BB%B6%E5%9B%BE%E7%89%87%E5%9B%BE%E5%BA%8A%E8%BD%AC%E6%8D%A2/%E8%87%AA%E5%8A%A8%E8%BD%AC%E6%8D%A2markdown%E6%96%87%E4%BB%B6%E4%B8%AD%E5%9B%BE%E7%89%87%E5%88%B0%E5%9B%BE%E5%BA%8A.md/)
-
-After all the hassle and trying this, I found it doesn't work either.
-![image.png](https://cdn.nlark.com/yuque/0/2022/png/26910220/1670091709979-52f8c3c4-a00f-4668-a236-29ad2c09d0da.png#averageHue=%23272c34&clientId=ubb991e0d-3414-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=928&id=u4a7a8376&margin=%5Bobject%20Object%5D&name=image.png&originHeight=928&originWidth=1050&originalType=binary&ratio=1&rotation=0&showTitle=false&size=201083&status=done&style=none&taskId=u27493dc0-9d78-4c07-929c-cc946d41409&title=&width=1050)
-
-In the end, PigGo is still the best. It provides a shortcut for uploading, and after uploading, you can directly xxxTODO.
-
-## 6.4 Pycasbin
-
-In pycasbin, I saw a colleague who frequently contributes to pycasbin. You can refer to some of his contributions:
-
-- [https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md](https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md)
-
-
-![image.png](https://cdn.nlark.com/yuque/0/2022/png/26910220/1670150012015-3a93ec6b-bb27-4ed3-b42f-252a0f70b65c.png#averageHue=%23fcfbf5&clientId=u86ce0a81-ec80-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=936&id=ube9c482c&margin=%5Bobject%20Object%5D&name=image.png&originHeight=936&originWidth=1920&originalType=binary&ratio=1&rotation=0&showTitle=false&size=205691&status=done&style=none&taskId=u6a6825da-aaf4-471c-ad0e-2280c325c66&title=&width=1920)
-```
-
-This content is the exported Markdown file from Yuque, and its image links are protected against external access. They need to be downloaded and replaced with local file paths in the Markdown.
-
-```python
-from imarkdown import MdFile, LocalFileAdapter, MdImageConverter
-
-def main():
-    adapter = LocalFileAdapter()
-    converter = MdImageConverter(adapter=adapter)
-    
-    md_file = MdFile(name="test.md")
-    converter.convert(md_file)
-
-if __name__ == '__main__':
-    main()
-```
-
-> In imarkdown, there are many places where you need to provide paths. You can use relative paths or absolute paths. It is recommended to use `/` as the path separator instead of `\\`.
-
-The converted result will generate a new Markdown file named `test_converted.md`, with the following content:
-
-```text
-## 6.3 Converting MD Image Addresses
-Only supports uploading to a local image hosting service.
-
-- [https://github.com/JyHu/useful_script.git](https://github.com/JyHu/useful_script.git)
-- [https://github.com/JyHu/useful_script/blob/](https://github.com/JyHu/useful_script/blob/master/Scripts/md%E6%96%87%E4%BB%B6%E5%9B%BE%E7%89%87%E5%9B%BE%E5%BA%8A%E8%BD%AC%E6%8D%A2/%E8%87%AA%E5%8A%A8%E8%BD%AC%E6%8D%A2markdown%E6%96%87%E4%BB%B6%E4%B8%AD%E5%9B%BE%E7%89%87%E5%88%B0%E5%9B%BE%E5%BA%8A.md/)
-
-After all the hassle and trying this, I found it doesn't work either.
-![image.png](./images/20230713_1356451324.png)
-
-In the end, PigGo is still the best. It provides a shortcut for uploading, and after uploading, you can directly xxxTODO.
-
-## 6.4 Pycasbin
-
-In pycasbin, I saw a colleague who frequently contributes to pycasbin. You can refer to some of his contributions:
-
-- [https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md](https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md)
-
-
-![image.png](./images/20230713_1356469646.png)
-```
-
-- Customizing the Output File Name
-When using imarkdown for conversion, the default name for the converted Markdown file is `{markdown_file_name}_converted.md`. If you want to customize the output file name, you can use the following configuration:
-
-```python
-md_converter.convert(md_file, name_prefix="new_", name_suffix="_converted")
-```
-
-Using this method of conversion will result in a file named `new_test_converted.md`. If you want to completely customize the converted name, you can use the following method:
-
-```python
-md_converter.convert(md_file, new_name="A new markdown.md")
-```
-
-With the above method, a file named `A new markdown.md` will be generated.
-
-### Converting Web URLs to Image Hosting Service URLs
-
-In the following example, we will use the `test.md` file provided earlier to demonstrate the conversion of image addresses from web URLs to URLs on the Alibaba Cloud OSS server, showcasing the functionality of converting web URLs to image hosting service URLs.
-
-```python
-from imarkdown import MdImageConverter, AliyunAdapter, MdFile
-
-
-def main():
-    aliyun_config = {
-        "access_key_id": "key_id",
-        "access_key_secret": "key_secret",
-        "bucket_name": "bucket_name",
-        "place": "bucket_place",
-        "storage_path_prefix": "prefix",
-    }
-    adapter = AliyunAdapter(**aliyun_config)
-    md_converter = MdImageConverter(adapter=adapter)
-    md_file = MdFile(name="markdown.md")
-    md_converter.convert(md_file)
-
-
-if __name__ == "__main__":
-    main()
-```
-
-In the example above, `storage_path_prefix` represents the file prefix in the bucket where the image is uploaded to OSS. If you want to store the image in the `/imarkdown` directory, you need to set `storage_path_prefix="/imarkdown"`. The remaining configuration details are specific to Alibaba Cloud OSS, so please fill them in accordingly.
-
-
-### Batch Conversion of Multiple Files: Web URL to Local
-
-The following example demonstrates a solution for batch conversion of multiple Markdown files, converting web image URLs to local image addresses.
-
-```python
-from imarkdown import LocalFileAdapter, MdFolder, MdImageConverter
-
-def main():
-    adapter = LocalFileAdapter()
-    converter = MdImageConverter(adapter=adapter)
-    
-    # Folder name is "mds"
-    md_folder = MdFolder(name="mds")
-    # Output files to "converted_mds"
-    converter.convert(md_folder, output_directory="converted_mds")
-```
-
-Using the above code snippet will create a folder named "converted_mds" where the converted files will be saved. The images will be saved in the `converted_mds/images` directory. If you want to output the images to a specific folder, you can set it as follows:
-
-```python
-md_folder = MdFolder(name="mds", image_directory="mds/my_images")
-```
-
-### Batch Conversion of Multiple Files: Local to Image Hosting Service
-
-The following example demonstrates a solution for batch conversion of multiple Markdown files, converting local image addresses to image hosting service URLs.
-
-```python
-from imarkdown import LocalFileAdapter, MdFolder, MdImageConverter
-
-def main():
-    adapter = LocalFileAdapter()
-    converter = MdImageConverter(adapter=adapter)
-    
-    # Folder name is "local_mds", images are of local type, and image URLs are saved in "local_mds/images"
-    md_folder = MdFolder(name="local_mds", image_type="local", image_directory="local_mds/images")
-    # Output files to "converted_mds"
-    converter.convert(md_folder, output_directory="converted_mds")
-```
-
-### Custom Image Hosting Service
-
-The following example demonstrates how to use imarkdown to upload images to a custom file server and retrieve the URL.
-
-First, you need to create a custom adapter by inheriting from `BaseMdAdapter` and implementing the `upload` and `get_replaced_url` methods. Then, you can inject the custom adapter into `MdImageConverter`.
-
-```python
-import os
-import json
-
-import requests
-from imarkdown import BaseMdAdapter, MdImageConverter, MdFolder
-
-class CustomMdAdapter(BaseMdAdapter):
-    name = "custom"
-    url = "https://server/upload/file/batch"
-    headers = {
-        "X-Upload-Token": "my_token"
-    }
-    cur_key = ""
-
-    def upload(self, key: str, file):
-        files = {"file": file}
-        response = requests.post(self.url, headers=self.headers, files=files)
-        if response.status_code == 200:
-            res_data = json.loads(response.content.decode("utf-8"))
-            self.cur_key = res_data["data"]["images"]["url"]
-        else:
-            raise Exception(response.content)
-
-    def get_replaced_url(self, key):
-        return self.cur_key
-
-def get_all_folder_names():
-    return os.listdir("my-blog")
-
-    
-def main():
-    adapter = CustomMdAdapter()
-    md_converter = MdImageConverter(adapter=adapter)
-
-    md_folders = []
-    for folder_name in get_all_folder_names():
-        md_folders.append(
-            MdFolder(
-                name=f"my-blog/{folder_name}",
-                image_directory=f"my-blog/{folder_name}/images",
-                image_type="local",
-            )
-        )
-    md_converter.convert(md_folders, output_directory="converted")
-
-
-if __name__ == "__main__":
-    main()
-```
-
-## Roadmap
-
-- [ ] Add client-side support
-- [ ] Support Tencent Cloud, Qiniu Cloud, and other image hosting services
-- [x] Support batch file modification
-- [x] Custom adapters
-- [ ] Support compression of large images
-- [ ] Support command-line interface
-- [x] Support PyPI for simplified operations
-- [ ] Provide file custom naming
-- [ ] Provide custom formatting for image names
-
-## FAQ
-
-**1. How can I extend to other image hosting services?**
-
-If you want to develop support for other image hosting services, all you need to do is implement an adapter similar to `AliyunAdapter` and inject it into `MdImageConverter` when using it. Refer to [Custom Image Hosting Service](#custom-image-hosting-service). That's all you need to do. In fact, I've wrapped it up nicely, so extending it is straightforward.
-
-**2. Usage of file addresses**
-
-In Python, both `/` and `\\` can be used as file path separators. However, there are some differences in their usage.
-
-- `/` (forward slash): In most operating systems, including Windows, Linux, and Mac, `/` is used as the file path separator. Using `/` as the separator can make your code portable across different operating systems. For example:
-
-```python
-path = "folder/file.txt"
-```
-
-- `\\` (backslash): In the Windows operating system, `\\` is used as the file path separator. This is because `\` is used as an escape character in Windows, so to represent a plain backslash, you need to use two consecutive backslashes. For example:
-
-```python
-path = "folder\\file.txt"
-```
-
-When using `\\` as the separator, keep the following points in mind:
-
-- When using `\\` in a string, you need to escape it as `\\\\` because the first `\` will be interpreted as an escape character.
-- You can use raw strings to avoid the hassle of escaping. In a raw string, `\` is not interpreted as an escape character. For example: `path = r"folder\file.txt"`
-
-In summary, if your code needs to run on different operating systems, it is recommended to use `/` as the file path separator to maintain code portability. If you are only running the code on Windows, using `\\` is also acceptable. However, in `imarkdown`, all `\\` paths will be converted to `/`. In this project, all `\\` paths will be converted to `/`.
-
-## Contribution
-
-Contributions are welcome! If you would like to contribute to this project, you can submit a pull request or an issue. There are some extensible features listed in the [Development Roadmap](#development-roadmap), and there are still many third-party image hosting services that need to be adapted. If you are working on these aspects, feel free to submit a pull request! I'm excited to see more people involved in improving and optimizing it.
+<h1 align="center">
+    imarkdown
+</h1>
+<p align="center">
+  <strong>imarkdown is a lightweight markdown image link converter that allows you to easily convert image links between local and image server, as well as between different image servers.</strong>
+</p>
+
+[English](/README.md) [中文](/README_zh.md)
+
+> When converting markdown from Yuque, the images are protected against external linking. If you want to publish the converted markdown on other platforms, you need to change all the image addresses in the markdown to local image addresses or custom image server addresses, so that others can view them correctly. This project aims to solve this problem by providing a converter that can batch convert image links in markdown and supports customized conversion in complex scenarios.
+
+## Features
+
+- Batch Download: imarkdown can batch download all the images in the markdown that are referenced using image links.
+- Multiple Conversion Methods: imarkdown supports various conversion methods for image links in markdown, such as converting to local image, converting web URL to local image, and converting web URL to image server URL.
+- Batch Conversion: It supports batch conversion of single or multiple files, as well as formatting and renaming of generated files.
+- Highly Customizable: By inheriting the `MdAdapter` class, you can easily implement custom URL conversion for different image servers.
+- Image Server Adapters: Currently, only Aliyun OSS is supported as an image server. Contributions are welcome to add support for more types of image servers.
+
+## Target Audience
+
+- People who need to batch convert image links in markdown.
+- Users who export markdown from Yuque and need to convert image links.
+- People who need to develop third-party extensions.
+
+## Technical Architecture
+
+`imarkdown` is designed with a modular architecture, allowing easy extension of each component. The following diagram provides a simplified overview of the technical architecture of imarkdown, which consists of the following components:
+
+- `MdImageConverter`: The image converter responsible for converting the image addresses in markdown and generating new markdown files.
+- `MdAdapter`: The adapter for converting `Image` objects to different types, such as `LocalFileAdapter` for local conversion, `AliyunAdapter` for Aliyun OSS conversion, and `CustomAdapter` for custom conversion. By injecting the adapter into `MdImageConverter`, you can define the type of address to convert `Image` objects to.
+- `MdMedium`: Includes `MdFile` and `MdFolder`, encapsulating some features used for data conversion in `MdImageConverter`.
+
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230713154424.png"/>
+
+The execution process of `imarkdown` is roughly as follows: after the `convert` method is called on `MdImageConverter`, `imarkdown` builds a virtual `MdTree` based on the provided `MdMedium`, and performs batch image URL conversion on the files according to this tree.
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230713155912.png"/>
+
+## Quick Start
+
+This project is developed in Python and distributed on PyPI. Users can easily use imarkdown by installing it with pip. The following sections will explain several usage scenarios and methods of imarkdown.
+
+- Third-Party Package Installation: Open a terminal or command prompt and run the following command.
+
+```sh
+pip install -U imarkdown
+```
+
+**Examples**
+- [Convert Web URLs to Local Addresses](#converting-web-urls-to-local-file-paths)
+- [Convert Web URLs to Image Server URLs](#converting-web-urls-to-image-hosting-service-urls)
+- [Batch Conversion: Web URLs to Local](#batch-conversion-of-multiple-files-web-url-to-local)
+- [Batch Conversion: Local to Image Server](#batch-conversion-of-multiple-files-local-to-image-hosting-service)
+- [Custom Image Hosting Service](#custom-image-hosting-service)
+
+
+### Converting Web URLs to Local File Paths
+
+If you have web URL links for images in your Markdown file and you want to download them in bulk to your local machine while converting the image addresses in Markdown to local file paths, the following example will solve your problem.
+
+Assuming the file you want to convert is `test.md` with the following content:
+
+> The examples below will be based on the initial Markdown file if it is a web URL. They are not repeated here.
+
+```text
+## 6.3 Converting MD Image Addresses
+Only supports uploading to a local image hosting service.
+
+- [https://github.com/JyHu/useful_script.git](https://github.com/JyHu/useful_script.git)
+- [https://github.com/JyHu/useful_script/blob/](https://github.com/JyHu/useful_script/blob/master/Scripts/md%E6%96%87%E4%BB%B6%E5%9B%BE%E7%89%87%E5%9B%BE%E5%BA%8A%E8%BD%AC%E6%8D%A2/%E8%87%AA%E5%8A%A8%E8%BD%AC%E6%8D%A2markdown%E6%96%87%E4%BB%B6%E4%B8%AD%E5%9B%BE%E7%89%87%E5%88%B0%E5%9B%BE%E5%BA%8A.md/)
+
+After all the hassle and trying this, I found it doesn't work either.
+![image.png](https://cdn.nlark.com/yuque/0/2022/png/26910220/1670091709979-52f8c3c4-a00f-4668-a236-29ad2c09d0da.png#averageHue=%23272c34&clientId=ubb991e0d-3414-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=928&id=u4a7a8376&margin=%5Bobject%20Object%5D&name=image.png&originHeight=928&originWidth=1050&originalType=binary&ratio=1&rotation=0&showTitle=false&size=201083&status=done&style=none&taskId=u27493dc0-9d78-4c07-929c-cc946d41409&title=&width=1050)
+
+In the end, PigGo is still the best. It provides a shortcut for uploading, and after uploading, you can directly xxxTODO.
+
+## 6.4 Pycasbin
+
+In pycasbin, I saw a colleague who frequently contributes to pycasbin. You can refer to some of his contributions:
+
+- [https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md](https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md)
+
+
+![image.png](https://cdn.nlark.com/yuque/0/2022/png/26910220/1670150012015-3a93ec6b-bb27-4ed3-b42f-252a0f70b65c.png#averageHue=%23fcfbf5&clientId=u86ce0a81-ec80-4&crop=0&crop=0&crop=1&crop=1&from=paste&height=936&id=ube9c482c&margin=%5Bobject%20Object%5D&name=image.png&originHeight=936&originWidth=1920&originalType=binary&ratio=1&rotation=0&showTitle=false&size=205691&status=done&style=none&taskId=u6a6825da-aaf4-471c-ad0e-2280c325c66&title=&width=1920)
+```
+
+This content is the exported Markdown file from Yuque, and its image links are protected against external access. They need to be downloaded and replaced with local file paths in the Markdown.
+
+```python
+from imarkdown import MdFile, LocalFileAdapter, MdImageConverter
+
+def main():
+    adapter = LocalFileAdapter()
+    converter = MdImageConverter(adapter=adapter)
+    
+    md_file = MdFile(name="test.md")
+    converter.convert(md_file)
+
+if __name__ == '__main__':
+    main()
+```
+
+> In imarkdown, there are many places where you need to provide paths. You can use relative paths or absolute paths. It is recommended to use `/` as the path separator instead of `\\`.
+
+The converted result will generate a new Markdown file named `test_converted.md`, with the following content:
+
+```text
+## 6.3 Converting MD Image Addresses
+Only supports uploading to a local image hosting service.
+
+- [https://github.com/JyHu/useful_script.git](https://github.com/JyHu/useful_script.git)
+- [https://github.com/JyHu/useful_script/blob/](https://github.com/JyHu/useful_script/blob/master/Scripts/md%E6%96%87%E4%BB%B6%E5%9B%BE%E7%89%87%E5%9B%BE%E5%BA%8A%E8%BD%AC%E6%8D%A2/%E8%87%AA%E5%8A%A8%E8%BD%AC%E6%8D%A2markdown%E6%96%87%E4%BB%B6%E4%B8%AD%E5%9B%BE%E7%89%87%E5%88%B0%E5%9B%BE%E5%BA%8A.md/)
+
+After all the hassle and trying this, I found it doesn't work either.
+![image.png](./images/20230713_1356451324.png)
+
+In the end, PigGo is still the best. It provides a shortcut for uploading, and after uploading, you can directly xxxTODO.
+
+## 6.4 Pycasbin
+
+In pycasbin, I saw a colleague who frequently contributes to pycasbin. You can refer to some of his contributions:
+
+- [https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md](https://github.com/Nekotoxin/nekotoxin.github.io/blob/gsoc_2022_summary/GSoC2022-summary.md)
+
+
+![image.png](./images/20230713_1356469646.png)
+```
+
+- Customizing the Output File Name
+When using imarkdown for conversion, the default name for the converted Markdown file is `{markdown_file_name}_converted.md`. If you want to customize the output file name, you can use the following configuration:
+
+```python
+md_converter.convert(md_file, name_prefix="new_", name_suffix="_converted")
+```
+
+Using this method of conversion will result in a file named `new_test_converted.md`. If you want to completely customize the converted name, you can use the following method:
+
+```python
+md_converter.convert(md_file, new_name="A new markdown.md")
+```
+
+With the above method, a file named `A new markdown.md` will be generated.
+
+### Converting Web URLs to Image Hosting Service URLs
+
+In the following example, we will use the `test.md` file provided earlier to demonstrate the conversion of image addresses from web URLs to URLs on the Alibaba Cloud OSS server, showcasing the functionality of converting web URLs to image hosting service URLs.
+
+```python
+from imarkdown import MdImageConverter, AliyunAdapter, MdFile
+
+
+def main():
+    aliyun_config = {
+        "access_key_id": "key_id",
+        "access_key_secret": "key_secret",
+        "bucket_name": "bucket_name",
+        "place": "bucket_place",
+        "storage_path_prefix": "prefix",
+    }
+    adapter = AliyunAdapter(**aliyun_config)
+    md_converter = MdImageConverter(adapter=adapter)
+    md_file = MdFile(name="markdown.md")
+    md_converter.convert(md_file)
+
+
+if __name__ == "__main__":
+    main()
+```
+
+In the example above, `storage_path_prefix` represents the file prefix in the bucket where the image is uploaded to OSS. If you want to store the image in the `/imarkdown` directory, you need to set `storage_path_prefix="/imarkdown"`. The remaining configuration details are specific to Alibaba Cloud OSS, so please fill them in accordingly.
+
+
+### Batch Conversion of Multiple Files: Web URL to Local
+
+The following example demonstrates a solution for batch conversion of multiple Markdown files, converting web image URLs to local image addresses.
+
+```python
+from imarkdown import LocalFileAdapter, MdFolder, MdImageConverter
+
+def main():
+    adapter = LocalFileAdapter()
+    converter = MdImageConverter(adapter=adapter)
+    
+    # Folder name is "mds"
+    md_folder = MdFolder(name="mds")
+    # Output files to "converted_mds"
+    converter.convert(md_folder, output_directory="converted_mds")
+```
+
+Using the above code snippet will create a folder named "converted_mds" where the converted files will be saved. The images will be saved in the `converted_mds/images` directory. If you want to output the images to a specific folder, you can set it as follows:
+
+```python
+md_folder = MdFolder(name="mds", image_directory="mds/my_images")
+```
+
+### Batch Conversion of Multiple Files: Local to Image Hosting Service
+
+The following example demonstrates a solution for batch conversion of multiple Markdown files, converting local image addresses to image hosting service URLs.
+
+```python
+from imarkdown import LocalFileAdapter, MdFolder, MdImageConverter
+
+def main():
+    adapter = LocalFileAdapter()
+    converter = MdImageConverter(adapter=adapter)
+    
+    # Folder name is "local_mds", images are of local type, and image URLs are saved in "local_mds/images"
+    md_folder = MdFolder(name="local_mds", image_type="local", image_directory="local_mds/images")
+    # Output files to "converted_mds"
+    converter.convert(md_folder, output_directory="converted_mds")
+```
+
+### Custom Image Hosting Service
+
+The following example demonstrates how to use imarkdown to upload images to a custom file server and retrieve the URL.
+
+First, you need to create a custom adapter by inheriting from `BaseMdAdapter` and implementing the `upload` and `get_replaced_url` methods. Then, you can inject the custom adapter into `MdImageConverter`.
+
+```python
+import os
+import json
+
+import requests
+from imarkdown import BaseMdAdapter, MdImageConverter, MdFolder
+
+class CustomMdAdapter(BaseMdAdapter):
+    name = "custom"
+    url = "https://server/upload/file/batch"
+    headers = {
+        "X-Upload-Token": "my_token"
+    }
+    cur_key = ""
+
+    def upload(self, key: str, file):
+        files = {"file": file}
+        response = requests.post(self.url, headers=self.headers, files=files)
+        if response.status_code == 200:
+            res_data = json.loads(response.content.decode("utf-8"))
+            self.cur_key = res_data["data"]["images"]["url"]
+        else:
+            raise Exception(response.content)
+
+    def get_replaced_url(self, key):
+        return self.cur_key
+
+def get_all_folder_names():
+    return os.listdir("my-blog")
+
+    
+def main():
+    adapter = CustomMdAdapter()
+    md_converter = MdImageConverter(adapter=adapter)
+
+    md_folders = []
+    for folder_name in get_all_folder_names():
+        md_folders.append(
+            MdFolder(
+                name=f"my-blog/{folder_name}",
+                image_directory=f"my-blog/{folder_name}/images",
+                image_type="local",
+            )
+        )
+    md_converter.convert(md_folders, output_directory="converted")
+
+
+if __name__ == "__main__":
+    main()
+```
+
+### Custom Regular Expression
+`imarkdown` use regular expression to find your images. It supports `![](image_url)` and `<img src="image_url"/>` format, but there are still some other format `imarkdown` can not find it.
+
+At this point, `imarkdown` supports custom regular expression to address this issue. You can customize a regular expression which can find your markdown image url and pass it to MdImageConverter. The following example show how to use it.
+
+```python
+from imarkdown import MdImageConverter, LocalFileAdapter, MdFolder
+
+
+def main():
+    custom_re = r"(?:!\[(.*?)\]\((.*?)\))|<img.*?src=[\'\"](.*?)[\'\"].*?>"
+    adapter = LocalFileAdapter()
+    md_converter = MdImageConverter(adapter=adapter)
+    
+    md_folder = MdFolder(name="mds")
+    md_converter.convert(md_folder, output_directory="output_mds", re_rule=custom_re)
+
+
+if __name__ == "__main__":
+    main()
+```
+
+## Roadmap
+
+- [ ] Add client-side support
+- [ ] Support Tencent Cloud, Qiniu Cloud, and other image hosting services
+- [x] Support batch file modification
+- [x] Custom adapters
+- [ ] Support compression of large images
+- [ ] Support command-line interface
+- [x] Support PyPI for simplified operations
+- [ ] Provide file custom naming
+- [ ] Provide custom formatting for image names
+
+## FAQ
+
+**1. How can I extend to other image hosting services?**
+
+If you want to develop support for other image hosting services, all you need to do is implement an adapter similar to `AliyunAdapter` and inject it into `MdImageConverter` when using it. Refer to [Custom Image Hosting Service](#custom-image-hosting-service). That's all you need to do. In fact, I've wrapped it up nicely, so extending it is straightforward.
+
+**2. Usage of file addresses**
+
+In Python, both `/` and `\\` can be used as file path separators. However, there are some differences in their usage.
+
+- `/` (forward slash): In most operating systems, including Windows, Linux, and Mac, `/` is used as the file path separator. Using `/` as the separator can make your code portable across different operating systems. For example:
+
+```python
+path = "folder/file.txt"
+```
+
+- `\\` (backslash): In the Windows operating system, `\\` is used as the file path separator. This is because `\` is used as an escape character in Windows, so to represent a plain backslash, you need to use two consecutive backslashes. For example:
+
+```python
+path = "folder\\file.txt"
+```
+
+When using `\\` as the separator, keep the following points in mind:
+
+- When using `\\` in a string, you need to escape it as `\\\\` because the first `\` will be interpreted as an escape character.
+- You can use raw strings to avoid the hassle of escaping. In a raw string, `\` is not interpreted as an escape character. For example: `path = r"folder\file.txt"`
+
+In summary, if your code needs to run on different operating systems, it is recommended to use `/` as the file path separator to maintain code portability. If you are only running the code on Windows, using `\\` is also acceptable. However, in `imarkdown`, all `\\` paths will be converted to `/`. In this project, all `\\` paths will be converted to `/`.
+
+## Contribution
+
+Contributions are welcome! If you would like to contribute to this project, you can submit a pull request or an issue. There are some extensible features listed in the [Development Roadmap](#development-roadmap), and there are still many third-party image hosting services that need to be adapted. If you are working on these aspects, feel free to submit a pull request! I'm excited to see more people involved in improving and optimizing it.
```

### Comparing `imarkdown-1.1.2/imarkdown.egg-info/SOURCES.txt` & `imarkdown-1.2.1/imarkdown.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 README.md
-license
 setup.py
 imarkdown/__init__.py
 imarkdown/config.py
 imarkdown/constant.py
 imarkdown/converter.py
 imarkdown/schema.py
 imarkdown.egg-info/PKG-INFO
```

### Comparing `imarkdown-1.1.2/setup.py` & `imarkdown-1.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-# Copyright 2022 Zeeland(https://github.com/Undertone0809/). All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import pathlib
-
-import setuptools
-
-here = pathlib.Path(__file__).parent.resolve()
-long_description = (here / "README.md").read_text(encoding="utf-8")
-
-setuptools.setup(
-    name="imarkdown",
-    version="1.1.2",
-    author="Zeeland",
-    author_email="zeeland@foxmail.com",
-    description="A practical Markdown image url converter",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/Undertone0809/imarkdown",
-    packages=setuptools.find_packages(),
-    install_requires=[
-        "requests",
-        "pydantic~=1.10.0",
-        "cushy-storage",
-        'broadcast-service==1.3.2',
-    ],
-    license="Apache 2.0",
-    classifiers=[
-        "Development Status :: 3 - Alpha",
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3 :: Only",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    keywords="Markdown, markdown, imarkdown, markdown converter",
-)
+# Copyright 2022 Zeeland(https://github.com/Undertone0809/). All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import pathlib
+
+import setuptools
+
+here = pathlib.Path(__file__).parent.resolve()
+long_description = (here / "README.md").read_text(encoding="utf-8")
+
+setuptools.setup(
+    name="imarkdown",
+    version="1.2.1",
+    author="Zeeland",
+    author_email="zeeland@foxmail.com",
+    description="A practical Markdown image url converter",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/Undertone0809/imarkdown",
+    packages=setuptools.find_packages(),
+    install_requires=[
+        "requests",
+        "pydantic~=1.10.0",
+        "cushy-storage",
+        'broadcast-service==1.3.2',
+    ],
+    license="Apache 2.0",
+    classifiers=[
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3 :: Only",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    keywords="Markdown, markdown, imarkdown, markdown converter",
+)
```

### Comparing `imarkdown-1.1.2/tests/test_adapter.py` & `imarkdown-1.2.1/tests/test_adapter.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-import logging
-from unittest import TestCase
-
-from imarkdown.adapter import AliyunAdapter, LocalFileAdapter
-from imarkdown.converter import MdImageConverter, MdFile, MdFolder
-
-logger = logging.getLogger(__name__)
-logging.basicConfig(level=logging.DEBUG)
-aliyun_config = {
-    "access_key_id": "key_id",
-    "access_key_secret": "key_secret",
-    "bucket_name": "bucket_name",
-    "place": "bucket_place",
-    "storage_path_prefix": "prefix",
-}
-
-
-class TestLocalFileAdapter(TestCase):
-    def test_local_adapter_init(self):
-        LocalFileAdapter()
-
-    def test_convert_md_file(self):
-        adapter = LocalFileAdapter()
-        md_converter = MdImageConverter(adapter=adapter)
-
-        md_file = MdFile(name="test.md")
-        md_converter.convert(md_file)
-
-    def test_convert_folder(self):
-        adapter = LocalFileAdapter()
-        md_converter = MdImageConverter(adapter=adapter)
-
-        folder = MdFolder(name="mds")
-        md_converter.convert(folder, output_directory="converted")
-
-
-class TestAliyunAdapter(TestCase):
-    def test_aliyun_adapter_init(self):
-        AliyunAdapter()
-
-    def test_convert_md_file(self):
-        adapter = AliyunAdapter()
-        md_converter = MdImageConverter(adapter=adapter)
-
-        md_file = MdFile(name="test.md")
-        md_converter.convert(md_file)
-
-    def test_convert_with_storage_prefix(self):
-        adapter = AliyunAdapter(storage_path_prefix="imarkdown")
-        md_converter = MdImageConverter(adapter=adapter)
-
-        md_file = MdFile(name="test.md")
-        md_converter.convert(md_file)
-
-    def test_convert_file(self):
-        adapter = AliyunAdapter()
-        md_converter = MdImageConverter(adapter=adapter)
-
-        md_folder = MdFolder(name="mds")
-        md_converter.convert(md_folder, output_directory="converted")
-
-    def test_local_to_remote(self):
-        adapter = LocalFileAdapter()
-        md_converter = MdImageConverter(adapter=adapter)
-        md_folder = MdFolder(name="mds")
-        md_converter.convert(md_folder, output_directory="local_mds")
-
-        adapter = AliyunAdapter()
-        md_converter = MdImageConverter(adapter=adapter)
-        md_folder = MdFolder(name="local_mds", image_type="local", image_directory="local_mds/images")
-        md_converter.convert(md_folder, output_directory="aliyun_converted")
+import logging
+from unittest import TestCase
+
+from imarkdown.adapter import AliyunAdapter, LocalFileAdapter
+from imarkdown.converter import MdImageConverter, MdFile, MdFolder
+
+logger = logging.getLogger(__name__)
+logging.basicConfig(level=logging.DEBUG)
+aliyun_config = {
+    "access_key_id": "key_id",
+    "access_key_secret": "key_secret",
+    "bucket_name": "bucket_name",
+    "place": "bucket_place",
+    "storage_path_prefix": "prefix",
+}
+
+
+class TestLocalFileAdapter(TestCase):
+    def test_local_adapter_init(self):
+        LocalFileAdapter()
+
+    def test_convert_md_file(self):
+        adapter = LocalFileAdapter()
+        md_converter = MdImageConverter(adapter=adapter)
+
+        md_file = MdFile(name="test.md")
+        md_converter.convert(md_file)
+
+    def test_convert_folder(self):
+        adapter = LocalFileAdapter()
+        md_converter = MdImageConverter(adapter=adapter)
+
+        folder = MdFolder(name="mds")
+        md_converter.convert(folder, output_directory="converted")
+
+
+class TestAliyunAdapter(TestCase):
+    def test_aliyun_adapter_init(self):
+        AliyunAdapter()
+
+    def test_convert_md_file(self):
+        adapter = AliyunAdapter()
+        md_converter = MdImageConverter(adapter=adapter)
+
+        md_file = MdFile(name="test.md")
+        md_converter.convert(md_file)
+
+    def test_convert_with_storage_prefix(self):
+        adapter = AliyunAdapter(storage_path_prefix="imarkdown")
+        md_converter = MdImageConverter(adapter=adapter)
+
+        md_file = MdFile(name="test.md")
+        md_converter.convert(md_file)
+
+    def test_convert_file(self):
+        adapter = AliyunAdapter()
+        md_converter = MdImageConverter(adapter=adapter)
+
+        md_folder = MdFolder(name="mds")
+        md_converter.convert(md_folder, output_directory="converted")
+
+    def test_local_to_remote(self):
+        adapter = LocalFileAdapter()
+        md_converter = MdImageConverter(adapter=adapter)
+        md_folder = MdFolder(name="mds")
+        md_converter.convert(md_folder, output_directory="local_mds")
+
+        adapter = AliyunAdapter()
+        md_converter = MdImageConverter(adapter=adapter)
+        md_folder = MdFolder(name="local_mds", image_type="local", image_directory="local_mds/images")
+        md_converter.convert(md_folder, output_directory="aliyun_converted")
```

### Comparing `imarkdown-1.1.2/tests/test_image_converter.py` & `imarkdown-1.2.1/tests/test_image_converter.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-import logging
-from unittest import TestCase
-
-from imarkdown.adapter import AliyunAdapter, LocalFileAdapter
-from imarkdown.constant import MdAdapterType
-from imarkdown.converter import MdImageConverter, BaseMdImageConverter
-from imarkdown.schema import MdFile, MdFolder
-
-logging.basicConfig(level=logging.DEBUG)
-logger = logging.getLogger(__name__)
-
-
-class TestBaseImageConverter(TestCase):
-    def test_base_usage(self):
-        # adapter = LocalFileAdapter()
-        adapter = AliyunAdapter()
-        converter = BaseMdImageConverter(adapter=adapter)
-        converter.convert(
-            "test.md",
-            image_local_storage_directory="mds/images",
-            output_md_directory="mds",
-            name_prefix="prefix_",
-            name_suffix="_converted",
-        )
-
-
-class TestImageConverter(TestCase):
-    def test_use_md_file(self):
-        adapter = LocalFileAdapter()
-        converter = MdImageConverter(adapter=adapter)
-
-        md_file = MdFile(name="test.md")
-        converter.convert(md_file)
-
-    def test_use_md_file_with_custom_name(self):
-        adapter = LocalFileAdapter()
-        converter = MdImageConverter(adapter=adapter)
-
-        md_file = MdFile(name="test.md")
-        converter.convert(md_file, name_prefix="prefix", name_suffix="_new")
-
-    def test_use_md_file_with_custom_image_path(self):
-        adapter = LocalFileAdapter()
-        converter = MdImageConverter(adapter=adapter)
-
-        md_file = MdFile(name="test.md", image_directory="custom_images")
-        converter.convert(md_file)
-
-    def test_use_md_folder(self):
-        adapter = LocalFileAdapter()
-        converter = MdImageConverter(adapter=adapter)
-
-        md_folder = MdFolder(name="mds")
-        converter.convert(md_folder, output_directory="converted")
-        for md_file in converter.md_medium_manager.md_files:
-            print(md_file.to_convert_params)
-
-    def test_last_adapter(self):
-        md_adapter = AliyunAdapter()
-        md_converter = MdImageConverter(adapter=md_adapter)
-        self.assertEqual(md_converter.adapter.name, MdAdapterType.Aliyun.value)
-        md_converter = MdImageConverter()
-        self.assertEqual(md_converter.adapter.name, MdAdapterType.Aliyun.value)
+import logging
+from unittest import TestCase
+
+from imarkdown.adapter import AliyunAdapter, LocalFileAdapter
+from imarkdown.constant import MdAdapterType
+from imarkdown.converter import MdImageConverter, BaseMdImageConverter
+from imarkdown.schema import MdFile, MdFolder
+
+logging.basicConfig(level=logging.DEBUG)
+logger = logging.getLogger(__name__)
+
+
+class TestBaseImageConverter(TestCase):
+    def test_base_usage(self):
+        # adapter = LocalFileAdapter()
+        adapter = AliyunAdapter()
+        converter = BaseMdImageConverter(adapter=adapter)
+        converter.convert(
+            "test.md",
+            image_local_storage_directory="mds/images",
+            output_md_directory="mds",
+            name_prefix="prefix_",
+            name_suffix="_converted",
+        )
+
+
+class TestImageConverter(TestCase):
+    def test_use_md_file(self):
+        adapter = LocalFileAdapter()
+        converter = MdImageConverter(adapter=adapter)
+
+        md_file = MdFile(name="test.md")
+        converter.convert(md_file)
+
+    def test_use_md_file_with_custom_name(self):
+        adapter = LocalFileAdapter()
+        converter = MdImageConverter(adapter=adapter)
+
+        md_file = MdFile(name="test.md")
+        converter.convert(md_file, name_prefix="prefix", name_suffix="_new")
+
+    def test_use_md_file_with_custom_image_path(self):
+        adapter = LocalFileAdapter()
+        converter = MdImageConverter(adapter=adapter)
+
+        md_file = MdFile(name="test.md", image_directory="custom_images")
+        converter.convert(md_file)
+
+    def test_use_md_folder(self):
+        adapter = LocalFileAdapter()
+        converter = MdImageConverter(adapter=adapter)
+
+        md_folder = MdFolder(name="mds")
+        converter.convert(md_folder, output_directory="converted")
+        for md_file in converter.md_medium_manager.md_files:
+            print(md_file.to_convert_params)
+
+    def test_last_adapter(self):
+        md_adapter = AliyunAdapter()
+        md_converter = MdImageConverter(adapter=md_adapter)
+        self.assertEqual(md_converter.adapter.name, MdAdapterType.Aliyun.value)
+        md_converter = MdImageConverter()
+        self.assertEqual(md_converter.adapter.name, MdAdapterType.Aliyun.value)
```

### Comparing `imarkdown-1.1.2/tests/test_md_file.py` & `imarkdown-1.2.1/tests/test_md_file.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-import logging
-from typing import List
-from unittest import TestCase
-
-from pydantic.error_wrappers import ValidationError
-
-from imarkdown.schema import MdFile, MdFolder, MdMediumManager
-
-logger = logging.getLogger(__name__)
-logging.basicConfig(level=logging.DEBUG)
-
-
-class TestMdFile(TestCase):
-    def test_md_file_initialization(self):
-        md_file = MdFile(name="test.md", image_type="remote")
-        logger.info(md_file.__dict__)
-
-        md_file = MdFile(name="test.md", image_type="local", image_directory="images")
-        logger.info(md_file.__dict__)
-
-        try:
-            MdFile(name="not_exist.md")
-            assert 1 == 0
-        except ValidationError as e:
-            pass
-
-        try:
-            MdFile(name="test.md", image_type="local")
-            assert 1 == 0
-        except ValidationError as e:
-            pass
-
-    def test_md_file_to_convert_params(self):
-        md_file = MdFile(name="test.md", image_type="remote")
-        params = md_file.to_convert_params
-        logger.info(params)
-
-    def test_md_folder_initialization(self):
-        md_folder = MdFolder(name="mds")
-        for node in md_folder.sub_nodes:
-            logger.info(f"{type(node)} {node.absolute_path_name}")
-
-        try:
-            MdFolder(name="mds", image_type="local")
-            assert 1 == 0
-        except ValidationError as e:
-            pass
-
-        md_folder = MdFolder(
-            name="mds/sub_mds", image_type="local", image_directory="mds\\images"
-        )
-        logger.info(md_folder.__dict__)
-
-
-class TestMdMediumManager(TestCase):
-    def test_get_all_files(self):
-        manager = MdMediumManager()
-        md_folder = MdFolder(name="single_mds", output_directory="converted")
-        md_files: List[MdFile] = manager.init_md_files([md_folder])
-        for md_file in md_files:
-            print(md_file.to_convert_params)
-
-    def test_update_config(self):
-        manager = MdMediumManager()
-        md_folder = MdFolder(name="mds")
-        manager.init_md_files([md_folder])
-        manager.update_config(output_directory="converted")
-        for md_file in manager.md_files:
-            print(md_file.to_convert_params)
+import logging
+from typing import List
+from unittest import TestCase
+
+from pydantic.error_wrappers import ValidationError
+
+from imarkdown.schema import MdFile, MdFolder, MdMediumManager
+
+logger = logging.getLogger(__name__)
+logging.basicConfig(level=logging.DEBUG)
+
+
+class TestMdFile(TestCase):
+    def test_md_file_initialization(self):
+        md_file = MdFile(name="test.md", image_type="remote")
+        logger.info(md_file.__dict__)
+
+        md_file = MdFile(name="test.md", image_type="local", image_directory="images")
+        logger.info(md_file.__dict__)
+
+        try:
+            MdFile(name="not_exist.md")
+            assert 1 == 0
+        except ValidationError as e:
+            pass
+
+        try:
+            MdFile(name="test.md", image_type="local")
+            assert 1 == 0
+        except ValidationError as e:
+            pass
+
+    def test_md_file_to_convert_params(self):
+        md_file = MdFile(name="test.md", image_type="remote")
+        params = md_file.to_convert_params
+        logger.info(params)
+
+    def test_md_folder_initialization(self):
+        md_folder = MdFolder(name="mds")
+        for node in md_folder.sub_nodes:
+            logger.info(f"{type(node)} {node.absolute_path_name}")
+
+        try:
+            MdFolder(name="mds", image_type="local")
+            assert 1 == 0
+        except ValidationError as e:
+            pass
+
+        md_folder = MdFolder(
+            name="mds/sub_mds", image_type="local", image_directory="mds\\images"
+        )
+        logger.info(md_folder.__dict__)
+
+
+class TestMdMediumManager(TestCase):
+    def test_get_all_files(self):
+        manager = MdMediumManager()
+        md_folder = MdFolder(name="single_mds", output_directory="converted")
+        md_files: List[MdFile] = manager.init_md_files([md_folder])
+        for md_file in md_files:
+            print(md_file.to_convert_params)
+
+    def test_update_config(self):
+        manager = MdMediumManager()
+        md_folder = MdFolder(name="mds")
+        manager.init_md_files([md_folder])
+        manager.update_config(output_directory="converted")
+        for md_file in manager.md_files:
+            print(md_file.to_convert_params)
```

### Comparing `imarkdown-1.1.2/tests/test_utils.py` & `imarkdown-1.2.1/tests/test_utils.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-import logging
-from unittest import TestCase
-
-from imarkdown.converter import supplementary_file_path, calculate_relative_path
-
-logging.basicConfig(level=logging.DEBUG)
-logger = logging.getLogger(__name__)
-
-
-class TestUtils(TestCase):
-    def test_supplementary_file_path(self):
-        a = supplementary_file_path("markdown.md")
-        b = supplementary_file_path("./markdown.md")
-        logger.info(f"<{a}> <{b}>")
-        self.assertEqual(a, b)
-        c = supplementary_file_path("../markdown.md")
-        logger.info(c)
-        d = supplementary_file_path("../../markdown.md")
-        logger.info(d)
-        e = supplementary_file_path("E:\\markdown.md")
-        logger.info(e)
-        f = supplementary_file_path("E:\\file")
-        logger.info(f)
-
-    def test_calculate_relative_path(self):
-        # same directory
-        image_storage_directory = "E:/project_hub/md-img-convert/tests/images/pic.png"
-        md_storage_directory = "E:/project_hub/md-img-convert/tests"
-        result = calculate_relative_path(image_storage_directory, md_storage_directory)
-        logger.info(result)
-        self.assertEqual(result, "./images/pic.png")
-
-        # image with deeper directory
-        image_storage_directory = (
-            "E:/project_hub/md-img-convert/tests/sub/images/pic.png"
-        )
-        md_storage_directory = "E:/project_hub/md-img-convert/tests/"
-        result = calculate_relative_path(image_storage_directory, md_storage_directory)
-        logger.info(result)
-        self.assertEqual(result, "./sub/images/pic.png")
-
-        # md with deeper directory
-        image_storage_directory = (
-            "E:/project_hub/md-img-convert/tests/converted/images/pic.png"
-        )
-        md_storage_directory = "E:/project_hub/md-img-convert/tests/converted/sub_mds2"
-        result = calculate_relative_path(image_storage_directory, md_storage_directory)
-        logger.info(result)
-        self.assertEqual(result, "../images/pic.png")
-
-        # md with deeper directory and file suffix
-        image_storage_directory = (
-            "E:/project_hub/md-img-convert/tests/converted/images/pic.png"
-        )
-        md_storage_directory = (
-            "E:/project_hub/md-img-convert/tests/converted/sub_mds/md.md"
-        )
-        result = calculate_relative_path(image_storage_directory, md_storage_directory)
-        logger.info(result)
-        self.assertEqual(result, "../images/pic.png")
-
-        # md with deeper directory than above
-        image_storage_directory = (
-            "E:/project_hub/md-img-convert/tests/converted/images/pic.png"
-        )
-        md_storage_directory = (
-            "E:/project_hub/md-img-convert/tests/converted/sub_mds/sub_sub_md"
-        )
-        result = calculate_relative_path(image_storage_directory, md_storage_directory)
-        logger.info(result)
-        self.assertEqual(result, "../../images/pic.png")
+import logging
+from unittest import TestCase
+
+from imarkdown.converter import supplementary_file_path, calculate_relative_path
+
+logging.basicConfig(level=logging.DEBUG)
+logger = logging.getLogger(__name__)
+
+
+class TestUtils(TestCase):
+    def test_supplementary_file_path(self):
+        a = supplementary_file_path("markdown.md")
+        b = supplementary_file_path("./markdown.md")
+        logger.info(f"<{a}> <{b}>")
+        self.assertEqual(a, b)
+        c = supplementary_file_path("../markdown.md")
+        logger.info(c)
+        d = supplementary_file_path("../../markdown.md")
+        logger.info(d)
+        e = supplementary_file_path("E:\\markdown.md")
+        logger.info(e)
+        f = supplementary_file_path("E:\\file")
+        logger.info(f)
+
+    def test_calculate_relative_path(self):
+        # same directory
+        image_storage_directory = "E:/project_hub/md-img-convert/tests/images/pic.png"
+        md_storage_directory = "E:/project_hub/md-img-convert/tests"
+        result = calculate_relative_path(image_storage_directory, md_storage_directory)
+        logger.info(result)
+        self.assertEqual(result, "./images/pic.png")
+
+        # image with deeper directory
+        image_storage_directory = (
+            "E:/project_hub/md-img-convert/tests/sub/images/pic.png"
+        )
+        md_storage_directory = "E:/project_hub/md-img-convert/tests/"
+        result = calculate_relative_path(image_storage_directory, md_storage_directory)
+        logger.info(result)
+        self.assertEqual(result, "./sub/images/pic.png")
+
+        # md with deeper directory
+        image_storage_directory = (
+            "E:/project_hub/md-img-convert/tests/converted/images/pic.png"
+        )
+        md_storage_directory = "E:/project_hub/md-img-convert/tests/converted/sub_mds2"
+        result = calculate_relative_path(image_storage_directory, md_storage_directory)
+        logger.info(result)
+        self.assertEqual(result, "../images/pic.png")
+
+        # md with deeper directory and file suffix
+        image_storage_directory = (
+            "E:/project_hub/md-img-convert/tests/converted/images/pic.png"
+        )
+        md_storage_directory = (
+            "E:/project_hub/md-img-convert/tests/converted/sub_mds/md.md"
+        )
+        result = calculate_relative_path(image_storage_directory, md_storage_directory)
+        logger.info(result)
+        self.assertEqual(result, "../images/pic.png")
+
+        # md with deeper directory than above
+        image_storage_directory = (
+            "E:/project_hub/md-img-convert/tests/converted/images/pic.png"
+        )
+        md_storage_directory = (
+            "E:/project_hub/md-img-convert/tests/converted/sub_mds/sub_sub_md"
+        )
+        result = calculate_relative_path(image_storage_directory, md_storage_directory)
+        logger.info(result)
+        self.assertEqual(result, "../../images/pic.png")
```

