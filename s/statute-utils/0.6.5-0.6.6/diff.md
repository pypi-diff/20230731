# Comparing `tmp/statute_utils-0.6.5.tar.gz` & `tmp/statute_utils-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statute_utils-0.6.5.tar", max compression
+gzip compressed data, was "statute_utils-0.6.6.tar", max compression
```

## Comparing `statute_utils-0.6.5.tar` & `statute_utils-0.6.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.6.5/LICENSE
--rw-r--r--   0        0        0     2825 2023-07-31 16:21:33.481263 statute_utils-0.6.5/README.md
--rw-r--r--   0        0        0     1461 2023-07-31 16:31:40.978664 statute_utils-0.6.5/pyproject.toml
--rw-r--r--   0        0        0      897 2023-07-29 18:29:16.464915 statute_utils-0.6.5/statute_utils/__init__.py
--rw-r--r--   0        0        0     3113 2023-07-30 00:42:26.232929 statute_utils-0.6.5/statute_utils/codification.py
--rw-r--r--   0        0        0      588 2023-07-16 08:01:39.314430 statute_utils-0.6.5/statute_utils/components/__init__.py
--rw-r--r--   0        0        0     6011 2023-07-29 18:29:59.938432 statute_utils-0.6.5/statute_utils/components/branch.py
--rw-r--r--   0        0        0     9721 2023-07-30 10:35:07.925035 statute_utils-0.6.5/statute_utils/components/builder.py
--rw-r--r--   0        0        0    12717 2023-07-30 01:34:15.178955 statute_utils-0.6.5/statute_utils/components/category.py
--rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.6.5/statute_utils/components/short.py
--rw-r--r--   0        0        0     3717 2023-07-16 05:41:42.450594 statute_utils-0.6.5/statute_utils/components/utils.py
--rw-r--r--   0        0        0     1288 2023-07-17 01:57:30.575440 statute_utils-0.6.5/statute_utils/config.py
--rw-r--r--   0        0        0     9858 2023-07-17 02:00:05.382207 statute_utils-0.6.5/statute_utils/main.py
--rw-r--r--   0        0        0     4170 2023-07-17 01:57:45.971391 statute_utils-0.6.5/statute_utils/models.py
--rw-r--r--   0        0        0     9892 2023-07-02 03:43:37.827535 statute_utils-0.6.5/statute_utils/models_names.py
--rw-r--r--   0        0        0     6699 2023-07-02 03:43:23.216281 statute_utils-0.6.5/statute_utils/models_serials.py
--rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.6.5/statute_utils/recipes/__init__.py
--rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.6.5/statute_utils/recipes/const.py
--rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.6.5/statute_utils/recipes/digits.py
--rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.6.5/statute_utils/recipes/roc.py
--rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.6.5/statute_utils/recipes/spain.py
--rw-r--r--   0        0        0     6696 2023-07-30 01:34:59.725837 statute_utils-0.6.5/statute_utils/statute.py
--rw-r--r--   0        0        0     1851 2023-07-16 08:51:22.676004 statute_utils-0.6.5/statute_utils/templater.py
--rw-r--r--   0        0        0      208 2023-07-16 07:34:21.108245 statute_utils-0.6.5/statute_utils/templates/crumbs.html
--rw-r--r--   0        0        0      164 2023-07-16 07:29:47.336036 statute_utils-0.6.5/statute_utils/templates/paragraph.html
--rw-r--r--   0        0        0      200 2023-07-16 07:34:28.065021 statute_utils-0.6.5/statute_utils/templates/subtree.html
--rw-r--r--   0        0        0     1117 2023-07-16 09:00:07.666662 statute_utils-0.6.5/statute_utils/templates/tree.css
--rw-r--r--   0        0        0     3150 2023-07-31 16:27:29.601172 statute_utils-0.6.5/statute_utils/templates/tree.html
--rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 statute_utils-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.6.6/LICENSE
+-rw-r--r--   0        0        0     2825 2023-07-31 16:21:33.481263 statute_utils-0.6.6/README.md
+-rw-r--r--   0        0        0     1461 2023-07-31 17:00:13.670540 statute_utils-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0      897 2023-07-29 18:29:16.464915 statute_utils-0.6.6/statute_utils/__init__.py
+-rw-r--r--   0        0        0     3113 2023-07-30 00:42:26.232929 statute_utils-0.6.6/statute_utils/codification.py
+-rw-r--r--   0        0        0      588 2023-07-16 08:01:39.314430 statute_utils-0.6.6/statute_utils/components/__init__.py
+-rw-r--r--   0        0        0     6011 2023-07-29 18:29:59.938432 statute_utils-0.6.6/statute_utils/components/branch.py
+-rw-r--r--   0        0        0     9721 2023-07-30 10:35:07.925035 statute_utils-0.6.6/statute_utils/components/builder.py
+-rw-r--r--   0        0        0    12717 2023-07-30 01:34:15.178955 statute_utils-0.6.6/statute_utils/components/category.py
+-rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.6.6/statute_utils/components/short.py
+-rw-r--r--   0        0        0     3717 2023-07-16 05:41:42.450594 statute_utils-0.6.6/statute_utils/components/utils.py
+-rw-r--r--   0        0        0     1288 2023-07-17 01:57:30.575440 statute_utils-0.6.6/statute_utils/config.py
+-rw-r--r--   0        0        0     9858 2023-07-17 02:00:05.382207 statute_utils-0.6.6/statute_utils/main.py
+-rw-r--r--   0        0        0     4170 2023-07-17 01:57:45.971391 statute_utils-0.6.6/statute_utils/models.py
+-rw-r--r--   0        0        0     9892 2023-07-02 03:43:37.827535 statute_utils-0.6.6/statute_utils/models_names.py
+-rw-r--r--   0        0        0     6699 2023-07-02 03:43:23.216281 statute_utils-0.6.6/statute_utils/models_serials.py
+-rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.6.6/statute_utils/recipes/__init__.py
+-rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.6.6/statute_utils/recipes/const.py
+-rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.6.6/statute_utils/recipes/digits.py
+-rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.6.6/statute_utils/recipes/roc.py
+-rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.6.6/statute_utils/recipes/spain.py
+-rw-r--r--   0        0        0     6696 2023-07-30 01:34:59.725837 statute_utils-0.6.6/statute_utils/statute.py
+-rw-r--r--   0        0        0     1851 2023-07-16 08:51:22.676004 statute_utils-0.6.6/statute_utils/templater.py
+-rw-r--r--   0        0        0      208 2023-07-16 07:34:21.108245 statute_utils-0.6.6/statute_utils/templates/crumbs.html
+-rw-r--r--   0        0        0      164 2023-07-16 07:29:47.336036 statute_utils-0.6.6/statute_utils/templates/paragraph.html
+-rw-r--r--   0        0        0      200 2023-07-16 07:34:28.065021 statute_utils-0.6.6/statute_utils/templates/subtree.html
+-rw-r--r--   0        0        0     1117 2023-07-16 09:00:07.666662 statute_utils-0.6.6/statute_utils/templates/tree.css
+-rw-r--r--   0        0        0     3076 2023-07-31 17:02:13.294454 statute_utils-0.6.6/statute_utils/templates/tree.html
+-rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 statute_utils-0.6.6/PKG-INFO
```

### Comparing `statute_utils-0.6.5/LICENSE` & `statute_utils-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.5/README.md` & `statute_utils-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.5/pyproject.toml` & `statute_utils-0.6.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "statute-utils"
-version = "0.6.5"
+version = "0.6.6"
 description = "Philippine statutory law pattern matching and unit retrieval."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 readme = "README.md"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/statute-utils"
 documentation = "https://justmars.github.io/statute-utils"
 classifiers = [
```

### Comparing `statute_utils-0.6.5/statute_utils/__init__.py` & `statute_utils-0.6.6/statute_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.5/statute_utils/codification.py` & `statute_utils-0.6.6/statute_utils/codification.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.5/statute_utils/components/__init__.py` & `statute_utils-0.6.6/statute_utils/components/__init__.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.5/statute_utils/components/branch.py` & `statute_utils-0.6.6/statute_utils/components/branch.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.5/statute_utils/components/builder.py` & `statute_utils-0.6.6/statute_utils/components/builder.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.5/statute_utils/components/category.py` & `statute_utils-0.6.6/statute_utils/components/category.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.5/statute_utils/components/short.py` & `statute_utils-0.6.6/statute_utils/components/short.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.5/statute_utils/components/utils.py` & `statute_utils-0.6.6/statute_utils/components/utils.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.5/statute_utils/config.py` & `statute_utils-0.6.6/statute_utils/config.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.5/statute_utils/main.py` & `statute_utils-0.6.6/statute_utils/main.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.5/statute_utils/models.py` & `statute_utils-0.6.6/statute_utils/models.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.5/statute_utils/models_names.py` & `statute_utils-0.6.6/statute_utils/models_names.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.5/statute_utils/models_serials.py` & `statute_utils-0.6.6/statute_utils/models_serials.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.5/statute_utils/recipes/digits.py` & `statute_utils-0.6.6/statute_utils/recipes/digits.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.5/statute_utils/recipes/spain.py` & `statute_utils-0.6.6/statute_utils/recipes/spain.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.5/statute_utils/statute.py` & `statute_utils-0.6.6/statute_utils/statute.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.5/statute_utils/templater.py` & `statute_utils-0.6.6/statute_utils/templater.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.5/statute_utils/templates/tree.css` & `statute_utils-0.6.6/statute_utils/templates/tree.css`

 * *Files identical despite different names*

### Comparing `statute_utils-0.6.5/statute_utils/templates/tree.html` & `statute_utils-0.6.6/statute_utils/templates/tree.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,93 +1,87 @@
 {# BRANCHING #}
 
 {%- macro summarize(unit) -%}
   {# The label class is added to style the combination of item + caption in styles.css #}
   {%- set clean_item = unit.item|default('Container')|string -%}
   {%- if clean_item|is_hidden -%}
-    {%- if unit.caption -%}
+    {% if unit.caption -%}
       <a class="label" data-slug="{{unit.id|set_mp_slug}}">
         <strong >{{unit.caption}}</strong>
       </a>
-    {%- endif -%}
+    {%- endif %}
   {%- else -%}
     <a class="label" data-slug="{{unit.id|set_mp_slug}}">
       <strong>{{clean_item}}</strong>
-      {%- if unit.caption -%}
+      {% if unit.caption -%}
         &nbsp;<em>{{unit.caption}}</em>{# Using literal &nbsp; (instead of adding a css style) makes converting from html to text easier. #}
-      {%- endif -%}
+      {%- endif %}
     </a>
   {%- endif -%}
 {%- endmacro -%}
 
 {%- macro create_branch(unit) -%}
   {{ summarize(unit)}} {# Create the label based on <strong> and <em> tags #}
-  {%- if unit.content -%}
+  {% if unit.content -%}
     {{unit.content|trim|safe|md_to_html }} {# Needs to be safe since some unit content may have html #}
-  {%- endif -%}
-  {% if unit|is_par %}
+  {%- endif %}
+  {% if unit|is_par -%}
     <a data-slug="{{unit.id|set_mp_slug}}" data-item="{{unit.item}}" class="par-branch"></a>
-  {% endif %}
+  {%- endif %}
 {%- endmacro -%}
 
 {%- macro create_branches(units) -%}
-  {%- if units -%}
+  {% if units -%}
     <ul>
       {%- for unit in units -%}
-        <li data-slug="{{unit.id|set_mp_slug}}" {#- id for branching -#}
-          {%- if unit|is_par %}
-            data-par="true" {#- helps indention via css -#}
-          {% endif -%}
-
+        <li data-slug="{{unit.id|set_mp_slug}}"
+          {%- if unit|is_par %}data-par="true"{% endif -%}
           {%- if unit|has_history %}
             data-last-history-action="{{unit|get_last_action}}"
             data-last-history-category="{{unit|get_last_category}}"
             data-last-history-cause="{{unit|get_last_cause}}"
-          {% endif -%}
-
-          {% if unit|get_last_action == "Originated" %}
-            title="{{unit|get_last_cause}} originates from older statute."
-          {% else %}
-            title="{{unit|get_last_action|lower}} in {{unit|get_last_cause}}"
-          {% endif %}
-        >
+            {% if unit|get_last_action == "Originated" %}
+              title="{{unit|get_last_cause}} originates from older statute."
+            {% else %}
+              title="{{unit|get_last_action|lower}} in {{unit|get_last_cause}}."
+            {% endif %}
+          {% endif -%}>
           {{ create_branch(unit) }}
           {%- set target_units = unit.units|from_json -%}
-
           {%- if target_units -%}
             {# determine whether par. 1 is in next ul tag or ul to start with par. 2.. #}
             {%- set child = target_units[0] -%}
             {%- if child|is_first_par -%}
               {{ create_branch(child) }}
               {{ create_branches(child.units) }}
               {% if target_units|length > 1 -%}
                 {%- set target_units = target_units[1:] -%}
                 {{ create_branches(target_units) }}
               {%- endif -%}
-            {% else %}
+            {%- else -%}
               {{ create_branches(target_units) }}
             {%- endif -%}
           {%- endif -%}
         </li>
       {%- endfor -%}
     </ul>
-  {%- endif -%}
+  {%- endif %}
 {%- endmacro -%}
 
 {%- macro connect_breadcrumbs(units) -%}
   <span class="crumbs">
     {% for unit in units -%}
       <span class="crumb">
         {{ unit|crumb }}
       </span>
     {%- endfor %}
   </span>
 {%- endmacro -%}
 
 {%- macro create_paragraphs(units) -%}
-{% if units %}
-  {%- for unit in units -%}
-    {{ unit|paragrapher }}
-    {{ create_paragraphs(unit.units|from_json) }}
-  {%- endfor -%}
-{% endif %}
+  {% if units -%}
+    {% for unit in units -%}
+      {{ unit|paragrapher }}
+      {{ create_paragraphs(unit.units|from_json) }}
+    {%- endfor %}
+  {%- endif %}
 {%- endmacro -%}
```

### Comparing `statute_utils-0.6.5/PKG-INFO` & `statute_utils-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statute-utils
-Version: 0.6.5
+Version: 0.6.6
 Summary: Philippine statutory law pattern matching and unit retrieval.
 Home-page: https://lawsql.com
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
```

