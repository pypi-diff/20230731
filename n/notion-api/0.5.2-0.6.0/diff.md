# Comparing `tmp/notion_api-0.5.2.tar.gz` & `tmp/notion_api-0.6.0.tar.gz`

## Comparing `notion_api-0.5.2.tar` & `notion_api-0.6.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0    13237 2020-02-02 00:00:00.000000 notion_api-0.5.2/README.md
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/py.typed
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/api/__init__.py
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/api/_about.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/api/_pkgv.py
--rw-r--r--   0        0        0     5950 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/api/blockmixin.py
--rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/api/client.py
--rw-r--r--   0        0        0    30361 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/api/notionblock.py
--rw-r--r--   0        0        0    25951 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/api/notiondatabase.py
--rw-r--r--   0        0        0    20093 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/api/notionpage.py
--rw-r--r--   0        0        0    13799 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/api/notionworkspace.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/api/block_ext/__init__.py
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/api/block_ext/code.py
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/api/block_ext/equation.py
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/api/block_ext/richtext.py
--rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/api/block_ext/table.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/api/block_ext/todo.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/exceptions/__init__.py
--rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/exceptions/errors.py
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/exceptions/validate.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/properties/__init__.py
--rw-r--r--   0        0        0    15294 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/properties/blocktypes.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/properties/build.py
--rw-r--r--   0        0        0     6660 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/properties/common.py
--rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/properties/files.py
--rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/properties/options.py
--rw-r--r--   0        0        0    14699 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/properties/propertyobjects.py
--rw-r--r--   0        0        0    14347 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/properties/propertyvalues.py
--rw-r--r--   0        0        0     7878 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/properties/richtext.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/propertyitems/__init__.py
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/propertyitems/base.py
--rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/propertyitems/call.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/query/__init__.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/query/compound.py
--rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/query/conditions.py
--rw-r--r--   0        0        0     7493 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/query/propfilter.py
--rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/query/sort.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 notion_api-0.5.2/notion/query/timestamp.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 notion_api-0.5.2/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 notion_api-0.5.2/LICENSE
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 notion_api-0.5.2/pyproject.toml
--rw-r--r--   0        0        0    14701 2020-02-02 00:00:00.000000 notion_api-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    14328 2020-02-02 00:00:00.000000 notion_api-0.6.0/README.md
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/py.typed
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/api/__init__.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/api/_about.py
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/api/_pagination.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/api/_pkgv.py
+-rw-r--r--   0        0        0     5814 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/api/blockmixin.py
+-rw-r--r--   0        0        0     6130 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/api/client.py
+-rw-r--r--   0        0        0    31042 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/api/notionblock.py
+-rw-r--r--   0        0        0    30258 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/api/notiondatabase.py
+-rw-r--r--   0        0        0    20217 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/api/notionpage.py
+-rw-r--r--   0        0        0    15951 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/api/notionworkspace.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/api/block_ext/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/api/block_ext/code.py
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/api/block_ext/equation.py
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/api/block_ext/richtext.py
+-rw-r--r--   0        0        0     5914 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/api/block_ext/table.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/api/block_ext/todo.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/exceptions/__init__.py
+-rw-r--r--   0        0        0     6656 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/exceptions/errors.py
+-rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/exceptions/validate.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/properties/__init__.py
+-rw-r--r--   0        0        0    15300 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/properties/blocktypes.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/properties/build.py
+-rw-r--r--   0        0        0     6660 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/properties/common.py
+-rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/properties/files.py
+-rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/properties/options.py
+-rw-r--r--   0        0        0    14640 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/properties/propertyobjects.py
+-rw-r--r--   0        0        0    14216 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/properties/propertyvalues.py
+-rw-r--r--   0        0        0     7618 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/properties/richtext.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/propertyitems/__init__.py
+-rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/propertyitems/base.py
+-rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/propertyitems/call.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/query/__init__.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/query/compound.py
+-rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/query/conditions.py
+-rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/query/propfilter.py
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/query/sort.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 notion_api-0.6.0/notion/query/timestamp.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 notion_api-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 notion_api-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 notion_api-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    15758 2020-02-02 00:00:00.000000 notion_api-0.6.0/PKG-INFO
```

### Comparing `notion_api-0.5.2/README.md` & `notion_api-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -21,56 +21,63 @@
 
 </p>
 
 __Disclaimer: This is an _unofficial_ package and has no affiliation with Notion.so__  
 
 A wrapper for Notion's API, aiming to simplify the dynamic nature of interacting with Notion.  
 README contains examples of the main functionality, including: creating Pages/Databases/Blocks, adding/removing/editing properties, retrieving property values, and database queries.  
-Some more in-depth walkthroughs can be be found in [`examples/`](https://github.com/ayvi-0001/notion-api/tree/main/examples)    
+Some more in-depth walkthroughs can be be found in [`examples/`](https://github.com/ayvi-0001/notion-api/tree/main/examples).    
 This package is not complete - new features will continue to be added, and current features may change.
 
 <br>
 
 <div border="0" align="center">
     <table>
         <tr>
             <td align="center"><b>Links: Notion API Updates</b></td>
         </tr>
             <td> <a href="https://developers.notion.com/reference/intro">API Reference</a></td><tr>
         </td>
             <td><a href="https://developers.notion.com/page/changelog">Notion API Changelog </img></a></tr>
             <td> <a href="https://www.notion.so/releases">Notion.so Releases</a></td></tr>
-            <td> <a href="https://developers.notion.com/page/notion-platform-roadmap">Notion Platform Roadmap</a></td>
         </tr>
     </table>
 </div>
 
+<br>
+
+If you haven't already, you'll need to setup a [Notion Integration](https://www.notion.so/my-integrations) and share specific pages/databases with the integration to interact with the API.  
+Information on integration types and setup can be found [here](https://developers.notion.com/docs/getting-started).
+
 ---
 
 ## Install
 ```
 pip install -U notion-api
 ```
 
 ## Usage
 ```py
 import dotenv
 
 import notion
 
-# client will check env variables for 'NOTION_TOKEN'
+# client will check for env var 'NOTION_TOKEN'
 dotenv.load_dotenv()  
 
 homepage = notion.Page('773b08ff38b44521b44b115827e850f2')
 parent_db = notion.Database(homepage.parent_id)
 
-# will also look for env var `TZ` to set the timezone for all notion objects. If not found, will default to local timezone.
+# will also look for env var `TZ` to set the default timezone. If not found, will default to local timezone.
 ```
 
-`__getitem__` searchs for page property values when indexing a Page, and for property objects when indexing a Database.
+Indexing a page will search for page property values, and indexing a Database will search for property objects.  
+A full list can be retrieved for both using;  
+- `retrieve()` method for a Page, with the optional `filter_properties` parameter.
+- `retrieve` attribute for a Database.
 
 ```py
 homepage['dependencies']
 # {
 #     "id": "WYYq",
 #     "type": "relation",
 #     "relation": [
@@ -120,31 +127,34 @@
 
 <p align="center"> <img src="https://github.com/ayvi-0001/notion-api/blob/main/examples/images/new_page.png?raw=true"> </p>
 
 <br>
 
 ## Creating Pages/Databases/Blocks
 
-The current version of the Notion api does not allow pages to be created to the parent `workspace`.  
-Create objects by passing an existing Page/Database instance as an arg to the `create` classmethods.
+Create objects by passing an existing Page/Database instance to the `create` classmethods.  
+The current version of the Notion api does not allow pages/databases to be created to the parent `workspace`.  
 
 ```py
 new_database = notion.Database.create(
     parent_instance=testpage,
     database_title="Example Database",
     name_column="page", # This is the column containing page names. Defaults to "Name".
     is_inline=True, # can also toggle inline with setters.
     description="Database description can go here.",
 )
 
 new_page = notion.Page.create(new_database, page_title="A new database row")
 ```
 
-Blocks are also created using the classmethods of `Block`. They all require a parent instance of either `Page` or `Block` to append the new block too.
-The newly created block is returned as an instance of `Block`, which can be used as the parent instance to a nested block. 
+Blocks are also created using classmethods. They require a parent instance of either `Page` or `Block` to append the new block too.
+The newly created block is returned as an instance of `Block`, which can be used as the parent instance to another nested block. 
+
+By default, blocks are appended to the bottom of the parent block.  
+To append the block somewhere else other than the bottom of the parent block, use the `after` parameter and set its value to the ID of the block that the new block should be appended after. The block_id used in the `after` paramater must still be a child to the parent instance.  
 ```py
 from notion import properties as prop
 
 # `original_synced_block` refers to the original synced block in the Notion UI.
 original_synced_block = notion.Block.original_synced_block(homepage)
 
 # Adding content to the synced block
@@ -210,15 +220,15 @@
                     bold=True,
                     italic=True,
                     underline=True,
                     color=prop.BlockColor.gray,
                 ),
             ),
             prop.RichText(":"),
-        ],
+        ]
     )
     # First method returned the newly created block that we append to here:
     notion.Block.paragraph(mentionblock, [prop.RichText(message)])
     notion.Block.divider(page)
 ```
 
 ```py
@@ -235,58 +245,61 @@
 
 The first argument for all database property methods is the name of the property,  
 If a property of that name does not exist, then a new property will be created. 
 If a property of that name already exists, but it's a different type than the method used - then the API will overwrite this and change the property object to the new type.  
 The original parameters will be saved if you decide to switch back (i.e. if you change a formula column to a select column, upon changing it back to a formula column, the original formula expression will still be there).   
 
 ```py
-new_database.formula_column("page id", expression="id()")
+new_database.formula_column("page_id", expression="id()")
 
 new_database.delete_property("url")
 
 new_database.multiselect_column(
-    "new options column",
+    "New Options Column",
     options=[
-        prop.Option("option-a", prop.PropertyColor.red),
-        prop.Option("option-b", prop.PropertyColor.green),
-        prop.Option("option-c", prop.PropertyColor.blue),
+        prop.Option("Option A", prop.PropertyColor.red),
+        prop.Option("Option B", prop.PropertyColor.green),
+        prop.Option("Option C", prop.PropertyColor.blue),
     ],
 )
 
 # if an option does not already exist, a new one will be created with a random color.
 # this is not true for `status` column types, which can only be edited via UI.
 
 new_page.set_multiselect("options", ["option-a", "option-b"])
 ```
 
 <br>
 
 ## Database Queries
 
 A single `notion.query.PropertyFilter` is equivalent to filtering one property type in Notion.
-To build filters equivalent to Notion's 'advanced filters', use `notion.query.CompoundFilter`.
+To build nested filters, use `notion.query.CompoundFilter` and group property filters chained together by `_and(...)` / `_or(...)`.
 
 The database method `query()` will return the raw response from the API.  
 The method `query_pages()` will extract the page ID for each object in the array of results, and return a list of `notion.Page` objects.
 
+> note: in v0.6.0, new query methods were added: `query_all()` & `query_all_pages()` - these handle pagination, and instead of providing the `next_cursor` and `has_more` keys,
+> they will iterate through all the results, or up to the `max_page_size` paramater. These 2 methods will replace the original ones in a later update.
+
 ```py
 from datetime import datetime
 from datetime import timedelta
 
 from notion import query
 
 TODAY = datetime.combine(datetime.today(), datetime.min.time())
 TOMORROW = TODAY + timedelta(1)
 
 query_filter = query.CompoundFilter()._and(
     query.PropertyFilter.date("date", "created_time", "on_or_after", TODAY.isoformat()),
     query.PropertyFilter.date("date", "created_time", "before", TOMORROW.isoformat()),
     query.CompoundFilter()._or(
         query.PropertyFilter.text("name", "title", "contains", "your page title"),
-        query.PropertyFilter.text("name", "title", "contains", "your other page title"),
+        query.PropertyFilter.text("name", "title", "contains", "your other page title")
     ),
 )
 
 query_sort = query.SortFilter(
     [
         query.PropertyValueSort.ascending("your property name"),
         query.EntryTimestampSort.created_time_descending(),
@@ -326,27 +339,29 @@
 File "c:\...\notion\exceptions\validate.py", line 48, in validate_response
     raise NotionValidationError(message)
 notion.exceptions.errors.NotionValidationError: body failed validation: body.an_incorrect_key should be not present, instead was `"value"`.
 Error 400: The request body does not match the schema for the expected parameters.
 ```
 
 Possible errors are:
+ - `NotionConflictError`
+ - `NotionDatabaseConnectionUnavailable`
+ - `NotionGatewayTimeout`
+ - `NotionInvalidGrant`
+ - `NotionInternalServerError`
  - `NotionInvalidJson`
- - `NotionInvalidRequestUrl`
  - `NotionInvalidRequest`
- - `NotionValidationError`
+ - `NotionInvalidRequestUrl`
  - `NotionMissingVersion`
- - `NotionUnauthorized`
- - `NotionRestrictedResource`
  - `NotionObjectNotFound`
- - `NotionConflictError`
  - `NotionRateLimited`
- - `NotionInternalServerError`
+ - `NotionRestrictedResource`
  - `NotionServiceUnavailable`
- - `NotionDatabaseConnectionUnavailable`
+ - `NotionUnauthorized`
+ - `NotionValidationError`
 
 A common error to look out for is `NotionObjectNotFound`. This error is often raised because your bot has not been added as a connection to the page. 
 
 <p align="center">
     <img src="https://github.com/ayvi-0001/notion-api/blob/main/examples/images/directory_add_connections.png?raw=true">  
 </p>
```

### Comparing `notion_api-0.5.2/notion/__init__.py` & `notion_api-0.6.0/notion/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,33 +32,28 @@
 
 #### Properties:
 >>> from notion import properties as prop
 
 #### Block Extensions:
 >>> notion.CodeBlock | notion.ToDoBlock | notion.EquationBlock | notion.RichTextBlock
 
----
-
-Uncomment `check_for_pkg_update` method to enable auto-update check.
-
 """
 from typing import Sequence
 
 from notion.api import Block, Database, Page, Workspace
 from notion.api._pkgv import check_for_pkg_update
 from notion.api.block_ext import (
     CodeBlock,
     EquationBlock,
     RichTextBlock,
     TableBlock,
     ToDoBlock,
 )
 
-# check_for_pkg_update()
-
+check_for_pkg_update()
 
 __all__: Sequence[str] = (
     "Page",
     "Database",
     "Block",
     "Workspace",
     "CodeBlock",
```

### Comparing `notion_api-0.5.2/notion/api/__init__.py` & `notion_api-0.6.0/notion/api/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.2/notion/api/_about.py` & `notion_api-0.6.0/notion/api/_about.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,28 +30,25 @@
     "__package_url__",
     "__package_json__",
 )
 
 __notion_version__: Final[str] = "2022-06-28"
 __content_type__: Final[str] = "application/json"
 __base_url__: Final[str] = "https://api.notion.com/v1/"
-__version__: Final[str] = "0.5.2"
+__version__: Final[str] = "0.6.0"
 __package_url__: Final[str] = "https://pypi.org/pypi/notion-api/"
 __package_json__: Final[str] = "https://pypi.org/pypi/notion-api/json"
 
 
 # Notion API Changlog
 # https://developers.notion.com/page/changelog
 
 # New changes to notion.so
 # https://www.notion.so/releases
 
-# Notion Platform Roadmap
-# https://developers.notion.com/page/notion-platform-roadmap
-
 # API Reference
 # https://developers.notion.com/reference/intro
 
 # Previous Notion-Version headers
 #  - "2021-05-11"
 #  - "2021-05-13"
 #  - "2021-08-16"
```

### Comparing `notion_api-0.5.2/notion/api/_pkgv.py` & `notion_api-0.6.0/notion/api/_pkgv.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,50 @@
+# mypy: disable-error-code="no-redef"
+
 import re
 from types import ModuleType
 from typing import Callable, Final, Pattern, Sequence, cast
 
 import requests
 
-from notion.api._about import *
+from notion.api._about import __package_json__, __package_url__, __version__
 from notion.api.client import _NLOG
 
 try:
     import orjson
 
-    default_json: ModuleType = orjson
+    _json: ModuleType = orjson
 except ModuleNotFoundError:
     import json
 
-    default_json: ModuleType = json
+    _json: ModuleType = json
 
 
 __all__: Sequence[str] = ["check_for_pkg_update"]
 
 
 get_version: Callable[[str], str] = lambda pkg: cast(
-    str, default_json.loads(requests.get(pkg).text)["info"]["version"]
+    str, _json.loads(requests.get(pkg).text)["info"]["version"]
 )
 
 
-def check_for_pkg_update() -> None:
-    """Check for package updates. Uncomment this function in `notion\__init__.py` to enable."""
+def check_for_pkg_update() -> bool | None:
     pkg_expr: Final[Pattern[str]] = re.compile(r"(\d).(\d)+.(\d)+", re.I)
 
     try:
         vPYPI = cast(re.Match[str], pkg_expr.match(get_version(__package_json__)))
         vPKG = cast(re.Match[str], pkg_expr.match(__version__))
 
         (pypi_major, pypi_minor, pypi_patch) = vPYPI.group(1, 2, 3)
         (pkg_major, pkg_minor, pkg_patch) = vPKG.group(1, 2, 3)
 
         pypi_version = (int(pypi_major), int(pypi_minor), int(pypi_patch))
         local_version = (int(pkg_major), int(pkg_minor), int(pkg_patch))
 
         if local_version < pypi_version:
             _NLOG.info(
-                "Newer package version available: %s - %s"
-                % (".".join(map(str, pypi_version)), __package_url__)
+                f"New package version available: {'.'.join(map(str, pypi_version))} - {__package_url__}"
             )
 
-        return None
+        return local_version < pypi_version
     except Exception:
         return None
```

### Comparing `notion_api-0.5.2/notion/api/blockmixin.py` & `notion_api-0.6.0/notion/api/blockmixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,20 +21,20 @@
 # SOFTWARE.
 
 from __future__ import annotations
 
 import os
 from datetime import datetime, tzinfo
 from functools import cached_property
-from typing import Any, MutableMapping, Optional, Sequence, Union, cast
+from typing import Any, MutableMapping, Optional, Sequence, cast
 
 from pytz import timezone
 from tzlocal import get_localzone_name
 
-from notion.api._about import *
+from notion.api._about import __base_url__
 from notion.api.client import _NotionClient
 
 LOCAL_TIMEZONE = get_localzone_name()
 
 
 __all__: Sequence[str] = ["_TokenBlockMixin"]
 
@@ -42,37 +42,30 @@
 class _TokenBlockMixin(_NotionClient):
     """
     Any object you interact with in Notion;
     Databases/Pages/individual child blocks, are all considered 'Blocks'
     This class assigns common attributes among all three types.
     """
 
-    def __init__(
-        self,
-        id: str,
-        /,
-        *,
-        token: Optional[str] = None,
-    ) -> None:
+    def __init__(self, id: str, /, *, token: Optional[str] = None) -> None:
         super().__init__(token=token)
 
         self.id: str = id.replace("-", "")
 
         try:
             self.tz = timezone(os.environ["TZ"])
         except KeyError:
             self.tz = timezone(LOCAL_TIMEZONE)
 
     def __repr__(self) -> str:
+        # This is to avoid certain errors occuring before the object is fully initialized
         id = getattr(self, "id", "")
-        # This is to avoid certain errors occuring
-        # before the object is fully initialized
         return f"notion.{self.__class__.__name__}('{id}')"
 
-    def set_tz(self, tz: Union[tzinfo, str]) -> None:
+    def set_tz(self, tz: tzinfo | str) -> None:
         """
         :param tz: (required) Set the instance timezone. Takes either str or pytz.timezone\
                     Use `pytz.all_timezones()` to retrieve list of tz options.\
                     Class will first check for environment variable `TZ`.\
                     If not found, class default checks the system-configured timezone.
         """
         if isinstance(tz, tzinfo):
@@ -80,15 +73,15 @@
         elif isinstance(tz, str):
             self.__setattr__("tz", timezone(tz))
 
     @cached_property
     def _block(self) -> MutableMapping[str, Any]:
         """
         Same result as retrieve() for notion.api.notionblock.Block.
-        If used with notion.api.notionpage.Page or notion.api.notiondatabase.Database,
+        If used with notion.Page or `notion.Database`,
         retrieves the page or database object from the blocks endpoint.
 
         https://developers.notion.com/reference/block#block-type-objects
         """
         return self._get(self._block_endpoint(self.id))
 
     @property
@@ -114,17 +107,17 @@
             return "workspace"
         return ptype
 
     @property
     def parent_id(self) -> str:
         _parent_id = self._block["parent"][self.parent_type]
         if _parent_id is True:  # parent is workspace
-            workspace = self._get("%s%s" % (__base_url__, "users/me"))
+            workspace = self._get(f"{__base_url__}users/me")
             # return workspace name
-            return "workspace-%s" % workspace["bot"]["workspace_name"]
+            return f"workspace:{workspace['bot']['workspace_name']}"
         else:
             return cast(str, _parent_id.replace("-", ""))
 
     @property
     def last_edited_time(self) -> datetime:
         """
         Returns date and time when this page/block/database was created.
