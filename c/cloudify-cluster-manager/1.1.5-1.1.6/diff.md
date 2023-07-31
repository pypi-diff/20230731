# Comparing `tmp/cloudify-cluster-manager-1.1.5.tar.gz` & `tmp/cloudify-cluster-manager-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudify-cluster-manager-1.1.5.tar", last modified: Thu Jul 13 14:55:41 2023, max compression
+gzip compressed data, was "cloudify-cluster-manager-1.1.6.tar", last modified: Mon Jul 31 11:15:53 2023, max compression
```

## Comparing `cloudify-cluster-manager-1.1.5.tar` & `cloudify-cluster-manager-1.1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 14:55:41.943630 cloudify-cluster-manager-1.1.5/
--rw-r--r--   0 root         (0) root         (0)    11325 2023-07-13 14:55:22.000000 cloudify-cluster-manager-1.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-13 14:55:22.000000 cloudify-cluster-manager-1.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10230 2023-07-13 14:55:41.943630 cloudify-cluster-manager-1.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9991 2023-07-13 14:55:22.000000 cloudify-cluster-manager-1.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 14:55:41.943630 cloudify-cluster-manager-1.1.5/cfy_cluster_manager/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-13 14:55:22.000000 cloudify-cluster-manager-1.1.5/cfy_cluster_manager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 14:55:41.943630 cloudify-cluster-manager-1.1.5/cfy_cluster_manager/cfy_cluster_config_files/
--rw-r--r--   0 root         (0) root         (0)     6581 2023-07-13 14:55:22.000000 cloudify-cluster-manager-1.1.5/cfy_cluster_manager/cfy_cluster_config_files/cfy_nine_nodes_cluster_config.yaml
--rw-r--r--   0 root         (0) root         (0)     5979 2023-07-13 14:55:22.000000 cloudify-cluster-manager-1.1.5/cfy_cluster_manager/cfy_cluster_config_files/cfy_nine_nodes_external_db_cluster_config.yaml
--rw-r--r--   0 root         (0) root         (0)     3919 2023-07-13 14:55:22.000000 cloudify-cluster-manager-1.1.5/cfy_cluster_manager/cfy_cluster_config_files/cfy_three_nodes_cluster_config.yaml
--rw-r--r--   0 root         (0) root         (0)     4666 2023-07-13 14:55:22.000000 cloudify-cluster-manager-1.1.5/cfy_cluster_manager/cfy_cluster_config_files/cfy_three_nodes_external_db_cluster_config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 14:55:41.943630 cloudify-cluster-manager-1.1.5/cfy_cluster_manager/config_files_templates/
--rw-r--r--   0 root         (0) root         (0)     2343 2023-07-13 14:55:22.000000 cloudify-cluster-manager-1.1.5/cfy_cluster_manager/config_files_templates/manager_config.yaml
--rw-r--r--   0 root         (0) root         (0)     1263 2023-07-13 14:55:22.000000 cloudify-cluster-manager-1.1.5/cfy_cluster_manager/config_files_templates/postgresql_config.yaml
--rw-r--r--   0 root         (0) root         (0)     1066 2023-07-13 14:55:22.000000 cloudify-cluster-manager-1.1.5/cfy_cluster_manager/config_files_templates/rabbitmq_config.yaml
--rw-r--r--   0 root         (0) root         (0)     1199 2023-07-13 14:55:22.000000 cloudify-cluster-manager-1.1.5/cfy_cluster_manager/logger.py
--rw-r--r--   0 root         (0) root         (0)    49817 2023-07-13 14:55:22.000000 cloudify-cluster-manager-1.1.5/cfy_cluster_manager/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 14:55:41.943630 cloudify-cluster-manager-1.1.5/cfy_cluster_manager/scripts/
--rw-r--r--   0 root         (0) root         (0)     8778 2023-07-13 14:55:22.000000 cloudify-cluster-manager-1.1.5/cfy_cluster_manager/scripts/create_installation_files.py
--rw-r--r--   0 root         (0) root         (0)    11541 2023-07-13 14:55:22.000000 cloudify-cluster-manager-1.1.5/cfy_cluster_manager/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 14:55:41.943630 cloudify-cluster-manager-1.1.5/cloudify_cluster_manager.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10230 2023-07-13 14:55:41.000000 cloudify-cluster-manager-1.1.5/cloudify_cluster_manager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1043 2023-07-13 14:55:41.000000 cloudify-cluster-manager-1.1.5/cloudify_cluster_manager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 14:55:41.000000 cloudify-cluster-manager-1.1.5/cloudify_cluster_manager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-07-13 14:55:41.000000 cloudify-cluster-manager-1.1.5/cloudify_cluster_manager.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-07-13 14:55:41.000000 cloudify-cluster-manager-1.1.5/cloudify_cluster_manager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-13 14:55:41.000000 cloudify-cluster-manager-1.1.5/cloudify_cluster_manager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 14:55:41.943630 cloudify-cluster-manager-1.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1541 2023-07-13 14:55:22.000000 cloudify-cluster-manager-1.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:15:53.004176 cloudify-cluster-manager-1.1.6/
+-rw-r--r--   0 root         (0) root         (0)    11325 2023-07-31 11:15:34.000000 cloudify-cluster-manager-1.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-31 11:15:34.000000 cloudify-cluster-manager-1.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10523 2023-07-31 11:15:53.004176 cloudify-cluster-manager-1.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10284 2023-07-31 11:15:34.000000 cloudify-cluster-manager-1.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:15:53.004176 cloudify-cluster-manager-1.1.6/cfy_cluster_manager/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 11:15:34.000000 cloudify-cluster-manager-1.1.6/cfy_cluster_manager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:15:53.004176 cloudify-cluster-manager-1.1.6/cfy_cluster_manager/cfy_cluster_config_files/
+-rw-r--r--   0 root         (0) root         (0)     6581 2023-07-31 11:15:34.000000 cloudify-cluster-manager-1.1.6/cfy_cluster_manager/cfy_cluster_config_files/cfy_nine_nodes_cluster_config.yaml
+-rw-r--r--   0 root         (0) root         (0)     5979 2023-07-31 11:15:34.000000 cloudify-cluster-manager-1.1.6/cfy_cluster_manager/cfy_cluster_config_files/cfy_nine_nodes_external_db_cluster_config.yaml
+-rw-r--r--   0 root         (0) root         (0)     3919 2023-07-31 11:15:34.000000 cloudify-cluster-manager-1.1.6/cfy_cluster_manager/cfy_cluster_config_files/cfy_three_nodes_cluster_config.yaml
+-rw-r--r--   0 root         (0) root         (0)     4666 2023-07-31 11:15:34.000000 cloudify-cluster-manager-1.1.6/cfy_cluster_manager/cfy_cluster_config_files/cfy_three_nodes_external_db_cluster_config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:15:53.004176 cloudify-cluster-manager-1.1.6/cfy_cluster_manager/config_files_templates/
+-rw-r--r--   0 root         (0) root         (0)     2369 2023-07-31 11:15:34.000000 cloudify-cluster-manager-1.1.6/cfy_cluster_manager/config_files_templates/manager_config.yaml
+-rw-r--r--   0 root         (0) root         (0)     1263 2023-07-31 11:15:34.000000 cloudify-cluster-manager-1.1.6/cfy_cluster_manager/config_files_templates/postgresql_config.yaml
+-rw-r--r--   0 root         (0) root         (0)     1066 2023-07-31 11:15:34.000000 cloudify-cluster-manager-1.1.6/cfy_cluster_manager/config_files_templates/rabbitmq_config.yaml
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-07-31 11:15:34.000000 cloudify-cluster-manager-1.1.6/cfy_cluster_manager/logger.py
+-rw-r--r--   0 root         (0) root         (0)    50494 2023-07-31 11:15:34.000000 cloudify-cluster-manager-1.1.6/cfy_cluster_manager/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:15:53.004176 cloudify-cluster-manager-1.1.6/cfy_cluster_manager/scripts/
+-rw-r--r--   0 root         (0) root         (0)     8778 2023-07-31 11:15:34.000000 cloudify-cluster-manager-1.1.6/cfy_cluster_manager/scripts/create_installation_files.py
+-rw-r--r--   0 root         (0) root         (0)    11541 2023-07-31 11:15:34.000000 cloudify-cluster-manager-1.1.6/cfy_cluster_manager/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:15:53.004176 cloudify-cluster-manager-1.1.6/cloudify_cluster_manager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10523 2023-07-31 11:15:52.000000 cloudify-cluster-manager-1.1.6/cloudify_cluster_manager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-07-31 11:15:52.000000 cloudify-cluster-manager-1.1.6/cloudify_cluster_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 11:15:52.000000 cloudify-cluster-manager-1.1.6/cloudify_cluster_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-31 11:15:52.000000 cloudify-cluster-manager-1.1.6/cloudify_cluster_manager.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-31 11:15:52.000000 cloudify-cluster-manager-1.1.6/cloudify_cluster_manager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-31 11:15:52.000000 cloudify-cluster-manager-1.1.6/cloudify_cluster_manager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 11:15:53.004176 cloudify-cluster-manager-1.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1541 2023-07-31 11:15:34.000000 cloudify-cluster-manager-1.1.6/setup.py
```

### Comparing `cloudify-cluster-manager-1.1.5/LICENSE` & `cloudify-cluster-manager-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudify-cluster-manager-1.1.5/PKG-INFO` & `cloudify-cluster-manager-1.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudify-cluster-manager
-Version: 1.1.5
+Version: 1.1.6
 Summary: Install a Cloudify cluster
 Author: Cloudify
 Author-email: cosmo-admin@cloudify.co
 License: LICENSE
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -54,35 +54,38 @@
 ### Installing the Cloudify Cluster Manager package
 You can run the Cloudify Cluster Manager package from one of the cluster's VMs, or from a different host in the
 cluster network. You can install the package either by using an RPM or by using `pip install`:
 
 #### Installing using an RPM
 Run the following command:
 ```bash
-sudo yum install -y http://repository.cloudifysource.org/cloudify/cloudify-cluster-manager/1.1.5/ga-release/cloudify-cluster-manager-1.1.5-ga.el7.x86_64.rpm
+sudo yum install -y http://repository.cloudifysource.org/cloudify/cloudify-cluster-manager/1.1.6/ga-release/cloudify-cluster-manager-1.1.6-ga.el7.x86_64.rpm
 
 # Installing haveged to avoid hanging executions
-sudo yum install -y epel-release
+curl https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm -o epel-release-latest-7.noarch.rpm
+sudo yum install -y epel-release-latest-7.noarch.rpm
 sudo yum install -y haveged
 sudo systemctl start haveged
 ```
 
 **NOTE:** On RHEL 8, install haveged as follows instead:
 ```bash
 curl https://dl.fedoraproject.org/pub/epel/epel-release-latest-8.noarch.rpm -o epel-release-latest-8.noarch.rpm
 sudo yum install -y epel-release-latest-8.noarch.rpm
 sudo yum install -y haveged
+sudo systemctl start haveged
 ```
 
 #### Installing using pip install
 ```bash
 pip install cloudify-cluster-manager
 
 # Installing haveged to avoid hanging executions
-sudo yum install -y epel-release
+curl https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm -o epel-release-latest-7.noarch.rpm
+sudo yum install -y epel-release-latest-7.noarch.rpm
 sudo yum install -y haveged
 sudo systemctl start haveged
 ```
 
 
 &nbsp;
 ## Using the Cloudify Cluster Manager package
