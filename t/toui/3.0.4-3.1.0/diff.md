# Comparing `tmp/toui-3.0.4.tar.gz` & `tmp/toui-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toui-3.0.4.tar", last modified: Sun Jul 30 07:55:13 2023, max compression
+gzip compressed data, was "toui-3.1.0.tar", last modified: Mon Jul 31 18:10:06 2023, max compression
```

## Comparing `toui-3.0.4.tar` & `toui-3.1.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 07:55:13.275747 toui-3.0.4/
--rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-3.0.4/LICENSE
--rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-3.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     4263 2023-07-30 07:55:13.271739 toui-3.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3890 2023-07-29 19:34:40.000000 toui-3.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 07:55:13.160646 toui-3.0.4/examples/
--rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-3.0.4/examples/__init__.py
--rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-3.0.4/examples/advanced_example_1_toui_blueprint.py
--rw-rw-rw-   0        0        0     1373 2023-06-02 13:33:35.000000 toui-3.0.4/examples/advanced_example_2_toui_with_javascript.py
--rw-rw-rw-   0        0        0     2119 2023-07-30 07:47:07.000000 toui-3.0.4/examples/advanced_example_3_toui_with_google_sign_in.py
--rw-rw-rw-   0        0        0     3663 2023-07-29 20:17:59.000000 toui-3.0.4/examples/advanced_example_4_toui_with_firebase.py
--rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-3.0.4/examples/example_1_simple_website.py
--rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-3.0.4/examples/example_2_simple_desktop_app.py
--rw-rw-rw-   0        0        0      762 2023-05-04 15:56:54.000000 toui-3.0.4/examples/example_3_updating_page.py
--rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-3.0.4/examples/example_4_function_with_arg.py
--rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-3.0.4/examples/example_5_user_variables.py
--rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-3.0.4/examples/example_6_quick_website.py
--rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-3.0.4/examples/example_7_quick_desktop_app.py
-drwxrwxrwx   0        0        0        0 2023-07-30 07:55:13.170019 toui-3.0.4/images/
--rw-rw-rw-   0        0        0    27837 2023-05-30 13:42:46.000000 toui-3.0.4/images/icon.png
--rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-3.0.4/images/logo.png
--rw-rw-rw-   0        0        0       42 2023-07-30 07:55:13.276796 toui-3.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1616 2023-07-29 18:04:09.000000 toui-3.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 07:55:13.172096 toui-3.0.4/tests/
--rw-rw-rw-   0        0        0      484 2023-05-15 13:04:45.000000 toui-3.0.4/tests/test_examples.py
-drwxrwxrwx   0        0        0        0 2023-07-30 07:55:13.254397 toui-3.0.4/toui/
--rw-rw-rw-   0        0        0      283 2023-07-30 07:21:34.000000 toui-3.0.4/toui/__init__.py
--rw-rw-rw-   0        0        0     2511 2023-07-29 20:14:41.000000 toui-3.0.4/toui/_cmd.py
--rw-rw-rw-   0        0        0      379 2023-06-12 17:59:51.000000 toui-3.0.4/toui/_defaults.py
--rw-rw-rw-   0        0        0     1406 2023-05-26 03:32:16.000000 toui-3.0.4/toui/_helpers.py
--rw-rw-rw-   0        0        0    10863 2023-05-26 03:45:07.000000 toui-3.0.4/toui/_javascript_templates.py
--rw-rw-rw-   0        0        0     8637 2023-05-26 03:42:45.000000 toui-3.0.4/toui/_signals.py
--rw-rw-rw-   0        0        0    48902 2023-07-30 07:53:04.000000 toui-3.0.4/toui/apps.py
--rw-rw-rw-   0        0        0    23208 2023-07-29 16:31:59.000000 toui-3.0.4/toui/elements.py
--rw-rw-rw-   0        0        0      451 2023-07-28 20:34:08.000000 toui-3.0.4/toui/exceptions.py
--rw-rw-rw-   0        0        0    20631 2023-07-29 12:11:25.000000 toui-3.0.4/toui/pages.py
--rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-3.0.4/toui/structure.py
-drwxrwxrwx   0        0        0        0 2023-07-30 07:55:13.271105 toui-3.0.4/toui.egg-info/
--rw-rw-rw-   0        0        0     4263 2023-07-30 07:55:12.000000 toui-3.0.4/toui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      948 2023-07-30 07:55:12.000000 toui-3.0.4/toui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 07:55:12.000000 toui-3.0.4/toui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-30 07:55:12.000000 toui-3.0.4/toui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      217 2023-07-30 07:55:12.000000 toui-3.0.4/toui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-30 07:55:12.000000 toui-3.0.4/toui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 18:10:06.757574 toui-3.1.0/
+-rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-3.1.0/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-3.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4263 2023-07-31 18:10:06.756574 toui-3.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3890 2023-07-29 19:34:40.000000 toui-3.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 18:10:06.478056 toui-3.1.0/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-3.1.0/examples/__init__.py
+-rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-3.1.0/examples/advanced_example_1_toui_blueprint.py
+-rw-rw-rw-   0        0        0     1373 2023-06-02 13:33:35.000000 toui-3.1.0/examples/advanced_example_2_toui_with_javascript.py
+-rw-rw-rw-   0        0        0     2119 2023-07-30 07:47:07.000000 toui-3.1.0/examples/advanced_example_3_toui_with_google_sign_in.py
+-rw-rw-rw-   0        0        0     3663 2023-07-31 16:08:00.000000 toui-3.1.0/examples/advanced_example_4_toui_with_firebase.py
+-rw-rw-rw-   0        0        0     2841 2023-07-31 18:06:31.000000 toui-3.1.0/examples/advanced_example_5_toui_with_sql_user_database.py
+-rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-3.1.0/examples/example_1_simple_website.py
+-rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-3.1.0/examples/example_2_simple_desktop_app.py
+-rw-rw-rw-   0        0        0      762 2023-05-04 15:56:54.000000 toui-3.1.0/examples/example_3_updating_page.py
+-rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-3.1.0/examples/example_4_function_with_arg.py
+-rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-3.1.0/examples/example_5_user_variables.py
+-rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-3.1.0/examples/example_6_quick_website.py
+-rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-3.1.0/examples/example_7_quick_desktop_app.py
+drwxrwxrwx   0        0        0        0 2023-07-31 18:10:06.483569 toui-3.1.0/images/
+-rw-rw-rw-   0        0        0    27837 2023-05-30 13:42:46.000000 toui-3.1.0/images/icon.png
+-rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-3.1.0/images/logo.png
+-rw-rw-rw-   0        0        0       42 2023-07-31 18:10:06.757574 toui-3.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1616 2023-07-29 18:04:09.000000 toui-3.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 18:10:06.484567 toui-3.1.0/tests/
+-rw-rw-rw-   0        0        0      484 2023-05-15 13:04:45.000000 toui-3.1.0/tests/test_examples.py
+drwxrwxrwx   0        0        0        0 2023-07-31 18:10:06.746452 toui-3.1.0/toui/
+-rw-rw-rw-   0        0        0      283 2023-07-31 16:05:00.000000 toui-3.1.0/toui/__init__.py
+-rw-rw-rw-   0        0        0     2511 2023-07-29 20:14:41.000000 toui-3.1.0/toui/_cmd.py
+-rw-rw-rw-   0        0        0      379 2023-06-12 17:59:51.000000 toui-3.1.0/toui/_defaults.py
+-rw-rw-rw-   0        0        0     1406 2023-05-26 03:32:16.000000 toui-3.1.0/toui/_helpers.py
+-rw-rw-rw-   0        0        0    10863 2023-05-26 03:45:07.000000 toui-3.1.0/toui/_javascript_templates.py
+-rw-rw-rw-   0        0        0     8637 2023-05-26 03:42:45.000000 toui-3.1.0/toui/_signals.py
+-rw-rw-rw-   0        0        0    50682 2023-07-31 18:08:02.000000 toui-3.1.0/toui/apps.py
+-rw-rw-rw-   0        0        0    23301 2023-07-30 11:21:47.000000 toui-3.1.0/toui/elements.py
+-rw-rw-rw-   0        0        0      451 2023-07-28 20:34:08.000000 toui-3.1.0/toui/exceptions.py
+-rw-rw-rw-   0        0        0    21645 2023-07-30 09:16:10.000000 toui-3.1.0/toui/pages.py
+-rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-3.1.0/toui/structure.py
+drwxrwxrwx   0        0        0        0 2023-07-31 18:10:06.755721 toui-3.1.0/toui.egg-info/
+-rw-rw-rw-   0        0        0     4263 2023-07-31 18:10:06.000000 toui-3.1.0/toui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1007 2023-07-31 18:10:06.000000 toui-3.1.0/toui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 18:10:06.000000 toui-3.1.0/toui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-31 18:10:06.000000 toui-3.1.0/toui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      217 2023-07-31 18:10:06.000000 toui-3.1.0/toui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-31 18:10:06.000000 toui-3.1.0/toui.egg-info/top_level.txt
```

### Comparing `toui-3.0.4/LICENSE` & `toui-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toui-3.0.4/PKG-INFO` & `toui-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 3.0.4
+Version: 3.1.0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Author: Mubarak Almehairbi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `toui-3.0.4/README.md` & `toui-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `toui-3.0.4/examples/advanced_example_1_toui_blueprint.py` & `toui-3.1.0/examples/advanced_example_1_toui_blueprint.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.4/examples/advanced_example_2_toui_with_javascript.py` & `toui-3.1.0/examples/advanced_example_2_toui_with_javascript.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.4/examples/advanced_example_3_toui_with_google_sign_in.py` & `toui-3.1.0/examples/advanced_example_3_toui_with_google_sign_in.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.4/examples/advanced_example_4_toui_with_firebase.py` & `toui-3.1.0/examples/advanced_example_4_toui_with_firebase.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 ToUI with Firebase
 
 ToUI can be used with Firebase. Create a Firebase app to use this example. In this example, ToUI is used with Firebase for:
 
 - User authentication
