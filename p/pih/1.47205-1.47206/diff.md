# Comparing `tmp/pih-1.47205.tar.gz` & `tmp/pih-1.47206.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.47205.tar", last modified: Fri Jul 28 13:42:35 2023, max compression
+gzip compressed data, was "pih-1.47206.tar", last modified: Mon Jul 31 09:00:30 2023, max compression
```

## Comparing `pih-1.47205.tar` & `pih-1.47206.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 13:42:34.173255 pih-1.47205/
-drwxrwxrwx   0        0        0        0 2023-07-28 13:42:34.471645 pih-1.47205/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-1.47205/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0   165201 2023-07-28 09:30:54.000000 pih-1.47205/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-1.47205/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9431 2023-07-28 13:39:51.000000 pih-1.47205/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-1.47205/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      261 2023-07-28 13:42:35.440373 pih-1.47205/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 13:42:35.206009 pih-1.47205/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.47205/pih/__init__.py
--rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.47205/pih/collection.py
--rw-rw-rw-   0        0        0    61076 2023-07-27 14:15:48.000000 pih-1.47205/pih/console_api.py
--rw-rw-rw-   0        0        0   110449 2023-07-28 11:57:21.000000 pih-1.47205/pih/const.py
--rw-rw-rw-   0        0        0   310256 2023-07-28 13:42:05.000000 pih-1.47205/pih/pih.py
--rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.47205/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.47205/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.47205/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2576 2023-06-14 04:29:04.000000 pih-1.47205/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.47205/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.47205/pih/service_example.py
--rw-rw-rw-   0        0        0    37996 2023-07-27 14:15:47.000000 pih-1.47205/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.47205/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-28 13:42:35.409126 pih-1.47205/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-07-28 13:42:33.000000 pih-1.47205/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      537 2023-07-28 13:42:33.000000 pih-1.47205/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 13:42:33.000000 pih-1.47205/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-28 13:42:33.000000 pih-1.47205/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-28 13:42:33.000000 pih-1.47205/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1644 2023-07-28 12:42:15.000000 pih-1.47205/pih_mio_setup.py
--rw-rw-rw-   0        0        0     2009 2023-07-27 14:02:40.000000 pih-1.47205/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-28 13:42:35.518507 pih-1.47205/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 09:00:29.492944 pih-1.47206/
+drwxrwxrwx   0        0        0        0 2023-07-31 09:00:29.805418 pih-1.47206/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-1.47206/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0   165320 2023-07-31 03:28:09.000000 pih-1.47206/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-1.47206/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9431 2023-07-28 13:39:51.000000 pih-1.47206/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-1.47206/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      261 2023-07-31 09:00:30.978801 pih-1.47206/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-31 09:00:30.650662 pih-1.47206/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.47206/pih/__init__.py
+-rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.47206/pih/collection.py
+-rw-rw-rw-   0        0        0    61076 2023-07-27 14:15:48.000000 pih-1.47206/pih/console_api.py
+-rw-rw-rw-   0        0        0   111114 2023-07-31 08:24:44.000000 pih-1.47206/pih/const.py
+-rw-rw-rw-   0        0        0   314112 2023-07-31 09:00:04.000000 pih-1.47206/pih/pih.py
+-rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.47206/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.47206/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.47206/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2576 2023-06-14 04:29:04.000000 pih-1.47206/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.47206/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.47206/pih/service_example.py
+-rw-rw-rw-   0        0        0    38229 2023-07-31 08:39:50.000000 pih-1.47206/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.47206/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:00:30.931910 pih-1.47206/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-07-31 09:00:28.000000 pih-1.47206/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      537 2023-07-31 09:00:29.000000 pih-1.47206/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 09:00:28.000000 pih-1.47206/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-31 09:00:28.000000 pih-1.47206/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-31 09:00:28.000000 pih-1.47206/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1644 2023-07-28 12:42:15.000000 pih-1.47206/pih_mio_setup.py
+-rw-rw-rw-   0        0        0     2009 2023-07-27 14:02:40.000000 pih-1.47206/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-07-31 09:00:30.994410 pih-1.47206/setup.cfg
```

### Comparing `pih-1.47205/MobileHelperCore/api.py` & `pih-1.47206/MobileHelperCore/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1034,15 +1034,15 @@
         #######################
         self.address_as_link_node: CommandNode = self.create_command_link(
             f"link|{LINK_SYMBOL}", LINK_SYMBOL, i("Адресовать ссылку на команду"), MobileHelper.ADM, True)
         self.address_as_link_node.order_value = 3
         additional_nodes.append(self.address_as_link_node)
         #######################
         about_pih_node: CommandNode = CommandNode(
-            "about|o", i("О PIH"), description="\n...", text=f"Я бот-помощник для решения Ваших задач. Моё имя составлено из первых букв нашей организации: *P* acific *I* nternational *H* ospital.\n\n_Автор: {i(b('Караченцев Никита Александрович'))}\nВерсия: {A.V.MIO.local()}", show_in_root_menu=True, wait_for_input=False, show_always=True)
+            "about|o", i("О PIH"), description="\n...", text=f"Я бот-помощник для решения Ваших задач. Моё имя составлено из первых букв нашей организации: {b('P')} acific {b('I')} nternational {b('H')} ospital или {b('П')} асифик {b('И')} нтернейшнл {b('Х')} оспитал.\n\n{i('Автор')}: {i(b('Караченцев Никита Александрович'))} \n{i('Версия')}: {b(A.V.MIO.local())}", show_in_root_menu=True, wait_for_input=False, show_always=True)
         about_pih_node.order_value = 4
         additional_nodes.append(about_pih_node)
         #######################
         self.exit_node: CommandNode = CommandNode(
             "exit", i("Выход"), self.session.exit, show_in_root_menu=True, wait_for_input=False, show_always=True, as_link=True)
         self.exit_node.order_value = 0
         additional_nodes.append(self.exit_node)