```

### Comparing `cloudify-cluster-manager-1.1.5/README.md` & `cloudify-cluster-manager-1.1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -44,35 +44,38 @@
 ### Installing the Cloudify Cluster Manager package
 You can run the Cloudify Cluster Manager package from one of the cluster's VMs, or from a different host in the
 cluster network. You can install the package either by using an RPM or by using `pip install`:
 
 #### Installing using an RPM
 Run the following command:
 ```bash
-sudo yum install -y http://repository.cloudifysource.org/cloudify/cloudify-cluster-manager/1.1.5/ga-release/cloudify-cluster-manager-1.1.5-ga.el7.x86_64.rpm
+sudo yum install -y http://repository.cloudifysource.org/cloudify/cloudify-cluster-manager/1.1.6/ga-release/cloudify-cluster-manager-1.1.6-ga.el7.x86_64.rpm
 
 # Installing haveged to avoid hanging executions
-sudo yum install -y epel-release
+curl https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm -o epel-release-latest-7.noarch.rpm
+sudo yum install -y epel-release-latest-7.noarch.rpm
 sudo yum install -y haveged
 sudo systemctl start haveged
 ```
 
 **NOTE:** On RHEL 8, install haveged as follows instead:
 ```bash
 curl https://dl.fedoraproject.org/pub/epel/epel-release-latest-8.noarch.rpm -o epel-release-latest-8.noarch.rpm
 sudo yum install -y epel-release-latest-8.noarch.rpm
 sudo yum install -y haveged
+sudo systemctl start haveged
 ```
 
 #### Installing using pip install
 ```bash
 pip install cloudify-cluster-manager
 
 # Installing haveged to avoid hanging executions
-sudo yum install -y epel-release
+curl https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm -o epel-release-latest-7.noarch.rpm
+sudo yum install -y epel-release-latest-7.noarch.rpm
 sudo yum install -y haveged
 sudo systemctl start haveged
 ```
 
 
 &nbsp;
 ## Using the Cloudify Cluster Manager package
