# Comparing `tmp/flowcontainer-7.1.tar.gz` & `tmp/flowcontainer-7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\flowcontainer-7.1.tar", last modified: Tue Jun  6 07:51:32 2023, max compression
+gzip compressed data, was "dist\flowcontainer-7.2.tar", last modified: Mon Jul 31 15:25:51 2023, max compression
```

## Comparing `flowcontainer-7.1.tar` & `flowcontainer-7.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 07:51:32.000000 flowcontainer-7.1/
-drwxrwxrwx   0        0        0        0 2023-06-06 07:51:32.000000 flowcontainer-7.1/flowcontainer/
--rw-rw-rw-   0        0        0     2860 2023-06-06 05:21:12.000000 flowcontainer-7.1/flowcontainer/extractor.py
--rw-rw-rw-   0        0        0     9052 2022-12-12 10:32:32.000000 flowcontainer-7.1/flowcontainer/flows.py
--rw-rw-rw-   0        0        0     1292 2023-04-16 15:46:47.000000 flowcontainer-7.1/flowcontainer/flow_generator.py
--rw-rw-rw-   0        0        0     4048 2022-12-10 13:25:03.000000 flowcontainer-7.1/flowcontainer/network_destination.py
--rw-rw-rw-   0        0        0    11795 2023-03-30 03:33:32.000000 flowcontainer-7.1/flowcontainer/reader.py
--rw-rw-rw-   0        0        0     1768 2023-06-06 07:50:05.000000 flowcontainer-7.1/flowcontainer/split_pcap.py
--rw-rw-rw-   0        0        0       50 2022-12-10 13:25:03.000000 flowcontainer-7.1/flowcontainer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:51:32.000000 flowcontainer-7.1/flowcontainer.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-06 07:51:32.000000 flowcontainer-7.1/flowcontainer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1504 2023-06-06 07:51:32.000000 flowcontainer-7.1/flowcontainer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2023-06-06 07:51:32.000000 flowcontainer-7.1/flowcontainer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       14 2023-06-06 07:51:32.000000 flowcontainer-7.1/flowcontainer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1504 2023-06-06 07:51:32.000000 flowcontainer-7.1/PKG-INFO
--rw-rw-rw-   0        0        0    18176 2021-03-21 05:33:11.000000 flowcontainer-7.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 07:51:32.000000 flowcontainer-7.1/setup.cfg
--rw-rw-rw-   0        0        0     1466 2023-06-04 08:26:24.000000 flowcontainer-7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:25:51.000000 flowcontainer-7.2/
+drwxrwxrwx   0        0        0        0 2023-07-31 15:25:51.000000 flowcontainer-7.2/flowcontainer/
+-rw-rw-rw-   0        0        0     2860 2023-06-06 05:21:12.000000 flowcontainer-7.2/flowcontainer/extractor.py
+-rw-rw-rw-   0        0        0     9052 2022-12-12 10:32:32.000000 flowcontainer-7.2/flowcontainer/flows.py
+-rw-rw-rw-   0        0        0     1292 2023-04-16 15:46:47.000000 flowcontainer-7.2/flowcontainer/flow_generator.py
+-rw-rw-rw-   0        0        0     4048 2022-12-10 13:25:03.000000 flowcontainer-7.2/flowcontainer/network_destination.py
+-rw-rw-rw-   0        0        0    11726 2023-07-30 22:50:55.000000 flowcontainer-7.2/flowcontainer/reader.py
+-rw-rw-rw-   0        0        0     1768 2023-06-06 07:50:05.000000 flowcontainer-7.2/flowcontainer/split_pcap.py
+-rw-rw-rw-   0        0        0       50 2022-12-10 13:25:03.000000 flowcontainer-7.2/flowcontainer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:25:51.000000 flowcontainer-7.2/flowcontainer.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-31 15:25:50.000000 flowcontainer-7.2/flowcontainer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1366 2023-07-31 15:25:50.000000 flowcontainer-7.2/flowcontainer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-07-31 15:25:50.000000 flowcontainer-7.2/flowcontainer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       14 2023-07-31 15:25:50.000000 flowcontainer-7.2/flowcontainer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2023-07-30 22:49:46.000000 flowcontainer-7.2/LICENSE
+-rw-rw-rw-   0        0        0     1366 2023-07-31 15:25:51.000000 flowcontainer-7.2/PKG-INFO
+-rw-rw-rw-   0        0        0    18176 2021-03-21 05:33:11.000000 flowcontainer-7.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-31 15:25:51.000000 flowcontainer-7.2/setup.cfg
+-rw-rw-rw-   0        0        0     1531 2023-07-30 22:52:40.000000 flowcontainer-7.2/setup.py
```

### Comparing `flowcontainer-7.1/flowcontainer/extractor.py` & `flowcontainer-7.2/flowcontainer/extractor.py`

 * *Files identical despite different names*

### Comparing `flowcontainer-7.1/flowcontainer/flows.py` & `flowcontainer-7.2/flowcontainer/flows.py`

 * *Files identical despite different names*

### Comparing `flowcontainer-7.1/flowcontainer/flow_generator.py` & `flowcontainer-7.2/flowcontainer/flow_generator.py`

 * *Files identical despite different names*

### Comparing `flowcontainer-7.1/flowcontainer/network_destination.py` & `flowcontainer-7.2/flowcontainer/network_destination.py`

 * *Files identical despite different names*

### Comparing `flowcontainer-7.1/flowcontainer/reader.py` & `flowcontainer-7.2/flowcontainer/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,15 @@
                    "-e", "tcp.dstport",
                    "-e", "udp.dstport", #only output one line
                    "-e", "ip.len",
                    "-e", "ipv6.plen",
                    '-e', "tcp.len",
                    "-e", "udp.length",   #only output one line,
                    "-e", 'ip.id',