@@ -1961,15 +1961,15 @@
         def sort_function(item: Mark) -> str:
             return item.TabNumber if sort_by_tab_number else item.GroupName
         self.output.write_result(A.R.sort(A.R_M.free_list(False), sort_function), False, title = "Свободные карты доступа:")
 
     def set_or_get_handler(self, get_action: bool = False) -> None:
         with self.output.personalized():
             storage_value_name: str | None = None if self.is_all else (self.arg() or self.input.input("Введите название"))
-            storage_value_holder_list: list[A.CT_S, A.CT_MR.TYPES] = A.D.find_variable(storage_value_name)
+            storage_value_holder_list: list[A.CT_S, A.CT_MR.TYPES] = A.D.find_variables(storage_value_name)
             def sort_function(item: A.CT_S | A.CT_MR.TYPES) -> int:
                 if isinstance(item, A.CT_S):
                     return 0
                 return 1
             storage_value_holder_list = sorted(storage_value_holder_list, key=sort_function)
             def label_function(item: A.CT_S | A.CT_MR.TYPES, _) -> str:
                 name: str = item.name
```

### Comparing `pih-1.47205/MobileHelperCore/service.py` & `pih-1.47206/MobileHelperCore/service.py`

 * *Files identical despite different names*

### Comparing `pih-1.47205/MobileHelperCore/service_api.py` & `pih-1.47206/MobileHelperCore/service_api.py`

 * *Files identical despite different names*

### Comparing `pih-1.47205/MobileHelperCore/tools.py` & `pih-1.47206/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.47205/pih/collection.py` & `pih-1.47206/pih/collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.47205/pih/console_api.py` & `pih-1.47206/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-1.47205/pih/const.py` & `pih-1.47206/pih/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,16 +64,16 @@
 class AD:
 
     SEARCH_ATTRIBUTES: list[str] = [USER_PROPERTIES.LOGIN, USER_PROPERTIES.NAME]
     SEARCH_ATTRIBUTE_DEFAULT: str = SEARCH_ATTRIBUTES[0]
     DOMAIN_NAME: str = "fmv"
     DOMAIN_ALIAS: str = "pih"
     DOMAIN_SUFFIX: str = "lan"
-    DOMAIN: str = ".".join([DOMAIN_NAME, DOMAIN_SUFFIX])
-    DOMAIN_MAIN: str = DOMAIN
+    DOMAIN_DNS: str = ".".join([DOMAIN_NAME, DOMAIN_SUFFIX])
+    DOMAIN_MAIN: str = DOMAIN_DNS
     USER_HOME_FOLDER_DISK: str = "U:"
     OU: str = "OU="
     ROOT_CONTAINER_DN: str = f"{OU}Unit,DC={DOMAIN_NAME},DC={DOMAIN_SUFFIX}"
     WORKSTATIONS_CONTAINER_DN: str = f"{OU}Workstations,{ROOT_CONTAINER_DN}"
     SERVERS_CONTAINER_DN: str = f"{OU}Servers,{ROOT_CONTAINER_DN}"
     USERS_CONTAINER_DN_SUFFIX: str = f"Users,{ROOT_CONTAINER_DN}"
     ACTIVE_USERS_CONTAINER_DN: str = f"{OU}{USERS_CONTAINER_DN_SUFFIX}"
@@ -116,17 +116,14 @@
         "RESERVED",
         "PARTIAL_SECRETS_ACCOUNT"
     ]
 
     WORKSTATION_PREFIX_LIST: list[str] = [
         "ws-", "nb-", "fmvulianna"]
 
-    ADMINISTRATOR: str = "Administrator"
-    ADMINISTRATOR_PASSOWORD: str = "Fortun@90"
-
     class USER:
         MARKETER: str = "marketer"
         CALL_CENTRE_ADMINISTRATOR: str = "callCentreAdmin"
         REGISTRATION_AND_CALL: str = "reg_and_call"
         CONTROL_SERVICE: str = "cctv"
         INDICATIONS_ALL: str = "indications_all"
         ADMINISTRATOR: str = "Administrator"