```

### Comparing `cloudify-cluster-manager-1.1.5/cfy_cluster_manager/cfy_cluster_config_files/cfy_nine_nodes_cluster_config.yaml` & `cloudify-cluster-manager-1.1.6/cfy_cluster_manager/cfy_cluster_config_files/cfy_nine_nodes_cluster_config.yaml`

 * *Files identical despite different names*

### Comparing `cloudify-cluster-manager-1.1.5/cfy_cluster_manager/cfy_cluster_config_files/cfy_nine_nodes_external_db_cluster_config.yaml` & `cloudify-cluster-manager-1.1.6/cfy_cluster_manager/cfy_cluster_config_files/cfy_nine_nodes_external_db_cluster_config.yaml`

 * *Files identical despite different names*

### Comparing `cloudify-cluster-manager-1.1.5/cfy_cluster_manager/cfy_cluster_config_files/cfy_three_nodes_cluster_config.yaml` & `cloudify-cluster-manager-1.1.6/cfy_cluster_manager/cfy_cluster_config_files/cfy_three_nodes_cluster_config.yaml`

 * *Files identical despite different names*

### Comparing `cloudify-cluster-manager-1.1.5/cfy_cluster_manager/cfy_cluster_config_files/cfy_three_nodes_external_db_cluster_config.yaml` & `cloudify-cluster-manager-1.1.6/cfy_cluster_manager/cfy_cluster_config_files/cfy_three_nodes_external_db_cluster_config.yaml`

 * *Files identical despite different names*

### Comparing `cloudify-cluster-manager-1.1.5/cfy_cluster_manager/config_files_templates/manager_config.yaml` & `cloudify-cluster-manager-1.1.6/cfy_cluster_manager/config_files_templates/manager_config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -62,18 +62,18 @@
   external_cert_path: {{ node.cert_path }}
   external_key_path: {{ node.key_path }}
   external_ca_cert_path: {{ ca_path }}
   external_ca_key_path: {{ ca_key_path }}
   {%-endif %}
   internal_cert_path: {{ node.cert_path }}
   internal_key_path: {{ node.key_path }}
