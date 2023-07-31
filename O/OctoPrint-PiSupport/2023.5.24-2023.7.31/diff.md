# Comparing `tmp/OctoPrint-PiSupport-2023.5.24.tar.gz` & `tmp/OctoPrint-PiSupport-2023.7.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/OctoPrint-PiSupport-2023.5.24.tar", last modified: Wed May 24 16:11:57 2023, max compression
+gzip compressed data, was "dist/OctoPrint-PiSupport-2023.7.31.tar", last modified: Mon Jul 31 13:44:19 2023, max compression
```

## Comparing `OctoPrint-PiSupport-2023.5.24.tar` & `OctoPrint-PiSupport-2023.7.31.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/
--rw-r--r--   0 runner    (1001) docker     (123)    34520 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/OctoPrint_PiSupport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-24 16:11:56.000000 OctoPrint-PiSupport-2023.5.24/OctoPrint_PiSupport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/OctoPrint_PiSupport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:11:56.000000 OctoPrint-PiSupport-2023.5.24/OctoPrint_PiSupport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-24 16:11:56.000000 OctoPrint-PiSupport-2023.5.24/OctoPrint_PiSupport.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:11:56.000000 OctoPrint-PiSupport-2023.5.24/OctoPrint_PiSupport.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:11:56.000000 OctoPrint-PiSupport-2023.5.24/OctoPrint_PiSupport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-24 16:11:56.000000 OctoPrint-PiSupport-2023.5.24/OctoPrint_PiSupport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/
--rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/static/clientjs/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/static/clientjs/pi_support.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/static/css/pi_support.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/static/js/pi_support.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/templates/pi_support_about_octopi.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/templates/pi_support_navbar.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/templates/pi_support_settings.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11164 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/translations/de/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-24 16:11:57.000000 OctoPrint-PiSupport-2023.5.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    24824 2023-05-24 16:11:51.000000 OctoPrint-PiSupport-2023.5.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:19.000000 OctoPrint-PiSupport-2023.7.31/
+-rw-r--r--   0 runner    (1001) docker     (123)    34520 2023-07-31 13:44:13.000000 OctoPrint-PiSupport-2023.7.31/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-31 13:44:13.000000 OctoPrint-PiSupport-2023.7.31/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:19.000000 OctoPrint-PiSupport-2023.7.31/OctoPrint_PiSupport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-07-31 13:44:19.000000 OctoPrint-PiSupport-2023.7.31/OctoPrint_PiSupport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-31 13:44:19.000000 OctoPrint-PiSupport-2023.7.31/OctoPrint_PiSupport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 13:44:19.000000 OctoPrint-PiSupport-2023.7.31/OctoPrint_PiSupport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-31 13:44:19.000000 OctoPrint-PiSupport-2023.7.31/OctoPrint_PiSupport.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 13:44:19.000000 OctoPrint-PiSupport-2023.7.31/OctoPrint_PiSupport.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 13:44:19.000000 OctoPrint-PiSupport-2023.7.31/OctoPrint_PiSupport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 13:44:19.000000 OctoPrint-PiSupport-2023.7.31/OctoPrint_PiSupport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-07-31 13:44:19.000000 OctoPrint-PiSupport-2023.7.31/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-31 13:44:13.000000 OctoPrint-PiSupport-2023.7.31/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:19.000000 OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/
+-rw-r--r--   0 runner    (1001) docker     (123)    20598 2023-07-31 13:44:13.000000 OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:19.000000 OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:19.000000 OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/static/clientjs/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-31 13:44:13.000000 OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/static/clientjs/pi_support.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:19.000000 OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-31 13:44:13.000000 OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/static/css/pi_support.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:19.000000 OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    14331 2023-07-31 13:44:13.000000 OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/static/js/pi_support.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:19.000000 OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-31 13:44:13.000000 OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/templates/pi_support_about_octopi.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-31 13:44:13.000000 OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/templates/pi_support_about_octopiuptodate.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-31 13:44:13.000000 OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/templates/pi_support_navbar.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-07-31 13:44:13.000000 OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/templates/pi_support_settings.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:19.000000 OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:19.000000 OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:19.000000 OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-07-31 13:44:13.000000 OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11164 2023-07-31 13:44:13.000000 OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/translations/de/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-31 13:44:19.000000 OctoPrint-PiSupport-2023.7.31/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    24824 2023-07-31 13:44:13.000000 OctoPrint-PiSupport-2023.7.31/setup.py
```

### Comparing `OctoPrint-PiSupport-2023.5.24/LICENSE` & `OctoPrint-PiSupport-2023.7.31/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoPrint-PiSupport-2023.5.24/OctoPrint_PiSupport.egg-info/PKG-INFO` & `OctoPrint-PiSupport-2023.7.31/OctoPrint_PiSupport.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoPrint-PiSupport
-Version: 2023.5.24
+Version: 2023.7.31
 Summary: Provides additional information about your Pi in the UI
 Home-page: https://github.com/OctoPrint/OctoPrint-PiSupport
 Author: Gina Häußge
 Author-email: gina@octoprint.org
 License: AGPLv3
 Description: # Pi Support