@@ -174,20 +171,23 @@
         PYTHON: str = "py"
         BASE64: str = "base64"
         EXE: str = "exe"
         TRUE_TYPE_FONT: str = "ttf"
 
 class HOSTS:
 
-    class SVSHOST:
+    class SERVICES:
 
         NAME: str = "svshost"
         ALIAS: str = "zabbix"
         IP: str = "192.168.100.95"
 
+        LOGIN_ALIAS: str = "SERVICES_LOGIN"
+        PASSWORD_ALIAS: str = "SERVICES_PASSWORD"
+
     class BACKUP_WORKER:
     
         NAME: str = "backup_worker"
         ALIAS: str = "backup_worker"
         IP: str = "192.168.100.11"
 
     class WS255:
@@ -296,14 +296,20 @@
 
     class PORTS:
 
         SMB: int = 445
 
 class CONST:
 
+    ADMINISTRATOR_PASSOWORD_ALIAS: str = "ADMINISTRATOR_PASSWORD"
+    ADMINISTRATOR_LOGIN_ALIAS: str = "ADMINISTRATOR_LOGIN"
+
+    DEVELOPER_LOGIN_ALIAS: str = "DEVELOPER_LOGIN"
+    DEVELOPER_PASSWORD_ALIAS: str = "DEVELOPER_PASSWORD"
+
     #in seconds
     HEAT_BEAT_PERIOD: int = 60
 
     NEW_LINE: str = "\n"
 
     class TEST:
 
@@ -427,17 +433,17 @@
 
     class SERVICE:
 
         NAME: str = "service"
 
     class FACADE:
 
+        NAME: str = "facade"
         SERVICE_FOLDER_SUFFIX: str = "Core"
-        PATH: str = "\\\\pih\\facade\\"
-
+      
     class VALENTA:
 
         PROCESS_NAME: str = "Vlwin"
 
     class POWERSHELL:
 
         NAME: str = "powershell"
@@ -761,14 +767,26 @@
     PERSONAL: int = auto()
 
 class PATH_SHARE:
 
     NAME: str = "shares"
     PATH: str = os.path.join(AD.PATH_ROOT, NAME)
 
+class PATH_FACADE:
+
+    SHARED_POINT: str = os.path.join("S$", CONST.FACADE.NAME)
+    LINUX_MOUNT_POINT_PATH: str = f"/mnt/{AD.DOMAIN_ALIAS}"
+
+    PATH: str = f"\\\\{AD.DOMAIN_ALIAS}\\{CONST.FACADE.NAME}\\"
+
+    @staticmethod
+    def STORAGE_PATH() -> str:
+        return os.path.join(HOSTS.DC1.NAME, PATH_FACADE.SHARED_POINT)
+
+
 class PATH_SCAN:
     
     NAME: str = "scan"
     VALUE: str = os.path.join(AD.PATH_ROOT, NAME)
 
 class PATH_SCAN_TEST:
     
@@ -809,20 +827,20 @@
     @staticmethod
     def NEW_EMPLOYEE(name: str) -> str:
         return os.path.join(os.path.join(PATH_IT.ROOT, PATH_IT.NEW_EMPLOYEES_NAME), name)
 
 class PATH_APP:
 
     NAME: str = "apps"
-    FOLDER: str = os.path.join(CONST.FACADE.PATH, NAME)
+    FOLDER: str = os.path.join(PATH_FACADE.PATH, NAME)
 
 class PATH_DOCS:
     
     NAME: str = f"Docs{CONST.FACADE.SERVICE_FOLDER_SUFFIX}"
-    FOLDER: str = os.path.join(CONST.FACADE.PATH, NAME)
+    FOLDER: str = os.path.join(PATH_FACADE.PATH, NAME)
 
 class PATH_FONTS:
 
     NAME: str = "fonts"
     FOLDER: str = os.path.join(PATH_DOCS.FOLDER, NAME)
 
     @staticmethod
@@ -885,15 +903,15 @@
 
 class PATH_POLIBASE_APP_DATA:
     
     NAME: str = "polibase"
     FOLDER: str = os.path.join(PATH_APP_DATA.FOLDER, NAME)
     PERSON_CARD_REGISTRY_FOLDER: str = os.path.join(FOLDER, "person card folder")
 
-    SERVICE_FOLDER_PATH: str = os.path.join(CONST.FACADE.PATH, f"{NAME}{CONST.FACADE.SERVICE_FOLDER_SUFFIX}")
+    SERVICE_FOLDER_PATH: str = os.path.join(PATH_FACADE.PATH, f"{NAME}{CONST.FACADE.SERVICE_FOLDER_SUFFIX}")
     
     class SETTINGS:
         MAIN: str = "polibase_main_settings.vbs"
         TEST: str = "polibase_test_settings.vbs"
 
 class PATH_USER:
 
@@ -926,29 +944,29 @@
             else:
                 root += PATH_POLIBASE.TEST_SUFFIX
         return os.path.join(os.path.join(f"//{root}", "polibaseData", "PERSONS"), str(pin))
 
 class PATH_WS:
 
     NAME: str = f"WS{CONST.FACADE.SERVICE_FOLDER_SUFFIX}"
