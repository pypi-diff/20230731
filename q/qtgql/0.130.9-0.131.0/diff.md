# Comparing `tmp/qtgql-0.130.9.tar.gz` & `tmp/qtgql-0.131.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.130.9.tar", max compression
+gzip compressed data, was "qtgql-0.131.0.tar", max compression
```

## Comparing `qtgql-0.130.9.tar` & `qtgql-0.131.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1064 2023-07-24 05:56:03.969978 qtgql-0.130.9/LICENSE
--rw-r--r--   0        0        0     1116 2023-07-24 05:56:03.969978 qtgql-0.130.9/README.md
--rw-r--r--   0        0        0     4337 2023-07-24 05:56:39.378214 qtgql-0.130.9/pyproject.toml
--rw-r--r--   0        0        0       29 2023-07-24 05:56:40.282220 qtgql-0.130.9/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     2194 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0     2116 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/config.py
--rw-r--r--   0        0        0        0 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/core/__init__.py
--rw-r--r--   0        0        0     1708 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/core/cppref.py
--rw-r--r--   0        0        0       41 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/core/exceptions.py
--rw-r--r--   0        0        0     3393 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/core/graphql_ref.py
--rw-r--r--   0        0        0     1216 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/core/template.py
--rw-r--r--   0        0        0     3855 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/generator.py
--rw-r--r--   0        0        0        0 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/operation/__init__.py
--rw-r--r--   0        0        0     3877 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/operation/definitions.py
--rw-r--r--   0        0        0    16149 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/operation/evaluation.py
--rw-r--r--   0        0        0     4441 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/operation/selections_injection.py
--rw-r--r--   0        0        0      864 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/operation/template.py
--rw-r--r--   0        0        0     2208 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/operation/utils.py
--rw-r--r--   0        0        0        0 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/schema/__init__.py
--rw-r--r--   0        0        0     4600 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/schema/definitions.py
--rw-r--r--   0        0        0     8512 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/schema/evaluation.py
--rw-r--r--   0        0        0     1625 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/schema/template.py
--rw-r--r--   0        0        0     2019 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0     1699 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
--rw-r--r--   0        0        0     3629 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     2985 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
--rw-r--r--   0        0        0      448 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/templates/macros/iterate_type_condition.jinja.hpp
--rw-r--r--   0        0        0     1137 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp
--rw-r--r--   0        0        0     4791 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     4157 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp
--rw-r--r--   0        0        0     5052 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/templates/operation.jinja.cpp
--rw-r--r--   0        0        0     6692 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     3237 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0    18386 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/types.py
--rw-r--r--   0        0        0     1579 2023-07-24 05:56:03.985978 qtgql-0.130.9/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     2030 1970-01-01 00:00:00.000000 qtgql-0.130.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-31 06:39:39.488650 qtgql-0.131.0/LICENSE
+-rw-r--r--   0        0        0     1116 2023-07-31 06:39:39.488650 qtgql-0.131.0/README.md
+-rw-r--r--   0        0        0     4337 2023-07-31 06:40:14.224894 qtgql-0.131.0/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-07-31 06:40:15.164901 qtgql-0.131.0/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     2194 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0     2116 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/core/__init__.py
+-rw-r--r--   0        0        0     1708 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/core/cppref.py
+-rw-r--r--   0        0        0       41 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/core/exceptions.py
+-rw-r--r--   0        0        0     3393 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/core/graphql_ref.py
+-rw-r--r--   0        0        0     1216 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/core/template.py
+-rw-r--r--   0        0        0     3855 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/generator.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/operation/__init__.py
+-rw-r--r--   0        0        0     3877 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/operation/definitions.py
+-rw-r--r--   0        0        0    16149 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/operation/evaluation.py
+-rw-r--r--   0        0        0     4441 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/operation/selections_injection.py
+-rw-r--r--   0        0        0      864 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/operation/template.py
+-rw-r--r--   0        0        0     2208 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/operation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-07-31 06:39:39.500651 qtgql-0.131.0/qtgqlcodegen/schema/__init__.py
+-rw-r--r--   0        0        0     4600 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/schema/definitions.py
+-rw-r--r--   0        0        0     8512 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/schema/evaluation.py
+-rw-r--r--   0        0        0     1625 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/schema/template.py
+-rw-r--r--   0        0        0     2019 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0     1699 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     3629 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     2985 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
+-rw-r--r--   0        0        0      448 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/templates/macros/iterate_type_condition.jinja.hpp
+-rw-r--r--   0        0        0     1137 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     4791 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     4164 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp
+-rw-r--r--   0        0        0     5052 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/templates/operation.jinja.cpp
+-rw-r--r--   0        0        0     6471 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     3237 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0    18386 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/types.py
+-rw-r--r--   0        0        0     1579 2023-07-31 06:39:39.504651 qtgql-0.131.0/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     2030 1970-01-01 00:00:00.000000 qtgql-0.131.0/PKG-INFO
```

### Comparing `qtgql-0.130.9/LICENSE` & `qtgql-0.131.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/README.md` & `qtgql-0.131.0/README.md`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/pyproject.toml` & `qtgql-0.131.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.130.9"
+version = "0.131.0"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qtgql-0.130.9/qtgqlcodegen/cli.py` & `qtgql-0.131.0/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/qtgqlcodegen/config.py` & `qtgql-0.131.0/qtgqlcodegen/config.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/qtgqlcodegen/core/cppref.py` & `qtgql-0.131.0/qtgqlcodegen/core/cppref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/qtgqlcodegen/core/graphql_ref.py` & `qtgql-0.131.0/qtgqlcodegen/core/graphql_ref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/qtgqlcodegen/core/template.py` & `qtgql-0.131.0/qtgqlcodegen/core/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/qtgqlcodegen/generator.py` & `qtgql-0.131.0/qtgqlcodegen/generator.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/qtgqlcodegen/operation/definitions.py` & `qtgql-0.131.0/qtgqlcodegen/operation/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/qtgqlcodegen/operation/evaluation.py` & `qtgql-0.131.0/qtgqlcodegen/operation/evaluation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/qtgqlcodegen/operation/selections_injection.py` & `qtgql-0.131.0/qtgqlcodegen/operation/selections_injection.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/qtgqlcodegen/operation/template.py` & `qtgql-0.131.0/qtgqlcodegen/operation/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/qtgqlcodegen/operation/utils.py` & `qtgql-0.131.0/qtgqlcodegen/operation/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/qtgqlcodegen/schema/definitions.py` & `qtgql-0.131.0/qtgqlcodegen/schema/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/qtgqlcodegen/schema/evaluation.py` & `qtgql-0.131.0/qtgqlcodegen/schema/evaluation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/qtgqlcodegen/schema/template.py` & `qtgql-0.131.0/qtgqlcodegen/schema/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/qtgqlcodegen/templates/CMakeLists.jinja.cmake` & `qtgql-0.131.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp` & `qtgql-0.131.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp` & `qtgql-0.131.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp` & `qtgql-0.131.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp` & `qtgql-0.131.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp` & `qtgql-0.131.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp` & `qtgql-0.131.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     auto new_data = 👉new_concrete👈;
     auto new_len = new_data.size();
     auto prev_len = 👉field.private_name👈->rowCount();
     if (new_len < prev_len){
         👉field.private_name👈->removeRows(prev_len - 1, prev_len - new_len);
     }
     for (int i = 0; i < new_len; i++){
-        auto concrete = new_data.at(i);
+        const auto& concrete = new_data.at(i);
     {% if field.type.of_type.is_queried_object_type -%}
         if (i > prev_len){
             👉field.private_name👈->insert(i, new 👉field.type.of_type.name👈(operation, concrete));
         } else {
             auto proxy_to_update = 👉field.private_name👈->get(i);
             if(proxy_to_update){
                 proxy_to_update->qtgql_replace_concrete(concrete);
```

