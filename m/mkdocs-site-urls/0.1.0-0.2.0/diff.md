# Comparing `tmp/mkdocs-site-urls-0.1.0.tar.gz` & `tmp/mkdocs-site-urls-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mkdocs-site-urls-0.1.0.tar", last modified: Fri Jul 28 13:40:58 2023, max compression
+gzip compressed data, was "dist/mkdocs-site-urls-0.2.0.tar", last modified: Mon Jul 31 09:00:46 2023, max compression
```

## Comparing `mkdocs-site-urls-0.1.0.tar` & `mkdocs-site-urls-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:40:58.000000 mkdocs-site-urls-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 13:40:55.000000 mkdocs-site-urls-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-28 13:40:58.000000 mkdocs-site-urls-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-28 13:40:55.000000 mkdocs-site-urls-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:40:58.000000 mkdocs-site-urls-0.1.0/mkdocs_site_urls/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-28 13:40:55.000000 mkdocs-site-urls-0.1.0/mkdocs_site_urls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:40:58.000000 mkdocs-site-urls-0.1.0/mkdocs_site_urls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-28 13:40:58.000000 mkdocs-site-urls-0.1.0/mkdocs_site_urls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-28 13:40:58.000000 mkdocs-site-urls-0.1.0/mkdocs_site_urls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:40:58.000000 mkdocs-site-urls-0.1.0/mkdocs_site_urls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-28 13:40:58.000000 mkdocs-site-urls-0.1.0/mkdocs_site_urls.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 13:40:58.000000 mkdocs-site-urls-0.1.0/mkdocs_site_urls.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-28 13:40:55.000000 mkdocs-site-urls-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-28 13:40:58.000000 mkdocs-site-urls-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-28 13:40:55.000000 mkdocs-site-urls-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:00:46.000000 mkdocs-site-urls-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 09:00:40.000000 mkdocs-site-urls-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-31 09:00:46.000000 mkdocs-site-urls-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-31 09:00:40.000000 mkdocs-site-urls-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:00:46.000000 mkdocs-site-urls-0.2.0/mkdocs_site_urls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-31 09:00:40.000000 mkdocs-site-urls-0.2.0/mkdocs_site_urls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:00:46.000000 mkdocs-site-urls-0.2.0/mkdocs_site_urls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-31 09:00:45.000000 mkdocs-site-urls-0.2.0/mkdocs_site_urls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-31 09:00:46.000000 mkdocs-site-urls-0.2.0/mkdocs_site_urls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:00:45.000000 mkdocs-site-urls-0.2.0/mkdocs_site_urls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-31 09:00:45.000000 mkdocs-site-urls-0.2.0/mkdocs_site_urls.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 09:00:45.000000 mkdocs-site-urls-0.2.0/mkdocs_site_urls.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-31 09:00:40.000000 mkdocs-site-urls-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-31 09:00:46.000000 mkdocs-site-urls-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-31 09:00:40.000000 mkdocs-site-urls-0.2.0/setup.py
```

### Comparing `mkdocs-site-urls-0.1.0/LICENSE` & `mkdocs-site-urls-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-site-urls-0.1.0/PKG-INFO` & `mkdocs-site-urls-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,69 @@
 Metadata-Version: 2.1
 Name: mkdocs-site-urls
-Version: 0.1.0
+Version: 0.2.0
 Summary: A MkDocs plugin that adds support for site-relative URLs
 Home-page: https://github.com/OctoPrint/mkdocs-site-urls
 Author: Gina Häußge
 Author-email: gina@octoprint.org
 License: MIT
 Project-URL: Source, https://github.com/OctoPrint/mkdocs-site-urls
-Description: # MkDocs Site URLs
+Description: # MkDocs Site URLs Plugin
         
         A MkDocs plugin that adds support for site-relative `site:` URLs.
         
         Example:
         
         | URL | site_url | resulting URL |
         | --- | -------- | ------------- |
         | `site:images/foo.png` | `https://example.com/` | `/images/foo.png` |
         | `site:images/foo.png` | `https://example.com/bar/` | `/bar/images/foo.png` |
         
-        ## Usage
+        **Please note**: This plugin requires MkDocs 1.5 or higher.
+        
+        ## Getting Started
         
         1. Install the plugin from PyPI
            ```bash
            pip install mkdocs-site-urls
            ```
         2. Add the `site-urls` plugin to your `mkdocs.yml` plugins section:
            ```yaml
            plugins:
              - site-urls
            ```
-           There are no configuration options.
         3. Start using site-relative URLs in your Markdown files by prefixing them with `site:`:
            ```markdown
            [Link to another page](site:another-page/relative/to/the/site/root)
         
            ![Image](site:images/foo.png)
            ```
         