-- Stroing user data in database
+- Storing user data in database
 - File storage
 - File retrieval
 
 
 This example uses the HTML file "test7.html":
 
 .. code-block:: html
```

### Comparing `toui-3.0.4/examples/example_1_simple_website.py` & `toui-3.1.0/examples/example_1_simple_website.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.4/examples/example_2_simple_desktop_app.py` & `toui-3.1.0/examples/example_2_simple_desktop_app.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.4/examples/example_3_updating_page.py` & `toui-3.1.0/examples/example_3_updating_page.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.4/examples/example_4_function_with_arg.py` & `toui-3.1.0/examples/example_4_function_with_arg.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.4/examples/example_5_user_variables.py` & `toui-3.1.0/examples/example_5_user_variables.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.4/images/icon.png` & `toui-3.1.0/images/icon.png`

 * *Files identical despite different names*

### Comparing `toui-3.0.4/images/logo.png` & `toui-3.1.0/images/logo.png`

 * *Files identical despite different names*

### Comparing `toui-3.0.4/setup.py` & `toui-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.4/toui/_cmd.py` & `toui-3.1.0/toui/_cmd.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.4/toui/_helpers.py` & `toui-3.1.0/toui/_helpers.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.4/toui/_javascript_templates.py` & `toui-3.1.0/toui/_javascript_templates.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.4/toui/_signals.py` & `toui-3.1.0/toui/_signals.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.4/toui/apps.py` & `toui-3.1.0/toui/apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -460,14 +460,37 @@
         flask.request
             https://flask.palletsprojects.com/en/2.2.x/api/#flask.request
 
         Page.on_url_request
 
         """
         return request
+    
+    def redirect_response(self, url):
+        """
+        Use it with `Page.on_url_request` to redirect the user to another page.
+
+        `Page.on_url_request` is called when the user makes an HTTP request to the page. If you want to redirect the user
+        to another page, define a function then use this method as the return value of a function. Then add the function to
+        `Page.on_url_request` and set `display_return_value` as ``True``.
+
+        Examples
+        --------
+        
+        >>> def redirect_function():
+        ...     return app.redirect_response("/another-page-url")
+        >>> home_page.on_url_request(redirect_function, display_return_value=True)
+
+        Parameters
+        ----------
+        url: str
+            The URL of the page that the user will be redirected to.
+
+        """
+        return redirect(url)
 
     def signup_user(self, username, password=None, email=None, **other_info):
         """
         Creates a new user in the database.
         
         Parameters
         ----------