@@ -147,15 +140,15 @@
         """
         dt = datetime.fromisoformat(self._block["created_time"])
         return dt.astimezone(tz=self.tz)
 
     @property
     def last_edited_by(self) -> str:
         user_id = self._block["last_edited_by"]["id"]
-        user = self._get("%s%s" % (__base_url__, "users/%s" % user_id))
+        user = self._get(f"{__base_url__}users/{user_id}")
         return cast(str, user)
 
     @property
     def created_by(self) -> str:
         user_id = self._block["created_by"]["id"]
-        user = self._get("%s%s" % (__base_url__, "users/%s" % user_id))
+        user = self._get(f"{__base_url__}users/{user_id}")
         return cast(str, user)
```

### Comparing `notion_api-0.5.2/notion/api/client.py` & `notion_api-0.6.0/notion/api/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,29 +16,31 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+# mypy: disable-error-code="no-redef"
+
 from __future__ import annotations
 
 import logging
 import os
 from types import ModuleType
-from typing import Any, MutableMapping, Optional, Sequence, Union, cast
+from typing import Any, MutableMapping, Optional, Sequence, cast
 
 try:
     import orjson
 
-    default_json: ModuleType = orjson
+    _json: ModuleType = orjson
 except ModuleNotFoundError:
     import json
 
-    default_json: ModuleType = json
+    _json: ModuleType = json
 
 import requests
 
 from notion.api._about import __base_url__, __content_type__
 from notion.exceptions import NotionUnauthorized, validate_response
 
 __all__: Sequence[str] = ["_NotionClient"]
@@ -47,140 +49,128 @@
 
 _NLOG = logging.getLogger("notion-api")
 
 
 class _NotionClient:
     """Base Class to inherit: token, headers, requests, and endpoints."""
 
-    def __init__(
-        self,
-        *,
-        token: Optional[str] = None,
-    ) -> None:
+    def __init__(self, *, token: Optional[str] = None) -> None:
         if token:
             self.token = token
         else:
             try:
                 self.token = os.environ["NOTION_TOKEN"]
             except KeyError:
                 raise NotionUnauthorized(
-                    "%s. %s."
-                    % (
-                        f"notion.{self.__class__.__name__}: Missing Token",
-                        "Check if `NOTION_TOKEN` is set in environment variables",
-                    )
+                    f"notion.{self.__class__.__name__}(): Missing Token. "
+                    "Check if `NOTION_TOKEN` is set in environment variables"
                 )
 
         try:
             __notion_version__ = os.environ["NOTION_VERSION"]
         except KeyError:
             from notion.api._about import __notion_version__
 
-        self.notion_version = __notion_version__
-
         __auth__ = f"Bearer {self.token}"
 
         self.headers: dict[str, str] = {
             "Authorization": __auth__,
             "Accept": __content_type__,
             "Content-type": __content_type__,
             "Notion-Version": __notion_version__,
         }
 
     @staticmethod
     def _block_endpoint(
-        object_id: Optional[str] = None,
+        block_id: Optional[str] = None,
         /,
         *,
-        children: Optional[bool] = None,
+        children: Optional[bool] = False,
         page_size: Optional[int] = None,
         start_cursor: Optional[str] = None,
     ) -> str:
-        return "%sblocks%s%s%s%s%s" % (
-            __base_url__,
-            f"/{object_id}" if object_id else "",
-            "/children" if children else "",
-            "?" if any([page_size, start_cursor]) else "",
-            f"&start_cursor={start_cursor}" if start_cursor else "",
-            f"&page_size={page_size}" if page_size else "",
+        return "".join(
+            [
+                __base_url__,
+                "blocks",
+                f"/{block_id}" if block_id else "",
+                "/children" if children else "",
+                "?" if any([page_size, start_cursor]) else "",
+                f"&start_cursor={start_cursor}" if start_cursor else "",
+                f"&page_size={page_size}" if page_size else "",
+            ]
         )
 
     @staticmethod
     def _database_endpoint(
-        object_id: Optional[str] = None, /, *, query: Optional[bool] = False
+        database_id: Optional[str] = None, /, *, query: Optional[bool] = False
     ) -> str:
-        return "%sdatabases%s%s" % (
-            __base_url__,
-            f"/{object_id}" if object_id else "",
-            "/query" if query else "",
+        return "".join(
+            [
+                __base_url__,
+                "databases",
+                f"/{database_id}" if database_id else "",
+                "/query" if query else "",
+            ]
         )
 
     @staticmethod
     def _pages_endpoint(
-        object_id: Optional[str] = None,
+        page_id: Optional[str] = None,
         /,
         *,
         properties: Optional[bool] = False,
         property_id: Optional[str] = None,
     ) -> str:
-        return "%spages%s%s%s" % (
-            __base_url__,
-            f"/{object_id}" if object_id else "",
-            "/properties" if properties else "",
-            f"/{property_id}" if property_id else "",
+        return "".join(
+            [
+                __base_url__,
+                "pages",
+                f"/{page_id}" if page_id else "",
+                "/properties" if properties else "",
+                f"/{property_id}" if property_id else "",
+            ]
         )
 
     def _get(
-        self,
-        url: str,
-        /,
-        *,
-        payload: Optional[Union[MutableMapping[str, Any], str, bytes, bytearray]] = None,
+        self, url: str, payload: MutableMapping[str, Any] | str | bytes | None = None
     ) -> MutableMapping[str, Any]:
         if not payload:
-            response = default_json.loads(requests.get(url, headers=self.headers).text)
+            response = _json.loads(requests.get(url, headers=self.headers).text)
         else:
             if isinstance(payload, dict):
-                payload = default_json.dumps(payload)
-            response = default_json.loads(
+                payload = _json.dumps(payload)
+            response = _json.loads(
                 requests.post(url, headers=self.headers, json=payload).text
             )
         validate_response(response)
         return cast(MutableMapping[str, Any], response)
 
     def _post(
-        self,
-        url: str,
-        /,
-        *,
-        payload: Optional[Union[MutableMapping[str, Any], str, bytes, bytearray]] = None,
+        self, url: str, payload: MutableMapping[str, Any] | str | bytes | None = None
     ) -> MutableMapping[str, Any]:
         if not payload:
-            response = default_json.loads(requests.post(url, headers=self.headers).text)
+            response = _json.loads(requests.post(url, headers=self.headers).text)
         else:
             if isinstance(payload, dict):
-                payload = default_json.dumps(payload)
-            response = default_json.loads(
+                payload = _json.dumps(payload)
+            response = _json.loads(
                 requests.post(url, headers=self.headers, data=payload).text
             )
         validate_response(response)
         return cast(MutableMapping[str, Any], response)
 
     def _patch(
-        self,
-        url: str,
-        /,
-        *,
-        payload: Union[MutableMapping[str, Any], str, bytes, bytearray],
+        self, url: str, payload: MutableMapping[str, Any] | str | bytes
     ) -> MutableMapping[str, Any]:
         if isinstance(payload, dict):
-            payload = default_json.dumps(payload)
-        response = default_json.loads(
+            payload = _json.dumps(payload)
+        response = _json.loads(
             requests.patch(url, headers=self.headers, data=payload).text
         )
         validate_response(response)
         return cast(MutableMapping[str, Any], response)
 
-    def _delete(self, url: str, /) -> MutableMapping[str, Any]:
-        response = default_json.loads(requests.delete(url, headers=self.headers).text)
+    def _delete(self, url: str) -> MutableMapping[str, Any]:
+        response = _json.loads(requests.delete(url, headers=self.headers).text)
         validate_response(response)
         return cast(MutableMapping[str, Any], response)
```

### Comparing `notion_api-0.5.2/notion/api/notionblock.py` & `notion_api-0.6.0/notion/api/notionblock.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,22 +15,21 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-""" 
-A block object represents content within Notion. Blocks can be text, lists, media, and more. A page is a type of block, too.
-Some blocks have more content nested inside them. Some examples are indented paragraphs, lists, and toggles. 
-The nested content is called children, and children are blocks, too.
-
+"""
+A block object represents a piece of content within Notion. 
+The API translates the headings, toggles, paragraphs, lists, media, and more that you can interact with in the Notion UI as different block type objects.
 Block types which support children are:
-    "paragraph", "bulleted_list_item", "numbered_list_item", "toggle", "to_do", "quote", "callout", 
-    "synced_block", "column", "child_page", "child_database", and "table". 
+    "paragraph", "bulleted_list_item", "numbered_list_item", "toggle", "to_do", "quote", "callout",
+    "synced_block", "column", "child_page", "child_database", and "table".
+    
     All heading blocks ("heading_1", "heading_2", and "heading_3") support children when the is_toggleable property is true.
 
 NOTE: The link_preview block will only be returned as part of a response. It cannot be created via the API.
 NOTE: As of March 27, 2023, Notion is no longer supporting the creation of template blocks. They are not included in this module.
 
 https://developers.notion.com/reference/block
 """
@@ -74,15 +73,15 @@
     TableOfContentsBlocktype,
     TableRowBlockType,
     ToDoBlocktype,
     ToggleBlocktype,
     VideoBlockType,
 )
 from notion.properties.options import BlockColor, CodeBlockLang
-from notion.properties.richtext import Equation, Mention, RichText
+from notion.properties.richtext import Mention, RichText
 
 if TYPE_CHECKING:
     from notion.api.notionpage import Page
 
 
 __all__: Sequence[str] = ["Block"]
 
@@ -90,37 +89,31 @@
 class Block(_TokenBlockMixin):
     """A block object represents content within Notion.
     Blocks can be text, lists, media, and more. A page is a type of block, too.
 
     These are the individual 'nodes' in a page that you typically interact with in Notion.
     Some blocks have more content nested inside them.
     Some examples are indented paragraphs, lists, and toggles.
-    The nested content is called children, and children are blocks, too. 
+    The nested content is called children, and children are blocks, too.
 
     ---
     ### Versioning:
     To use a previous version of the API, set the envrionment variable `NOTION_VERSION`.
     For more info see: https://developers.notion.com/reference/versioning
 
     ---
-    :param id: (required) `block_id` of object in Notion.
-    :param token: Bearer token provided when you create an integration.\
+    :param id:    (required) `block_id` of object in Notion.
+    :param token: (optional) Bearer token provided when you create an integration.\
                   Set notion secret in environment variables as `NOTION_TOKEN`, or set variable here.\
                   See https://developers.notion.com/reference/authentication.
 
     https://developers.notion.com/reference/block
     """
 
-    def __init__(
-        self,
-        id: str,
-        /,
-        *,
-        token: Optional[str] = None,
-    ) -> None:
+    def __init__(self, id: str, /, *, token: Optional[str] = None) -> None:
         super().__init__(id, token=token)
         self.logger = _NLOG.getChild(self.__repr__())
 
     @cached_property
     def retrieve(self) -> MutableMapping[str, Any]:
         """
         Retrieves a Block object using the ID specified.
@@ -147,23 +140,20 @@
         return self._get(
             self._block_endpoint(
                 self.id, children=True, page_size=page_size, start_cursor=start_cursor
             )
         )
 
     def _append(
-        self,
-        payload: MutableMapping[str, Any] | str | bytes | bytearray,
+        self, payload: MutableMapping[str, Any] | str | bytes | bytearray
     ) -> MutableMapping[str, Any]:
         """
         Creates/appends new children blocks to the parent block_id specified.
         Returns a paginated list of newly created children block objects.
 
-        Used internally by notion.api.blocktypefactory.target.
-
         https://developers.notion.com/reference/patch-block-children
         """
         return self._patch(self._block_endpoint(self.id, children=True), payload=payload)
 
     @property
     def delete_self(self) -> None:
         """
@@ -206,16 +196,15 @@
             return
 
         if children_id:
             for id in children_id:
                 self._delete(self._block_endpoint(id))
 
     def update(
-        self,
-        payload: MutableMapping[str, Any] | str | bytes | bytearray,
+        self, payload: MutableMapping[str, Any] | str | bytes | bytearray
     ) -> MutableMapping[str, Any]:
         """
         Updates content for the specified block_id based on the block
         type. Supported fields based on the block object type.
         Note: The update replaces the entire value for a given field.
         If a field is omitted (ex: omitting checked when updating a to_do block),
         the value will not be changed.
@@ -229,35 +218,33 @@
 
         https://developers.notion.com/reference/update-a-block
         """
         return self._patch(self._block_endpoint(self.id), payload=payload)
 
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ BLOCK FACTORY METHODS ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
 
-    # Factory to write block types as a child of the target
-    # `notion.api.notionblock.Block` or `notion.api.notionpage.Page`.
-    # Returns an instance of `notion.api.notionblock.Block`.
-
-    # Factory methods used to create a `Block` object.
-    # All methods require a parent instance of either
-    #   `notion.api.notionblock.Block` or `notion.api.notionpage.Page`
+    # Factory methods used to create and append new children blocks to the parent block_id specified.
+    # Blocks can be parented by other blocks, pages, or databases
+    # All methods require a parent instance of either notion.Block or notion.Page
+    # By default, blocks are appended to the bottom of the parent block.
+    # To append a block in a specific place other than the bottom of the parent block,
+    # use the "after" parameter and set its value to the ID of the block that the new block should be appended after.
+    # Once a block is appended as a child, it can't be moved elsewhere via the API.
 
     # Most methods return a `Block` object, which can be used to continously nest blocks.
     # For blocks that allow children, Notion allows up to two levels of nesting in a single request.
     # Each method of `Block` is a separate request to the API and is not affected by this limitation.
 
-    # Some methods return a specialized `Block` object, these are:
+    # Some methods return a specialized `Block` object, these include:
     # Codeblock, EquationBlock, TodoBlock, TableBlock, and RichTextBlock.
     # RichTextBlock refers to any block that contains text that can be formatted.
     # These are:  "paragraph", "to_do", "toggle", "quote", "callout"
     #             "bulleted_list_item", "numbered_list_item",
     #             "headings", "toggle_headings"
-
-    # See examples in repo for specific functions for blocks above,
-    # or docstrings in source code at `notion.api.notionblock.Block`
+    # See examples in repo for specific functions for blocks above.
 
     # Example
     # ```py
     # notion.Block.divider(
     #     notion.Block.paragraph(
     #         notion.Block.paragraph(
     #             notion.Block('87aadab8ce4b407682197c922e51511f'
@@ -273,15 +260,17 @@
     #         This is the child
     #             ---
     # ```
 
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ SYNCED BLOCK TYPES ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
 
     @classmethod
-    def original_synced_block(cls, parent_object: Page | Block) -> Block:
+    def original_synced_block(
+        cls, parent_object: Page | Block, after: Optional[str] = None
+    ) -> Block:
         """Creates an empty synced block that can be appended to other blocks with `notion.Block.duplicate_synced_block(...)`.
 
         ### Original Synced Block
         Similar to the UI, there are two versions of a synced_block --
         the original block that was created first and doesn't yet sync with anything else,
         and the reference blocks that are synced to the original synced block.
 
@@ -291,74 +280,78 @@
 
         Note that all of the blocks available to be synced in another synced_block must be captured in the children property.
 
         `synced_from` Value is always null to signify that this is an original synced block and that is not referring to another block
 
         https://developers.notion.com/reference/block#original-synced-block
 
-        :returns: A new `notion.api.notionblock.Block` object with the `block_id` of the original synced block.
+        :returns: A new `notion.api.Block` object with the `block_id` of the original synced block.
         """
         block_mapping = parent_object._append(
-            BlockChildren([OriginalSyncedBlockType(children=[])])
+            BlockChildren([OriginalSyncedBlockType(children=[])], after=after)
         )
-        original_synced_block = cls(_result_id(block_mapping))
-        return original_synced_block
+        return cls(cast(str, block_mapping["results"][0]["id"]))
 
     @classmethod
-    def duplicate_synced_block(cls, parent_object: Page | Block, block_id: str) -> Block:
+    def duplicate_synced_block(
+        cls, parent_object: Page | Block, block_id: str, after: Optional[str] = None
+    ) -> Block:
         """### Reference Synced Block
         To sync the content of the original synced_block with another synced_block,
         the developer simply needs to refer to that synced_block using the synced_from property.
 
         Note that only "original" synced blocks can be referenced in the synced_from property.
 
         https://developers.notion.com/reference/block#duplicate-synced-block
 
         :param block_id: (required) string (UUIDv4). Identifier of an original synced_block
-        :returns: A new `notion.api.notionblock.Block` object with the `block_id` of the duplicate synced block.
+        :returns: A new `notion.api.Block` object with the `block_id` of the duplicate synced block.
         """
         block_mapping = parent_object._append(
-            BlockChildren([DuplicateSyncedBlockType(block_id)])
+            BlockChildren([DuplicateSyncedBlockType(block_id)], after=after)
         )
-        duplicate_synced_block = cls(_result_id(block_mapping))
-        return duplicate_synced_block
+        return cls(cast(str, block_mapping["results"][0]["id"]))
 
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ BLOCK EXTENSIONS ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # ~~~~~~~~~~~ These return custom blocks with unique methods to their block type ~~~~~~~~~~~ #
 
     @staticmethod
     def code(
         parent_object: Page | Block,
         code_text: Optional[str] = None,
-        /,
         *,
         language: Optional[CodeBlockLang | str] = None,
         caption: Optional[Sequence[RichText | Mention | str]] = None,
+        after: Optional[str] = None,
     ) -> CodeBlock:
         """Creates a code block. https://developers.notion.com/reference/block#code-blocks
 
         :returns: `notion.api.block_ext.CodeBlock` object.
         :raises: NotionValidationError if code block is >= 2000 characters.
         """
         block_mapping = parent_object._append(
             BlockChildren(
-                [CodeBlocktype([RichText(code_text)], language=language, caption=caption)]
-            ),
+                [
+                    CodeBlocktype(
+                        [RichText(code_text)], language=language, caption=caption
+                    )
+                ],
+                after=after,
+            )
         )
-        code_block = CodeBlock(_result_id(block_mapping))
-        return code_block
+        return CodeBlock(cast(str, block_mapping["results"][0]["id"]))
 
     @staticmethod
     def table(
         parent_object: Page | Block,
-        /,
         *,
         table_width: int = 2,
         has_column_header: bool = False,
         has_row_header: bool = False,
+        after: Optional[str] = None,
     ) -> TableBlock:
         """
         Note that the number of columns in a table can only be set when the table is first created.
         Calls to the Update block endpoint to update table_width fail.
         See examples in repo for more details.
 
         Table:      https://developers.notion.com/reference/block#table
@@ -375,271 +368,278 @@
         """
         cells: CELLS_ARRAY = [[] for _ in range(table_width)]
         rows = [TableRowBlockType(cells)]
         block_mapping = parent_object._append(
             BlockChildren(
                 [
                     TableBlockType(
-                        table_width,
-                        has_column_header,
-                        has_row_header,
-                        children=rows,
+                        table_width, has_column_header, has_row_header, children=rows
                     )
-                ]
+                ],
+                after=after,
             )
         )
-        table_block = TableBlock(_result_id(block_mapping))
-        return table_block
+        return TableBlock(cast(str, block_mapping["results"][0]["id"]))
 
     @staticmethod
     def to_do(
         parent_object: Page | Block,
         rich_text: Sequence[RichText | Mention],
-        /,
         *,
         block_color: Optional[BlockColor | str] = None,
         checked: Optional[bool] = False,
+        after: Optional[str] = None,
     ) -> ToDoBlock:
         """Creates a to-do block. https://developers.notion.com/reference/block#to-do-blocks
 
         :returns: `notion.api.block.ToDoBlock` object.
         """
         block_mapping = parent_object._append(
             BlockChildren(
-                [ToDoBlocktype(rich_text, block_color=block_color, checked=checked)]
-            ),
+                [ToDoBlocktype(rich_text, block_color=block_color, checked=checked)],
+                after=after,
+            )
         )
-        to_do_block = ToDoBlock(_result_id(block_mapping))
-        return to_do_block
+        return ToDoBlock(cast(str, block_mapping["results"][0]["id"]))
 
     @staticmethod
-    def equation(parent_object: Page | Block, expression: str, /) -> EquationBlock:
+    def equation(
+        parent_object: Page | Block, expression: str, /, *, after: Optional[str] = None
+    ) -> EquationBlock:
         """Creates an equation block. https://developers.notion.com/reference/block#equation-blocks
 
         :param expression: (required) A KaTeX compatible string.
-        :returns: `notion.api.notionblock.Block`
+        :returns: `notion.api.Block`
         """
-
         block_mapping = parent_object._append(
-            BlockChildren([EquationBlocktype(expression)])
+            BlockChildren([EquationBlocktype(expression)], after=after)
         )
-        equation_block = EquationBlock(_result_id(block_mapping))
-        return equation_block
+        return EquationBlock(cast(str, block_mapping["results"][0]["id"]))
 
     # ~~~~~~~~~~~~~~ TEXT-EDITABLE BLOCKS (Can be used by `notion.RichTextBlock`) ~~~~~~~~~~~~~~ #
 
     @classmethod
     def paragraph(
         cls,
         parent_object: Page | Block,
         rich_text: Sequence[RichText | Mention],
-        /,
         *,
+        after: Optional[str] = None,
         block_color: Optional[BlockColor | str] = None,
     ) -> Block:
         """Creates a paragraph block. https://developers.notion.com/reference/block#paragraph-blocks
 
         :param rich_text: list of `notion.properties.RichText` objects.
-        :returns: `notion.api.notionblock.Block`
+        :param after: The ID of the existing block that the new block should be appended after.
+
+        :returns: `notion.api.Block`
         """
         block_mapping = parent_object._append(
-            BlockChildren([ParagraphBlocktype(rich_text, block_color=block_color)]),
+            BlockChildren(
+                [ParagraphBlocktype(rich_text, block_color=block_color)], after=after
+            )
         )
-        paragraph_block = cls(_result_id(block_mapping))
-        return paragraph_block
+
+        return cls(cast(str, block_mapping["results"][0]["id"]))
 
     @classmethod
     def quote(
         cls,
         parent_object: Page | Block,
         rich_text: Sequence[RichText | Mention],
-        /,
         *,
+        after: Optional[str] = None,
         block_color: Optional[BlockColor | str] = None,
     ) -> Block:
         """Creates a quote block. https://developers.notion.com/reference/block#quote-blocks
 
         :param rich_text: list of `notion.properties.RichText` objects.
-        :returns: `notion.api.notionblock.Block`
+        :returns: `notion.api.Block`
         """
         block_mapping = parent_object._append(
-            BlockChildren([QuoteBlocktype(rich_text, block_color=block_color)])
+            BlockChildren(
+                [QuoteBlocktype(rich_text, block_color=block_color)], after=after
+            )
         )
-        quote_block = cls(_result_id(block_mapping))
-        return quote_block
+        return cls(cast(str, block_mapping["results"][0]["id"]))
 
     @classmethod
     def callout(
         cls,
         parent_object: Page | Block,
         rich_text: Sequence[RichText | Mention],
-        /,
         *,
         icon: Optional[str] = None,
+        after: Optional[str] = None,
         block_color: Optional[BlockColor | str] = None,
     ) -> Block:
         """Creates a callout block. https://developers.notion.com/reference/block#callout-blocks
 
         :param rich_text: list of `notion.properties.RichText` objects.
         :param icon: url to external source for icon.
-        :returns: `notion.api.notionblock.Block`
+        :returns: `notion.api.Block`
         """
-
         block_mapping = parent_object._append(
             BlockChildren(
-                [CalloutBlocktype(rich_text, icon=icon, block_color=block_color)]
-            ),
+                [CalloutBlocktype(rich_text, icon=icon, block_color=block_color)],
+                after=after,
+            )
         )
-        callout_block = cls(_result_id(block_mapping))
-        return callout_block
+        return cls(cast(str, block_mapping["results"][0]["id"]))
 
     @classmethod
     def heading1(
         cls,
         parent_object: Page | Block,
         rich_text: Sequence[RichText | Mention],
-        /,
         *,
-        block_color: Optional[BlockColor | str] = None,
         is_toggleable: Optional[bool] = False,
+        after: Optional[str] = None,
+        block_color: Optional[BlockColor | str] = None,
     ) -> Block:
         """Creates a heading 1 block. https://developers.notion.com/reference/block#heading-one-blocks
 
-        :returns: `notion.api.notionblock.Block`
+        :returns: `notion.api.Block`
         """
         block_mapping = parent_object._append(
             BlockChildren(
                 [
                     Heading1BlockType(
                         rich_text, block_color=block_color, is_toggleable=is_toggleable
                     )
-                ]
-            ),
+                ],
+                after=after,
+            )
         )
-        heading1_block = cls(_result_id(block_mapping))
-        return heading1_block
+        return cls(cast(str, block_mapping["results"][0]["id"]))
 
     @classmethod
     def heading2(
         cls,
         parent_object: Page | Block,
         rich_text: Sequence[RichText | Mention],
-        /,
         *,
-        block_color: Optional[BlockColor | str] = None,
         is_toggleable: Optional[bool] = False,
+        after: Optional[str] = None,
+        block_color: Optional[BlockColor | str] = None,
     ) -> Block:
         """Creates a heading 2 block. https://developers.notion.com/reference/block#heading-two-blocks
 
-        :returns: `notion.api.notionblock.Block`
+        :returns: `notion.api.Block`
         """
         block_mapping = parent_object._append(
             BlockChildren(
                 [
                     Heading2BlockType(
                         rich_text, block_color=block_color, is_toggleable=is_toggleable
                     )
-                ]
-            ),
+                ],
+                after=after,
+            )
         )
-        heading2_block = cls(_result_id(block_mapping))
-        return heading2_block
+        return cls(cast(str, block_mapping["results"][0]["id"]))
 
     @classmethod
     def heading3(
         cls,
         parent_object: Page | Block,
         rich_text: Sequence[RichText | Mention],
-        /,
         *,
-        block_color: Optional[BlockColor | str] = None,
         is_toggleable: Optional[bool] = False,
+        after: Optional[str] = None,
+        block_color: Optional[BlockColor | str] = None,
     ) -> Block:
         """Creates a heading 3 block. https://developers.notion.com/reference/block#heading-three-blocks
 
-        :returns: `notion.api.notionblock.Block`
+        :returns: `notion.api.Block`
         """
         block_mapping = parent_object._append(
             BlockChildren(
                 [
                     Heading3BlockType(
                         rich_text, block_color=block_color, is_toggleable=is_toggleable
                     )
-                ]
-            ),
+                ],
+                after=after,
+            )
         )
-        heading3_block = cls(_result_id(block_mapping))
-        return heading3_block
+        return cls(cast(str, block_mapping["results"][0]["id"]))
 
     @classmethod
     def bulleted_list(
         cls,
         parent_object: Page | Block,
         rich_text: Sequence[RichText | Mention],
-        /,
         *,
+        after: Optional[str] = None,
         block_color: Optional[BlockColor | str] = None,
     ) -> Block:
         """Creates a bulleted list block. https://developers.notion.com/reference/block#bulleted-list-item-blocks
 
-        :returns: `notion.api.notionblock.Block`
+        :returns: `notion.api.Block`
         """
         block_mapping = parent_object._append(
             BlockChildren(
-                [BulletedListItemBlocktype(rich_text, block_color=block_color)]
-            ),
+                [BulletedListItemBlocktype(rich_text, block_color=block_color)],
+                after=after,
+            )
         )