-  postgresql_client_cert_path: {{ node.cert_path }}
-  postgresql_client_key_path: {{ node.key_path }}
-  postgresql_superuser_client_cert_path: {{ node.cert_path }}
-  postgresql_superuser_client_key_path: {{ node.key_path }}
+  postgresql_client_cert_path: {{ db_client_cert_path }}
+  postgresql_client_key_path: {{ db_client_key_path }}
+  postgresql_superuser_client_cert_path: {{ db_client_su_cert_path }}
+  postgresql_superuser_client_key_path: {{ db_client_su_key_path }}
   ca_cert_path: {{ ca_path }}
   ca_key_path: {{ ca_key_path }}
 
 prometheus:
   credentials:
     username: {{ creds.prometheus.username }}
     password: {{ creds.prometheus.password }}
```

### Comparing `cloudify-cluster-manager-1.1.5/cfy_cluster_manager/config_files_templates/postgresql_config.yaml` & `cloudify-cluster-manager-1.1.6/cfy_cluster_manager/config_files_templates/postgresql_config.yaml`

 * *Files identical despite different names*

### Comparing `cloudify-cluster-manager-1.1.5/cfy_cluster_manager/config_files_templates/rabbitmq_config.yaml` & `cloudify-cluster-manager-1.1.6/cfy_cluster_manager/config_files_templates/rabbitmq_config.yaml`

 * *Files identical despite different names*

### Comparing `cloudify-cluster-manager-1.1.5/cfy_cluster_manager/logger.py` & `cloudify-cluster-manager-1.1.6/cfy_cluster_manager/logger.py`

 * *Files identical despite different names*

### Comparing `cloudify-cluster-manager-1.1.5/cfy_cluster_manager/main.py` & `cloudify-cluster-manager-1.1.6/cfy_cluster_manager/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,18 @@
 CERTS_DIR = join(CLUSTER_INSTALL_DIR, CERTS_DIR_NAME)
 CONFIG_FILES_DIR = join(CLUSTER_INSTALL_DIR, CONFIG_FILES)
 
 CA_PATH = join(CERTS_DIR, 'ca.pem')
 CA_KEY_PATH = join(CERTS_DIR, 'ca.key')
 EXTERNAL_DB_CA_PATH = join(CERTS_DIR, 'external_db_ca.pem')
 LDAP_CA_PATH = join(CERTS_DIR, 'ldap_ca.pem')