-    PATH: str = os.path.join(CONST.FACADE.PATH, NAME)
+    PATH: str = os.path.join(PATH_FACADE.PATH, NAME)
 
 
 class PATH_BACKUP:
 
     class ROBOCOPY_CONFIG:
 
         NAME: str = "robocopy_config"
-        ROOT: str = os.path.join(CONST.FACADE.PATH, f"Backup{CONST.FACADE.SERVICE_FOLDER_SUFFIX}", NAME)
+        ROOT: str = os.path.join(PATH_FACADE.PATH, f"Backup{CONST.FACADE.SERVICE_FOLDER_SUFFIX}", NAME)
 
     class COMMAND:
 
         NAME: str = "command"
         ROOT: str = os.path.join(
-            CONST.FACADE.PATH, f"Backup{CONST.FACADE.SERVICE_FOLDER_SUFFIX}", NAME)
+            PATH_FACADE.PATH, f"Backup{CONST.FACADE.SERVICE_FOLDER_SUFFIX}", NAME)
         
         ATTACH_SHARED_DISKS: str = os.path.join(ROOT, "attach_shared_disks.ps1")
 
     
 
 class PATHS:
 
@@ -967,14 +985,15 @@
     BACKUP: PATH_BACKUP = PATH_BACKUP()
     DOCS: PATH_DOCS = PATH_DOCS()
     FONTS: PATH_FONTS = PATH_FONTS()
     MOBILE_HELPER: PATH_MOBILE_HELPER = PATH_MOBILE_HELPER()
     APP_DATA: PATH_APP_DATA = PATH_APP_DATA()
     INDICATIONS: PATH_INDICATIONS = PATH_INDICATIONS()
     STATISTICS: PATH_STATISTICS = PATH_STATISTICS()
+    FACADE: PATH_FACADE = PATH_FACADE()
 
 class MarkType(Enum):
 
     NORMAL: int = auto()
     FREE: int = auto()
     GUEST: int = auto()
     TEMPORARY: int = auto()