-        bulleted_list_block = cls(_result_id(block_mapping))
-        return bulleted_list_block
+        return cls(cast(str, block_mapping["results"][0]["id"]))
 
     @classmethod
     def numbered_list(
         cls,
         parent_object: Page | Block,
         rich_text: Sequence[RichText | Mention],
-        /,
         *,
+        after: Optional[str] = None,
         block_color: Optional[BlockColor | str] = None,
     ) -> Block:
         """Creates a numbered list block. https://developers.notion.com/reference/block#numbered-list-item-blocks
 
-        :returns: `notion.api.notionblock.Block`
+        :returns: `notion.api.Block`
         """
         block_mapping = parent_object._append(
             BlockChildren(
-                [NumberedListItemBlocktype(rich_text, block_color=block_color)]
-            ),
+                [NumberedListItemBlocktype(rich_text, block_color=block_color)],
+                after=after,
+            )
         )
-        numbered_list_block = cls(_result_id(block_mapping))
-        return numbered_list_block
+        return cls(cast(str, block_mapping["results"][0]["id"]))
 
     @classmethod
     def toggle(
         cls,
         parent_object: Page | Block,
         rich_text: Sequence[RichText | Mention],
-        /,
         *,
+        after: Optional[str] = None,
         block_color: Optional[BlockColor | str] = None,
     ) -> Block:
         """Creates a toggle block. https://developers.notion.com/reference/block#toggle-blocks
 
-        :returns: `notion.api.notionblock.Block`
+        :returns: `notion.api.Block`
         """
-
         block_mapping = parent_object._append(
-            BlockChildren([ToggleBlocktype(rich_text, block_color=block_color)])
+            BlockChildren(
+                [ToggleBlocktype(rich_text, block_color=block_color)], after=after
+            )
         )
-        toggle_block = cls(_result_id(block_mapping))
-        return toggle_block
+        return cls(cast(str, block_mapping["results"][0]["id"]))
 
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ EXTERNAL URL BLOCKS ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
 
     @classmethod
-    def embed_url(cls, parent_object: Page | Block, embedded_url: str, /) -> Block:
+    def embed_url(
+        cls,
+        parent_object: Page | Block,
+        embedded_url: str,
+        /,
+        after: Optional[str] = None,
+    ) -> Block:
         """
         ##### WARNING: embed block types through the API are not reliable and often cause errors.
 
         Embed block types are:
         Framer, Twitter (tweets), Google Drive documents, Gist, Figma,
         Invision, Loom, Typeform, Codepen, PDFs, Google Maps, Whimisical,
         Miro, Abstract, excalidraw, Sketch, Replit
@@ -656,122 +656,124 @@
         This would result in a slow and potentially confusing experience as the block in the response would
         not match the block sent in the request.
         The result is that embed blocks created via the API may not look exactly
         like their counterparts created in the Notion app.
 
         https://developers.notion.com/reference/block#embed-blocks
 
-        :returns: `notion.api.notionblock.Block`
+        :returns: `notion.api.Block`
         """
-
         block_mapping = parent_object._append(
-            BlockChildren([EmbedBlocktype(embedded_url)])
+            BlockChildren([EmbedBlocktype(embedded_url)], after=after)
         )
-        embed_url_block = cls(_result_id(block_mapping))
-        return embed_url_block
+        return cls(cast(str, block_mapping["results"][0]["id"]))
 
     @classmethod
-    def video(cls, parent_object: Page | Block, url: str, /) -> Block:
+    def video(
+        cls, parent_object: Page | Block, url: str, /, after: Optional[str] = None
+    ) -> Block:
         """Creates a video block. https://developers.notion.com/reference/block#video
         Supported video types:
         .amv .asf .avi .f4v .flv .gifv .mkv .mov .mpg .mpeg .mpv .mp4 .m4v .qt .wmv
 
-        :returns: `notion.api.notionblock.Block`
+        :returns: `notion.api.Block`
         """
-        block_mapping = parent_object._append(BlockChildren([VideoBlockType(url)]))
-        video_block = cls(_result_id(block_mapping))
-        return video_block
+        block_mapping = parent_object._append(
+            BlockChildren([VideoBlockType(url)], after=after)
+        )
+        return cls(cast(str, block_mapping["results"][0]["id"]))
 
     @classmethod
-    def image(cls, parent_object: Page | Block, url: str, /) -> Block:
+    def image(
+        cls, parent_object: Page | Block, url: str, /, after: Optional[str] = None
+    ) -> Block:
         """Creates an image block.
         Supported image types: .bmp .gif .heic .jpeg .jpg .png .svg .tif .tiff
         https://developers.notion.com/reference/block#image
         """
-        block_mapping = parent_object._append(BlockChildren([ImageBlockType(url)]))
-        image_block = cls(_result_id(block_mapping))
-        return image_block
+        block_mapping = parent_object._append(
+            BlockChildren([ImageBlockType(url)], after=after)
+        )
+        return cls(cast(str, block_mapping["results"][0]["id"]))
 
     @classmethod
     def bookmark(
         cls,
         parent_object: Page | Block,
         bookmark_url: str,
-        /,
         *,
+        after: Optional[str] = None,
         caption: Optional[Sequence[RichText | Mention]] = None,
     ) -> Block:
         """Creates a bookmark block. https://developers.notion.com/reference/block#bookmark-blocks
 
-        :returns: `notion.api.notionblock.Block`
+        :returns: `notion.api.Block`
         """
-
         block_mapping = parent_object._append(
-            BlockChildren([BookmarkBlocktype(bookmark_url, caption=caption)])
+            BlockChildren([BookmarkBlocktype(bookmark_url, caption=caption)], after=after)
         )
-        bookmark_block = cls(_result_id(block_mapping))
-        return bookmark_block
+        return cls(cast(str, block_mapping["results"][0]["id"]))
 
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ MISC BLOCKS ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
 
     @classmethod
-    def link_to_page(cls, parent_object: Page | Block, page_id: str, /) -> Block:
+    def link_to_page(
+        cls, parent_object: Page | Block, page_id: str, /, after: Optional[str] = None
+    ) -> Block:
         """Creates a link_to_page block. https://developers.notion.com/reference/block#link-to-page-blocks
 
-        :returns: `notion.api.notionblock.Block`
+        :returns: `notion.api.Block`
         """
-
         block_mapping = parent_object._append(
-            BlockChildren([LinkToPageBlockType(page_id)])
+            BlockChildren([LinkToPageBlockType(page_id)], after=after)
         )
-        link_to_page_block = cls(_result_id(block_mapping))
-        return link_to_page_block
+        return cls(cast(str, block_mapping["results"][0]["id"]))
 
     @classmethod
     def table_of_contents(
         cls,
         parent_object: Page | Block,
-        /,
         *,
+        after: Optional[str] = None,
         block_color: Optional[BlockColor | str] = None,
     ) -> Block:
         """Creates a table of contents block.
         https://developers.notion.com/reference/block#table-of-contents-blocks
 
-        :returns: `notion.api.notionblock.Block`
+        :returns: `notion.api.Block`
         """
-
         block_mapping = parent_object._append(
-            BlockChildren([TableOfContentsBlocktype(block_color=block_color)])
+            BlockChildren(
+                [TableOfContentsBlocktype(block_color=block_color)], after=after
+            )
         )
-        table_of_contents_block = cls(_result_id(block_mapping))
-        return table_of_contents_block
+        return cls(cast(str, block_mapping["results"][0]["id"]))
 
     @classmethod
-    def breadcrumb(cls, parent_object: Page | Block) -> Block:
+    def breadcrumb(
+        cls, parent_object: Page | Block, after: Optional[str] = None
+    ) -> Block:
         """Creates a breadcrumb block.
         https://developers.notion.com/reference/block#breadcrumb-blocks
         """
-        block_mapping = parent_object._append(BlockChildren([BreadcrumbBlock()]))
-        breadcrumb_block = cls(_result_id(block_mapping))
-        return breadcrumb_block
+        block_mapping = parent_object._append(
+            BlockChildren([BreadcrumbBlock()], after=after)
+        )
+        return cls(cast(str, block_mapping["results"][0]["id"]))
 
     @classmethod
-    def divider(cls, parent_object: Page | Block) -> Block:
+    def divider(cls, parent_object: Page | Block, after: Optional[str] = None) -> Block:
         """Creates a divider block.
         https://developers.notion.com/reference/block#divider-blocks
         """
-        block_mapping = parent_object._append(BlockChildren([DividerBlock()]))
-        divider_block = cls(_result_id(block_mapping))
-        return divider_block
+        block_mapping = parent_object._append(
+            BlockChildren([DividerBlock()], after=after)
+        )
+        return cls(cast(str, block_mapping["results"][0]["id"]))
 
     @classmethod
-    def newline(cls, parent_object: Page | Block) -> Block:
+    def newline(cls, parent_object: Page | Block, after: Optional[str] = None) -> Block:
         """Creates a newline break."""
-        block_mapping = parent_object._append(BlockChildren([NewLineBreak]))
-        newline_block = cls(_result_id(block_mapping))
-        return newline_block
-
-    # Column blocks are not currently supported.
+        block_mapping = parent_object._append(BlockChildren([NewLineBreak], after=after))
+        return cls(cast(str, block_mapping["results"][0]["id"]))
 
-def _result_id(block_mapping: MutableMapping[str, Any]) -> str:
-    return cast(str, block_mapping["results"][0]["id"])
+    # Column blocks are not currently supported by this library.
```

### Comparing `notion_api-0.5.2/notion/api/notiondatabase.py` & `notion_api-0.6.0/notion/api/notiondatabase.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,34 +16,28 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+# mypy: disable-error-code="no-redef"
+
 from __future__ import annotations
 
 from functools import cached_property
 from types import ModuleType
-from typing import TYPE_CHECKING, Any, MutableMapping, Optional, Sequence, Union, cast
-
-try:
-    import orjson
-
-    default_json: ModuleType = orjson
-except ModuleNotFoundError:
-    import json
-
-    default_json: ModuleType = json
+from typing import TYPE_CHECKING, Any, MutableMapping, Optional, Sequence, cast
 
+from notion.api._pagination import paginated_response_payload
 from notion.api.blockmixin import _TokenBlockMixin
 from notion.api.client import _NLOG
 from notion.api.notionblock import Block
 from notion.exceptions.errors import NotionValidationError
-from notion.properties.build import NotionObject, build_payload
+from notion.properties.build import build_payload
 from notion.properties.common import Parent
 from notion.properties.files import Cover, Icon
 from notion.properties.options import FunctionFormat, NumberFormat
 from notion.properties.propertyobjects import (
     CheckboxPropertyObject,
     CreatedByPropertyObject,
     CreatedTimePropertyObject,
@@ -72,14 +66,23 @@
 from notion.query.propfilter import PropertyFilter
 from notion.query.sort import SortFilter
 from notion.query.timestamp import TimestampFilter
 
 if TYPE_CHECKING:
     from notion.api.notionpage import Page
 
+try:
+    import orjson
+
+    _json: ModuleType = orjson
+except ModuleNotFoundError:
+    import json
+
+    _json: ModuleType = json
+
 __all__: Sequence[str] = ["Database"]
 
 
 class Database(_TokenBlockMixin):
     """
     Database objects describe the property schema of a database in Notion.
     Pages are the items (or children) in a database. The API treats database rows as pages.
@@ -96,42 +99,30 @@
     ---
     ### Versioning:
     To use a previous version of the API, set the envrionment variable `NOTION_VERSION`.
     For more info see: https://developers.notion.com/reference/versioning
 
     ---
     :param id: (required) `database_id` of object in Notion.
-    :param token: Bearer token provided when you create an integration.\
+    :param token: (optional) Bearer token provided when you create an integration.\
                   Set notion secret in environment variables as `NOTION_TOKEN`, or set variable here.\
                   See https://developers.notion.com/reference/authentication.
 
     https://developers.notion.com/reference/database
     """
 
-    def __new__(
-        cls,
-        id: str,
-        /,
-        token: Optional[str] = None,
-    ) -> Database:
-        # notion api will not throw an error if the uuid isn't a database until you make a call.
-        # this is to throw an error right away if trying to create a database instance
-        # with a uuid that is not a database and catch the error sooner.
+    def __new__(cls, id: str, /, token: Optional[str] = None) -> Database:
+        # notion api will not throw an error if the id is not a database until you make a call.
+        # this is to raise right away if the id is not a database and catch the error sooner.
         target_block = Block(id, token=token)
         if target_block.type != "child_database":
             raise TypeError(f"{target_block.__repr__()} does not reference a Database.")
         return super().__new__(cls)
 
-    def __init__(
-        self,
-        id: str,
-        /,
-        *,
-        token: Optional[str] = None,
-    ) -> None:
+    def __init__(self, id: str, /, *, token: Optional[str] = None) -> None:
         super().__init__(id, token=token)
         self.logger = _NLOG.getChild(self.__repr__())
 
     @classmethod
     def create(
         cls,
         parent_instance: Page,
@@ -159,31 +150,31 @@
         """
         payload = build_payload(
             Parent.page(parent_instance.id),
             TitlePropertyValue([RichText(database_title)]),
             Properties(TitlePropertyObject(name_column if name_column else "Name")),
         )
 
-        new_db = cls._post(parent_instance, cls._database_endpoint(), payload=payload)
+        new_db_map = cls._post(parent_instance, cls._database_endpoint(), payload=payload)
 
-        cls_ = cls(new_db["id"])
-        cls_.logger.debug(
-            f"Database created in {parent_instance.__repr__()}. Url: {new_db['url']}"
+        database = cls(new_db_map["id"])
+        database.logger.debug(
+            f"Database created in {parent_instance.__repr__()}. Url: {new_db_map['url']}"
         )
 
         if is_inline:
-            cls_.is_inline = is_inline
+            database.is_inline = is_inline
         if description:
-            cls_.description = description
+            database.description = description
         if icon_url:
-            cls_.icon = icon_url
+            database.icon = icon_url
         if cover_url:
-            cls_.cover = cover_url
+            database.cover = cover_url
 
-        return cls_
+        return database
 
     def __getitem__(self, property_name: str) -> MutableMapping[str, Any]:
         if property_name in self.property_schema:
             return cast(MutableMapping[str, Any], self.property_schema[property_name])
         raise KeyError(f"{property_name} not found in page property values.")
 
     def __delitem__(self, property_name_or_id: str) -> None:
@@ -223,60 +214,59 @@
         Otherwise has the value false if the database appears as a child page.
         """
         return cast(bool, (self.retrieve["is_inline"]))
 
     @is_inline.setter
     def is_inline(self, __inline: bool) -> None:
         self._patch(
-            self._database_endpoint(self.id),
-            payload=default_json.dumps({"is_inline": __inline}),
+            self._database_endpoint(self.id), payload=_json.dumps({"is_inline": __inline})
         )
 
     @property
     def description(self) -> str:
         """
         :return: (str) description of database. Empty string if no description is set.
 
         description.setter:
-            >>> database.description = "This is a description of the database."
+        >>> database.description = "This is a description of the database."
         """
         try:
             description = self.retrieve["description"][0]["text"]["content"]
             return cast(str, description)
         except IndexError:
             return ""  # description is empty.
 
     @description.setter
     def description(self, description: str) -> None:
         self._update(DatabaseDescription([RichText(description)]))
 
     @property
-    def icon(self) -> Union[str, None]:
+    def icon(self) -> str | None:
         """
         :return: (str) url of icon. None if no icon is set.
 
         icon.setter:
-            >>> database.icon = "https://www.notion.so/icons/code_gray.svg"
+        >>> database.icon = "https://www.notion.so/icons/code_gray.svg"
         """
         icon = self.retrieve["icon"]
         if icon:
             return cast(str, icon["external"]["url"])
         return None
 
     @icon.setter
     def icon(self, icon_url: str) -> None:
         self._update(Icon(icon_url))
 
     @property
-    def cover(self) -> Union[str, None]:
+    def cover(self) -> str | None:
         """
         :return: (str) url of cover. None if no cover is set.
 
         cover.setter:
-            >>> database.cover = "https://www.notion.so/images/page-cover/webb1.jpg"
+        >>> database.cover = "https://www.notion.so/images/page-cover/webb1.jpg"
         """
         cover = self.retrieve["cover"]
         if cover:
             return cast(str, cover["external"]["url"])
         return None
 
     @cover.setter
@@ -285,135 +275,212 @@
 
     @property
     def url(self) -> str:
         """:return: (str) url of database"""
         return cast(str, (self.retrieve["url"]))
 
     @property
+    def public_url(self) -> str:
+        """When a page or database has been shared publicly, the response body will include a public_url value"""
+        return cast(str, (self.retrieve["public_url"]))
+
+    @property
     def delete_self(self) -> None:
         if self.is_archived:
             return
 
         self._delete(self._block_endpoint(self.id))
 
     @property
     def restore_self(self) -> None:
         if not self.is_archived:
             return None
 
         self._patch(self._database_endpoint(self.id), payload=(b'{"archived": false}'))
 
-    def _update(
-        self,
-        payload: MutableMapping[str, Any],
-    ) -> MutableMapping[str, Any]:
-        """
-        Updates an existing database as specified by the parameters.
+    def _update(self, payload: MutableMapping[str, Any]) -> MutableMapping[str, Any]:
+        """Updates an existing database as specified by the parameters.
 
         :param payload: (required) json payload for updated properties parameters.
 
         https://developers.notion.com/reference/update-a-database
         """
         return self._patch(self._database_endpoint(self.id), payload=payload)
 
     def delete_property(self, name_or_id: str) -> None:
-        """
-        :param name_or_id: (required) name or id of property described in database schema
+        """https://developers.notion.com/reference/update-property-schema-object#removing-a-property
 
-        https://developers.notion.com/reference/update-property-schema-object#removing-a-property
+        :param name_or_id: (required) name or id of property described in database schema
         """
         self._update({"properties": {name_or_id: None}})
 
     def rename_property(self, old_name: str, new_name: str) -> None:
-        """
-        https://developers.notion.com/reference/update-property-schema-object#renaming-a-property
-        """
-        self._update(default_json.dumps({"properties": {old_name: {"name": new_name}}}))
+        """https://developers.notion.com/reference/update-property-schema-object#renaming-a-property"""
+        self._update(_json.dumps({"properties": {old_name: {"name": new_name}}}))
 
     def query(
         self,
         *,
-        filter: Optional[Union[CompoundFilter, PropertyFilter, TimestampFilter]] = None,
+        filter: Optional[CompoundFilter | PropertyFilter | TimestampFilter] = None,
         sort: Optional[SortFilter] = None,
         filter_property_values: Optional[list[str]] = None,
         page_size: Optional[int] = 100,
         start_cursor: Optional[str] = None,
     ) -> MutableMapping[str, Any]:
         """
-        Gets a list of Pages contained in the database, 
-        filtered/ordered to the filter conditions/sort criteria provided in request.
+        **query() method deprecated in > v0.5.2.**
+        **In a future update, this will be replaced with the new method `query_all()` added in v0.6.0 that iterates through all pages from results.**
+        **This method will still remain under a new name for anyone wanting the original request.**
+
+        Gets a list of Pages contained in the database, filtered/ordered to the filter conditions/sort criteria provided in request.
         Responses from paginated endpoints contain a `next_cursor` property,
         which can be used in a query payload to continue the list.
 
         ---
         :param filter: (optional) notion.query.compound.CompoundFilter or notion.query.propfilter.PropertyFilter
         :param sort: (optional) notion.query.sort.SortFilter
         :param page_size: (optional) The number of items from the full list desired in the response.\
                            Default: 100 page_size Maximum: 100.
         :param start_cursor: (optional) When supplied, returns a page of results starting after the cursor provided.\
                               If not supplied, this endpoint will return the first page of results.
         :param filter_property_values: (optional) Return only the selected properties.
 
         https://developers.notion.com/reference/post-database-query
         """
-        payload: NotionObject = NotionObject()
-        url = self._database_endpoint(self.id, query=True)
+        self.logger.warning(_QUERY_DEPRECATION_NOTICE)
+
+        payload: dict[str, Any] = {}
+        endpoint = self._database_endpoint(self.id, query=True)
 
         if filter_property_values:
-            url += "?"
+            endpoint += "?"
             for name in filter_property_values:
                 name_id = self[name].get("id")
-                url += f"filter_properties={name_id}&"
+                endpoint += f"filter_properties={name_id}&"
 
         if filter:
             payload |= filter
         if sort:
             payload |= sort
         if page_size:
             payload |= {"page_size": page_size}
         if start_cursor:
             payload |= {"start_cursor": start_cursor}
 
-        return self._post(url, payload=payload)
+        return self._post(endpoint, payload=payload)
 
     def query_pages(
         self,
         *,
-        filter: Optional[Union[CompoundFilter, PropertyFilter, TimestampFilter]] = None,
+        filter: Optional[CompoundFilter | PropertyFilter | TimestampFilter] = None,
         sort: Optional[SortFilter] = None,
         page_size: Optional[int] = 100,
         start_cursor: Optional[str] = None,
     ) -> list[Page]:
         """
-        :return: list of notion.Page objects
+        **query_pages() method deprecated in > v0.5.2.**
+        **In a future update, this will be replaced with the new method `query_all_pages()` added in v0.6.0 that iterates through all pages from results.**
+
+        Runs Database.query(...) but returns a notion.Page object for every page_id in the query response.
 
         :param filter: (optional) notion.query.compound.CompoundFilter or notion.query.propfilter.PropertyFilter
         :param sort: (optional) notion.query.sort.SortFilter
         :param page_size: (optional) The number of items from the full list desired in the response.\
                            Default: 100 page_size Maximum: 100.
         :param start_cursor: (optional) When supplied, returns a page of results starting after the cursor provided.\
                               If not supplied, this endpoint will return the first page of results.
 
+        :return: list of notion.Page objects
+
         https://developers.notion.com/reference/post-database-query
         """
+        self.logger.warning(_QUERY_PAGES_DEPRECATION_NOTICE)
+
         query = self.query(
             filter=filter,
             sort=sort,
             page_size=page_size,
             start_cursor=start_cursor,
         )
 
         from notion.api.notionpage import Page
 
         return [Page(_object["id"]) for _object in query.get("results", [])]
 
+    def query_all(
+        self,
+        *,
+        filter: Optional[CompoundFilter | PropertyFilter | TimestampFilter] = None,
+        sort: Optional[SortFilter] = None,
+        filter_property_values: Optional[list[str]] = None,
+        max_page_size: Optional[int] = None,
+    ) -> list[MutableMapping[str, Any]]:
+        """
+        Queries all pages in a database, filtered/ordered to the filter conditions/sort criteria provided in request.
+        Will iterate through all pages in response where a `next_cursor` key is present and the list of results is
+        less than `max_page_size`.
+
+        :param filter: (optional) notion.query.compound.CompoundFilter or notion.query.propfilter.PropertyFilter
+        :param sort: (optional) notion.query.sort.SortFilter
+        :param filter_property_values: (optional) Return only the selected properties.
+        :param max_page_size: (optional) The max number of pages to include in results.\
+                               If left blank, will iterate until all pages in results are included.
+
+        :return: list of page object mappings.
+
+        https://developers.notion.com/reference/post-database-query
+        """
+        endpoint = self._database_endpoint(self.id, query=True)
+        payload: dict[str, Any] = {}
+
+        if filter_property_values:
+            endpoint += "?"
+            for name in filter_property_values:
+                name_id = self[name].get("id")
+                endpoint += f"filter_properties={name_id}&"
+
+        if filter:
+            payload |= filter
+        if sort:
+            payload |= sort
+
+        return paginated_response_payload(self._post, endpoint, payload, max_page_size)
+
+    def query_all_pages(
+        self,
+        *,
+        filter: Optional[CompoundFilter | PropertyFilter | TimestampFilter] = None,
+        sort: Optional[SortFilter] = None,
+        max_page_size: Optional[int] = None,
+    ) -> list[Page]:
+        """
+        Runs Database.query_all(...) but returns a notion.Page object for every page_id in the query response.
+
+        :param filter: (optional) notion.query.compound.CompoundFilter or notion.query.propfilter.PropertyFilter
+        :param sort: (optional) notion.query.sort.SortFilter
+        :param max_page_size: (optional) The max number of pages to include in results.\
+                               If left blank, will iterate until all pages in results are included.
+
+        :return: list of notion.Page objects
+
+        https://developers.notion.com/reference/post-database-query
+        """
+        from notion.api.notionpage import Page
+
+        return [
+            Page(row["id"])
+            for row in self.query_all(
+                filter=filter, sort=sort, max_page_size=max_page_size
+            )
+        ]
+
     def dual_relation_column(
         self, property_name: str, /, database_id: str, synced_property_name: str
     ) -> None:
-        """ Creates a `Relation` property with `Separate Directions` toggled on.
+        """Creates or replaces a `Relation` property with `Separate Directions` toggled on.
 
         :param property_name: (required) Name to give to property.
         :param database_id: (required) The database that the relation property refers to.\
                              The corresponding linked page values must belong to the database in order to be valid.
         :param synced_property_name: (required) The name of the corresponding property that is\
                                       updated in the related database when this property is changed.
         
@@ -432,15 +499,15 @@
             Database(database_id).rename_property(
                 f"Related to {self.title} ({property_name})", synced_property_name
             )
         except NotionValidationError:
             pass
 
     def single_relation_column(self, property_name: str, /, database_id: str) -> None:
-        """ Creates a `Relation` property with `Separate Directions` toggled off.
+        """Creates or replaces a `Relation` property with `Separate Directions` toggled off.
 
         :param property_name: (required) Name to give to property.
         :param database_id: (required) The database id that this property will relate to.\
                              The corresponding linked page values must belong to the database in order to be valid.
         
         https://developers.notion.com/reference/property-object#relation
         """
@@ -450,19 +517,17 @@
 
     def rollup_column(
         self,
         property_name: str,
         /,
         relation_property_name: str,
         rollup_property_name: str,
-        function: Optional[
-            Union[FunctionFormat, str]
-        ] = FunctionFormat.show_original.value,
+        function: Optional[FunctionFormat | str] = FunctionFormat.show_original.value,
     ) -> None:
-        """ Creates a `Rollup` property.
+        """Creates or replaces a `Rollup` property.
         A rollup database property is rendered in the Notion UI as a column with 
         values that are rollups, specific properties that are pulled from a related database.
 
         :param property_name: (required) Name to give to property.
         :param relation_property_name: (required) The name of the related database property that is rolled up.\
                                         i.e. if this class is databaseA, and has a column named "Related to databaseB",\
                                         then `relation_property_name` would be "Related to databaseB".
@@ -472,23 +537,20 @@
                                       then `rollup_property_name` would be "Number of items". 
         :param function: (required) The function that computes the rollup value from the related pages.\
                           notion.properties.options.FunctionFormat or string.
 
         https://developers.notion.com/reference/property-object#rollup
         """
         rollup_property = RollupPropertyObject(
-            property_name,
-            relation_property_name,
-            rollup_property_name,
-            function,
+            property_name, relation_property_name, rollup_property_name, function
         )
         self._update((Properties(rollup_property)))
 
-    def select_column(self, property_name: str, /, options: list[Option]) -> None:
-        """ Creates a `Select` property.
+    def select_column(self, property_name: str, /, options: Sequence[Option]) -> None:
+        """Creates or replaces a `Select` property.
 
         If `property_name` is a select column that already exists,
         then this method will overwrite the current options - UNLESS
         if one of the options already exists and you try to change the color.
         This will raise:
         ```sh
         notion.exceptions.errors.NotionValidationError: Cannot update color of select with name: `property_name`
@@ -500,16 +562,18 @@
         :param options: (required) List of options to be available in the select column.\
                          `notion.properties.propertyobjects.Option`.
                          
         https://developers.notion.com/reference/property-object#select
         """
         self._update(Properties(SelectPropertyObject(property_name, options=options)))
 
-    def multiselect_column(self, property_name: str, /, options: list[Option]) -> None:
-        """ Creates a `Multi-select` property.
+    def multiselect_column(
+        self, property_name: str, /, options: Sequence[Option]
+    ) -> None:
+        """Creates or replaces a `Multi-select` property.
 
         If `property_name` is a multi_select column that already exists,
         then this method will overwrite the current options - UNLESS
         if one of the options already exists and you try to change the color.
         This will raise:
         ```sh
         notion.exceptions.errors.NotionValidationError: Cannot update color of select with name: `property_name`
@@ -527,108 +591,103 @@
             Properties(MultiSelectPropertyObject(property_name, options=options))
         )
 
     def number_column(
         self,
         property_name: str,
         /,
-        format: Optional[Union[NumberFormat, str]] = NumberFormat.number.value,
+        format: Optional[NumberFormat | str] = NumberFormat.number.value,
     ) -> None:
-        """Creates a `Number` property.
-
+        """Creates or replaces a `Number` property.
         https://developers.notion.com/reference/property-object#number
         """
         self._update(Properties(NumberPropertyObject(property_name, format)))
 
     def checkbox_column(self, property_name: str, /) -> None:
-        """Creates a `Checkbox` property.
-
+        """Creates or replaces a `Checkbox` property.
         https://developers.notion.com/reference/property-object#checkbox
         """
         self._update(Properties(CheckboxPropertyObject(property_name)))
 
     def date_column(self, property_name: str, /) -> None:
-        """Creates a `Date` property.
-
+        """Creates or replaces a `Date` property.
         https://developers.notion.com/reference/property-object#date
         """
         self._update(Properties(DatePropertyObject(property_name)))
 
     def text_column(self, property_name: str, /) -> None:
-        """Creates a `Text` property.
-
+        """Creates or replaces a `Text` property.
         https://developers.notion.com/reference/property-object#rich-text
         """
         self._update(Properties(RichTextPropertyObject(property_name)))
 
     def formula_column(self, property_name: str, /, expression: str) -> None:
-        """ Creates a `Formula` property.
+        """Creates or replaces a `Formula` property.
 
         :param expression: (required) The formula that is used to compute the values for this property.\
                             Refer to https://www.notion.so/help/formulas for more information about formula syntax.
             
         https://developers.notion.com/reference/property-object#formula
         """
         self._update(Properties(FormulaPropertyObject(property_name, expression)))
 
     def created_time_column(self, property_name: str, /) -> None:
-        """Creates a `Created time` property.
-
+        """Creates or replaces a `Created time` property.
         https://developers.notion.com/reference/property-object#created-time
         """
         self._update(Properties(CreatedTimePropertyObject(property_name)))
 
     def created_by_column(self, property_name: str, /) -> None:
-        """Creates a `Created by` property.
-
+        """Creates or replaces a `Created by` property.
         https://developers.notion.com/reference/property-object#created-by
         """
         self._update(Properties(CreatedByPropertyObject(property_name)))
 
     def last_edited_time_column(self, property_name: str, /) -> None:
-        """Creates a `Last edited time` property.
-
+        """Creates or replaces a `Last edited time` property.
         https://developers.notion.com/reference/property-object#last-edited-time
         """
         self._update(Properties(LastEditedTimePropertyObject(property_name)))
 
     def last_edited_by_column(self, property_name: str, /) -> None:
-        """Creates a `Last edited by` property.
-
+        """Creates or replaces a `Last edited by` property.
         https://developers.notion.com/reference/property-object#last-edited-by
         """
         self._update(Properties(LastEditedByPropertyObject(property_name)))
 
     def files_column(self, property_name: str, /) -> None:
-        """Creates a `Files` property.
-
+        """Creates or replaces a `Files` property.
         https://developers.notion.com/reference/property-object#files
         """
         self._update(Properties(FilesPropertyObject(property_name)))
 
     def email_column(self, property_name: str, /) -> None:
         """Creates an `Email` property.
-
         https://developers.notion.com/reference/property-object#email
         """
         self._update(Properties(EmailPropertyObject(property_name)))
 
     def url_column(self, property_name: str, /) -> None:
-        """Creates a `URL` property.
-
+        """Creates or replaces a `URL` property.
         https://developers.notion.com/reference/property-object#url
         """
         self._update(Properties(URLPropertyObject(property_name)))
 
     def phone_number_column(self, property_name: str, /) -> None:
-        """Creates a `Phone` property.
-
+        """Creates or replaces a `Phone` property.
         https://developers.notion.com/reference/property-object#phone-number
         """
         self._update(Properties(PhoneNumberPropertyObject(property_name)))
 
     def person_column(self, property_name: str, /) -> None:
-        """Creates a `Person` property.
-
+        """Creates or replaces a `Person` property.
         https://developers.notion.com/reference/property-object#people
         """
         self._update(Properties(PeoplePropertyObject(property_name)))
+
+
+_QUERY_DEPRECATION_NOTICE = """query() method deprecated in > v0.5.2. \
+In a future update, this will be replaced with new method `query_all()` added in v0.6.0 that iterates through all pages from results. \
+This method will still remain under a new name for anyone wanting the original request."""
+
+_QUERY_PAGES_DEPRECATION_NOTICE = """query_pages() method deprecated in > v0.5.2. \
+In a future update, this will be replaced with new method `query_all_pages()` added in v0.6.0 that iterates through all pages from results."""
```

### Comparing `notion_api-0.5.2/notion/api/notionpage.py` & `notion_api-0.6.0/notion/api/notionpage.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from __future__ import annotations
 
-from datetime import datetime
+from datetime import datetime, timedelta
 from functools import cached_property
-from typing import TYPE_CHECKING, Any, MutableMapping, Optional, Sequence, Union, cast
+from typing import Any, MutableMapping, Optional, Sequence, cast
 
 from notion.api.blockmixin import _TokenBlockMixin
 from notion.api.client import _NLOG
 from notion.api.notionblock import Block
 from notion.api.notiondatabase import Database
 from notion.properties.build import build_payload
 from notion.properties.common import Parent, UserObject, _NotionUUID
@@ -55,17 +55,14 @@
     StatusPropertyValue,
     TitlePropertyValue,
     URLPropertyValue,
 )
 from notion.properties.richtext import RichText
 from notion.propertyitems.base import PropertyItem
 
-if TYPE_CHECKING:
-    from datetime import timedelta
-
 __all__: Sequence[str] = ["Page"]
 
 
 class Page(_TokenBlockMixin):
     """
     The Page object contains the page property values of a single Notion page.
     All pages have a Parent. If the parent is a database, 
@@ -81,36 +78,30 @@
 
     ---
     ### Versioning:
     To use a previous version of the API, set the envrionment variable `NOTION_VERSION`.
     For more info see: https://developers.notion.com/reference/versioning
 
     ---
-    :param id: (required) `page_id` of object in Notion.
-    :param token: Bearer token provided when you create an integration.\
+    :param id:    (required) `page_id` of object in Notion.
+    :param token: (optional) Bearer token provided when you create an integration.\
                   Set notion secret in environment variables as `NOTION_TOKEN`, or set variable here.\
                   See https://developers.notion.com/reference/authentication.
 
     https://developers.notion.com/reference/page
     """
 
-    def __init__(
-        self,
-        id: str,
-        /,
-        *,
-        token: Optional[str] = None,
-    ) -> None:
+    def __init__(self, id: str, /, *, token: Optional[str] = None) -> None:
         super().__init__(id, token=token)
         self.logger = _NLOG.getChild(self.__repr__())
 
     @classmethod
     def create(
         cls,
-        parent_instance: Union[Page, Database, Block],
+        parent_instance: Page | Database | Block,
         page_title: str,
         *,
         cover_url: Optional[str] = None,
         icon_url: Optional[str] = None,
     ) -> Page:
         """
         Creates a blank page.
@@ -132,27 +123,27 @@
             )
         else:
             payload = build_payload(
                 Parent.page(parent_instance.id),
                 Properties(TitlePropertyValue([RichText(page_title)])),
             )
 