@@ -589,22 +612,31 @@
             The value of the data.
         """
         self._confirm_user_database_created()
         if not self.is_signed_in():
             error("No user is signed in.")
             return None
         if self._user_db_type == "sql":
+            if not key in current_user.__table__.columns:
+                error(f"'{key}' was not added as a column in users table")
+                return None
             return getattr(current_user, key)
         elif self._user_db_type == "firebase":
             return self._firebase_db.document(self._user_vars._get("user-id")).get().to_dict().get(key)
 
     def set_current_user_data(self, key, value):
         """
         Sets data specific to the currently signed in user in the database.
 
+        Warning
+        -------
+        Currently, if you are using SQL database, you can only set data that
+        was already added as a column in the users table.
+
+
         Parameters
         ----------
         key: str
             The key (name) of the data. For example: "username", "email", "age", etc.
 
         value: Any
             The value of the data.
@@ -616,14 +648,17 @@
 
         """
         self._confirm_user_database_created()
         if not self.is_signed_in():
             error("No user is signed in.")
             return False
         if self._user_db_type == "sql":
+            if not key in current_user.__table__.columns:
+                error(f"'{key}' was not added as a column in users table")
+                return False
             setattr(current_user, key, value)
             self._db.session.commit()
             return True
         elif self._user_db_type == "firebase":
             self._firebase_db.document(self._user_vars._get("user-id")).update({key: value})
             return True
         
@@ -793,22 +828,27 @@
         """
         self._auth = BasicAuth(self.flask_app)
         self.flask_app.config['BASIC_AUTH_USERNAME'] = username
         self.flask_app.config['BASIC_AUTH_PASSWORD'] = password
 
     def set_ws_validation(self, func):
         """
-        Validate `simple_websocket.ws.Server` object before sending and accepting data.
+        Validates a WebSocket connection before sending and accepting data.
 
         ToUI uses Flask-Sock for websocket communication. Flask-Sock generates a
-        `simple_websocket.ws.Server` object when a connection is established. If you
-        wanted to access this object before sending and receiving data, input a function
-        that has one argument `ws`. This function should either return ``True`` or ``False``.
-        If the function returns ``False``, no data will be sent or received using ToUI with
-        the client.
+        `simple_websocket.ws.Server <https://simple-websocket.readthedocs.io/en/latest/api.html#the-server-class>`_
+        object when a connection is established. If you wanted to access this object before
+        sending and receiving data, input a function that has one argument `ws`. This function
+        should either return ``True`` or ``False``. If the function returns ``False``, no data
+        will be sent or received using ToUI with the client.
+
+        The `ws` argument is a `simple_websocket.ws.Server` object which you can learn about in its
+        `documentation <https://simple-websocket.readthedocs.io/en/latest/api.html#the-server-class>`_.
+        You might need to do some testing in order to explore the types of data that you can find in
+        this object.
 
         Parameters
         ----------
         func: Callable
             A function that validates the Server object. It should have one argument `ws` and
             should either return ``True`` or ``False``.
 
@@ -818,15 +858,15 @@
         simple_websockets
 
         """
         self._validate_ws = func
 
     def set_data_validation(self, func):
         """
-        Validate data received from JavaScript before using it.
+        Validates data received from JavaScript before using it.
 
         ToUI receives data from JavaScript in the form of a JSON object. To validate this data
         before allowing ToUI to use it, input a function that checks the data. This function
         should have one argument `data` and should either return ``True`` or ``False``.
         If the function returns ``False``, the data will not be used by ToUI.
 
         You can check the structures of the data received from JavaScript in
```

### Comparing `toui-3.0.4/toui/elements.py` & `toui-3.1.0/toui/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,15 +349,18 @@
         str
          If the attribute exists.
 
         None
             If the attribute does not exist.
 
         """