```

### Comparing `OctoPrint-PiSupport-2023.5.24/OctoPrint_PiSupport.egg-info/SOURCES.txt` & `OctoPrint-PiSupport-2023.7.31/OctoPrint_PiSupport.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -11,11 +11,12 @@
 OctoPrint_PiSupport.egg-info/requires.txt
 OctoPrint_PiSupport.egg-info/top_level.txt
 octoprint_pi_support/__init__.py
 octoprint_pi_support/static/clientjs/pi_support.js
 octoprint_pi_support/static/css/pi_support.css
 octoprint_pi_support/static/js/pi_support.js
 octoprint_pi_support/templates/pi_support_about_octopi.jinja2
+octoprint_pi_support/templates/pi_support_about_octopiuptodate.jinja2
 octoprint_pi_support/templates/pi_support_navbar.jinja2
 octoprint_pi_support/templates/pi_support_settings.jinja2
 octoprint_pi_support/translations/de/LC_MESSAGES/messages.mo
 octoprint_pi_support/translations/de/LC_MESSAGES/messages.po
```

### Comparing `OctoPrint-PiSupport-2023.5.24/PKG-INFO` & `OctoPrint-PiSupport-2023.7.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoPrint-PiSupport
-Version: 2023.5.24
+Version: 2023.7.31
 Summary: Provides additional information about your Pi in the UI
 Home-page: https://github.com/OctoPrint/OctoPrint-PiSupport
 Author: Gina Häußge
 Author-email: gina@octoprint.org
 License: AGPLv3
 Description: # Pi Support
```

### Comparing `OctoPrint-PiSupport-2023.5.24/README.md` & `OctoPrint-PiSupport-2023.7.31/README.md`

 * *Files identical despite different names*

### Comparing `OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/__init__.py` & `OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,14 +378,22 @@
             result["throttle_state"] = self._throttle_state.raw_value_hex
 
         if is_octopi():
             result["octopi_version"] = get_octopi_version()
 
         if is_octopiuptodate():
             result["octopiuptodate_build"] = get_octopiuptodate_build()
+            try:
+                build = result["octopiuptodate_build"].split("-")[-1]
+
+                result["octopiuptodate_build_short"] = (
+                    build[0:4] + "." + build[4:6] + "." + build[6:8] + "." + build[8:]
+                )
+            except Exception:
+                pass
 
         return result
 
     # ~~ SimpleApiPlugin
 
     def on_api_get(self, request):
         if not Permissions.PLUGIN_PI_SUPPORT_STATUS.can():
@@ -422,15 +430,23 @@
                 "type": "settings",
                 "name": gettext("Pi Support"),
                 "template": "pi_support_settings.jinja2",
                 "custom_bindings": False,
             }
         ]
 
-        if is_octopi():
+        if is_octopiuptodate():
+            configs.append(
+                {
+                    "type": "about",
+                    "name": "About OctoPi",
+                    "template": "pi_support_about_octopiuptodate.jinja2",
+                }
+            )
+        elif is_octopi():
             configs.append(
                 {
                     "type": "about",
                     "name": "About OctoPi",
                     "template": "pi_support_about_octopi.jinja2",
                 }
             )
```

### Comparing `OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/static/clientjs/pi_support.js` & `OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/static/clientjs/pi_support.js`

 * *Files identical despite different names*

### Comparing `OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/static/js/pi_support.js` & `OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/static/js/pi_support.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -164,23 +164,38 @@
                     self.notifications.default_password = undefined;
                 }
 
                 // OctoPi version
                 $("#pi_support_footer").remove();
                 if (!response.octopi_version) return;
 