-        new_page = cls._post(parent_instance, cls._pages_endpoint(), payload=payload)
+        new_page_map = cls._post(parent_instance, cls._pages_endpoint(), payload=payload)
 
-        cls_ = cls(new_page["id"])
-        cls_.logger.debug(
-            f"Page created in {parent_instance.__repr__()}. Url: {new_page['url']}"
+        page = cls(new_page_map["id"])
+        page.logger.debug(
+            f"Page created in {parent_instance.__repr__()}. Url: {new_page_map['url']}"
         )
 
         if icon_url:
-            cls_.icon = icon_url
+            page.icon = icon_url
         if cover_url:
-            cls_.cover = cover_url
+            page.cover = cover_url
 
-        return cls_
+        return page
 
     def __getattr__(self, attr: str) -> PropertyItem:
         def lower_alnum(s: str) -> str:
             return "".join([c if c.isalnum() else "_" for c in s]).lower()
 
         for property in self.properties:
             if lower_alnum(attr) == lower_alnum(property):
@@ -169,59 +160,56 @@
 
     @cached_property
     def properties(self) -> MutableMapping[str, Any]:
         return cast(MutableMapping[str, Any], self.retrieve()["properties"])
 
     @property
     def title(self) -> str:
-        """
-        :return: (str) title of page. Empty string if no title is set.
+        """:return: (str) title of page. Empty string if no title is set.
 
         title setter:
-            >>> page.title = "New Title"
+        >>> page.title = "New Title"
         """
         try:
             if ("workspace" or "page_id") in self.parent_type:
                 return cast(str, self.properties["title"]["title"][0]["plain_text"])
-
-            database_title_property = self.properties[
-                [k for k, v in self.properties.items() if "title" in v][0]
-            ]
-            return cast(str, database_title_property["title"][0]["plain_text"])
+            else:
+                database_title_property = self.properties[
+                    [k for k, v in self.properties.items() if "title" in v][0]
+                ]
+                return cast(str, database_title_property["title"][0]["plain_text"])
         except IndexError:
             return ""  # title is empty
 
     @title.setter
     def title(self, new_title: str) -> None:
         self._patch_properties(Properties(TitlePropertyValue([RichText(new_title)])))
 
     @property
-    def icon(self) -> Union[str, None]:
-        """
-        :return: (str) url of icon. None if no icon is set.
+    def icon(self) -> str | None:
+        """:return: (str) url of icon. None if no icon is set.
 
         icon setter:
-            >>> page.icon = "https://www.notion.so/icons/code_gray.svg"
+        >>> page.icon = "https://www.notion.so/icons/code_gray.svg"
         """
         icon = self.retrieve()["icon"]
         if icon:
             return cast(str, icon["external"]["url"])
         return None
 
     @icon.setter
     def icon(self, icon_url: str) -> None:
         self._patch_properties(Icon(icon_url))
 
     @property
-    def cover(self) -> Union[str, None]:
-        """
-        :return: (str) url of cover. None if no cover is set.
+    def cover(self) -> str | None:
+        """:return: (str) url of cover. None if no cover is set.
 
         cover setter:
-            >>> page.cover = "https://www.notion.so/images/page-cover/webb1.jpg"
+        >>> page.cover = "https://www.notion.so/images/page-cover/webb1.jpg"
         """
         cover = self.retrieve()["cover"]
         if cover:
             return cast(str, cover["external"]["url"])
         return None
 
     @cover.setter
@@ -230,14 +218,19 @@
 
     @property
     def url(self) -> str:
         """:return: (str) url of page"""
         return cast(str, self.retrieve()["url"])
 
     @property
+    def public_url(self) -> str:
+        """When a page or database has been shared publicly, the response body will include a public_url value"""
+        return cast(str, (self.retrieve()["public_url"]))
+
+    @property
     def delete_self(self) -> None:
         if self.is_archived:
             return
 
         self._delete(self._block_endpoint(self.id))
 
     @property
@@ -267,29 +260,24 @@
 
         return self._get(self._pages_endpoint(self.id))
 
     def _retrieve_property_id(self, property_name: str) -> str:
         """Internal function to retrieve the id of a property."""
         return cast(str, self[property_name]["id"])
 
-    def retrieve_property_item(
-        self,
-        property_name: str,
-    ) -> MutableMapping[str, Any]:
-        """
-        Retrieves a property_item object for a given page_id and property_id.
+    def retrieve_property_item(self, property_name: str) -> MutableMapping[str, Any]:
+        """Retrieves a property_item object for a given page_id and property_id.
         The object returned will either be:
             - a value.
             - a paginated list of property item values.
 
         :param property_name: (required) property name in Notion *case-sensitive.
 
-        https://developers.notion.com/reference/property-item-object
-
-        https://developers.notion.com/reference/retrieve-a-page-property
+        Property Item Object: https://developers.notion.com/reference/property-item-object \n
+        Retrieve a page property: https://developers.notion.com/reference/retrieve-a-page-property
         """
         property_id = self._retrieve_property_id(property_name)
         return self._get(
             self._pages_endpoint(self.id, properties=True, property_id=property_id)
         )
 
     def _patch_properties(
@@ -301,17 +289,15 @@
         If parent is a database, new property values must conform to the parent database's property schema.
 
         https://developers.notion.com/reference/patch-page
         """
         return self._patch(self._pages_endpoint(self.id), payload=payload)
 
     def retrieve_page_content(
-        self,
-        start_cursor: Optional[str] = None,
-        page_size: Optional[int] = None,
+        self, start_cursor: Optional[str] = None, page_size: Optional[int] = None
     ) -> MutableMapping[str, Any]:
         """
         Returns only the first level of children for the specified block.
         See block objects for more detail on determining if that block has nested children.
         In order to receive a complete representation of a block, you
         may need to recursively retrieve block children of child blocks.
 
@@ -393,26 +379,28 @@
 
         self._patch_properties(Properties(StatusPropertyValue(property_name, option)))
 
     def set_date(
         self,
         property_name: str,
         /,
-        start: Union[str, datetime],
-        end: Optional[Union[str, datetime]] = None,
+        *,
+        start: str | datetime,
+        end: Optional[str | datetime] = None,
     ) -> None:
         """
         :param start: (required) A date, with an optional time.\
+                       If not time is set, then date will appear in Notion without a time.\
                        If value is a string, it must be ISO 8601 format.\
-                       If value is datetime.datetime, it will be converted to self.tz, in isoformat.
+                       If value is datetime, it will be converted to ISOformat astimezone(self.tz).
         :param end: (optional) A date, with an optional time.\
                      If value is provided, then date property becomes a range, with start and end values.\
                      If value is not provided, then the date value is not a range.
                      If value is a string, it must be ISO 8601 format.\
-                     If value is datetime.datetime, it will be converted to self.tz, in isoformat.
+                     If value is datetime, it will be converted to ISOformat astimezone(self.tz).
 
         https://developers.notion.com/reference/page-property-values#date
         """
         if isinstance(start, datetime):
             start = start.astimezone(self.tz).isoformat()
         if end and isinstance(end, datetime):
             end = end.astimezone(self.tz).isoformat()
@@ -424,28 +412,24 @@
     def set_text(self, property_name: str, /, text: str) -> None:
         """https://developers.notion.com/reference/page-property-values#rich-text"""
         self._patch_properties(
             Properties(RichTextPropertyValue(property_name, [RichText(text)]))
         )
 
     def set_files(
-        self,
-        property_name: str,
-        /,
-        array_of_files: Sequence[Union[InternalFile, ExternalFile]],
+        self, property_name: str, /, array_of_files: Sequence[InternalFile | ExternalFile]
     ) -> None:
         """
         When updating a file property, the value is overwritten by the array of files passed.
         Although Notion doesn't support uploading files, if you pass a file object containing a file hosted by Notion,
         it remains one of the files. To remove any file, just don't pass it in the update response.
 
         InternalFiles are a file object corresponding to a file that has been uploaded to Notion.
         ExternalFiles are a file object corresponding to an external file that has been linked to in Notion.
 
-        ---
         :param array_of_files: (required) An array of objects containing information about the files.\
                                 Either InternalFile(), ExternalFile() or a combination of both.
 
         https://developers.notion.com/reference/page-property-values#files
         """
         self._patch_properties(
             Properties(FilesPropertyValue(property_name, array_of_files))
@@ -454,32 +438,31 @@
     def set_phone_number(self, property_name: str, /, phone_number: str) -> None:
         """https://developers.notion.com/reference/page-property-values#phone-number"""
         self._patch_properties(
             Properties(PhoneNumberPropertyValue(property_name, phone_number))
         )
 
     def set_related(self, property_name: str, /, related_ids: Sequence[str]) -> None:
-        """
+        """https://developers.notion.com/reference/page-property-values#relation
+
         :param related_ids: (required) An array of related page references.\
                              A page reference is an object with an id key and a string value (UUIDv4)\
                              corresponding to a page ID in another database.
-        
-        https://developers.notion.com/reference/page-property-values#relation
         """
         list_related_ids = [_NotionUUID(id) for id in related_ids]
         self._patch_properties(
             Properties(RelationPropertyValue(property_name, list_related_ids))
         )
 
     def set_checkbox(self, property_name: str, /, value: bool) -> None:
         """https://developers.notion.com/reference/page-property-values#checkbox"""
         self._patch_properties(Properties(CheckboxPropertyValue(property_name, value)))
 
     def set_number(
-        self, property_name: str, /, new_number: Union[float, timedelta]
+        self, property_name: str, /, new_number: int | float | timedelta
     ) -> None:
         """https://developers.notion.com/reference/page-property-values#number"""
         self._patch_properties(Properties(NumberPropertyValue(property_name, new_number)))
 
     def set_people(self, property_name: str, /, user_array: Sequence[UserObject]) -> None:
         """https://developers.notion.com/reference/page-property-values#people"""
         self._patch_properties(Properties(PeoplePropertyValue(property_name, user_array)))
```

### Comparing `notion_api-0.5.2/notion/api/notionworkspace.py` & `notion_api-0.6.0/notion/api/notionworkspace.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,18 +16,20 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+from functools import partial, partialmethod
 from typing import Any, MutableMapping, Optional, Sequence, cast
 
 from notion.api._about import __base_url__
-from notion.api.client import _NotionClient
+from notion.api._pagination import paginated_response_endpoint
+from notion.api.client import _NLOG, _NotionClient
 from notion.api.notionblock import Block
 from notion.api.notionpage import Page
 from notion.properties.build import NotionObject, build_payload
 from notion.properties.common import Parent, UserObject
 from notion.properties.richtext import Mention, RichText
 from notion.query.sort import EntryTimestampSort
 
@@ -45,51 +47,54 @@
         - [Search](https://developers.notion.com/reference/post-search)
             - search workspace by title, page/database objects
         - [Comments](https://developers.notion.com/reference/create-a-comment)
             - create a comment
             - retrieve comments
     """
 
-    def __init__(
-        self,
-        token: Optional[str] = None,
-    ) -> None:
+    def __init__(self, token: Optional[str] = None) -> None:
         super().__init__(token=token)
+        self.logger = _NLOG.getChild(self.__repr__())
 
     def __repr__(self) -> str:
         return f"notion.{self.__class__.__name__}()"
 
     @staticmethod
     def _workspace_endpoint(
         *,
         users: Optional[bool] = False,
         search: Optional[bool] = None,
         user_id: Optional[str] = None,
         me: Optional[bool] = None,
     ) -> str:
-        return "%s%s%s%s%s" % (
-            __base_url__,
-            "search" if search else "",
-            "users" if users else "",
-            f"/{user_id}" if user_id else "",
-            "/me" if me else "",
+        return "".join(
+            [
+                __base_url__,
+                "search" if search else "",
+                "users" if users else "",
+                f"/{user_id}" if user_id else "",
+                "/me" if me else "",
+            ]
         )
 
     @staticmethod
     def _comments_endpoint(
         *,
         block_id: Optional[str] = None,
         page_size: Optional[int] = None,
         start_cursor: Optional[str] = None,
     ) -> str:
-        return "%scomments%s%s%s" % (
-            __base_url__,
-            f"?block_id={block_id}" if block_id else "",
-            f"&page_size={page_size}" if page_size else "",
-            f"&start_cursor={start_cursor}" if start_cursor else "",
+        return "".join(
+            [
+                __base_url__,
+                "comments",
+                f"?block_id={block_id}" if block_id else "",
+                f"&page_size={page_size}" if page_size else "",
+                f"&start_cursor={start_cursor}" if start_cursor else "",
+            ]
         )
 
     def retrieve_token_bot(self) -> MutableMapping[str, Any]:
         """Retrieves the bot User associated with the API token provided in the authorization header.
         The bot will have an owner field with information about the person who authorized the integration.
 
         https://developers.notion.com/reference/get-self
@@ -144,50 +149,83 @@
                 id=user["id"],
                 name=user["name"],
                 avatar_url=user["avatar_url"] if user["avatar_url"] else None,
                 email=user["person"]["email"] if user["person"]["email"] else None,
             )
         except KeyError:
             raise ValueError(
-                f"{self.__repr__()}: Could not find user with name: {user_name}. ",
-                "Only members and guests in the integration's workspace are visible.",
+                f"{self.__repr__()}: Could not find user with name: {user_name}. "
+                "Only members and guests in the integration's workspace are visible."
             )
 
     def retrieve_comments(
         self,
         /,
         thread: Page | Block | str,
         *,
         page_size: Optional[int] = None,
         start_cursor: Optional[str] = None,
     ) -> MutableMapping[str, Any]:
-        """ When retrieving comments, one or more Comment objects will be returned in the form of an array,
+        """
+        **retrieve_comments() method deprecated in > v0.5.2.**
+        **In a future update, this will be replaced with the new method `retrieve_all_comments()` added in v0.6.0 that iterates through all pages from results.**
+        **This method will still remain under a new name for anyone wanting the original request.**
+
+        When retrieving comments, one or more Comment objects will be returned in the form of an array,
         sorted in ascending chronological order.
 
-        Retrieving comments from a page parent will return all comments on the page, 
+        Retrieving comments from a page parent will return all comments on the page,
         but not comments from any blocks inside the page.
 
-        :param thread: (required) Either a `notion.Page`/`notion.Block` object, or the string of\
-                        a page/block/discussion_thread ID.
+        :param thread: (required) Either a notion.Page or notion.Block object,
+                       or the string of a page/block/discussion_thread ID.
 
         https://developers.notion.com/reference/retrieve-a-comment
         """
-        if isinstance(thread, Page) or isinstance(thread, Block):
+        self.logger.warning(_RETRIEVE_COMMENTS_DEPRECATION_NOTICE)
+
+        if isinstance(thread, Page | Block):
             block_id = thread.id
         else:
             block_id = thread
 
         comments_endpoint = self._comments_endpoint(
             block_id=block_id, page_size=page_size, start_cursor=start_cursor
         )
         return self._get(comments_endpoint)
 
+    def retrieve_all_comments(
+        self, thread: Page | Block | str, *, max_page_size: Optional[int] = None
+    ) -> list[MutableMapping[str, Any]]:
+        """When retrieving comments, one or more Comment objects will be returned in the form of an array,
+        sorted in ascending chronological order.
+
+        Retrieving comments from a page parent will return all comments on the page,
+        but not comments from any blocks inside the page.
+
+        :param thread: (required) Either a notion.Page or notion.Block object,
+                       or the string of a page/block/discussion_thread ID.
+        :param max_page_size: (optional) The max number of pages to include in results.\
+                               If left blank, will iterate until all comments in results are included.
+
+        https://developers.notion.com/reference/retrieve-a-comment
+        """
+        if isinstance(thread, Page | Block):
+            block_id = thread.id
+        else:
+            block_id = thread
+
+        return paginated_response_endpoint(
+            partialmethod(self._get),
+            partial(self._comments_endpoint, block_id=block_id),
+            max_page_size,
+        )
+
     def comment(
         self,
-        /,
         comment: Sequence[RichText | Mention],
         *,
         page: Optional[Page | Block | str] = None,
         block: Optional[Block | str] = None,
         discussion_id: Optional[str] = None,
     ) -> MutableMapping[str, Any] | None:
         """ Creates a comment in a page or existing discussion thread.
@@ -240,67 +278,71 @@
                 comment_thread = self.retrieve_comments(thread=block).get("results")
 
             if not comment_thread:
                 raise ValueError(
                     "Did not find a comment thread in this block. ",
                     "Starting new comment threads on a block not supported.",
                 )
-            # Regardless of which discussion_id in a comment thread is used,
-            # The next comment will always appear last, so we only get the first discussion_id.
+            # The next comment will always appear last regardless of which discussion_id
+            # in a comment thread is used,, so we only get the first discussion_id.
             thread_id = comment_thread[0]["discussion_id"]
             payload = build_payload({"discussion_id": thread_id}, comment_object)
             return self._post(self._comments_endpoint(), payload=payload)
 
         if discussion_id:
             payload = build_payload({"discussion_id": discussion_id}, comment_object)
             return self._post(self._comments_endpoint(), payload=payload)
 
-        raise ValueError(
-            "Either a parent page/block, or a discussion_id is required (not both)"
-        )
+        raise ValueError("One of page/block/discussion_id must be provided.")
 
     def search(
         self,
+        query_string: Optional[str] = None,
         *,
-        page_size: Optional[int] = 100,
-        query: Optional[str] = None,
         filter_pages: Optional[bool] = False,
         filter_databases: Optional[bool] = False,
+        page_size: Optional[int] = 100,
         start_cursor: Optional[str] = None,
         sort_ascending: Optional[bool] = None,
     ) -> MutableMapping[str, Any]:
         """
         Searches all parent or child pages and databases that have been shared with an integration.
         Returns all pages or databases, excluding duplicated linked databases, that have titles that include the query param.
         If no query param is provided, then the response contains all pages or databases that have been shared with the integration.
         The results adhere to any limitations related to an integration's capabilities.
         To limit the request to search only pages or to search only databases, use the filter param.
 
         For more information on the limitations/optimizations of search,
         see [Search optimizations and limitations](https://developers.notion.com/reference/post-search).
 
         ---
-        :param page_size: (optional) The number of items from the full list to include in the response. Maximum: 100. Default: 100.
-        :param query: (optional) The text that the API compares page and database titles against.
+        :param query_string: (optional) The text that the API compares page and database titles against.
         :param filter_pages: (optional) If set to True, limits results to only `page` objects.
         :param filter_databases:(optional) If set to True, limits results to only `database` objects.
+        :param page_size: (optional) The number of items from the full list to include in the response. Maximum: 100. Default: 100.
         :param sort_ascending: (optional) If sort is not provided, then default sort is last_edited_time descending.
         :param start_cursor: (optional) If supplied, will return a page of results starting after provided cursor.
 
         https://developers.notion.com/reference/post-search
         """
-        payload: NotionObject = NotionObject()
+        payload = NotionObject()
         payload.set("page_size", page_size)
-        if query:
-            payload.set("query", query)
+
+        if query_string:
+            payload.set("query", query_string)
         if filter_pages:
             payload.nest("filter", "property", "object")
             payload.nest("filter", "value", "page")
         if filter_databases:
             payload.nest("filter", "property", "object")
             payload.nest("filter", "value", "database")
         if start_cursor:
             payload.set("start_cursor", start_cursor)
         if sort_ascending:
             payload.set("sort", EntryTimestampSort.last_edited_time_ascending())
 
         return self._post(self._workspace_endpoint(search=True), payload=payload)
+
+
+_RETRIEVE_COMMENTS_DEPRECATION_NOTICE = """retrieve_comments() method deprecated in > v0.5.2. \
+In a future update, this will be replaced with the new method `retrieve_all_comments()` added in v0.6.0 that iterates through all pages from results. \
+This method will still remain under a new name for anyone wanting the original request."""
```

### Comparing `notion_api-0.5.2/notion/api/block_ext/code.py` & `notion_api-0.6.0/notion/api/block_ext/code.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from typing import Optional, Sequence, Union, cast
+from typing import Optional, Sequence, cast
 
 from notion.api.blockmixin import _TokenBlockMixin
 from notion.properties.options import CodeBlockLang
 
 __all__: Sequence[str] = ["CodeBlock"]
 
 
@@ -38,15 +38,15 @@
             )
 
     @property
     def language(self) -> str:
         return cast(str, self._block["code"]["language"])
 
     @language.setter
-    def language(self, value: Union[CodeBlockLang, str]) -> None:
+    def language(self, value: CodeBlockLang | str) -> None:
         self._patch(
             self._block_endpoint(self.id), payload={self.type: {"language": value}}
         )
 
     @property
     def code(self) -> str:
         try:
```

### Comparing `notion_api-0.5.2/notion/api/block_ext/equation.py` & `notion_api-0.6.0/notion/api/block_ext/equation.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.2/notion/api/block_ext/richtext.py` & `notion_api-0.6.0/notion/api/block_ext/richtext.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from typing import Optional, Sequence, Union, cast
+from typing import Any, MutableMapping, Optional, Sequence, cast
 
 from notion.api.blockmixin import _TokenBlockMixin
 from notion.properties.options import BlockColor
 from notion.properties.richtext import Annotations, RichText
 
 __all__: Sequence[str] = ["RichTextBlock"]
 
@@ -63,16 +63,14 @@
 
     @property
     def text(self) -> str:
         block = self._block[self.type]
 
         try:
             if len(block["rich_text"]) > 1:
-                print("here")
-
                 text = []
                 for rc in block["rich_text"]:
                     text.append(rc["text"]["content"])
 
                 return "".join(text)
 
             else:
@@ -106,15 +104,15 @@
     def annotate(
         self,
         bold: Optional[bool] = None,
         italic: Optional[bool] = None,
         strikethrough: Optional[bool] = None,
         underline: Optional[bool] = None,
         code: Optional[bool] = None,
-        color: Union[Optional[BlockColor], str] = None,
+        color: Optional[BlockColor | str] = None,
     ) -> None:
         text = self._block[self.type]
         annotations = Annotations(
             bold=bold,
             italic=italic,
             strikethrough=strikethrough,
             underline=underline,
```

### Comparing `notion_api-0.5.2/notion/api/block_ext/table.py` & `notion_api-0.6.0/notion/api/block_ext/table.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,47 +16,44 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+# mypy: disable-error-code="no-redef"
+
 from __future__ import annotations
 
 from typing import Any, Collection, MutableMapping, Optional, Sequence
 
 from notion.api.blockmixin import _TokenBlockMixin
 from notion.api.client import _NLOG
 from notion.properties.blocktypes import BlockChildren, TableRowBlockType
 from notion.properties.richtext import RichText
 
 __all__: Sequence[str] = ("TableBlock", "CELLS_ARRAY")
 
 
 CELLS_ARRAY = Sequence[list[dict[str, Collection[str]]]]
-""" An array of cell contents in horizontal display order. Each cell is an array of rich text objects. """
+""" An array of cell contents in horizontal display order. 
+Each cell is an array of rich text objects. """
 
 
 class TableBlock(_TokenBlockMixin):
     """
     Note that the number of columns in a table can only be set when the table is first created.
     Calls to the Update block endpoint to update table_width fail.
-    See examples in repo `examples/block_extensions.md` for more details.
+    See examples in [examples/block_extensions.md](https://github.com/ayvi-0001/notion-api/blob/main/examples/block_extensions.md) for more details.
 
     Table:      https://developers.notion.com/reference/block#table
     Table Rows: https://developers.notion.com/reference/block#table-rows
     """
 
-    def __init__(
-        self,
-        id: str,
-        /,
-        *,
-        token: Optional[str] = None,
-    ) -> None:
+    def __init__(self, id: str, /, *, token: Optional[str] = None) -> None:
         super().__init__(id, token=token)
         self.logger = _NLOG.getChild(self.__repr__())
 
         if self.type != "table":
             raise TypeError(
                 f"Block type must be 'table', not '{self.type}' for TableBlock."
             )
@@ -99,24 +96,22 @@
         """:raises: NotionValidationError
         if the length of values_array is not equal to the number of cells in table row.
         """
         if not values_array:
             cells: CELLS_ARRAY = [[] for _ in range(self.table_width)]
             row = [TableRowBlockType(cells)]
             self._patch(
-                self._block_endpoint(self.id, children=True),
-                payload=BlockChildren(row),
+                self._block_endpoint(self.id, children=True), payload=BlockChildren(row)
             )
 
         else:
             cells: CELLS_ARRAY = [[RichText(value)] for value in values_array]
             row = [TableRowBlockType(cells)]
             self._patch(
-                self._block_endpoint(self.id, children=True),
-                payload=BlockChildren(row),
+                self._block_endpoint(self.id, children=True), payload=BlockChildren(row)
             )
 
     def overwrite_row(self, row_index: int, values_array: list[str]) -> None:
         table_row = self.rows[row_index]
         table_row_id = table_row["id"]
         table_row["table_row"]["cells"] = [[RichText(value)] for value in values_array]
```

### Comparing `notion_api-0.5.2/notion/api/block_ext/todo.py` & `notion_api-0.6.0/notion/api/block_ext/todo.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.2/notion/exceptions/__init__.py` & `notion_api-0.6.0/notion/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.2/notion/exceptions/errors.py` & `notion_api-0.6.0/notion/exceptions/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,145 +19,159 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from typing import Sequence
 
 __all__: Sequence[str] = (
-    "_NotionErrors",
+    "NotionConflictError",
+    "NotionDatabaseConnectionUnavailable",
+    "NotionGatewayTimeout",
+    "NotionInvalidGrant",
+    "NotionInternalServerError",
     "NotionInvalidJson",
-    "NotionInvalidRequestUrl",
     "NotionInvalidRequest",
-    "NotionValidationError",
+    "NotionInvalidRequestUrl",
     "NotionMissingVersion",
-    "NotionUnauthorized",
-    "NotionRestrictedResource",
     "NotionObjectNotFound",
-    "NotionConflictError",
     "NotionRateLimited",
-    "NotionInternalServerError",
+    "NotionRestrictedResource",
     "NotionServiceUnavailable",
-    "NotionDatabaseConnectionUnavailable",
+    "NotionUnauthorized",
+    "NotionValidationError",
+    "_NotionErrors",
 )
 
 
 class _NotionErrors(BaseException):
     """Base for an error raised by this API. Any exceptions should derive from this.
 
     More info on Errors and Request Limits:
-     - https://developers.notion.com/reference/errors
+     - https://developers.notion.com/reference/status-codes
      - https://developers.notion.com/reference/request-limits
     """
 
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
 
 class NotionInvalidJson(_NotionErrors):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
-
         self.__notes__: list[str] = [
             "Error 400: The request body could not be decoded as JSON."
         ]
 
 
 class NotionInvalidRequestUrl(_NotionErrors):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
-
         self.__notes__: list[str] = ["Error 400: The request URL is not valid."]
 
 
 class NotionInvalidRequest(_NotionErrors):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
-
         self.__notes__: list[str] = ["Error 400: This request is not supported."]
 
 
-class NotionValidationError(_NotionErrors):
+
+class NotionInvalidGrant(_NotionErrors):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
+        self.__notes__: list[str] = [
+            "Error 400: The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is", 
+            "invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client.", 
+            "See OAuth 2.0 documentation for more information."
+            ]
+
 
+class NotionValidationError(_NotionErrors):
+    def __init__(self, *args: object) -> None:
+        super().__init__(*args)
         self.__notes__: list[str] = [
             "Error 400: The request body does not match the schema for the expected parameters."
         ]
 
 
 class NotionMissingVersion(_NotionErrors):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
-
         self.__notes__: list[str] = [
             "Error 400: The request is missing the required Notion-Version header. See Versioning."
         ]
 
 
 class NotionUnauthorized(_NotionErrors):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
-
         self.__notes__: list[str] = ["Error 401: The bearer token is not valid."]
 
 
 class NotionRestrictedResource(_NotionErrors):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
-
         self.__notes__: list[str] = [
-            "Error 403: Given the bearer token used, the client doesn't have permission to perform this operation."
+            "Error 403: Given the bearer token used, "
+            "the client doesn't have permission to perform this operation."
         ]
 
 
 class NotionObjectNotFound(_NotionErrors):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
-
         self.__notes__: list[str] = [
-            "Error 404: Given the bearer token used, the resource does not exist. This error can also indicate that the resource has not been shared with owner of the bearer token."
+            "Error 404: Given the bearer token used, the resource does not exist. ",
+            "This error can also indicate that the resource has not been shared with owner of the bearer token.",
         ]
 
 
 class NotionConflictError(_NotionErrors):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
-
         self.__notes__: list[str] = [
-            "Error 409: The transaction could not be completed, potentially due to a data collision. Make sure the parameters are up to date and try again."
+            "Error 409: The transaction could not be completed, potentially due to a data collision. ",
+            "Make sure the parameters are up to date and try again.",
         ]
 
 
 class NotionRateLimited(_NotionErrors):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
-
         self.__notes__: list[str] = [
-            "Error 429: This request exceeds the number of requests allowed. Slow down and try again. More details on rate limits."
+            "Error 429: This request exceeds the number of requests allowed. ",
+            "Slow down and try again. More details on rate limits.",
         ]
 
 
 class NotionInternalServerError(_NotionErrors):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
-
         self.__notes__: list[str] = [
             "Error 500: An unexpected error occurred. Reach out to Notion support."
         ]
 
 
 class NotionServiceUnavailable(_NotionErrors):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
-
         self.__notes__: list[str] = [
-            "Error 503: Notion is unavailable. Try again later. This can occur when the time to respond to a request takes longer than 60 seconds, the maximum request timeout."
+            "Error 503: Notion is unavailable. Try again later. ",
+            "This can occur when the time to respond to a request takes longer than 60 seconds, ",
+            "the maximum request timeout.",
         ]
 
 
 class NotionDatabaseConnectionUnavailable(_NotionErrors):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
-
         self.__notes__: list[str] = [
             "Error 503: Notion's database is unavailable or in an unqueryable state. Try again later."
         ]
+
+
+class NotionGatewayTimeout(_NotionErrors):
+    def __init__(self, *args: object) -> None:
+        super().__init__(*args)
+        self.__notes__: list[str] = [
+            "Error 504: Notion timed out while attempting to complete this request. Please try again later."
+        ]
```

### Comparing `notion_api-0.5.2/notion/exceptions/validate.py` & `notion_api-0.6.0/notion/exceptions/validate.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,79 +16,96 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from typing import Any, MutableMapping, Sequence, Union
+from typing import Any, MutableMapping, Sequence
 
-from notion.exceptions.errors import *
+from notion.exceptions.errors import (
+    NotionConflictError,
+    NotionDatabaseConnectionUnavailable,
+    NotionGatewayTimeout,
+    NotionInternalServerError,
+    NotionInvalidGrant,
+    NotionInvalidJson,
+    NotionInvalidRequest,
+    NotionInvalidRequestUrl,
+    NotionMissingVersion,
+    NotionObjectNotFound,
+    NotionRateLimited,
+    NotionRestrictedResource,
+    NotionServiceUnavailable,
+    NotionUnauthorized,
+    NotionValidationError,
+    _NotionErrors,
+)
 
 __all__: Sequence[str] = ["validate_response"]
 
 
-def validate_response(response: MutableMapping[str, Any]) -> Union[_NotionErrors, None]:
-    r"""
-    Example:
-    ```py
-    page = notion.Page("12345")
-
-    # Object for invalid Notion requests:
-    # {
-    #   'object': 'error',
-    #   'status': 400,
-    #   'code': 'validation_error',
-    #   'message': 'path failed validation: path.page_id should be a valid uuid, instead was `"12345"`.'
-    # }
+def validate_response(response: MutableMapping[str, Any]) -> _NotionErrors | None:
+    r"""Example:
+    >>> page = notion.Page("12345")
+
+    ```json
+    // Object for invalid Notion requests:
+    {
+      "object": "error",
+      "status": 400,
+      "code": "validation_error",
+      "message": "path failed validation: path.page_id should be a valid uuid, instead was `"12345"`."
+    }
     ```
-    ------
-    ```sh
+    ---
+    ```shell
     Traceback (most recent call last):
       File "c:\path\to\file\_.py", line 212, in <module>
         validate_response(response)
       File "c:\path\to\file\_.py", line 186, in validate_response
-        raise NotionValidationError(message)
+        raise NotionValidationError(response["message"])
     notion.exceptions.errors.NotionValidationError: path failed validation: path.page_id should be a valid uuid, instead was `"12345"`.
     Error 400:
     The request body does not match the schema for the expected parameters.
     ```
 
     More info on Errors and Request Limits:
-     - https://developers.notion.com/reference/errors
+     - https://developers.notion.com/reference/status-codes
      - https://developers.notion.com/reference/request-limits
     """
     if not "error" in response.values():
         return None
 
-    code = response["code"]
-    message = response["message"]
-
-    match code:
+    match response["code"]:
         case "invalid_json":
-            raise NotionInvalidJson(message)
+            raise NotionInvalidJson(response["message"])
         case "invalid_request_url":
-            raise NotionInvalidRequestUrl(message)
+            raise NotionInvalidRequestUrl(response["message"])
         case "invalid_request":
-            raise NotionInvalidRequest(message)
+            raise NotionInvalidRequest(response["message"])
         case "validation_error":
-            raise NotionValidationError(message)
+            raise NotionValidationError(response["message"])
         case "missing_version":
-            raise NotionMissingVersion(message)
+            raise NotionMissingVersion(response["message"])
         case "unauthorized":
-            raise NotionUnauthorized(message)
+            raise NotionUnauthorized(response["message"])
         case "restricted_resource":
-            raise NotionRestrictedResource(message)
+            raise NotionRestrictedResource(response["message"])
         case "object_not_found":
-            raise NotionObjectNotFound(message)
+            raise NotionObjectNotFound(response["message"])
         case "conflict_error":
-            raise NotionConflictError(message)
+            raise NotionConflictError(response["message"])
         case "rate_limited":
-            raise NotionRateLimited(message)
+            raise NotionRateLimited(response["message"])
         case "internal_server_error":
-            raise NotionInternalServerError(message)
+            raise NotionInternalServerError(response["message"])
         case "service_unavailable":
-            raise NotionServiceUnavailable(message)
+            raise NotionServiceUnavailable(response["message"])
         case "database_connection_unavailable":
-            raise NotionDatabaseConnectionUnavailable(message)
+            raise NotionDatabaseConnectionUnavailable(response["message"])
+        case "gateway_timeout":
+            raise NotionGatewayTimeout(response["message"])
+        case "invalid_grant":
+            raise NotionInvalidGrant(response["message"])
         case _:
             return None
```

### Comparing `notion_api-0.5.2/notion/properties/__init__.py` & `notion_api-0.6.0/notion/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.2/notion/properties/blocktypes.py` & `notion_api-0.6.0/notion/properties/blocktypes.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from typing import Any, Collection, MutableMapping, Optional, Sequence, Union
+from typing import Any, Collection, MutableMapping, Optional, Sequence
 
 from notion.properties.build import NotionObject
 from notion.properties.common import _NotionURL
 from notion.properties.files import ExternalFile
 from notion.properties.options import BlockColor, CodeBlockLang
 from notion.properties.richtext import Mention, RichText
 
@@ -63,21 +63,24 @@
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
         block_type_objects_array: Optional[
             Sequence[NotionObject | MutableMapping[str, Any]]
         ] = None,
+        after: Optional[str] = None,
     ) -> None:
         """https://developers.notion.com/reference/block"""
         super().__init__()
         if not block_type_objects_array:
             block_type_objects_array = []
 
         self.set("children", block_type_objects_array)
+        if after:
+            self.set("after", after)
 
 
 class OriginalSyncedBlockType(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(self, children: Optional[list[str]]) -> None:
         """https://developers.notion.com/reference/block#original-synced-block"""
@@ -105,15 +108,15 @@
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
         rich_text: Sequence[RichText | Mention],
         /,
         *,
-        block_color: Optional[Union[BlockColor, str]] = None,
+        block_color: Optional[BlockColor | str] = None,
     ) -> None:
         """https://developers.notion.com/reference/block#paragraph"""
         super().__init__()
         if not block_color:
             block_color = BlockColor.default.value
 
         self.set("type", "paragraph")
@@ -129,15 +132,15 @@
 
     def __init__(
         self,
         rich_text: Sequence[RichText | Mention],
         /,
         *,
         icon: Optional[str] = None,
-        block_color: Optional[Union[BlockColor, str]] = None,
+        block_color: Optional[BlockColor | str] = None,
     ) -> None:
         """https://developers.notion.com/reference/block#callout"""
         super().__init__()
         if not block_color:
             block_color = BlockColor.default.value
 
         self.set("type", "callout")
@@ -151,15 +154,15 @@
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
         rich_text: Sequence[RichText | Mention],
         /,
         *,
-        block_color: Optional[Union[BlockColor, str]] = None,
+        block_color: Optional[BlockColor | str] = None,
     ) -> None:
         """https://developers.notion.com/reference/block#quote"""
         super().__init__()
         if not block_color:
             block_color = BlockColor.default.value
 
         self.set("type", "quote")
@@ -171,15 +174,15 @@
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
         rich_text: Sequence[RichText | Mention],
         /,
         *,
-        block_color: Optional[Union[BlockColor, str]] = None,
+        block_color: Optional[BlockColor | str] = None,
     ) -> None:
         """https://developers.notion.com/reference/block#bulleted-list-item"""
         super().__init__()
         if not block_color:
             block_color = BlockColor.default.value
 
         self.set("type", "bulleted_list_item")
@@ -191,15 +194,15 @@
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
         rich_text: Sequence[RichText | Mention],
         /,
         *,
-        block_color: Optional[Union[BlockColor, str]] = None,
+        block_color: Optional[BlockColor | str] = None,
     ) -> None:
         """https://developers.notion.com/reference/block#numbered-list-item"""
         super().__init__()
         if not block_color:
             block_color = BlockColor.default.value
 
         self.set("type", "numbered_list_item")