@@ -1734,18 +1753,17 @@
                   ServiceCommands.get_unix_free_space_information_by_drive_name]
     )
 
     WS_735: ServiceDescription = ServiceDescription(
         name="ws_735",
         description="ws-735 service",
         host=CONST.HOST.WS735.NAME,
-        login="nak",
-        password="Soad7623!",
-        pyton_executor_path=r"C:\Users\nak\AppData\Local\Programs\Python\Python310\python.exe",
-        run_from_system_account=True,
+        login= "{" + f"{CONST.DEVELOPER_LOGIN_ALIAS}" + "}",
+        password="{" + f"{CONST.DEVELOPER_PASSWORD_ALIAS}" + "}",
+        #pyton_executor_path=r"C:\Users\nak\AppData\Local\Programs\Python\Python310\python.exe",
         commands=[ServiceCommands.print_image],
         modules=["pywin32", "Pillow"]
     )
 
     RECOGNIZE: ServiceDescription = ServiceDescription(
         name="Recognize",
         description="Recognize service",
```

### Comparing `pih-1.47205/pih/pih.py` & `pih-1.47206/pih/pih.py`

 * *Files 1% similar despite different names*

```diff
@@ -1632,19 +1632,19 @@
 
     class VERSION:
 
         class MIO:
             
             @staticmethod
             def local() -> str:
-                return "1.48013"  
+                return "1.48016"  
 
         @staticmethod
         def local() -> str:
-            return "1.47205"
+            return "1.47206"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.local() < PIH.VERSION.remote()
     
     class INPUT_WAIT:
@@ -1826,15 +1826,15 @@
             return PIH.DATA.CONVERT.settings_to_datetime(value)
         
         @staticmethod
         def to_datetime_list(value: SETTINGS) -> list[datetime]:
             return PIH.DATA.CONVERT.settings_to_datetime_list(value)
 
         @staticmethod
-        def set(settings_item: SETTINGS, value: Any) -> bool:
+        def set(settings_item: SETTINGS | str, value: Any) -> bool:
             return PIH.ACTION.SETTINGS.set(settings_item, value)
 
         @staticmethod
         def set_default(settings_item: SETTINGS) -> bool:
             return PIH.ACTION.SETTINGS.set_default(settings_item)
 
         @staticmethod
@@ -1991,16 +1991,16 @@
         @staticmethod
         def get_executor_path(executor_name: str) -> str:
             return os.path.join(
                 PATHS.WS.PATH, CONST.PSTOOLS.NAME, executor_name)
 
         @staticmethod
         def create_command_list_for_command(executor_name: str, command_list: list[str], login: str | None = None, password: str | None = None) -> list[str]:
-            login = "\\".join([AD.DOMAIN_NAME, AD.ADMINISTRATOR if DataTool.is_empty(login) else login])
-            password = password or AD.ADMINISTRATOR_PASSOWORD
+            login = "\\".join([AD.DOMAIN_NAME, login or PIH.OS.get_variable(CONST.ADMINISTRATOR_LOGIN_ALIAS)])
+            password = password or PIH.OS.get_variable(CONST.ADMINISTRATOR_PASSOWORD_ALIAS)
             return [PIH.PSTOOLS.get_executor_path(executor_name), CONST.PSTOOLS.NO_BANNER, CONST.PSTOOLS.ACCEPTEULA, "-u", login, "-p", password]  + command_list
         
         @staticmethod
         def create_command_list_for_psexec_command(command_list: list[str], host: str | None = None, login: str | None = None, password: str | None = None, interactive: bool | None = False, run_from_system_account: bool = False, run_with_elevetion: bool = False) -> list[str]:
             result_command_list: list[str] = DataTool.check_not_none(interactive, lambda: [["-d", "-i"][interactive]], [])
             host_start: str = r"\\"
             if not DataTool.is_empty(host):
@@ -2014,43 +2014,46 @@
         @staticmethod
         def create_command_list_for_psexec_command_local(command_list: list[str], login: str | None = None, password: str | None = None) -> list[str]:
             return PIH.PSTOOLS.create_command_list_for_command(CONST.PSTOOLS.PS_EXECUTOR, command_list, login, password)
 
         @staticmethod
         def create_remote_process_executor_for_service(role_or_information: ServiceRoles | ServiceInformationBase, interactive: bool | None = False) -> list[str]:
             description: ServiceDescription = ServiceRoles.description(role_or_information)
-            return PIH.PSTOOLS.create_command_list_for_psexec_command([role_or_information.pyton_executor_path or CONST.PYTHON.EXECUTOR_ALIAS], PIH.SERVICE.get_host(description), description.login, description.password, interactive, description.run_from_system_account)
+            login: str | None = DataTool.check_not_none(description.login, lambda: PIH.DATA.FORMAT.variable(description.login))
+            password: str | None = DataTool.check_not_none(description.password, lambda: PIH.DATA.FORMAT.variable(description.password))
+            return PIH.PSTOOLS.create_command_list_for_psexec_command([role_or_information.pyton_executor_path or CONST.PYTHON.EXECUTOR_ALIAS], PIH.SERVICE.get_host(description), login, password, interactive, description.run_from_system_account)
 
         @staticmethod
-        def execute_command_list(command_list: list[str] | str, show_output: bool, capture_output: bool = False, as_text: bool = True, as_shell: bool = False) -> CompletedProcess:
+        def execute_command_list(command: list[str] | str, show_output: bool, capture_output: bool = False, as_text: bool = True, as_shell: bool = False) -> CompletedProcess:
             if show_output:
                 if capture_output:
                     process_result = subprocess.run(
-                        command_list, capture_output=True, text=as_text, shell=as_shell)
+                        command, capture_output=True, text=as_text, shell=as_shell)
                 else:
                     process_result = subprocess.run(
-                        command_list, text=as_text)
+                        command, text=as_text)
             else:
                 process_result = subprocess.run(
-                    command_list, stdout=DEVNULL, stderr=STDOUT, text=as_text)
+                    command, stdout=DEVNULL, stderr=STDOUT, text=as_text)
             return process_result
 
         @staticmethod
         def kill_process(name_or_pid: str | int, host: str, via_taskkill: bool = True, show_output: bool = False) -> bool:
            if via_taskkill:
                 is_string: bool = isinstance(name_or_pid, str)
                 return PIH.PSTOOLS.execute_command_list(["taskkill", "/s", host, "/t", "/f", "/im" if is_string else "/pid", PIH.PATH.add_extension(name_or_pid, FILE.EXTENSION.EXE) if is_string else str(name_or_pid)], show_output).returncode < 2
            return PIH.PSTOOLS.execute_command_list(PIH.PSTOOLS.create_command_list_for_command(CONST.PSTOOLS.PS_KILL_EXECUTOR, [PIH.DATA.FORMAT.host(host), "-t", str(name_or_pid)]), show_output).returncode == 0
 
         @staticmethod
         def process_is_exists(pid: int, host: str | None = None, login: str | None = None, password: str | None = None) -> str:
             command_list: list[str] = ["tasklist", "/fi", f"pid eq {pid}", "/fo", "list"]
             login = "\\".join(
-                [AD.DOMAIN_NAME, AD.ADMINISTRATOR if DataTool.is_empty(login) else login])
-            password = password or AD.ADMINISTRATOR_PASSOWORD
+                [AD.DOMAIN_NAME, login or PIH.OS.get_variable(CONST.ADMINISTRATOR_LOGIN_ALIAS)])
+            password = password or PIH.OS.get_variable(
+                CONST.ADMINISTRATOR_PASSOWORD_ALIAS)
             if not DataTool.is_empty(host):
                 command_list += ["/s", host]
                 command_list += ["/u", login]
                 command_list += ["/p", password]
             output: str = PIH.PSTOOLS.execute_command_list(
                 command_list, True, True, as_text=False).stdout.decode(WINDOWS.CHARSETS.ALTERNATIVE).lower()
             return output.find("pid") != -1