-        return self._element.attrs.get(name)
+        value = self._element.attrs.get(name)
+        if type(value) == list:
+            value = ' '.join(value)
+        return value
 
     @_ElementSignal()
     def set_attr(self, name, value):
         """
         Sets the value of an HTML element attribute.
 
         Parameters
```

### Comparing `toui-3.0.4/toui/pages.py` & `toui-3.1.0/toui/pages.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,26 +151,28 @@
         self._app = None
         self._signal_mode = False
         self._signals = []
         self._functions = {}
         self._view_func = self._on_url_request
         self._uid = None
         self._navigation_bar = ""
+        self._footer = ""
 
     def __str__(self):
         return self.to_str()
 
     def __repr__(self):
         return self.to_str()
 
     def __copy__(self):
         new_pg = Page(html_file=self._html_file, url=self.url)
         new_pg.from_bs4_soup(self.to_bs4_soup())
         new_pg._signal_mode = self._signal_mode
         new_pg._navigation_bar = self._navigation_bar
+        new_pg._footer = self._footer
         new_pg._app = self._app
         return new_pg
     
     @_PageSignal()
     def from_str(self, html_str):
         """
         Converts HTML code to a `Page` object.
@@ -482,29 +484,59 @@
             If ``True``, the browser will display the return value of the function when the URL is loaded. If ``False``,
             the return value will be ignored.
 
         """
         new_func = lambda: self._on_url_request(func=func, display_return_value=display_return_value)
         self._view_func = new_func
 
-    def set_navigation_bar(self, html_str):
+    def set_navigation_bar(self, html_file=None, html_str=None):
         """
         Adds a navigation bar to the page.
 
         Parameters
         ----------