@@ -212,15 +215,15 @@
 
     def __init__(
         self,
         rich_text: Sequence[RichText | Mention],
         /,
         *,
         checked: Optional[bool] = False,
-        block_color: Optional[Union[BlockColor, str]] = None,
+        block_color: Optional[BlockColor | str] = None,
     ) -> None:
         """https://developers.notion.com/reference/block#to-do"""
         super().__init__()
         if not block_color:
             block_color = BlockColor.default.value
 
         self.set("type", "to_do")
@@ -233,15 +236,15 @@
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
         rich_text: Sequence[RichText | Mention],
         /,
         *,
-        block_color: Optional[Union[BlockColor, str]] = None,
+        block_color: Optional[BlockColor | str] = None,
     ) -> None:
         """https://developers.notion.com/reference/block#toggle-blocks"""
         super().__init__()
         if not block_color:
             block_color = BlockColor.default.value
 
         self.set("type", "toggle")
@@ -253,15 +256,15 @@
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
         rich_text: Optional[Sequence[RichText | Mention]] = None,
         /,
         *,
-        language: Optional[Union[CodeBlockLang, str]] = None,
+        language: Optional[CodeBlockLang | str] = None,
         caption: Optional[Sequence[RichText | Mention | str]] = None,
     ) -> None:
         """https://developers.notion.com/reference/block#code"""
         super().__init__()
         if not language:
             language = CodeBlockLang.plain_text.value
 