+DB_CLIENT_CERT_PATH = join(CERTS_DIR, 'cloudify.crt')
+DB_CLIENT_KEY_PATH = join(CERTS_DIR, 'cloudify.key')
+DB_CLIENT_SU_CERT_PATH = join(CERTS_DIR, 'postgres.crt')
+DB_CLIENT_SU_KEY_PATH = join(CERTS_DIR, 'postgres.key')
 
 CREDENTIALS_FILE_PATH = join(os.getcwd(), 'secret_credentials.yaml')
 CLUSTER_CONFIG_FILES_DIR = pkg_resources.resource_filename(
     'cfy_cluster_manager', 'cfy_cluster_config_files')
 CLUSTER_CONFIG_FILE_NAME = 'cfy_cluster_config.yaml'
 CLUSTER_INSTALL_CONFIG_PATH = join(os.getcwd(), CLUSTER_CONFIG_FILE_NAME)
 
@@ -121,14 +125,20 @@
 
 def _generate_certs(instances_dict):
     logger.info('Generating certificates')
     for instances_list in instances_dict.values():
         for instance in instances_list:
             _generate_instance_certificate(instance)
     copy(join(CFY_CERTS_PATH, 'ca.crt'), join(CFY_CERTS_PATH, 'ca.pem'))
+
+    # Client cert requires DB user as its CN
+    run(['cfy_manager', 'generate-test-cert', '-s', 'cloudify'])
+    # Client superuser cert requires DB superuser as its CN
+    run(['cfy_manager', 'generate-test-cert', '-s', 'postgres'])
+
     if not exists(CERTS_DIR):
         os.mkdir(CERTS_DIR)
     copy(join(CFY_CERTS_PATH, '.'), CERTS_DIR)
     shutil.rmtree(CFY_CERTS_PATH)
 
 
 def _get_postgresql_cluster_members(postgresql_instances):