### Comparing `qtgql-0.130.9/qtgqlcodegen/templates/operation.jinja.cpp` & `qtgql-0.131.0/qtgqlcodegen/templates/operation.jinja.cpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.131.0/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {%- from "macros/deserialize_concrete_field.jinja.hpp" import  deserialize_concrete_field -%}
 {%- from "macros/proxy_type_fields.jinja.hpp" import  proxy_type_fields -%}
 {%- from "macros/update_proxy_field.jinja.cpp" import  update_proxy_field -%}
 #pragma once
 #include "./schema.hpp"
-#include <qtgql/gqlwstransport/gqlwstransport.hpp>
+#include <qtgql/bases/bases.hpp>
 #include <QObject>
 #include <QtQml/qqmlregistration.h>
 
 namespace 👉 context.config.env_name 👈::👉context.ns👈{
 class 👉 context.operation.name 👈;
 
 namespace deserializers{
@@ -79,71 +79,66 @@
     __ret.insert("👉 var.name 👈",  👉 var.json_repr() 👈);
     }
     {% endfor -%}
     return __ret;
     }
 };
 
-class 👉 context.operation.name 👈: public qtgql::gqlwstransport::OperationHandlerABC{
+class 👉 context.operation.name 👈: public qtgql::bases::OperationHandlerABC{
     Q_OBJECT
     Q_PROPERTY(const 👉 context.operation.root_type.name 👈 * data READ data NOTIFY dataChanged);
     QML_ELEMENT
-    QML_UNCREATABLE("Must be instantiated as with shared.")
+    QML_UNCREATABLE("Must be instantiated as shared pointer.")
 
 std::optional<👉 context.operation.root_type.name 👈 *> m_data = {};
 
 
 
-inline const QString &ENV_NAME() override{
+inline const QString &ENV_NAME() final{
     static const auto ret = QString("👉 context.config.env_name 👈");
     return ret;
     }
 signals:
     void dataChanged();
 
 public:
 👉 context.operation.generated_variables_type 👈 vars_inst;
 
-👉 context.operation.name 👈(): qtgql::gqlwstransport::OperationHandlerABC(qtgql::gqlwstransport::GqlWsTrnsMsgWithID(qtgql::gqlwstransport::OperationPayload(
+👉 context.operation.name 👈(): qtgql::bases::OperationHandlerABC(qtgql::bases::GraphQLMessage(
         {%- for line in context.operation.query.splitlines() %}"👉 line 👈"{% endfor -%}
-        ))){
-m_message_template.op_id = m_operation_id;
-};
+        )){};
 
 
 QTGQL_STATIC_MAKE_SHARED(👉 context.operation.name 👈)
 
-inline const QUuid & operation_id() const override{
-return m_operation_id;
-}
 
 
-void on_next(const QJsonObject &message) override{
-    auto data = message.value("data").toObject();
+
+void on_next(const QJsonObject &data_) override{
     if (!m_data){
-        👉 context.operation.root_type.updater_name👈(👉 context.operation.root_type.concrete.name👈::instance(), data, this);
+        👉 context.operation.root_type.updater_name👈(👉 context.operation.root_type.concrete.name👈::instance(), data_, this);
         m_data = new 👉 context.operation.root_type.name👈(this);
         emit dataChanged();
     }
     else{
-        👉 context.operation.root_type.updater_name👈(👉 context.operation.root_type.concrete.name👈::instance(), data, this);
+        👉 context.operation.root_type.updater_name👈(👉 context.operation.root_type.concrete.name👈::instance(), data_, this);
     }
 }
 
 inline const 👉 context.operation.root_type.name 👈 * data() const{
     if (m_data){
         return m_data.value();
     }
     return nullptr;
 }
 
 {% if context.operation.variables %}
-void set_variables(👉 context.operation.generated_variables_type 👈 vars){
+void set_variables(const 👉 context.operation.generated_variables_type 👈 & vars){
 vars_inst = vars;
-m_variables = vars_inst.to_json();
+qtgql::bases::OperationHandlerABC::set_vars(vars_inst.to_json());
 }
 {% endif %}
 
 };
 
 {# // This class exists as an alias class to an operation for qml, since operations
 // must be created with shared pointers. -#}
```

### Comparing `qtgql-0.130.9/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.131.0/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/qtgqlcodegen/types.py` & `qtgql-0.131.0/qtgqlcodegen/types.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/qtgqlcodegen/utils.py` & `qtgql-0.131.0/qtgqlcodegen/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.130.9/PKG-INFO` & `qtgql-0.131.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.130.9
+Version: 0.131.0
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.8,<3.12
```