@@ -310,15 +313,15 @@
         self.set("type", "equation")
         self.nest("equation", "expression", expression)
 
 
 class TableOfContentsBlocktype(NotionObject):
     __slots__: Sequence[str] = ()
 
-    def __init__(self, block_color: Optional[Union[BlockColor, str]] = None) -> None:
+    def __init__(self, block_color: Optional[BlockColor | str] = None) -> None:
         """https://developers.notion.com/reference/block#table-of-contents"""
         super().__init__()
         if not block_color:
             block_color = BlockColor.default.value
 
         self.set("type", "table_of_contents")
         self.nest("table_of_contents", "color", block_color)
@@ -328,15 +331,15 @@
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
         rich_text: Sequence[RichText | Mention],
         /,
         *,
-        block_color: Optional[Union[BlockColor, str]] = None,
+        block_color: Optional[BlockColor | str] = None,
         is_toggleable: Optional[bool] = False,
     ) -> None:
         """https://developers.notion.com/reference/block#headings"""
         super().__init__()
         if not block_color:
             block_color = BlockColor.default.value
 
@@ -350,15 +353,15 @@
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
         rich_text: Sequence[RichText | Mention],
         /,
         *,
-        block_color: Optional[Union[BlockColor, str]] = None,
+        block_color: Optional[BlockColor | str] = None,
         is_toggleable: Optional[bool] = False,
     ) -> None:
         """https://developers.notion.com/reference/block#headings"""
         super().__init__()
         if not block_color:
             block_color = BlockColor.default.value
 
@@ -372,15 +375,15 @@
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
         rich_text: Sequence[RichText | Mention],
         /,
         *,
-        block_color: Optional[Union[BlockColor, str]] = None,
+        block_color: Optional[BlockColor | str] = None,
         is_toggleable: Optional[bool] = False,
     ) -> None:
         """https://developers.notion.com/reference/block#headings"""
         super().__init__()
         if not block_color:
             block_color = BlockColor.default.value
 