-                   "-2","-R", "ip or ipv6 and not icmp and not tcp.analysis.retransmission and not tcp.analysis.out_of_order and not tcp.analysis.duplicate_ack and not mdns and not ssdp{0}"]
+                   "-2","-R", "ip or ipv6 and not icmp and not tcp.analysis.retransmission and not mdns and not ssdp{0}"]
         else:
             command = ["tshark", "-r", path, "-Tfields", "-E", "separator=`",
                    "-e", "frame.time_epoch",
                    "-e", "tcp.stream",
                    "-e", "udp.stream", #only output one line
                    "-e", "ip.proto",
                    "-e", "ipv6.nxt",  ##only output one line,
```

### Comparing `flowcontainer-7.1/flowcontainer/split_pcap.py` & `flowcontainer-7.2/flowcontainer/split_pcap.py`

 * *Files identical despite different names*

### Comparing `flowcontainer-7.1/flowcontainer.egg-info/PKG-INFO` & `flowcontainer-7.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,37 @@
-Metadata-Version: 2.1
-Name: flowcontainer
-Version: 7.1
-Summary: A python lib to parse traffic flow information from pcaps
-Home-page: https://github.com/jmhIcoding/flowcontainer
-Author: Minghao Jiang
-Author-email: jiangminghao@iie.ac.cn
-License: UNKNOWN
-Description: 
-        A python lib to parse traffic flow information from pcaps.
-        
-        Homepage : https://github.com/jmhIcoding/flowcontainer.
-        
-        Fix bugs:
-        
-        	 set the default filter string to be `tcp or udp or gre`.
-        
-        	 update help information for errors. 
-        
-        	 supports ipv6 parse. 
-        
-        	 fix separator bugs, replace separator from '+' to '`'  
-        
-        	 fix separator bugs, for http payload, the separator char would separate the payload wrongly.  
-        
-        	 support extract the extended protocol name, e.g. TLSv1, TLSv2, IPSEC etc. 
-        
-        	 fix http payload bugs. 
-        
-        	 2023-03-30: check the version of wireshark, ensure the version is not greater than 4.0.0. 
-        
-        	 20203-4-16: fix the bugs of separating flow into multi-flows due to the application protocol. 
-        
-        	 v7.x : 2023-06-05: support load and parse very large pcap file. 
-        
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
+#coding:utf8
+__author__ = 'dk'
+import setuptools
+long_desp = \
+'''
+A python lib to parse traffic flow information from pcaps.\n
+Homepage : https://github.com/jmhIcoding/flowcontainer.\n
+Fix bugs:\n
+\t set the default filter string to be `tcp or udp or gre`.\n
+\t update help information for errors. \n
+\t supports ipv6 parse. \n
+\t fix separator bugs, replace separator from '+' to '`'  \n
+\t fix separator bugs, for http payload, the separator char would separate the payload wrongly.  \n
+\t support extract the extended protocol name, e.g. TLSv1, TLSv2, IPSEC etc. \n
+\t fix http payload bugs. \n
+\t 2023-03-30: check the version of wireshark, ensure the version is not greater than 4.0.0. \n
+\t 20203-4-16: fix the bugs of separating flow into multi-flows due to the application protocol. \n
+\t v7.1 : 2023-06-05: support load and parse very large pcap file. \n
+\t v7.2 : 2023-07-13: fixed the TCP dupack bugs for TLS/SSL. \n
+'''
+
+setuptools.setup(
+    name="flowcontainer",
+    version="7.2",
+    author="Minghao Jiang",
+    author_email="jiangminghao@iie.ac.cn",
+    description="A python lib to parse traffic flow information from pcaps",
+    url="https://github.com/jmhIcoding/flowcontainer",
+    long_description=long_desp,
+    long_description_content_type="text/markdown",
+    packages=setuptools.find_packages(),
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+)
```

### Comparing `flowcontainer-7.1/PKG-INFO` & `flowcontainer-7.2/flowcontainer.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 Metadata-Version: 2.1
 Name: flowcontainer
-Version: 7.1
+Version: 7.2
 Summary: A python lib to parse traffic flow information from pcaps
 Home-page: https://github.com/jmhIcoding/flowcontainer
 Author: Minghao Jiang
 Author-email: jiangminghao@iie.ac.cn
 License: UNKNOWN
-Description: 
-        A python lib to parse traffic flow information from pcaps.
-        
-        Homepage : https://github.com/jmhIcoding/flowcontainer.
-        
-        Fix bugs:
-        
-        	 set the default filter string to be `tcp or udp or gre`.
-        
-        	 update help information for errors. 
-        
-        	 supports ipv6 parse. 
-        
-        	 fix separator bugs, replace separator from '+' to '`'  
-        
-        	 fix separator bugs, for http payload, the separator char would separate the payload wrongly.  
-        
-        	 support extract the extended protocol name, e.g. TLSv1, TLSv2, IPSEC etc. 
-        
-        	 fix http payload bugs. 
-        
-        	 2023-03-30: check the version of wireshark, ensure the version is not greater than 4.0.0. 
-        
-        	 20203-4-16: fix the bugs of separating flow into multi-flows due to the application protocol. 
-        
-        	 v7.x : 2023-06-05: support load and parse very large pcap file. 
-        
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+A python lib to parse traffic flow information from pcaps.
+
+Homepage : https://github.com/jmhIcoding/flowcontainer.
+
+Fix bugs:
+
+	 set the default filter string to be `tcp or udp or gre`.
+
+	 update help information for errors. 
+
+	 supports ipv6 parse. 
+
+	 fix separator bugs, replace separator from '+' to '`'  
+
+	 fix separator bugs, for http payload, the separator char would separate the payload wrongly.  
+
+	 support extract the extended protocol name, e.g. TLSv1, TLSv2, IPSEC etc. 
+
+	 fix http payload bugs. 
+
+	 2023-03-30: check the version of wireshark, ensure the version is not greater than 4.0.0. 
+
+	 20203-4-16: fix the bugs of separating flow into multi-flows due to the application protocol. 
+
+	 v7.1 : 2023-06-05: support load and parse very large pcap file. 
+
+	 v7.2 : 2023-07-13: fixed the TCP dupack bugs for TLS/SSL. 
+
+
+
```

### Comparing `flowcontainer-7.1/README.md` & `flowcontainer-7.2/README.md`

 * *Files identical despite different names*