@@ -212,14 +222,18 @@
         if exists(CA_KEY_PATH):
             ca_key_path = CA_KEY_PATH
         rendered_data = template.render(
             node=node,
             creds=credentials,
             ca_path=CA_PATH,
             ca_key_path=ca_key_path,
+            db_client_cert_path=DB_CLIENT_CERT_PATH,
+            db_client_key_path=DB_CLIENT_KEY_PATH,
+            db_client_su_cert_path=DB_CLIENT_SU_CERT_PATH,
+            db_client_su_key_path=DB_CLIENT_SU_KEY_PATH,
             license_path=join(CLUSTER_INSTALL_DIR, 'license.yaml'),
             load_balancer_ip=load_balancer_ip,
             rabbitmq_cluster=_get_rabbitmq_cluster_members(
                 instances_dict['rabbitmq'], load_balancer_ip),
             postgresql_cluster={} if external_db_config else
             _get_postgresql_cluster_members(instances_dict['postgresql']),
             external_db_configuration=external_db_config,
```

### Comparing `cloudify-cluster-manager-1.1.5/cfy_cluster_manager/scripts/create_installation_files.py` & `cloudify-cluster-manager-1.1.6/cfy_cluster_manager/scripts/create_installation_files.py`

 * *Files identical despite different names*

### Comparing `cloudify-cluster-manager-1.1.5/cfy_cluster_manager/utils.py` & `cloudify-cluster-manager-1.1.6/cfy_cluster_manager/utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-cluster-manager-1.1.5/cloudify_cluster_manager.egg-info/PKG-INFO` & `cloudify-cluster-manager-1.1.6/cloudify_cluster_manager.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudify-cluster-manager
-Version: 1.1.5
+Version: 1.1.6
 Summary: Install a Cloudify cluster
 Author: Cloudify
 Author-email: cosmo-admin@cloudify.co
 License: LICENSE
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -54,35 +54,38 @@
 ### Installing the Cloudify Cluster Manager package
 You can run the Cloudify Cluster Manager package from one of the cluster's VMs, or from a different host in the
 cluster network. You can install the package either by using an RPM or by using `pip install`:
 
 #### Installing using an RPM
 Run the following command:
 ```bash
-sudo yum install -y http://repository.cloudifysource.org/cloudify/cloudify-cluster-manager/1.1.5/ga-release/cloudify-cluster-manager-1.1.5-ga.el7.x86_64.rpm
+sudo yum install -y http://repository.cloudifysource.org/cloudify/cloudify-cluster-manager/1.1.6/ga-release/cloudify-cluster-manager-1.1.6-ga.el7.x86_64.rpm
 
 # Installing haveged to avoid hanging executions
-sudo yum install -y epel-release
+curl https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm -o epel-release-latest-7.noarch.rpm
+sudo yum install -y epel-release-latest-7.noarch.rpm
 sudo yum install -y haveged
 sudo systemctl start haveged
 ```
 
 **NOTE:** On RHEL 8, install haveged as follows instead:
 ```bash
 curl https://dl.fedoraproject.org/pub/epel/epel-release-latest-8.noarch.rpm -o epel-release-latest-8.noarch.rpm
 sudo yum install -y epel-release-latest-8.noarch.rpm
 sudo yum install -y haveged
+sudo systemctl start haveged
 ```
 
 #### Installing using pip install
 ```bash
 pip install cloudify-cluster-manager
 
 # Installing haveged to avoid hanging executions
-sudo yum install -y epel-release
+curl https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm -o epel-release-latest-7.noarch.rpm
+sudo yum install -y epel-release-latest-7.noarch.rpm
 sudo yum install -y haveged
 sudo systemctl start haveged
 ```
 
 
 &nbsp;
 ## Using the Cloudify Cluster Manager package
```

### Comparing `cloudify-cluster-manager-1.1.5/cloudify_cluster_manager.egg-info/SOURCES.txt` & `cloudify-cluster-manager-1.1.6/cloudify_cluster_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudify-cluster-manager-1.1.5/setup.py` & `cloudify-cluster-manager-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         return f.read()
 
 
 setup(
     name='cloudify-cluster-manager',
     long_description=get_readme_contents(),
     long_description_content_type='text/markdown',
-    version='1.1.5',
+    version='1.1.6',
     author='Cloudify',
     author_email='cosmo-admin@cloudify.co',
     packages=['cfy_cluster_manager'],
     include_package_data=True,
     license='LICENSE',
     description="Install a Cloudify cluster",
     entry_points={
```