@@ -460,14 +463,13 @@
         self.nest("table", "children", children)
 
 
 class TableRowBlockType(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(
-        self,
-        cells: Sequence[list[dict[str, Collection[str]]]] | None = None,
+        self, cells: Sequence[list[dict[str, Collection[str]]]] | None = None
     ) -> None:
         """https://developers.notion.com/reference/block#table-rows"""
         super().__init__()
         self.set("type", "table_row")
         self.nest("table_row", "cells", cells)
```

### Comparing `notion_api-0.5.2/notion/properties/build.py` & `notion_api-0.6.0/notion/properties/build.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,48 +19,42 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from __future__ import annotations
 
 from types import ModuleType
-from typing import Any, MutableMapping, Optional, Sequence, Union, cast
+from typing import Any, MutableMapping, Optional, Sequence, cast
 
 try:
     import orjson
 
-    default_json: ModuleType = orjson
+    _json: ModuleType = orjson
 except ModuleNotFoundError:
     import json
 
-    default_json: ModuleType = json
+    _json: ModuleType = json  # type: ignore[no-redef]
 
 __all__: Sequence[str] = ["build_payload"]
 
 
-def build_payload(*__obj: MutableMapping[str, Any]) -> Union[str, bytes]:
+def build_payload(*__obj: MutableMapping[str, Any]) -> str | bytes:
     final: dict[str, Any] = {}
     for o in __obj:
         final.update(o)
-    return cast(Union[str, bytes], default_json.dumps(final))
+    return cast(str | bytes, _json.dumps(final))
 
 
 class NotionObject(dict[str, Any]):
     def set(self, __key: str, __val: Any) -> None:
         self[__key] = __val
 
     def nest(self, __Pkey: str, __Ckey: Optional[str], __val: Any) -> None:
         if __Pkey not in self:
             self.set(__Pkey, {__Ckey: __val})
         else:
             self[__Pkey].update({__Ckey: __val})
 
     def set_array(
-        self,
-        __key: str,
-        values: Union[
-            bytes,
-            MutableMapping[str, Any],
-            Sequence[Union[bytes, Any]],
-        ],
+        self, __key: str, values: bytes | MutableMapping[str, Any] | Sequence[bytes | Any]
     ) -> None:
         self[__key] = list(values)
```

### Comparing `notion_api-0.5.2/notion/properties/common.py` & `notion_api-0.6.0/notion/properties/common.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.2/notion/properties/files.py` & `notion_api-0.6.0/notion/properties/files.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,37 +25,35 @@
 Page, embed, image, video, file, pdf, and bookmark block types all contain file objects. 
 Icon and cover page object values also contain file objects.
 
 A file with type `file` must contain a Notion hosted file url. Use type `external` for externally hosted files.
 """
 from __future__ import annotations
 
-from typing import Optional, Sequence, Union
+from typing import Optional, Sequence
 
 from notion.properties.build import NotionObject
 from notion.properties.common import _NotionURL
 from notion.properties.propertyvalues import PagePropertyValue
-from notion.properties.richtext import Equation, Mention, RichText
+from notion.properties.richtext import Mention, RichText
 
 __all__: Sequence[str] = (
     "Icon",
     "Cover",
     "ExternalFile",
     "InternalFile",
     "FilesPropertyValue",
 )
 
 
 class FilesPropertyValue(PagePropertyValue, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
     def __init__(
-        self,
-        property_name: str,
-        array_of_files: Sequence[Union[InternalFile, ExternalFile]],
+        self, property_name: str, array_of_files: Sequence[InternalFile | ExternalFile]
     ) -> None:
         """
         When updating a file property, the value is overwritten by the array of files passed.
         Although Notion doesn't support uploading files, if you pass a file object containing a file hosted by Notion,
         it remains one of the files. To remove any file, just don't pass it in the update response.
 
         InternalFiles are a file object corresponding to a file that has been uploaded to Notion.
@@ -96,19 +94,15 @@
         self.set("cover", ExternalFile(file_url))
 
 
 class ExternalFile(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(
-        self,
-        url: str,
-        /,
-        *,
-        caption: Optional[Sequence[RichText | Mention]] = None,
+        self, url: str, /, *, caption: Optional[Sequence[RichText | Mention]] = None
     ) -> None:
         """
         The Notion API supports adding, retrieving, and updating links to external files.
         For "external" file objects, the name is the same as the file's host URL.
 
         https://developers.notion.com/reference/file-object#external-files
         """
@@ -126,15 +120,15 @@
         name: str,
         url: str,
         *,
         caption: Optional[Sequence[RichText | Mention]] = None,
     ) -> None:
         """
         Internal files are any files hosted on Notion
-        They begin with: https://s3.us-west-2.amazonaws.com/secure.notion-static.com/{block_id}/...
+        They begin with: https://s3.{region}.amazonaws.com/secure.notion-static.com/{block_id}/...
         You can retrieve links to Notion-hosted files via the Retrieve block children endpoint.
 
         https://developers.notion.com/reference/file-object#notion-hosted-files
         """
         super().__init__()
         self.set("type", "file")
         self.set("file", _NotionURL(url))
```

### Comparing `notion_api-0.5.2/notion/properties/options.py` & `notion_api-0.6.0/notion/properties/options.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.2/notion/properties/propertyobjects.py` & `notion_api-0.6.0/notion/properties/propertyobjects.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
       Update these values from the Notion UI, instead.
 
 https://developers.notion.com/reference/property-object
 """
 from __future__ import annotations
 
 from abc import ABCMeta
-from typing import Optional, Sequence, Union
+from typing import Optional, Sequence
 
 from notion.properties.build import NotionObject
 from notion.properties.options import FunctionFormat, NumberFormat, PropertyColor
 from notion.properties.richtext import RichText
 
 __all__: Sequence[str] = (
     "DatabaseDescription",
@@ -131,15 +131,15 @@
 
 class RelationPropertyObject(PropertyObject, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
     def __init__(
         self,
         property_name: str,
-        relation_type: Optional[Union[_DualProperty, _SingleProperty]] = None,
+        relation_type: Optional[_DualProperty | _SingleProperty] = None,
     ) -> None:
         """
         Use classmethods:
          - `dual`
          - `single`
 
         https://developers.notion.com/reference/property-object#relation
@@ -169,15 +169,15 @@
         return cls(property_name, _SingleProperty(database_id))
 
 
 class Option(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(
-        self, option_name: str, color: Optional[Union[PropertyColor, str]] = None, /
+        self, option_name: str, color: Optional[PropertyColor | str] = None, /
     ) -> None:
         """
         :param name: (required) The name of the option as it appears in the Notion UI.\
                       Note: Commas (",") are not valid for select values.
         :param color: (required) The color of the option as rendered in the Notion UI.\
                        Use `notion.properties.PropertyColor` for reference.
         """
@@ -185,39 +185,39 @@
         self.set("name", option_name)
         self.set("color", color) if color else None
 
 
 class MultiSelectPropertyObject(PropertyObject, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
-    def __init__(self, property_name: str, /, options: list[Option]) -> None:
+    def __init__(self, property_name: str, /, options: Sequence[Option]) -> None:
         """https://developers.notion.com/reference/property-object#multi-select"""
         super().__init__(property_name=property_name)
         self.set("type", "multi_select")
         self.nest("multi_select", "options", options)
 
 
 class SelectPropertyObject(PropertyObject, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
-    def __init__(self, property_name: str, /, options: list[Option]) -> None:
+    def __init__(self, property_name: str, /, options: Sequence[Option]) -> None:
         """https://developers.notion.com/reference/property-object#select"""
         super().__init__(property_name=property_name)
         self.set("type", "select")
         self.nest("select", "options", options)
 
 
 class NumberPropertyObject(PropertyObject, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
     def __init__(
         self,
         property_name: str,
         /,
-        format: Optional[Union[NumberFormat, str]] = NumberFormat.number.value,
+        format: Optional[NumberFormat | str] = NumberFormat.number.value,
     ) -> None:
         """https://developers.notion.com/reference/property-object#number"""
         super().__init__(property_name=property_name)
         self.set("type", "number")
         self.nest("number", "format", format)
 
 
@@ -360,18 +360,15 @@
     __slots__: Sequence[str] = ["name"]
 
     def __init__(
         self,
         property_name: str,
         relation_property_name: str,
         rollup_property_name: str,
-        function: Optional[
-            Union[FunctionFormat, str]
-        ] = FunctionFormat.show_original.value,
-        /,
+        function: Optional[FunctionFormat | str] = FunctionFormat.show_original.value,
     ) -> None:
         """https://developers.notion.com/reference/property-object#rollup"""
         super().__init__(property_name=property_name)
         self.set("type", "rollup")
         self.nest("rollup", "relation_property_name", relation_property_name)
         self.nest("rollup", "rollup_property_name", rollup_property_name)
         self.nest("rollup", "function", function)
```

### Comparing `notion_api-0.5.2/notion/properties/propertyvalues.py` & `notion_api-0.6.0/notion/properties/propertyvalues.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,21 +47,21 @@
 
 https://developers.notion.com/reference/page-property-values
 """
 from __future__ import annotations
 
 from abc import ABCMeta
 from datetime import datetime
-from typing import TYPE_CHECKING, Optional, Sequence, Union
+from typing import TYPE_CHECKING, Optional, Sequence
 
 from notion.properties.build import NotionObject
 from notion.properties.common import UserObject, _NotionUUID
 from notion.properties.options import FunctionFormat
 from notion.properties.propertyobjects import Option, PropertyObject
-from notion.properties.richtext import Equation, Mention, RichText
+from notion.properties.richtext import Mention, RichText
 
 if TYPE_CHECKING:
     from datetime import timedelta
 
 __all__: Sequence[str] = (
     "Properties",
     "RichTextPropertyValue",
@@ -85,15 +85,15 @@
     def __init__(self, property_name: str) -> None:
         self.name = property_name
 
 
 class Properties(NotionObject):
     __slots__: Sequence[str] = ()
 
-    def __init__(self, *properties: Union[PropertyObject, PagePropertyValue]) -> None:
+    def __init__(self, *properties: PropertyObject | PagePropertyValue) -> None:
         """
         A page object is made up of page properties that contain data about the page.
         When you send a request to Create a page, you set the page properties in the properties object body param.
         Retrieve a page gets the identifier, type, and value of a page's properties.
         Retrieve a page property item returns information about a single property ID.
 
         https://developers.notion.com/reference/page-property-values"""
@@ -108,18 +108,15 @@
                 self.nest("properties", prop.name, prop)
 
 
 class RichTextPropertyValue(PagePropertyValue, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
     def __init__(
-        self,
-        property_name: str,
-        /,
-        rich_text: Sequence[RichText | Mention],
+        self, property_name: str, /, rich_text: Sequence[RichText | Mention]
     ) -> None:
         """
         The purpose of the rich text property value is to provide the key `rich_text`,
         whereas the object `notion.properties.RichText` has the key `text`.
 
         :param rich_text: (required) An array of rich text objects.
 
@@ -130,15 +127,15 @@
         self.set("type", "rich_text")
         self.set("rich_text", rich_text)
 
 
 class TitlePropertyValue(PagePropertyValue, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
-    def __init__(self, title_: Sequence[Union[RichText, Mention]]) -> None:
+    def __init__(self, title_: Sequence[RichText | Mention]) -> None:
         """
         :param title: (required) An array of rich text objects
 
         https://developers.notion.com/reference/page-property-values#title
         """
         super().__init__(property_name="title")
         self.set_array(self.name, title_)
@@ -148,16 +145,16 @@
     __slots__: Sequence[str] = ["name"]
 
     def __init__(
         self,
         property_name: str,
         /,
         *,
-        start: Union[str, datetime],
-        end: Optional[Union[str, datetime]] = None,
+        start: str | datetime,
+        end: Optional[str | datetime] = None,
     ) -> None:
         """
         Notion uses ISO 8601 date and time for some endpoints, and YYYY/MM/DD for others.
         If a datetime object is passed to either parameter, they'll be converted to isoformat.
 
         ---
         :param start: (required) A date, with an optional time.\
@@ -171,20 +168,15 @@
         self.nest("date", "start", start)
         self.nest("date", "end", end) if end else None
 
 
 class RelationPropertyValue(PagePropertyValue, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
-    def __init__(
-        self,
-        property_name: str,
-        /,
-        related_ids: Sequence[_NotionUUID],
-    ) -> None:
+    def __init__(self, property_name: str, /, related_ids: Sequence[_NotionUUID]) -> None:
         """
         NOTE: updating a relation property value with an empty array will clear the list.
 
         ---
         :param related_ids: (required) An array of related page references.\
                              A page reference is an object with an id key and a string value (UUIDv4)\
                              corresponding to a page ID in another database.
@@ -230,15 +222,15 @@
         self.set("type", "select")
         self.set("select", select_option)
 
 
 class MultiSelectPropertyValue(PagePropertyValue, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
-    def __init__(self, property_name: str, /, options_array: list[Option]) -> None:
+    def __init__(self, property_name: str, /, options_array: Sequence[Option]) -> None:
         """
         The MultiSelectPropertyValue contains an array of `notion.properties.Option` objects.
         When selecting options, If the multi-select database property does not yet have an option by the input name,
         then the name will be added to the database schema if the integration also has write access to the parent database.
 
         ---
         :param options_array: (required) array of `notion.properties.Option`\
@@ -279,17 +271,15 @@
         self.set("type", "people")
         self.set("people", user_array)
 
 
 class RollupPropertyValue(PagePropertyValue, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
-    def __init__(
-        self, property_name: str, /, function: Union[FunctionFormat, str]
-    ) -> None:
+    def __init__(self, property_name: str, /, function: FunctionFormat | str) -> None:
         """
         If the results of the rollup is a date (e.g. function = latest date),
         the results will be a DatePropertyValue.
 
         If the results of the rollup is a number (e.g. function = sum),
         the results will be a NumberPropertyValue.
 
@@ -314,15 +304,15 @@
         self.set("type", "email")
         self.set("email", email)
 
 
 class NumberPropertyValue(PagePropertyValue, NotionObject):
     __slots__: Sequence[str] = ["name"]
 
-    def __init__(self, property_name: str, /, number: Union[float, timedelta]) -> None:
+    def __init__(self, property_name: str, /, number: int | float | timedelta) -> None:
         """https://developers.notion.com/reference/page-property-values#number"""
         super().__init__(property_name=property_name)
         self.set("type", "number")
         self.set("number", number)
 
 
 class PhoneNumberPropertyValue(PagePropertyValue, NotionObject):
```

### Comparing `notion_api-0.5.2/notion/properties/richtext.py` & `notion_api-0.6.0/notion/properties/richtext.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from __future__ import annotations
 
-from typing import Optional, Sequence, Union
+from typing import Optional, Sequence
 
 from notion.properties.build import NotionObject
 from notion.properties.common import UserObject, _NotionURL
 from notion.properties.options import BlockColor
 
 __all__: Sequence[str] = (
     "Annotations",
@@ -40,15 +40,14 @@
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
         content: Optional[str] = None,
         /,
         annotations: Optional[Annotations] = None,
-        *,
         link: Optional[str] = None,
     ) -> None:
         """
         Rich text objects contain the data that Notion uses to display
         formatted text,mentions, and inline equations.
         Arrays of rich text objects within database property objects and page property value objects
         are used to create what a user experiences as a single text value in Notion.
@@ -78,18 +77,17 @@
 
 
 class Mention(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
-        /,
         *,
         type: str,
-        mention_type_object: Union[UserObject, NotionObject],
+        mention_type_object: UserObject | NotionObject,
         annotations: Optional[Annotations] = None,
     ) -> None:
         """
         Use Classmethods:
          - `user`
          - `today`
          - `database`
@@ -105,36 +103,28 @@
         self.nest("mention", type, mention_type_object)
 
         if annotations and annotations != {}:
             self.set("annotations", annotations)
 
     @classmethod
     def user(
-        cls,
-        user_object: UserObject,
-        /,
-        *,
-        annotations: Optional[Annotations] = None,
+        cls, user_object: UserObject, /, *, annotations: Optional[Annotations] = None
     ) -> Mention:
         """
         If your integration doesn't yet have access to the mentioned user,
         then the plain_text that would include a user's name reads as "@Anonymous".
         To update the integration to get access to the user,
         update the integration capabilities on the integration settings page.
 
         :raises: `notion.exceptions.errors.NotionValidationError` if trying to mention a Bot.
 
         https://developers.notion.com/reference/rich-text#user-mention-type-object
         """
 
-        return cls(
-            type="user",
-            mention_type_object=user_object,
-            annotations=annotations,
-        )
+        return cls(type="user", mention_type_object=user_object, annotations=annotations)
 
     @classmethod
     def today(cls, *, annotations: Optional[Annotations] = None) -> Mention:
         """https://developers.notion.com/reference/rich-text#template-mention-type-object"""
         template_mention_date = NotionObject()
         template_mention_date.set("type", "template_mention_date")
         template_mention_date.set("template_mention_date", "today")
@@ -150,30 +140,24 @@
         cls, database_id: str, *, annotations: Optional[Annotations] = None
     ) -> Mention:
         """https://developers.notion.com/reference/rich-text#database-mention-type-object"""
         database_mention = NotionObject()
         database_mention.set("id", database_id)
 
         return cls(
-            type="database",
-            mention_type_object=database_mention,
-            annotations=annotations,
+            type="database", mention_type_object=database_mention, annotations=annotations
         )
 
     @classmethod
     def page(cls, page_id: str, *, annotations: Optional[Annotations] = None) -> Mention:
         """https://developers.notion.com/reference/rich-text#page-mention-type-object"""
         page_mention = NotionObject()
         page_mention.set("id", page_id)
 
-        return cls(
-            type="page",
-            mention_type_object=page_mention,
-            annotations=annotations,
-        )
+        return cls(type="page", mention_type_object=page_mention, annotations=annotations)
 
     @classmethod
     def link_preview(
         cls, url: str, *, annotations: Optional[Annotations] = None
     ) -> Mention:
         """https://developers.notion.com/reference/rich-text#link-preview-mention-type-object"""
         link_preview_mention = NotionObject()
@@ -194,32 +178,28 @@
         annotations: Optional[Annotations] = None,
     ) -> Mention:
         """https://developers.notion.com/reference/rich-text#date-mention-type-object"""
         date_mention = NotionObject()
         date_mention.set("start", start)
         date_mention.set("end", end) if end else None
 
-        return cls(
-            type="date",
-            mention_type_object=date_mention,
-            annotations=annotations,
-        )
+        return cls(type="date", mention_type_object=date_mention, annotations=annotations)
 
 
 class Annotations(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
         bold: Optional[bool] = None,
         italic: Optional[bool] = None,
         strikethrough: Optional[bool] = None,
         underline: Optional[bool] = None,
         code: Optional[bool] = None,
-        color: Union[Optional[BlockColor], str] = None,
+        color: Optional[BlockColor | str] = None,
     ) -> None:
         """https://developers.notion.com/reference/rich-text#the-annotation-object"""
         super().__init__()
 
         self.set("bold", bold) if bold else None
         self.set("italic", italic) if italic else None
         self.set("strikethrough", strikethrough) if strikethrough else None
```

### Comparing `notion_api-0.5.2/notion/propertyitems/__init__.py` & `notion_api-0.6.0/notion/propertyitems/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.2/notion/propertyitems/base.py` & `notion_api-0.6.0/notion/propertyitems/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,15 @@
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, MutableMapping, Optional, Sequence, cast
 
 import pytz
 
-__all__: Sequence[str] = (
-    "PropertyItem",
-    "UserPropertyItem",
-)
+__all__: Sequence[str] = ("PropertyItem", "UserPropertyItem")
 
 
 class PropertyItem:
     def __init__(self, map: MutableMapping[str, Any], source_page: str) -> None:
         self.map = map
         self.source_page = source_page
         self._type = map["type"]
@@ -87,15 +84,15 @@
 
 
 def _function_type(property: PropertyItem) -> str:
     return cast(str, property.map["property_item"]["rollup"]["function"])
 
 
 def _retrieve_datetime(property: PropertyItem) -> datetime | tuple[datetime, datetime]:
-    if property._type == "rollup":
+    if property._type == "rollup" or property._type == "formula":
         date = property.item["date"]
         start = date["start"]
         end = date["end"]
         time_zone = date["time_zone"]
     else:
         start = property.item["start"]
         end = property.item["end"]
```

### Comparing `notion_api-0.5.2/notion/propertyitems/call.py` & `notion_api-0.6.0/notion/propertyitems/call.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.2/notion/query/__init__.py` & `notion_api-0.6.0/notion/query/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,18 @@
 
     Create a separate CompoundFilter object to nest an and/or operator inside another and/or.
 
 notion.query.SortFilter takes a list of either *notion.query.PropertyValueSort | notion.query.EntryTimestampSort
 """
 from typing import Sequence
 
-from notion.query.compound import *
-from notion.query.conditions import *
-from notion.query.propfilter import *
-from notion.query.sort import *
-from notion.query.timestamp import *
+from notion.query.compound import CompoundFilter
+from notion.query.propfilter import PropertyFilter
+from notion.query.sort import EntryTimestampSort, PropertyValueSort, SortFilter
+from notion.query.timestamp import TimestampFilter
 
 __all__: Sequence[str] = (
     "SortFilter",
     "PropertyFilter",
     "CompoundFilter",
     "TimestampFilter",
     "EntryTimestampSort",
```

### Comparing `notion_api-0.5.2/notion/query/compound.py` & `notion_api-0.6.0/notion/query/compound.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,53 +15,49 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-
 from __future__ import annotations
 
-from typing import Sequence, Union
+from typing import Sequence
+
+from typing_extensions import Self
 
 from notion.properties.build import NotionObject
 from notion.query.propfilter import PropertyFilter
 from notion.query.timestamp import TimestampFilter
 
 __all__: Sequence[str] = ["CompoundFilter"]
 
 
 class CompoundFilter(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(self) -> None:
-        """NOTE: only up to two nesting levels deep.
+        """Create a separate CompoundFilter object to nest an `and` operator inside another `and` or `or`.
+        NOTE: only up to two nesting levels deep.
 
         :method: _and() combine all filters in an `and` grouping.
         :method: _or() combine all filters in an `or` grouping.
 
-        Create a separate CompoundFilter object to nest an `and` operator inside another `and` or `or`.
-
         https://developers.notion.com/reference/post-database-query-filter#compound-filter-object
         """
         super().__init__()
 
-    def _and(
-        self, *filters: Union[PropertyFilter, CompoundFilter, TimestampFilter]
-    ) -> CompoundFilter:
-        """
-        Example compound filter conditions
+    def _and(self, *filters: PropertyFilter | CompoundFilter | TimestampFilter) -> Self:
+        """Example compound filter conditions
         https://developers.notion.com/reference/post-database-query-filter#example-compound-filter-conditions
         """
-        self.nest("filter", "and", [f["filter"] if "filter" in f else f for f in filters])
+        filter_objects = [f["filter"] if "filter" in f else f for f in filters]
+        self.nest("filter", "and", filter_objects)
         return self
 
-    def _or(
-        self, *filters: Union[PropertyFilter, CompoundFilter, TimestampFilter]
-    ) -> CompoundFilter:
-        """
-        Example compound filter conditions
+    def _or(self, *filters: PropertyFilter | CompoundFilter | TimestampFilter) -> Self:
+        """Example compound filter conditions
         https://developers.notion.com/reference/post-database-query-filter#example-compound-filter-conditions
         """
-        self.nest("filter", "or", [f["filter"] if "filter" in f else f for f in filters])
+        filter_objects = [f["filter"] if "filter" in f else f for f in filters]
+        self.nest("filter", "or", filter_objects)
         return self
```

### Comparing `notion_api-0.5.2/notion/query/conditions.py` & `notion_api-0.6.0/notion/query/conditions.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """ Type-specific filter conditions
 https://developers.notion.com/reference/post-database-query-filter#type-specific-filter-conditionss
 """
 from __future__ import annotations
 
-from typing import Literal, Sequence, TypeAlias, Union
+from typing import Literal, Sequence, TypeAlias
 
 __all__: Sequence[str] = (
     "FilesConditions",
     "CheckboxConditions",
     "RollupConditions",
     "SelectConditions",
     "MultiSelectConditions",
@@ -42,111 +42,141 @@
     "NumberConditions",
     "DateConditions",
     "FormulaConditions",
     "FilterConditions",
 )
 
 
-FilesConditions: TypeAlias = Literal["is_empty", "is_not_empty"]
+FilesConditions: TypeAlias = Literal[
+    "is_empty", 
+    "is_not_empty"
+]
 
-CheckboxConditions: TypeAlias = Literal["equals", "does_not_equal"]
+CheckboxConditions: TypeAlias = Literal[
+    "equals", 
+    "does_not_equal"
+]
 
-RollupConditions: TypeAlias = Literal["any", "every", "none", "number", "date"]
+DateTypes: TypeAlias = Literal[
+    "date", 
+    "created_time", 
+    "last_edited_time"
+]
+
+PeopleTypes: TypeAlias = Literal[
+    "people", 
+    "created_by", 
+    "last_edited_by"
+]
 
 SelectConditions: TypeAlias = Literal[
-    "equals", "does_not_equal", "is_empty", "is_not_empty"
+    "equals", 
+    "does_not_equal", 
+    "is_empty", 
+    "is_not_empty" 
 ]
 
 MultiSelectConditions: TypeAlias = Literal[
-    "contains", "does_not_contain", "is_empty", "is_not_empty"
+    "contains", 
+    "does_not_contain", 
+    "is_empty", 
+    "is_not_empty" 
 ]
 
 StatusConditions: TypeAlias = Literal[
-    "equals", "does_not_equal", "is_empty", "is_not_empty"
+    "equals", 
+    "does_not_equal", 
+    "is_empty", 
+    "is_not_empty" 
 ]
 
 PeopleConditions: TypeAlias = Literal[
-    "contains", "does_not_contain", "is_empty", "is_not_empty"
+    "contains", 
+    "does_not_contain", 
+    "is_empty", 
+    "is_not_empty" 
 ]
 
 RelationConditions: TypeAlias = Literal[
-    "contains", "does_not_contain", "is_empty", "is_not_empty"
+    "contains", 
+    "does_not_contain", 
+    "is_empty", 
+    "is_not_empty" 
 ]
 
-DateTypes: TypeAlias = Literal[
-    "date",
-    "created_time",
-    "last_edited_time",
-]
-
-PeopleTypes: TypeAlias = Literal[
-    "people",
-    "created_by",
-    "last_edited_by",
+TextTypes: TypeAlias = Literal[
+    "title", 
+    "rich_text", 
+    "url", 
+    "email"
 ]
 
-TextTypes: TypeAlias = Literal[
-    "title",
-    "rich_text",
-    "url",
-    "email",
+RollupConditions: TypeAlias = Literal[
+    "any", 
+    "every", 
+    "none", 
+    "number", 
+    "date"
 ]
 
 TextConditions: TypeAlias = Literal[
-    "equals",
-    "does_not_equal",
-    "contains",
-    "does_not_contain",
-    "starts_with",
-    "ends_with",
-    "is_empty",
-    "is_not_empty",
+    "equals", 
+    "does_not_equal", 
+    "contains", 
+    "does_not_contain", 
+    "starts_with", 
+    "ends_with", 
+    "is_empty", 
+    "is_not_empty"
 ]
 
 NumberConditions: TypeAlias = Literal[
-    "equals",
-    "does_not_equal",
-    "greater_than",
-    "less_than",
-    "greater_than_or_equal_to",
-    "less_than_or_equal_to",
-    "is_empty",
-    "is_not_empty",
+    "equals", 
+    "does_not_equal", 
+    "greater_than", 
+    "less_than", 
+    "greater_than_or_equal_to", 
+    "less_than_or_equal_to", 
+    "is_empty", 
+    "is_not_empty"
 ]
 
 DateConditions: TypeAlias = Literal[
-    "equals",
-    "before",
-    "after",
-    "on_or_before",
-    "is_empty",
-    "is_not_empty",
-    "on_or_after",
-    "past_week",
-    "past_month",
-    "past_year",
-    "this_week",
-    "next_week",
-    "next_month",
-    "next_year",
-]
-
-FormulaConditions: TypeAlias = Union[
-    TextConditions, NumberConditions, CheckboxConditions, DateConditions
-]
-
-FilterConditions: TypeAlias = Union[
-    TextConditions,
-    TextTypes,
-    NumberConditions,
-    CheckboxConditions,
-    SelectConditions,
-    MultiSelectConditions,
-    StatusConditions,
-    DateConditions,
-    DateTypes,
-    PeopleConditions,
-    PeopleTypes,
-    FilesConditions,
-    RelationConditions,
-    RollupConditions,
-]
+    "equals", 
+    "before", 
+    "after", 
+    "on_or_before", 
+    "is_empty", 
+    "is_not_empty", 
+    "on_or_after", 
+    "past_week", 
+    "past_month", 
+    "past_year", 
+    "this_week", 
+    "next_week", 
+    "next_month", 
+    "next_year"
+]
+
+FormulaConditions: TypeAlias = (
+    TextConditions
+    | NumberConditions
+    | CheckboxConditions
+    | DateConditions
+)
+
+FilterConditions: TypeAlias = (
+    TextConditions
+    | TextTypes
+    | NumberConditions
+    | CheckboxConditions
+    | SelectConditions
+    | MultiSelectConditions
+    | StatusConditions
+    | DateConditions
+    | DateTypes
+    | PeopleConditions
+    | PeopleTypes
+    | FilesConditions
+    | RelationConditions
+    | RollupConditions
+)
```

### Comparing `notion_api-0.5.2/notion/query/propfilter.py` & `notion_api-0.6.0/notion/query/propfilter.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 from __future__ import annotations
 
 from datetime import datetime
-from typing import Any, Sequence, Union
+from typing import Any, Sequence
 
 from notion.properties.build import NotionObject
 from notion.query.conditions import *
 
 __all__: Sequence[str] = ["PropertyFilter"]
 
 
@@ -73,15 +73,15 @@
 
     @classmethod
     def text(
         cls,
         property_name: str,
         property_type: TextTypes,
         filter_condition: TextConditions,
-        filter_value: Union[str, bool],
+        filter_value: str | bool,
         /,
     ) -> PropertyFilter:
         """https://developers.notion.com/reference/post-database-query-filter#rich-text"""
 
         return cls(property_name, filter_condition, filter_value, property_type)
 
     @classmethod
@@ -99,88 +99,89 @@
         return cls(property_name, filter_condition, filter_value, property_type)
 
     @classmethod
     def number(
         cls,
         property_name: str,
         filter_condition: NumberConditions,
-        filter_value: Union[str, float, bool],
+        filter_value: str | int | float | bool,
         /,
+        *,
         property_type: str = "number",
     ) -> PropertyFilter:
         """https://developers.notion.com/reference/post-database-query-filter#number"""
 
         return cls(property_name, filter_condition, filter_value, property_type)
 
     @classmethod
     def select(
         cls,
         property_name: str,
         filter_condition: SelectConditions,
-        filter_value: Union[str, bool],
+        filter_value: str | bool,
         /,
         property_type: str = "select",
     ) -> PropertyFilter:
         """https://developers.notion.com/reference/post-database-query-filter#select"""
 
         return cls(property_name, filter_condition, filter_value, property_type)
 
     @classmethod
     def multi_select(
         cls,
         property_name: str,
         filter_condition: MultiSelectConditions,
-        filter_value: Union[str, bool],
+        filter_value: str | bool,
         /,
         property_type: str = "multi_select",
     ) -> PropertyFilter:
         """https://developers.notion.com/reference/post-database-query-filter#multi-select"""
 
         return cls(property_name, filter_condition, filter_value, property_type)
 
     @classmethod
     def status(
         cls,
         property_name: str,
         filter_condition: StatusConditions,
-        filter_value: Union[str, bool],
+        filter_value: str | bool,
         /,
         property_type: str = "status",
     ) -> PropertyFilter:
         """https://developers.notion.com/reference/post-database-query-filter#status"""
 
         return cls(property_name, filter_condition, filter_value, property_type)
 
     @classmethod
     def date(
         cls,
         property_name: str,
         property_type: DateTypes,
         filter_condition: DateConditions,
-        filter_value: Union[str, bool, dict[str, Any], datetime],
+        filter_value: str | bool | dict[str, Any] | datetime,
         /,
     ) -> PropertyFilter:
         """
-        :param filter_value: - When selecting any DateCondition containing `past`, `this`, or `next`, set filter value to `{}`\
-                             - If value is datetime, it will be converted to ISO 8601 format.
+        :param filter_value: When selecting any DateCondition containing `past`, `this`, or `next`, set filter value to `{}`\
+                             If value is datetime, it will be converted to ISO 8601 format.
 
         https://developers.notion.com/reference/post-database-query-filter#date
         """
         if isinstance(filter_value, datetime):
             filter_value = filter_value.isoformat()
 
         return cls(property_name, filter_condition, filter_value, property_type)
 
     @classmethod
     def people(
         cls,
         property_name: str,
         property_type: PeopleTypes,
         filter_condition: PeopleConditions,
-        filter_value: Union[str, bool],
+        filter_value: str | bool,
         /,
     ) -> PropertyFilter:
         """https://developers.notion.com/reference/post-database-query-filter#people"""
 
         return cls(property_name, filter_condition, filter_value, property_type)
 
     @classmethod
@@ -188,27 +189,25 @@
         cls,
         property_name: str,
         filter_condition: FilesConditions,
         /,
         filter_value: bool = True,
         property_type: str = "files",
     ) -> PropertyFilter:
-        """
-        Only available `filter_value` is `true`.
-
+        """Only available `filter_value` is `true`.
         https://developers.notion.com/reference/post-database-query-filter#files-filter-condition
         """
 
         return cls(property_name, filter_condition, filter_value, property_type)
 
     @classmethod
     def relation(
         cls,
         property_name: str,
         filter_condition: RelationConditions,
-        filter_value: Union[str, bool],
+        filter_value: str | bool,
         /,
         property_type: str = "relation",
     ) -> PropertyFilter:
         """https://developers.notion.com/reference/post-database-query-filter#relation"""
 
         return cls(property_name, filter_condition, filter_value, property_type)
```

### Comparing `notion_api-0.5.2/notion/query/sort.py` & `notion_api-0.6.0/notion/query/sort.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 from __future__ import annotations
 
-from typing import Sequence, Union
+from typing import Sequence
 
 from notion.properties.build import NotionObject
 
 __all__: Sequence[str] = ("SortFilter", "PropertyValueSort", "EntryTimestampSort")
 
 
 class SortFilter(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(
-        self, sort_object: Sequence[Union[PropertyValueSort, EntryTimestampSort]]
+        self, sort_object: Sequence[PropertyValueSort | EntryTimestampSort]
     ) -> None:
         """
         A database query can be sorted by a property and/or timestamp and in a given direction.
         Database queries can also be sorted by two or more properties.
 
         :param sort_object: (required) A list containing PropertyValueSort/EntryTimestampSort\
                              The sort object listed first in the nested sort list takes precedence.
@@ -47,16 +47,15 @@
         self.set("sorts", sort_object)
 
 
 class PropertyValueSort(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(self, property_name: str, /, *, direction: str) -> None:
-        """
-        This sort orders the database query by a particular property.
+        """This sort orders the database query by a particular property.
 
         Use one of the following classmethods:
         - `ascending`
         - `descending`
 
         https://developers.notion.com/reference/post-database-query-sort#property-value-sort
         """
@@ -73,16 +72,15 @@
         return cls(property_name, direction="descending")
 
 
 class EntryTimestampSort(NotionObject):
     __slots__: Sequence[str] = ("timestamp", "direction")
 
     def __init__(self, *, timestamp: str, direction: str) -> None:
-        """
-        This sort orders the database query by the timestamp associated with a database entry.
+        """This sort orders the database query by the timestamp associated with a database entry.
 
         Use one of the following classmethods:
         - `created_time_ascending`
         - `created_time_descending`
         - `last_edited_time_ascending`
         - `last_edited_time_descending`
```

### Comparing `notion_api-0.5.2/notion/query/timestamp.py` & `notion_api-0.6.0/notion/query/timestamp.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,29 +18,29 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from __future__ import annotations
 
-from typing import Any, MutableMapping, Optional, Sequence, Union
+from typing import Any, MutableMapping, Optional, Sequence
 
 from notion.properties.build import NotionObject
 from notion.query.conditions import DateConditions
 
 __all__: Sequence[str] = ["TimestampFilter"]
 
 
 class TimestampFilter(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(
         self,
         filter_condition: DateConditions,
-        filter_value: Union[str, MutableMapping[str, Any]],
+        filter_value: str | MutableMapping[str, Any],
         type: Optional[str] = None,
     ) -> None:
         """
         Use classmethods:
          - created_time
          - last_edited_time
 
@@ -50,15 +50,15 @@
         self.nest("filter", "timestamp", type)
         self.nest("filter", type, {filter_condition: filter_value})
 
     @classmethod
     def created_time(
         cls,
         filter_condition: DateConditions,
-        filter_value: Union[str, MutableMapping[str, Any]],
+        filter_value: str | MutableMapping[str, Any],
     ) -> TimestampFilter:
         """
         :param filter_condition: One of the available DateConditions. Must be a string (ISO 8601 date).\
                                  For the following date conditions, the filter_value must be '{}':\
                                  [past_week, past_month, past_year, this_week, next_week, next_month, next_year]
 
         :param filter_value: Value to filter for.\
@@ -69,15 +69,15 @@
         """
         return cls(filter_condition, filter_value, type="created_time")
 
     @classmethod
     def last_edited_time(
         cls,
         filter_condition: DateConditions,
-        filter_value: Union[str, MutableMapping[str, Any]],
+        filter_value: str | MutableMapping[str, Any],
     ) -> TimestampFilter:
         """
         :param filter_condition: One of the available DateConditions. Must be a string (ISO 8601 date).\
                                  For the following date conditions, the filter_value must be '{}':\
                                  [past_week, past_month, past_year, this_week, next_week, next_month, next_year]
 
         :param filter_value: Value to filter for.\
```

### Comparing `notion_api-0.5.2/.gitignore` & `notion_api-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.2/LICENSE` & `notion_api-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.2/pyproject.toml` & `notion_api-0.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
 ]
 dependencies = [
-    "python-dotenv==1.0.0",
     "requests==2.28.2",
     "pytz==2022.7.1",
     "tzlocal==4.2",
 ]
 
 [project.urls]
 Homepage = "https://github.com/ayvi-0001/notion-api"
@@ -61,40 +60,39 @@
   ".gitattributes",
   "/images",
   "/tests",
 ]
 
 [project.optional-dependencies]
 orjson = [
-    "orjson==3.8.9"
+    "orjson==3.8.12"
 ]
 dev = [
-    "black==23.3.0",
-    "isort==5.12.0",
-    "mypy==1.1.1",
-    "mypy-extensions==1.0.0",
-    "typing_extensions==4.5.0",
-    "types-pytz==2022.7.1.2",
-    "types-requests==2.28.11.15",
-    "types-tzlocal==4.2.2.3",
-    "types-urllib3==1.26.25.8"
+    "black>=23.3.0",
+    "isort>=5.12.0",
+    "mypy>=1.3.0",
+    "mypy-extensions>=1.0.0",
+    "typing_extensions>=4.5.0",
+    "types-pytz>=2023.3.0.0",
+    "types-requests>=2.28.11.17",
+    "types-tzlocal>=4.3.0.0",
+    "types-urllib3>=1.26.25.10"
 ]
 
 [tool.black]
 line-length = 90
-target-version = ['py37']
 reportWildcardImportFromLibrary = false
-force-exclude = '''.*validate.py'''
+force-exclude = '''.*conditions.py|.*errors.py'''
 
 [tool.isort]
 profile = "black"
+line_length = 90
 skip_gitignore = true
 
 [tool.mypy]
-python_version = "3.10"
 strict = true
 pretty = true
 show_error_codes = true
 incremental = true
 disallow_untyped_defs = true
 show_column_numbers = true
 show_error_context = true
```

### Comparing `notion_api-0.5.2/PKG-INFO` & `notion_api-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: notion-api
-Version: 0.5.2
+Version: 0.6.0
 Summary: An unofficial wrapper for Notion's API, aiming to simplify the dynamic nature of interacting with Notion.
 Project-URL: Homepage, https://github.com/ayvi-0001/notion-api
 Project-URL: Source Code, https://github.com/ayvi-0001/notion-api
 Author-email: Alan Vickers <alan.k.vickers@gmail.com>
 License-File: LICENSE
 Keywords: notion-api,notion-version-2022-06-28,wrapper
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
-Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: pytz==2022.7.1
 Requires-Dist: requests==2.28.2
 Requires-Dist: tzlocal==4.2
 Provides-Extra: dev
-Requires-Dist: black==23.3.0; extra == 'dev'
-Requires-Dist: isort==5.12.0; extra == 'dev'
-Requires-Dist: mypy-extensions==1.0.0; extra == 'dev'
-Requires-Dist: mypy==1.1.1; extra == 'dev'
-Requires-Dist: types-pytz==2022.7.1.2; extra == 'dev'
-Requires-Dist: types-requests==2.28.11.15; extra == 'dev'
-Requires-Dist: types-tzlocal==4.2.2.3; extra == 'dev'
-Requires-Dist: types-urllib3==1.26.25.8; extra == 'dev'
-Requires-Dist: typing-extensions==4.5.0; extra == 'dev'
+Requires-Dist: black>=23.3.0; extra == 'dev'
+Requires-Dist: isort>=5.12.0; extra == 'dev'
+Requires-Dist: mypy-extensions>=1.0.0; extra == 'dev'
+Requires-Dist: mypy>=1.3.0; extra == 'dev'
+Requires-Dist: types-pytz>=2023.3.0.0; extra == 'dev'
+Requires-Dist: types-requests>=2.28.11.17; extra == 'dev'
+Requires-Dist: types-tzlocal>=4.3.0.0; extra == 'dev'
+Requires-Dist: types-urllib3>=1.26.25.10; extra == 'dev'
+Requires-Dist: typing-extensions>=4.5.0; extra == 'dev'
 Provides-Extra: orjson
-Requires-Dist: orjson==3.8.9; extra == 'orjson'
+Requires-Dist: orjson==3.8.12; extra == 'orjson'
 Description-Content-Type: text/markdown
 
 # notion-api
 
 <p align="center">
     <a href="https://pypi.org/project/notion-api"><img alt="PYPI" src="https://img.shields.io/pypi/v/notion-api"></a>
     &nbsp;
@@ -55,56 +54,63 @@
 
 </p>
 
 __Disclaimer: This is an _unofficial_ package and has no affiliation with Notion.so__  
 
 A wrapper for Notion's API, aiming to simplify the dynamic nature of interacting with Notion.  
 README contains examples of the main functionality, including: creating Pages/Databases/Blocks, adding/removing/editing properties, retrieving property values, and database queries.  
-Some more in-depth walkthroughs can be be found in [`examples/`](https://github.com/ayvi-0001/notion-api/tree/main/examples)    
+Some more in-depth walkthroughs can be be found in [`examples/`](https://github.com/ayvi-0001/notion-api/tree/main/examples).    
 This package is not complete - new features will continue to be added, and current features may change.
 
 <br>
 
 <div border="0" align="center">
     <table>
         <tr>
             <td align="center"><b>Links: Notion API Updates</b></td>
         </tr>
             <td> <a href="https://developers.notion.com/reference/intro">API Reference</a></td><tr>
         </td>
             <td><a href="https://developers.notion.com/page/changelog">Notion API Changelog </img></a></tr>
             <td> <a href="https://www.notion.so/releases">Notion.so Releases</a></td></tr>
-            <td> <a href="https://developers.notion.com/page/notion-platform-roadmap">Notion Platform Roadmap</a></td>
         </tr>
     </table>
 </div>
 
+<br>
+
+If you haven't already, you'll need to setup a [Notion Integration](https://www.notion.so/my-integrations) and share specific pages/databases with the integration to interact with the API.  
+Information on integration types and setup can be found [here](https://developers.notion.com/docs/getting-started).
+
 ---
 
 ## Install
 ```
 pip install -U notion-api
 ```
 
 ## Usage
 ```py
 import dotenv
 
 import notion
 
-# client will check env variables for 'NOTION_TOKEN'
+# client will check for env var 'NOTION_TOKEN'
 dotenv.load_dotenv()  
 
 homepage = notion.Page('773b08ff38b44521b44b115827e850f2')
 parent_db = notion.Database(homepage.parent_id)
 
-# will also look for env var `TZ` to set the timezone for all notion objects. If not found, will default to local timezone.
+# will also look for env var `TZ` to set the default timezone. If not found, will default to local timezone.
 ```
 
-`__getitem__` searchs for page property values when indexing a Page, and for property objects when indexing a Database.
+Indexing a page will search for page property values, and indexing a Database will search for property objects.  
+A full list can be retrieved for both using;  
+- `retrieve()` method for a Page, with the optional `filter_properties` parameter.
+- `retrieve` attribute for a Database.
 
 ```py
 homepage['dependencies']
 # {
 #     "id": "WYYq",
 #     "type": "relation",
 #     "relation": [
@@ -154,31 +160,34 @@
 
 <p align="center"> <img src="https://github.com/ayvi-0001/notion-api/blob/main/examples/images/new_page.png?raw=true"> </p>
 
 <br>
 
 ## Creating Pages/Databases/Blocks
 
-The current version of the Notion api does not allow pages to be created to the parent `workspace`.  
-Create objects by passing an existing Page/Database instance as an arg to the `create` classmethods.
+Create objects by passing an existing Page/Database instance to the `create` classmethods.  
+The current version of the Notion api does not allow pages/databases to be created to the parent `workspace`.  
 
 ```py
 new_database = notion.Database.create(
     parent_instance=testpage,
     database_title="Example Database",
     name_column="page", # This is the column containing page names. Defaults to "Name".
     is_inline=True, # can also toggle inline with setters.
     description="Database description can go here.",
 )
 
 new_page = notion.Page.create(new_database, page_title="A new database row")
 ```
 
-Blocks are also created using the classmethods of `Block`. They all require a parent instance of either `Page` or `Block` to append the new block too.
-The newly created block is returned as an instance of `Block`, which can be used as the parent instance to a nested block. 
+Blocks are also created using classmethods. They require a parent instance of either `Page` or `Block` to append the new block too.
+The newly created block is returned as an instance of `Block`, which can be used as the parent instance to another nested block. 
+
+By default, blocks are appended to the bottom of the parent block.  
+To append the block somewhere else other than the bottom of the parent block, use the `after` parameter and set its value to the ID of the block that the new block should be appended after. The block_id used in the `after` paramater must still be a child to the parent instance.  
 ```py
 from notion import properties as prop
 
 # `original_synced_block` refers to the original synced block in the Notion UI.
 original_synced_block = notion.Block.original_synced_block(homepage)
 
 # Adding content to the synced block
@@ -244,15 +253,15 @@
                     bold=True,
                     italic=True,
                     underline=True,
                     color=prop.BlockColor.gray,
                 ),
             ),
             prop.RichText(":"),
-        ],
+        ]
     )
     # First method returned the newly created block that we append to here:
     notion.Block.paragraph(mentionblock, [prop.RichText(message)])
     notion.Block.divider(page)
 ```
 
 ```py
@@ -269,58 +278,61 @@
 
 The first argument for all database property methods is the name of the property,  
 If a property of that name does not exist, then a new property will be created. 
 If a property of that name already exists, but it's a different type than the method used - then the API will overwrite this and change the property object to the new type.  
 The original parameters will be saved if you decide to switch back (i.e. if you change a formula column to a select column, upon changing it back to a formula column, the original formula expression will still be there).   
 
 ```py
-new_database.formula_column("page id", expression="id()")
+new_database.formula_column("page_id", expression="id()")
 
 new_database.delete_property("url")
 
 new_database.multiselect_column(
-    "new options column",
+    "New Options Column",
     options=[
-        prop.Option("option-a", prop.PropertyColor.red),
-        prop.Option("option-b", prop.PropertyColor.green),
-        prop.Option("option-c", prop.PropertyColor.blue),
+        prop.Option("Option A", prop.PropertyColor.red),
+        prop.Option("Option B", prop.PropertyColor.green),
+        prop.Option("Option C", prop.PropertyColor.blue),
     ],
 )
 
 # if an option does not already exist, a new one will be created with a random color.
 # this is not true for `status` column types, which can only be edited via UI.
 
 new_page.set_multiselect("options", ["option-a", "option-b"])
 ```
 
 <br>
 
 ## Database Queries
 
 A single `notion.query.PropertyFilter` is equivalent to filtering one property type in Notion.
-To build filters equivalent to Notion's 'advanced filters', use `notion.query.CompoundFilter`.
+To build nested filters, use `notion.query.CompoundFilter` and group property filters chained together by `_and(...)` / `_or(...)`.
 
 The database method `query()` will return the raw response from the API.  
 The method `query_pages()` will extract the page ID for each object in the array of results, and return a list of `notion.Page` objects.
 
+> note: in v0.6.0, new query methods were added: `query_all()` & `query_all_pages()` - these handle pagination, and instead of providing the `next_cursor` and `has_more` keys,
+> they will iterate through all the results, or up to the `max_page_size` paramater. These 2 methods will replace the original ones in a later update.
+
 ```py
 from datetime import datetime
 from datetime import timedelta
 
 from notion import query
 
 TODAY = datetime.combine(datetime.today(), datetime.min.time())
 TOMORROW = TODAY + timedelta(1)
 
 query_filter = query.CompoundFilter()._and(
     query.PropertyFilter.date("date", "created_time", "on_or_after", TODAY.isoformat()),
     query.PropertyFilter.date("date", "created_time", "before", TOMORROW.isoformat()),
     query.CompoundFilter()._or(
         query.PropertyFilter.text("name", "title", "contains", "your page title"),
-        query.PropertyFilter.text("name", "title", "contains", "your other page title"),
+        query.PropertyFilter.text("name", "title", "contains", "your other page title")
     ),
 )
 
 query_sort = query.SortFilter(
     [
         query.PropertyValueSort.ascending("your property name"),
         query.EntryTimestampSort.created_time_descending(),
@@ -360,27 +372,29 @@
 File "c:\...\notion\exceptions\validate.py", line 48, in validate_response
     raise NotionValidationError(message)
 notion.exceptions.errors.NotionValidationError: body failed validation: body.an_incorrect_key should be not present, instead was `"value"`.
 Error 400: The request body does not match the schema for the expected parameters.
 ```
 
 Possible errors are:
+ - `NotionConflictError`
+ - `NotionDatabaseConnectionUnavailable`
+ - `NotionGatewayTimeout`
+ - `NotionInvalidGrant`
+ - `NotionInternalServerError`
  - `NotionInvalidJson`
- - `NotionInvalidRequestUrl`
  - `NotionInvalidRequest`
- - `NotionValidationError`
+ - `NotionInvalidRequestUrl`
  - `NotionMissingVersion`
- - `NotionUnauthorized`
- - `NotionRestrictedResource`
  - `NotionObjectNotFound`
- - `NotionConflictError`
  - `NotionRateLimited`
- - `NotionInternalServerError`
+ - `NotionRestrictedResource`
  - `NotionServiceUnavailable`
- - `NotionDatabaseConnectionUnavailable`
+ - `NotionUnauthorized`
+ - `NotionValidationError`
 
 A common error to look out for is `NotionObjectNotFound`. This error is often raised because your bot has not been added as a connection to the page. 
 
 <p align="center">
     <img src="https://github.com/ayvi-0001/notion-api/blob/main/examples/images/directory_add_connections.png?raw=true">  
 </p>
```

#### html2text {}

```diff
@@ -1,87 +1,97 @@
-Metadata-Version: 2.1 Name: notion-api Version: 0.5.2 Summary: An unofficial
+Metadata-Version: 2.1 Name: notion-api Version: 0.6.0 Summary: An unofficial
 wrapper for Notion's API, aiming to simplify the dynamic nature of interacting
 with Notion. Project-URL: Homepage, https://github.com/ayvi-0001/notion-api
 Project-URL: Source Code, https://github.com/ayvi-0001/notion-api Author-email:
 Alan Vickers
 k.vickers@gmail.com> License-File: LICENSE Keywords: notion-api,notion-version-
 2022-06-28,wrapper Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.10 Requires-Dist: python-dotenv==1.0.0 Requires-Dist:
-pytz==2022.7.1 Requires-Dist: requests==2.28.2 Requires-Dist: tzlocal==4.2
-Provides-Extra: dev Requires-Dist: black==23.3.0; extra == 'dev' Requires-Dist:
-isort==5.12.0; extra == 'dev' Requires-Dist: mypy-extensions==1.0.0; extra ==
-'dev' Requires-Dist: mypy==1.1.1; extra == 'dev' Requires-Dist: types-
-pytz==2022.7.1.2; extra == 'dev' Requires-Dist: types-requests==2.28.11.15;
-extra == 'dev' Requires-Dist: types-tzlocal==4.2.2.3; extra == 'dev' Requires-
-Dist: types-urllib3==1.26.25.8; extra == 'dev' Requires-Dist: typing-
-extensions==4.5.0; extra == 'dev' Provides-Extra: orjson Requires-Dist:
-orjson==3.8.9; extra == 'orjson' Description-Content-Type: text/markdown #
-notion-api
+Requires-Python: >=3.10 Requires-Dist: pytz==2022.7.1 Requires-Dist:
+requests==2.28.2 Requires-Dist: tzlocal==4.2 Provides-Extra: dev Requires-Dist:
+black>=23.3.0; extra == 'dev' Requires-Dist: isort>=5.12.0; extra == 'dev'
+Requires-Dist: mypy-extensions>=1.0.0; extra == 'dev' Requires-Dist:
+mypy>=1.3.0; extra == 'dev' Requires-Dist: types-pytz>=2023.3.0.0; extra ==
+'dev' Requires-Dist: types-requests>=2.28.11.17; extra == 'dev' Requires-Dist:
+types-tzlocal>=4.3.0.0; extra == 'dev' Requires-Dist: types-
+urllib3>=1.26.25.10; extra == 'dev' Requires-Dist: typing-extensions>=4.5.0;
+extra == 'dev' Provides-Extra: orjson Requires-Dist: orjson==3.8.12; extra ==
+'orjson' Description-Content-Type: text/markdown # notion-api
                         [PYPI]   [PYPI]   [pyversions]
    [last commit]
    [notion_versioning]  
           [license:_MIT]   [code_style:_black]   [code_style:_black]
 __Disclaimer: This is an _unofficial_ package and has no affiliation with
 Notion.so__ A wrapper for Notion's API, aiming to simplify the dynamic nature
 of interacting with Notion. README contains examples of the main functionality,
 including: creating Pages/Databases/Blocks, adding/removing/editing properties,
 retrieving property values, and database queries. Some more in-depth
 walkthroughs can be be found in [`examples/`](https://github.com/ayvi-0001/
-notion-api/tree/main/examples) This package is not complete - new features will
-continue to be added, and current features may change.
+notion-api/tree/main/examples). This package is not complete - new features
+will continue to be added, and current features may change.
                            Links: Notion API Updates
                            Notion_API_Changelog
+
+If you haven't already, you'll need to setup a [Notion Integration](https://
+www.notion.so/my-integrations) and share specific pages/databases with the
+integration to interact with the API. Information on integration types and
+setup can be found [here](https://developers.notion.com/docs/getting-started).
 --- ## Install ``` pip install -U notion-api ``` ## Usage ```py import dotenv
-import notion # client will check env variables for 'NOTION_TOKEN'
-dotenv.load_dotenv() homepage = notion.Page('773b08ff38b44521b44b115827e850f2')
-parent_db = notion.Database(homepage.parent_id) # will also look for env var
-`TZ` to set the timezone for all notion objects. If not found, will default to
-local timezone. ``` `__getitem__` searchs for page property values when
-indexing a Page, and for property objects when indexing a Database. ```py
-homepage['dependencies'] # { # "id": "WYYq", # "type": "relation", #
-"relation": [ # { # "id": "7bcbc8e6-e237-434b-bd0d-6b56e044200b" # } # ], #
-"has_more": false # } parent_db['dependencies'] # { # "id": "WYYq", # "name":
-"dependencies", # "type": "relation", # "relation": { # "database_id":
-"f5984a7e-2257-4ab0-9d0a-23ea12324031", # "type": "dual_property", #
-"dual_property": { # "synced_property_name": "blocked", # "synced_property_id":
-"wx%7DQ" # } # } # } ``` **_See usage of retrieving values from a page in
-[examples/retrieving-property-items.md](https://github.com/ayvi-0001/notion-
-api/blob/main/examples/retrieving-property-items.md)_** Below is a brief
-example if we were wanting to get the page id from the above property
-`dependencies` in `homepage`. ```py from notion import propertyitems
-related_id: list[str] = propertyitems.relation(homepage.dependencies) ``` ```py
->>> ["7bcbc8e6-e237-434b-bd0d-6b56e044200b"] ``` Both Page's and Database's
-have setters for title/icon/cover. ```py homepage.title = "new page"
-homepage.cover = "https://www.notion.so/images/page-cover/webb1.jpg"
-homepage.icon = "https://www.notion.so/icons/alien-pixel_purple.svg" ```
+import notion # client will check for env var 'NOTION_TOKEN' dotenv.load_dotenv
+() homepage = notion.Page('773b08ff38b44521b44b115827e850f2') parent_db =
+notion.Database(homepage.parent_id) # will also look for env var `TZ` to set
+the default timezone. If not found, will default to local timezone. ```
+Indexing a page will search for page property values, and indexing a Database
+will search for property objects. A full list can be retrieved for both using;
+- `retrieve()` method for a Page, with the optional `filter_properties`
+parameter. - `retrieve` attribute for a Database. ```py homepage
+['dependencies'] # { # "id": "WYYq", # "type": "relation", # "relation": [ #
+{ # "id": "7bcbc8e6-e237-434b-bd0d-6b56e044200b" # } # ], # "has_more": false #
+} parent_db['dependencies'] # { # "id": "WYYq", # "name": "dependencies", #
+"type": "relation", # "relation": { # "database_id": "f5984a7e-2257-4ab0-9d0a-
+23ea12324031", # "type": "dual_property", # "dual_property": { #
+"synced_property_name": "blocked", # "synced_property_id": "wx%7DQ" # } # } # }
+``` **_See usage of retrieving values from a page in [examples/retrieving-
+property-items.md](https://github.com/ayvi-0001/notion-api/blob/main/examples/
+retrieving-property-items.md)_** Below is a brief example if we were wanting to
+get the page id from the above property `dependencies` in `homepage`. ```py
+from notion import propertyitems related_id: list[str] = propertyitems.relation
+(homepage.dependencies) ``` ```py >>> ["7bcbc8e6-e237-434b-bd0d-6b56e044200b"]
+``` Both Page's and Database's have setters for title/icon/cover. ```py
+homepage.title = "new page" homepage.cover = "https://www.notion.so/images/
+page-cover/webb1.jpg" homepage.icon = "https://www.notion.so/icons/alien-
+pixel_purple.svg" ```
       [https://github.com/ayvi-0001/notion-api/blob/main/examples/images/
                             new_page.png?raw=true]
 
-## Creating Pages/Databases/Blocks The current version of the Notion api does
-not allow pages to be created to the parent `workspace`. Create objects by
-passing an existing Page/Database instance as an arg to the `create`
-classmethods. ```py new_database = notion.Database.create
+## Creating Pages/Databases/Blocks Create objects by passing an existing Page/
+Database instance to the `create` classmethods. The current version of the
+Notion api does not allow pages/databases to be created to the parent
+`workspace`. ```py new_database = notion.Database.create
 ( parent_instance=testpage, database_title="Example Database",
 name_column="page", # This is the column containing page names. Defaults to
 "Name". is_inline=True, # can also toggle inline with setters.
 description="Database description can go here.", ) new_page =
 notion.Page.create(new_database, page_title="A new database row") ``` Blocks
-are also created using the classmethods of `Block`. They all require a parent
-instance of either `Page` or `Block` to append the new block too. The newly
-created block is returned as an instance of `Block`, which can be used as the
-parent instance to a nested block. ```py from notion import properties as prop
-# `original_synced_block` refers to the original synced block in the Notion UI.
-original_synced_block = notion.Block.original_synced_block(homepage) # Adding
-content to the synced block notion.Block.paragraph(original_synced_block,
-[prop.RichText("This is a synced block.")]) # Referencing the synced block in a
-new page. notion.Block.duplicate_synced_block(new_page,
-original_synced_block.id) ```
+are also created using classmethods. They require a parent instance of either
+`Page` or `Block` to append the new block too. The newly created block is
+returned as an instance of `Block`, which can be used as the parent instance to
+another nested block. By default, blocks are appended to the bottom of the
+parent block. To append the block somewhere else other than the bottom of the
+parent block, use the `after` parameter and set its value to the ID of the
+block that the new block should be appended after. The block_id used in the
+`after` paramater must still be a child to the parent instance. ```py from
+notion import properties as prop # `original_synced_block` refers to the
+original synced block in the Notion UI. original_synced_block =
+notion.Block.original_synced_block(homepage) # Adding content to the synced
+block notion.Block.paragraph(original_synced_block, [prop.RichText("This is a
+synced block.")]) # Referencing the synced block in a new page.
+notion.Block.duplicate_synced_block(new_page, original_synced_block.id) ```
 There are few extensions to the `Block` class that have specific functions
 unique to their block-type. Below is an example using `CodeBlock`. The others
 are `TableBlock`, `EquationBlock`, `RichTextBlock`, and `ToDoBlock`. You can
 see usage for them in [`examples/block_extensions.md`](https://github.com/ayvi-
 0001/notion-api/blob/main/examples/block_extensions.md). ```py code_block =
 notion.CodeBlock("84c5721d8a954667902a757f0033f9e0") git_graph = r""" %%{init:
 { 'logLevel': 'debug', 'theme': 'default' , 'themeVariables': { 'darkMode':
@@ -99,15 +109,15 @@
 appending blocks in a page to mention user/date._** ```py def inline_mention
 (page: notion.Page, message: str, user_name: str) -> None: mentionblock =
 notion.Block.paragraph( page, [ prop.Mention.user( notion.Workspace
 ().retrieve_user(user_name=user_name), annotations=prop.Annotations( code=True,
 bold=True, color=prop.BlockColor.purple ), ), prop.RichText(" - "),
 prop.Mention.date( datetime.now().astimezone(page.tz).isoformat(),
 annotations=prop.Annotations( code=True, bold=True, italic=True,
-underline=True, color=prop.BlockColor.gray, ), ), prop.RichText(":"), ], ) #
+underline=True, color=prop.BlockColor.gray, ), ), prop.RichText(":"), ] ) #
 First method returned the newly created block that we append to here:
 notion.Block.paragraph(mentionblock, [prop.RichText(message)])
 notion.Block.divider(page) ``` ```py >>> homepage = notion.Page
 ("0b9eccfa890e4c3390175ee10c664a35") >>> inline_mention(page=homepage,
 message="example", user_name="AYVI") ```
       [https://github.com/ayvi-0001/notion-api/blob/main/examples/images/
                     example_function_reminder.png?raw=true]
@@ -116,36 +126,41 @@
 first argument for all database property methods is the name of the property,
 If a property of that name does not exist, then a new property will be created.
 If a property of that name already exists, but it's a different type than the
 method used - then the API will overwrite this and change the property object
 to the new type. The original parameters will be saved if you decide to switch
 back (i.e. if you change a formula column to a select column, upon changing it
 back to a formula column, the original formula expression will still be there).
-```py new_database.formula_column("page id", expression="id()")
-new_database.delete_property("url") new_database.multiselect_column( "new
-options column", options=[ prop.Option("option-a", prop.PropertyColor.red),
-prop.Option("option-b", prop.PropertyColor.green), prop.Option("option-c",
+```py new_database.formula_column("page_id", expression="id()")
+new_database.delete_property("url") new_database.multiselect_column( "New
+Options Column", options=[ prop.Option("Option A", prop.PropertyColor.red),
+prop.Option("Option B", prop.PropertyColor.green), prop.Option("Option C",
 prop.PropertyColor.blue), ], ) # if an option does not already exist, a new one
 will be created with a random color. # this is not true for `status` column
 types, which can only be edited via UI. new_page.set_multiselect("options",
 ["option-a", "option-b"]) ```
 ## Database Queries A single `notion.query.PropertyFilter` is equivalent to
-filtering one property type in Notion. To build filters equivalent to Notion's
-'advanced filters', use `notion.query.CompoundFilter`. The database method
-`query()` will return the raw response from the API. The method `query_pages()`
-will extract the page ID for each object in the array of results, and return a
-list of `notion.Page` objects. ```py from datetime import datetime from
+filtering one property type in Notion. To build nested filters, use
+`notion.query.CompoundFilter` and group property filters chained together by
+`_and(...)` / `_or(...)`. The database method `query()` will return the raw
+response from the API. The method `query_pages()` will extract the page ID for
+each object in the array of results, and return a list of `notion.Page`
+objects. > note: in v0.6.0, new query methods were added: `query_all()` &
+`query_all_pages()` - these handle pagination, and instead of providing the
+`next_cursor` and `has_more` keys, > they will iterate through all the results,
+or up to the `max_page_size` paramater. These 2 methods will replace the
+original ones in a later update. ```py from datetime import datetime from
 datetime import timedelta from notion import query TODAY = datetime.combine
 (datetime.today(), datetime.min.time()) TOMORROW = TODAY + timedelta(1)
 query_filter = query.CompoundFilter()._and( query.PropertyFilter.date("date",
 "created_time", "on_or_after", TODAY.isoformat()), query.PropertyFilter.date
 ("date", "created_time", "before", TOMORROW.isoformat()), query.CompoundFilter
 ()._or( query.PropertyFilter.text("name", "title", "contains", "your page
 title"), query.PropertyFilter.text("name", "title", "contains", "your other
-page title"), ), ) query_sort = query.SortFilter(
+page title") ), ) query_sort = query.SortFilter(
 [ query.PropertyValueSort.ascending("your property name"),
 query.EntryTimestampSort.created_time_descending(), ] ) query_result =
 new_database.query( filter=query_filter, sort=query_sort, page_size=5,
 filter_property_values=["name", "options"], ) ```
 ## Exceptions & Validating Responses Errors in Notion requests return an object
 with the keys: 'object', 'status', 'code', and 'message'. Exceptions are raised
 by matching the error code and returning the message. For example: ```py
@@ -155,22 +170,22 @@
 body.an_incorrect_key should be not present, instead was `"value"`.' # } ```
 ```sh Traceback (most recent call last): File "c:\path\to\file\_.py", line 6,
 in  homepage._patch_properties(payload={'an_incorrect_key':'value'}) File "c:
 \...\notion\exceptions\validate.py", line 48, in validate_response raise
 NotionValidationError(message) notion.exceptions.errors.NotionValidationError:
 body failed validation: body.an_incorrect_key should be not present, instead
 was `"value"`. Error 400: The request body does not match the schema for the
-expected parameters. ``` Possible errors are: - `NotionInvalidJson` -
-`NotionInvalidRequestUrl` - `NotionInvalidRequest` - `NotionValidationError` -
-`NotionMissingVersion` - `NotionUnauthorized` - `NotionRestrictedResource` -
-`NotionObjectNotFound` - `NotionConflictError` - `NotionRateLimited` -
-`NotionInternalServerError` - `NotionServiceUnavailable` -
-`NotionDatabaseConnectionUnavailable` A common error to look out for is
-`NotionObjectNotFound`. This error is often raised because your bot has not
-been added as a connection to the page.
+expected parameters. ``` Possible errors are: - `NotionConflictError` -
+`NotionDatabaseConnectionUnavailable` - `NotionGatewayTimeout` -
+`NotionInvalidGrant` - `NotionInternalServerError` - `NotionInvalidJson` -
+`NotionInvalidRequest` - `NotionInvalidRequestUrl` - `NotionMissingVersion` -
+`NotionObjectNotFound` - `NotionRateLimited` - `NotionRestrictedResource` -
+`NotionServiceUnavailable` - `NotionUnauthorized` - `NotionValidationError` A
+common error to look out for is `NotionObjectNotFound`. This error is often
+raised because your bot has not been added as a connection to the page.
       [https://github.com/ayvi-0001/notion-api/blob/main/examples/images/
                     directory_add_connections.png?raw=true]
 By default, a bot will have access to the children of any Parent object it has
 access too. Be sure to double check this connection when moving pages. If
 you're working on a page that your token has access to via its parent page/
 database, but you never explicitly granted access to the child page - and you
 later move that child page out, then it will lose access. ---
```