@@ -2616,15 +2619,15 @@
                 if check_if_started:
                     if PIH.SERVICE.check_accessibility(description):
                         return None
                 remote_executor_command_list: list[str] = PIH.PSTOOLS.create_remote_process_executor_for_service(description, False)
                 service_file_path: str | None = None
                 if DataTool.is_empty(description.service_path):
                     service_file_path = os.path.join(
-                        CONST.FACADE.PATH, f"{description.name}{CONST.FACADE.SERVICE_FOLDER_SUFFIX}", PathTool.add_extension(CONST.SERVICE.NAME, FILE.EXTENSION.PYTHON))
+                        PATH_FACADE.PATH, f"{description.name}{CONST.FACADE.SERVICE_FOLDER_SUFFIX}", PathTool.add_extension(CONST.SERVICE.NAME, FILE.EXTENSION.PYTHON))
                 else:
                     service_file_path = os.path.join(
                         description.service_path, PathTool.add_extension(CONST.SERVICE.NAME, FILE.EXTENSION.PYTHON))
                 remote_executor_command_list.append(service_file_path)
                 remote_executor_command_list.append("false")
                 process_result: CompletedProcess = PIH.PSTOOLS.execute_command_list(remote_executor_command_list, show_output)
                 returncode = process_result.returncode
@@ -2783,15 +2786,15 @@
                         service_command_item: ServiceCommands = service_command_item
                         PIH.SERVICE.command_map[service_command_item.name] = description
             return PIH.SERVICE.command_map[value.name] if value.name in PIH.SERVICE.command_map else None
 
         @staticmethod
         def get_host(role_or_information: ServiceRoles | ServiceInformationBase) -> str:
             def add_donain(value: str) -> str:
-                return if_else(value.endswith(AD.DOMAIN), value, lambda: j((value, AD.DOMAIN), "."))
+                return if_else(value.endswith(AD.DOMAIN_DNS), value, lambda: j((value, AD.DOMAIN_DNS), "."))
             information: ServiceInformationBase | None = ServiceRoles.description(role_or_information)
             if isinstance(information, ServiceDescription):
                 if not DataTool.is_empty(information.port):
                     return add_donain(information.host)
             return add_donain((PIH.SERVICE.get_information(role_or_information) or ServiceInformationBase()).host or information.host)
 
         @staticmethod
@@ -2812,14 +2815,23 @@
             return PIH.OS.host() if description.isolated or DataTool.is_empty(description.host) else description.host
 
     class PATH(PATHS, PathTool):
 
         DIRECTORY_INFO_PREFIX: str = "directory_info_"
 
         @staticmethod
+        def mount_storage_on_linux_host(storage_path: str, linux_mount_point: str, linux_host: str, linux_host_user_password: str, storage_host_user_login: str, storage_host_user_password) -> bool:
+            def get_command(value: str, password: str, use_sudo: bool) -> list[str]:
+                if use_sudo:
+                    value = f"echo -e '{password}\n' | sudo -S " + value
+                return value
+            commnad: str = get_command(f"mount -t cifs {PathTool.convert_for_unix(storage_path)} {linux_mount_point} -o username={storage_host_user_login},password={storage_host_user_password}", linux_host_user_password, True)
+            PIH.RESULT.SSH.execute(commnad, linux_host)
+
+        @staticmethod
         def get_file_list_by_directory_info(path: str) -> list[str] | None:
             return PIH.PATH.get_file_list(path, DataTool.if_not_empty(PIH.RESULT.DATA_STORAGE.value(PIH.PATH.get_directory_info_name(
                 None, path), DirectoryInfo()).data, lambda info: info.last_created_file_timestamp))
 
         @staticmethod
         def get_directory_info_name(file_path: str | None, directory_path: str | None = None) -> float :
             return  PIH.PATH.DIRECTORY_INFO_PREFIX + (directory_path or A.PTH.get_file_directory(file_path))
@@ -2857,20 +2869,29 @@
             @staticmethod
             def mobile_helper_command(name: str) -> str:
                 name = PIH.DATA.FORMAT.mobile_helper_command(name)
                 return os.path.join(PATHS.MOBILE_HELPER.QR_CODE_FOLDER, PathTool.replace_prohibited_symbols_from_path_with_symbol(PathTool.add_extension(name, FILE.EXTENSION.PNG)))
 
     class DATA(DataTool, StringTool, ListTool, DateTimeTool, EnumTool, FullNameTool):
 
+        @staticmethod
         def translit(value, language_code=None, reversed=False, strict=False):
             return translit(value, language_code, reversed, strict)
 
-        def find_variable(name: str | None) -> list[StorageValue]:
+        @staticmethod
+        def find_variables(name: str | None) -> list[StorageValue]:
             return PIH.DATA.MATERIALIZED_RESOURCES.find(name) + PIH.SETTINGS.find(name)
         