+        ## Configuration
+        
+        By default the plugin will replace URLs in `href`, `src` and `data` attributes. You can configure the attributes to replace
+        by setting the `attributes` option in your `mkdocs.yml`, e.g.:
+        
+        ```yaml
+        plugins:
+          - site-urls:
+              attributes:
+                - href
+                - src
+                - data
+                - data-url
+        ```
+        
+        Be advised that in case of any customization on your part you need to include the default attributes as well if you want
+        to keep them, as the default list will not be included automatically anymore.
+        
         ## How it works
         
         The plugin hooks into the [`on_page_content` event](https://www.mkdocs.org/dev-guide/plugins/#on_page_content)
-        and replaces all URLs in `href` or `src` attributes in the rendered HTML with the corresponding site-relative URLs.
+        and replaces all URLs in the configured attributes (by default `href`, `src` or `data`) in the rendered HTML with the corresponding site-relative URLs.
         
         ## License
         
         This project is licensed under the MIT license, see the [LICENSE](https://github.com/OctoPrint/mkdocs-site-urls/blob/main/LICENSE) file for details.
         
 Keywords: mkdocs,plugin
 Platform: UNKNOWN
```

### Comparing `mkdocs-site-urls-0.1.0/mkdocs_site_urls/__init__.py` & `mkdocs-site-urls-0.2.0/mkdocs_site_urls/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 import re
 import urllib.parse
 
 import mkdocs.plugins
-
-SITE_URLS_REGEX = re.compile(r'(href|src)="site:([^"]+)"', re.IGNORECASE)
+from mkdocs.config import config_options as c
+from mkdocs.config.defaults import MkDocsConfig
 
 logger = mkdocs.plugins.get_plugin_logger(__name__)
 
 
-class SiteUrlsPlugin(mkdocs.plugins.BasePlugin):
+class SiteUrlsConfig(mkdocs.config.base.Config):
+    attributes = c.Type(list, default=["href", "src", "data"])
+
+
+class SiteUrlsPlugin(mkdocs.plugins.BasePlugin[SiteUrlsConfig]):
+    def on_pre_build(self, *, config: MkDocsConfig) -> None:
+        self._regex = re.compile(
+            r"(" + "|".join(self.config["attributes"]) + r')="site:([^"]+)"',
+            re.IGNORECASE,
+        )
+
     @mkdocs.plugins.event_priority(50)
     def on_page_content(self, html, page, config, files):
         site_url = config["site_url"]
         path = urllib.parse.urlparse(site_url).path
 
         if not path:
             path = "/"
@@ -21,11 +31,11 @@
 
         def _replace(match):
             param = match.group(1)
             url = match.group(2)
             if url.startswith("/"):
                 url = url[1:]
 
-            logger.info(f"Replacing site:{match.group(2)} with {path}{url}...")
+            logger.info(f"Replacing site:{match.group(2)} with {path}{url}")
             return f'{param}="{path}{url}"'
 
-        return SITE_URLS_REGEX.sub(_replace, html)
+        return self._regex.sub(_replace, html)
```

### Comparing `mkdocs-site-urls-0.1.0/mkdocs_site_urls.egg-info/PKG-INFO` & `mkdocs-site-urls-0.2.0/mkdocs_site_urls.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,69 @@
 Metadata-Version: 2.1
 Name: mkdocs-site-urls
-Version: 0.1.0
+Version: 0.2.0
 Summary: A MkDocs plugin that adds support for site-relative URLs
 Home-page: https://github.com/OctoPrint/mkdocs-site-urls
 Author: Gina Häußge
 Author-email: gina@octoprint.org
 License: MIT
 Project-URL: Source, https://github.com/OctoPrint/mkdocs-site-urls
-Description: # MkDocs Site URLs
+Description: # MkDocs Site URLs Plugin
         
         A MkDocs plugin that adds support for site-relative `site:` URLs.
         
         Example:
         
         | URL | site_url | resulting URL |
         | --- | -------- | ------------- |
         | `site:images/foo.png` | `https://example.com/` | `/images/foo.png` |
         | `site:images/foo.png` | `https://example.com/bar/` | `/bar/images/foo.png` |
         
-        ## Usage
+        **Please note**: This plugin requires MkDocs 1.5 or higher.
+        
+        ## Getting Started
         
         1. Install the plugin from PyPI
            ```bash
            pip install mkdocs-site-urls
            ```
         2. Add the `site-urls` plugin to your `mkdocs.yml` plugins section:
            ```yaml
            plugins:
              - site-urls
            ```
-           There are no configuration options.
         3. Start using site-relative URLs in your Markdown files by prefixing them with `site:`:
            ```markdown
            [Link to another page](site:another-page/relative/to/the/site/root)
         
            ![Image](site:images/foo.png)
            ```
         
+        ## Configuration
+        
+        By default the plugin will replace URLs in `href`, `src` and `data` attributes. You can configure the attributes to replace
+        by setting the `attributes` option in your `mkdocs.yml`, e.g.:
+        
+        ```yaml
+        plugins:
+          - site-urls:
+              attributes:
+                - href
+                - src
+                - data
+                - data-url
+        ```
+        
+        Be advised that in case of any customization on your part you need to include the default attributes as well if you want
+        to keep them, as the default list will not be included automatically anymore.
+        
         ## How it works
         
         The plugin hooks into the [`on_page_content` event](https://www.mkdocs.org/dev-guide/plugins/#on_page_content)
-        and replaces all URLs in `href` or `src` attributes in the rendered HTML with the corresponding site-relative URLs.
+        and replaces all URLs in the configured attributes (by default `href`, `src` or `data`) in the rendered HTML with the corresponding site-relative URLs.
         
         ## License
         
         This project is licensed under the MIT license, see the [LICENSE](https://github.com/OctoPrint/mkdocs-site-urls/blob/main/LICENSE) file for details.
         
 Keywords: mkdocs,plugin
 Platform: UNKNOWN
```