-                var octoPiVersion = $(
-                    "<li id='pi_support_footer'><small>" +
-                    gettext("OctoPi") +
-                    " " +
-                    "<span class='octopi_version'>" +
-                    response.octopi_version +
-                    "</span></small></li>"
-                );
-                $("#footer_version").append(octoPiVersion);
+                if (response.octopiuptodate_build_short) {
+                    var octoPiVersion = $(
+                        "<li id='pi_support_footer'><small>" +
+                        gettext("OctoPi") +
+                        "* " +
+                        "<span class='octopi_version'>" +
+                        response.octopi_version +
+                        " (build " +
+                        response.octopiuptodate_build_short +
+                        ")" +
+                        "</span></small></li>"
+                    );
+                    $("#footer_version").append(octoPiVersion);
+                } else {
+                    var octoPiVersion = $(
+                        "<li id='pi_support_footer'><small>" +
+                        gettext("OctoPi") +
+                        " " +
+                        "<span class='octopi_version'>" +
+                        response.octopi_version +
+                        "</span></small></li>"
+                    );
+                    $("#footer_version").append(octoPiVersion);
+                }
             });
         };
 
         self.fromThrottleState = function(state) {
             self.currentUndervoltage(state.current_undervoltage);
             self.pastUndervoltage(state.past_undervoltage);
             self.currentOverheat(state.current_overheat);
```

### Comparing `OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/templates/pi_support_about_octopi.jinja2` & `OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/templates/pi_support_about_octopi.jinja2`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <h3>{{ _('About OctoPi') }}</h3>
 
 <h4>The ready-to-go Raspberry Pi image with OctoPrint</h4>
 
 <p>Version <span class="plugin_pi_support_octopi_version">{{ plugin_pi_support_octopi_version }}</span>, running on <span class="plugin_pi_support_model">{{ plugin_pi_support_model }}</span></p>
 
-<ul>
-    <li>Website: <a href="https://octoprint.org/download/" target="_blank" rel="noreferrer noopener">octoprint.org/download</a></li>
-    <li>Source Code: <a href="https://github.com/guysoft/OctoPi" target="_blank" rel="noreferrer noopener">github.com/guysoft/OctoPi</a></li>
+<ul class="fa-ul">
+    <li><i class="fa-li fab fa-github"></i> Source Code: <a href="https://github.com/guysoft/OctoPi" target="_blank" rel="noreferrer noopener">github.com/guysoft/OctoPi</a></li>
+    <li><i class="fa-li fas fa-code-branch"></i> Changelog: <a href="https://github.com/guysoft/OctoPi/releases/tag/{{ plugin_pi_support_octopi_version }}" target="_blank" rel="noreferrer noopener">github.com/guysoft/OctoPi/releases/tag/{{ plugin_pi_support_octopi_version }}</a></li>
 </ul>
 
 <p>
     &copy; 2013-{{ now.strftime("%Y") }} <a href="https://github.com/guysoft/OctoPi/graphs/contributors" target="_blank" rel="noreferrer noopener">The OctoPi Authors</a>
 </p>
 
 <p>
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 **** {{ _('About OctoPi') }} ****
 *** The ready-to-go Raspberry Pi image with OctoPrint ***
 Version {{ plugin_pi_support_octopi_version }}, running on {
 { plugin_pi_support_model }}
-    * Website: octoprint.org/download
-    * Source Code: github.com/guysoft/OctoPi
+    *  Source Code: github.com/guysoft/OctoPi
+    *  Changelog: github.com/guysoft/OctoPi/releases/tag/{
+      {_plugin_pi_support_octopi_version_}}
 © 2013-{{ now.strftime("%Y") }} The_OctoPi_Authors
 OctoPi is free software: you can redistribute it and/or modify it under the
 terms of the GNU General Public License as published by the Free Software
 Foundation, either version 3 of the License, or (at your option) any later
 version.
 OctoPi is distributed in the hope that it will be useful, but WITHOUT ANY
 WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
```

### Comparing `OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/templates/pi_support_navbar.jinja2` & `OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/templates/pi_support_navbar.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/templates/pi_support_settings.jinja2` & `OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/templates/pi_support_settings.jinja2`

 * *Files identical despite different names*

### Comparing `OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/translations/de/LC_MESSAGES/messages.mo` & `OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `OctoPrint-PiSupport-2023.5.24/octoprint_pi_support/translations/de/LC_MESSAGES/messages.po` & `OctoPrint-PiSupport-2023.7.31/octoprint_pi_support/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `OctoPrint-PiSupport-2023.5.24/setup.py` & `OctoPrint-PiSupport-2023.7.31/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 plugin_package = "octoprint_pi_support"
 
 # The plugin's human readable name. Can be overwritten within OctoPrint's internal data via __plugin_name__ in the
 # plugin module
 plugin_name = "OctoPrint-PiSupport"
 
 # The plugin's version. Can be overwritten within OctoPrint's internal data via __plugin_version__ in the plugin module
-plugin_version = "2023.5.24"
+plugin_version = "2023.7.31"
 
 # The plugin's description. Can be overwritten within OctoPrint's internal data via __plugin_description__ in the plugin
 # module
 plugin_description = """Provides additional information about your Pi in the UI"""
 
 # The plugin's author. Can be overwritten within OctoPrint's internal data via __plugin_author__ in the plugin module
 plugin_author = "Gina Häußge"
```