+        @staticmethod
+        def get_variable_value(variable_name: str, only_local: bool = False) -> Any | None:
+            variable_handler: Callable[[str], Any] = PIH.OS.get_variable
+            if only_local:
+                return variable_handler(variable_name)
+            return variable_handler(variable_name) or PIH.DATA.MATERIALIZED_RESOURCES.get_count(variable_name) or PIH.SETTINGS.get(variable_name)
+        
         class VARIABLE:
 
             NAME: str = "variable"
 
             @staticmethod
             def get(name: str) -> Any:
                 return PIH.RESULT.DATA_STORAGE.value(name, None, PIH.DATA.VARIABLE.NAME).data
@@ -2899,16 +2920,16 @@
                 result: list[SETTINGS] = []
                 for item in MATERIALIZED_RESOURCES.TYPES:
                     if DataTool.is_none(value) or StringTool.contains(item.name, value) or StringTool.contains(item.value.key_name, value) or StringTool.contains(item.value.description, value):
                         result.append(item)
                 return result
 
             @staticmethod
-            def get_count(type: MATERIALIZED_RESOURCES.TYPES) -> int:
-                return PIH.RESULT.DATA_STORAGE.value(type.name, None, MATERIALIZED_RESOURCES.NAME).data
+            def get_count(type: MATERIALIZED_RESOURCES.TYPES | str) -> int:
+                return PIH.RESULT.DATA_STORAGE.value(if_else(isinstance(type, str), type, lambda: type.name), None, MATERIALIZED_RESOURCES.NAME).data
 
             @staticmethod
             def set_count(type: MATERIALIZED_RESOURCES.TYPES, value: int) -> bool:
                 return PIH.ACTION.DATA_STORAGE.value(value, type.name, MATERIALIZED_RESOURCES.NAME)
 
             @staticmethod
             def add_count(type: MATERIALIZED_RESOURCES.TYPES, value: int) -> bool:
@@ -3212,14 +3233,20 @@
             
             @staticmethod
             def settings_to_datetime_list(item: SETTINGS, format: str = CONST.SECONDLESS_TIME_FORMAT) -> list[datetime]:
                 return list(map( lambda item: DateTimeTool.datetime_from_string(item, format), A.S.get(item)))
 
             @staticmethod
             def file_to_base64(path: str) -> str | None:
+                if PIH.OS.is_linux():
+                    path = PIH.PATH.convert_for_unix(path.lower())
+                    alias: str = PIH.PATH.convert_for_unix(PATH_FACADE.PATH)
+                    if path.find(alias) == 0:
+                        path = path[len(alias):]
+                        path = j((PATHS.FACADE.LINUX_MOUNT_POINT_PATH, path), os.sep)
                 while True:
                     try:
                         with open(path, "rb") as file:
                             return PIH.DATA.CONVERT.bytes_to_base64(file.read())
                     except Exception:
                         pass
                 return None
@@ -3302,14 +3329,22 @@
                 @staticmethod
                 def chiller_value_valid(value: ChillerIndicationsValue) -> bool:
                     return not DataTool.is_empty(value.temperature)
 
         class FORMAT:
 
             @staticmethod
+            def variable(value: str, parse: bool = True) -> str:
+                fields: list[str] | None = if_else(parse, [name for _, name, _, _ in Formatter().parse(value) if name], [value])
+                if DataTool.is_empty(fields):
+                    return None
+                variable_name: str = fields[0]
+                return PIH.OS.get_variable(variable_name) or PIH.SETTINGS.get(variable_name)
+
+            @staticmethod
             def statistics(type: MATERIALIZED_RESOURCES.TYPES) -> str | None:
                 statistics: TimeSeriesStatistics | None = PIH.DATA.STATISTICS.by_name(type.name)
                 if DataTool.is_none(statistics):
                     return None
                 count: int = PIH.DATA.MATERIALIZED_RESOURCES.get_count(type)
                 def to_days(value: int) -> int:
                     return int(DateTimeTool.seconds_to_days(value))
@@ -3534,15 +3569,15 @@
                     return user.telephoneNumber is not None
                 def map_function(user: User) -> str:
                     return PIH.DATA.FORMAT.telephone_number(user.telephoneNumber)
                 return ResultTool.map(ResultTool.filter(PIH.RESULT.USER.by_name(AD.SEARCH_ALL_PATTERN, active=active), filter_function), map_function).data
 
             @staticmethod
             def it_administrator() -> str:
-                return PIH.DATA.TELEPHONE_NUMBER.by_login(AD.ADMINISTRATOR)
+                return PIH.DATA.TELEPHONE_NUMBER.by_login(PIH.OS.get_variable(CONST.ADMINISTRATOR_LOGIN_ALIAS))
 
             @staticmethod
             def call_centre_administrator() -> str:
                 return PIH.DATA.TELEPHONE_NUMBER.by_login(AD.USER.CALL_CENTRE_ADMINISTRATOR)
 
             @staticmethod
             def marketer() -> str:
@@ -3639,25 +3674,59 @@
                     return sort_function
                 value.sort(key=sort_function)
                 return value
 
     class OS:
 
         @staticmethod