-        html_str: str
+        html_file: str, default=None
+            Path to the HTML file that contains the navigation bar.
+
+        html_str: str, default=None
             HTML code of the navigation bar.
 
         Returns
         -------
         None
 
         """
-        self._navigation_bar = html_str
+        if html_file is not None:
+            with open(html_file, "r") as f:
+                self._navigation_bar = f.read()
+        if html_str is not None:
+            self._navigation_bar = html_str
+
+    def set_footer(self, html_file=None, html_str=None):
+        """
+        Adds a footer to the page.
+
+        Parameters
+        ----------
+        html_file: str, default=None
+            Path to the HTML file that contains the footer.
+
+        html_str: str
+            HTML code of the footer.
+
+        Returns
+        -------
+        None
+
+        """
+        if html_file is not None:
+            with open(html_file, "r") as f:
+                self._footer = f.read()
+        if html_str is not None:
+            self._footer = html_str
 
     def get_window(self):
         for window in webview.windows:
             if window.uid == self._uid:
                 return window
             
     def _on_url_request(self, func=None, display_return_value=False):
@@ -525,16 +557,17 @@
                         return response
                     else:   
                         return new_return
             pg = session['user page']
             body_element = pg.get_body_element()
             if body_element:
                 body_element.set_content(pg._navigation_bar + body_element.to_str()) 
+                body_element.add_content(pg._footer)
             else:
-                pg.from_str(pg._navigation_bar + pg.to_str())
+                pg.from_str(pg._navigation_bar + pg.to_str() + pg._footer)
             del session['user page']
             if "toui-response" in session:
                 response = session['toui-response']
                 response.set_data(pg.to_str())
                 del session['toui-response']
                 return response
             else:
```

### Comparing `toui-3.0.4/toui/structure.py` & `toui-3.1.0/toui/structure.py`

 * *Files identical despite different names*

### Comparing `toui-3.0.4/toui.egg-info/PKG-INFO` & `toui-3.1.0/toui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 3.0.4
+Version: 3.1.0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Author: Mubarak Almehairbi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `toui-3.0.4/toui.egg-info/SOURCES.txt` & `toui-3.1.0/toui.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 setup.py
 examples/__init__.py
 examples/advanced_example_1_toui_blueprint.py
 examples/advanced_example_2_toui_with_javascript.py
 examples/advanced_example_3_toui_with_google_sign_in.py
 examples/advanced_example_4_toui_with_firebase.py
+examples/advanced_example_5_toui_with_sql_user_database.py
 examples/example_1_simple_website.py
 examples/example_2_simple_desktop_app.py
 examples/example_3_updating_page.py
 examples/example_4_function_with_arg.py
 examples/example_5_user_variables.py
 examples/example_6_quick_website.py
 examples/example_7_quick_desktop_app.py
```