+        def python_path() -> str | None:
+            name: str = "\\Python\\Python"
+            for item in PIH.OS.get_variable("PATH").split(";"):
+                index: int = item.find(name)
+                if index != -1 and len(item) - (index + len(name)) <= 4:
+                    return os.path.join(item, j((CONST.PYTHON.EXECUTOR, FILE.EXTENSION.EXE), "."))
+            return None   
+
+        @staticmethod
+        def name() -> str:
+            return platform.system()
+
+        @staticmethod
+        def is_linux() -> bool:
+            return PIH.OS.name() == "Linux"
+
+        @staticmethod
         def get_login() -> str:
             return os.getlogin()
 
         @staticmethod
         def host() -> str:
             return platform.node()
 
         @staticmethod
         def get_pid() -> int:
             return os.getppid()
 
+        @staticmethod
+        def get_variable(name: str) -> str:
+            return os.getenv(name)
+        
+        @staticmethod
+        def os_name() -> str:
+            return PIH.OS.get_variable("OS")
+
+        @staticmethod
+        def domain_dns() -> str:
+            return PIH.OS.get_variable("USERDNSDOMAIN")
+        
+        @staticmethod
+        def domain() -> str:
+            return PIH.OS.get_variable("USERDOMAIN")
+
+
     class RESULT(ResultTool):
 
         class EVENTS:
 
            @staticmethod
            def get(value: Events, parameters: tuple[Any] | None = None) -> Result[list[EventDS]]:
                 def extractor(data: Any) -> EventDS:
@@ -4693,14 +4762,19 @@
         def login(value: str) -> bool:
             pattern: str = r"^[a-z]+[a-z_0-9]{"+str(CONST.NAME_POLICY.PART_ITEM_MIN_LENGTH - 1) + ",}"
             return re.fullmatch(pattern, value, re.IGNORECASE) is not None
 
         class WORKSTATION:
 
             @staticmethod
+            def python_version(host: str) -> str:
+                return PIH.PSTOOLS.execute_command_list(PIH.PSTOOLS.create_command_list_for_psexec_command(
+                    [CONST.PYTHON.EXECUTOR_ALIAS, "--version"], host), True, True).stdout
+
+            @staticmethod
             def accessibility(name: str) -> bool | None:
                 try:
                     return PIH.RESULT.WORKSTATION.by_name(name).data.accessable
                 except NotFound as _:
                     return None
 
             @staticmethod
@@ -5406,16 +5480,16 @@
 
             @staticmethod
             def key(key: str, value: Any) -> bool:
                 return DataTool.rpc_unrepresent(
                     PIH.SERVICE.call_command(ServiceCommands.set_settings_value, (key, value)))
 
             @staticmethod
-            def set(settings_item: SETTINGS, value: Any) -> bool:
-                return PIH.ACTION.SETTINGS.key(settings_item.value.key_name or settings_item.name, value)
+            def set(settings_item: SETTINGS | str, value: Any) -> bool:
+                return PIH.ACTION.SETTINGS.key(if_else(isinstance(settings_item, str), settings_item, lambda: settings_item.value.key_name or settings_item.name), value)
 
             @staticmethod
             def set_default(settings_item: SETTINGS) -> bool:
                 return PIH.ACTION.SETTINGS.set(settings_item, settings_item.value.default_value)
 
         class USER:
```

### Comparing `pih-1.47205/pih/rpc.py` & `pih-1.47206/pih/rpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.47205/pih/rpcCommandCall_pb2.py` & `pih-1.47206/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.47205/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.47206/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.47205/pih/rpc_collection.py` & `pih-1.47206/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.47205/pih/rpc_const.py` & `pih-1.47206/pih/rpc_const.py`

 * *Files identical despite different names*

### Comparing `pih-1.47205/pih/service_example.py` & `pih-1.47206/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.47205/pih/tools.py` & `pih-1.47206/pih/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -662,14 +662,19 @@
    
 class PathTool:
      
     @staticmethod
     def exists(path: str) -> bool:
         return os.path.exists(path)
 
+    @staticmethod
+    def convert_for_unix(value: str) -> str:
+        start: str = os.sep*2
+        value = value.replace("\\", os.sep).replace("\\\\", os.sep)
+        return if_else(value.startswith(start), "", start) + value
 
     @staticmethod
     def get_file_list(path: str, created_after: float | None = None) -> list[str]:
         file_list = [(file_path, os.path.getctime(file_path))
                      for file_path in [os.path.join(path, file_path) for file_path in [
                          file_path for file_path in next(walk(path), (None, None, []))[2]]]]
         if created_after is not None:
```

### Comparing `pih-1.47205/pih/widgets.py` & `pih-1.47206/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.47205/pih.egg-info/SOURCES.txt` & `pih-1.47206/pih.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pih-1.47205/pih_mio_setup.py` & `pih-1.47206/pih_mio_setup.py`

 * *Files identical despite different names*

### Comparing `pih-1.47205/pih_setup.py` & `pih-1.47206/pih_setup.py`

 * *Files identical despite different names*

