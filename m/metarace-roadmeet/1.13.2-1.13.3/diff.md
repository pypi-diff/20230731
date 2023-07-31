# Comparing `tmp/metarace-roadmeet-1.13.2.tar.gz` & `tmp/metarace-roadmeet-1.13.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metarace-roadmeet-1.13.2.tar", last modified: Fri Jul 21 05:04:06 2023, max compression
+gzip compressed data, was "metarace-roadmeet-1.13.3.tar", last modified: Mon Jul 31 17:00:32 2023, max compression
```

## Comparing `metarace-roadmeet-1.13.2.tar` & `metarace-roadmeet-1.13.3.tar`

### file list

```diff
@@ -1,32 +1,29 @@
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-21 05:04:06.075077 metarace-roadmeet-1.13.2/
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1063 2023-07-07 01:56:04.000000 metarace-roadmeet-1.13.2/LICENSE
--rw-r--r--   0 ndf       (1000) ndf       (1000)       26 2022-11-24 00:09:22.000000 metarace-roadmeet-1.13.2/MANIFEST.in
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1970 2023-07-21 05:04:06.075077 metarace-roadmeet-1.13.2/PKG-INFO
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1411 2023-07-17 02:48:09.000000 metarace-roadmeet-1.13.2/README.md
--rw-r--r--   0 ndf       (1000) ndf       (1000)      746 2023-07-21 05:03:25.000000 metarace-roadmeet-1.13.2/pyproject.toml
--rw-r--r--   0 ndf       (1000) ndf       (1000)       38 2023-07-21 05:04:06.075077 metarace-roadmeet-1.13.2/setup.cfg
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-21 05:04:06.067076 metarace-roadmeet-1.13.2/src/
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-21 05:04:06.067076 metarace-roadmeet-1.13.2/src/metarace_roadmeet.egg-info/
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1970 2023-07-21 05:04:05.000000 metarace-roadmeet-1.13.2/src/metarace_roadmeet.egg-info/PKG-INFO
--rw-r--r--   0 ndf       (1000) ndf       (1000)      708 2023-07-21 05:04:06.000000 metarace-roadmeet-1.13.2/src/metarace_roadmeet.egg-info/SOURCES.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)        1 2023-07-21 05:04:05.000000 metarace-roadmeet-1.13.2/src/metarace_roadmeet.egg-info/dependency_links.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)       43 2023-07-21 05:04:05.000000 metarace-roadmeet-1.13.2/src/metarace_roadmeet.egg-info/entry_points.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)       16 2023-07-21 05:04:05.000000 metarace-roadmeet-1.13.2/src/metarace_roadmeet.egg-info/requires.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)        9 2023-07-21 05:04:05.000000 metarace-roadmeet-1.13.2/src/metarace_roadmeet.egg-info/top_level.txt
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-21 05:04:06.071076 metarace-roadmeet-1.13.2/src/roadmeet/
--rw-r--r--   0 ndf       (1000) ndf       (1000)    83826 2023-07-21 04:48:30.000000 metarace-roadmeet-1.13.2/src/roadmeet/__init__.py
--rw-r--r--   0 ndf       (1000) ndf       (1000)       79 2022-11-24 06:32:10.000000 metarace-roadmeet-1.13.2/src/roadmeet/__main__.py
--rw-r--r--   0 ndf       (1000) ndf       (1000)   110436 2023-07-20 09:05:00.000000 metarace-roadmeet-1.13.2/src/roadmeet/irtt.py
--rw-r--r--   0 ndf       (1000) ndf       (1000)   189881 2023-07-20 14:47:52.000000 metarace-roadmeet-1.13.2/src/roadmeet/rms.py
--rw-r--r--   0 ndf       (1000) ndf       (1000)    60325 2023-07-20 06:54:09.000000 metarace-roadmeet-1.13.2/src/roadmeet/trtt.py
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-21 05:04:06.075077 metarace-roadmeet-1.13.2/src/roadmeet/ui/
--r--r--r--   0 ndf       (1000) ndf       (1000)        0 2023-06-28 12:18:14.000000 metarace-roadmeet-1.13.2/src/roadmeet/ui/__init__.py
--r--r--r--   0 ndf       (1000) ndf       (1000)     4496 2023-05-30 11:27:50.000000 metarace-roadmeet-1.13.2/src/roadmeet/ui/irtt.ui
--r--r--r--   0 ndf       (1000) ndf       (1000)     7206 2023-06-01 06:00:37.000000 metarace-roadmeet-1.13.2/src/roadmeet/ui/new_start.ui
--r--r--r--   0 ndf       (1000) ndf       (1000)     2356 2023-06-24 03:51:06.000000 metarace-roadmeet-1.13.2/src/roadmeet/ui/rider_context.ui
--r--r--r--   0 ndf       (1000) ndf       (1000)     5625 2023-05-30 11:27:50.000000 metarace-roadmeet-1.13.2/src/roadmeet/ui/rms.ui
--r--r--r--   0 ndf       (1000) ndf       (1000)     5657 2023-06-14 12:44:18.000000 metarace-roadmeet-1.13.2/src/roadmeet/ui/rms_context.ui
--r--r--r--   0 ndf       (1000) ndf       (1000)    42196 2023-07-16 04:51:22.000000 metarace-roadmeet-1.13.2/src/roadmeet/ui/roadmeet.ui
--r--r--r--   0 ndf       (1000) ndf       (1000)     8749 2023-05-30 11:27:50.000000 metarace-roadmeet-1.13.2/src/roadmeet/ui/swap_rider.ui
--r--r--r--   0 ndf       (1000) ndf       (1000)     4389 2023-05-30 11:27:50.000000 metarace-roadmeet-1.13.2/src/roadmeet/ui/tod_context.ui
--rw-r--r--   0 ndf       (1000) ndf       (1000)    45889 2023-07-21 04:36:10.000000 metarace-roadmeet-1.13.2/src/roadmeet/uiutil.py
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-31 17:00:32.746825 metarace-roadmeet-1.13.3/
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     1063 2023-07-07 01:56:04.000000 metarace-roadmeet-1.13.3/LICENSE
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       26 2022-11-24 00:09:22.000000 metarace-roadmeet-1.13.3/MANIFEST.in
+-rw-r--r--   0 ndf       (1000) ndf       (1000)    10734 2023-07-31 17:00:32.746825 metarace-roadmeet-1.13.3/PKG-INFO
+-rw-r--r--   0 ndf       (1000) ndf       (1000)    10175 2023-07-31 15:26:14.000000 metarace-roadmeet-1.13.3/README.md
+-rw-r--r--   0 ndf       (1000) ndf       (1000)      746 2023-07-31 16:58:12.000000 metarace-roadmeet-1.13.3/pyproject.toml
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       38 2023-07-31 17:00:32.746825 metarace-roadmeet-1.13.3/setup.cfg
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-31 17:00:32.738825 metarace-roadmeet-1.13.3/src/
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-31 17:00:32.742825 metarace-roadmeet-1.13.3/src/metarace_roadmeet.egg-info/
+-rw-r--r--   0 ndf       (1000) ndf       (1000)    10734 2023-07-31 17:00:32.000000 metarace-roadmeet-1.13.3/src/metarace_roadmeet.egg-info/PKG-INFO
+-rw-r--r--   0 ndf       (1000) ndf       (1000)      613 2023-07-31 17:00:32.000000 metarace-roadmeet-1.13.3/src/metarace_roadmeet.egg-info/SOURCES.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)        1 2023-07-31 17:00:32.000000 metarace-roadmeet-1.13.3/src/metarace_roadmeet.egg-info/dependency_links.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       43 2023-07-31 17:00:32.000000 metarace-roadmeet-1.13.3/src/metarace_roadmeet.egg-info/entry_points.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       16 2023-07-31 17:00:32.000000 metarace-roadmeet-1.13.3/src/metarace_roadmeet.egg-info/requires.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)        9 2023-07-31 17:00:32.000000 metarace-roadmeet-1.13.3/src/metarace_roadmeet.egg-info/top_level.txt
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-31 17:00:32.742825 metarace-roadmeet-1.13.3/src/roadmeet/
+-rw-r--r--   0 ndf       (1000) ndf       (1000)    85094 2023-07-24 16:23:44.000000 metarace-roadmeet-1.13.3/src/roadmeet/__init__.py
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       79 2022-11-24 06:32:10.000000 metarace-roadmeet-1.13.3/src/roadmeet/__main__.py
+-rw-r--r--   0 ndf       (1000) ndf       (1000)   109940 2023-07-31 12:13:04.000000 metarace-roadmeet-1.13.3/src/roadmeet/irtt.py
+-rw-r--r--   0 ndf       (1000) ndf       (1000)   189509 2023-07-31 12:13:20.000000 metarace-roadmeet-1.13.3/src/roadmeet/rms.py
+-rw-r--r--   0 ndf       (1000) ndf       (1000)    60246 2023-07-24 16:09:39.000000 metarace-roadmeet-1.13.3/src/roadmeet/trtt.py
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-31 17:00:32.746825 metarace-roadmeet-1.13.3/src/roadmeet/ui/
+-r--r--r--   0 ndf       (1000) ndf       (1000)        0 2023-06-28 12:18:14.000000 metarace-roadmeet-1.13.3/src/roadmeet/ui/__init__.py
+-r--r--r--   0 ndf       (1000) ndf       (1000)     5280 2023-07-24 16:30:33.000000 metarace-roadmeet-1.13.3/src/roadmeet/ui/irtt.ui
+-r--r--r--   0 ndf       (1000) ndf       (1000)     7206 2023-07-24 16:15:03.000000 metarace-roadmeet-1.13.3/src/roadmeet/ui/new_start.ui
+-r--r--r--   0 ndf       (1000) ndf       (1000)     8202 2023-07-24 16:19:43.000000 metarace-roadmeet-1.13.3/src/roadmeet/ui/rms.ui
+-r--r--r--   0 ndf       (1000) ndf       (1000)    35760 2023-07-24 16:20:12.000000 metarace-roadmeet-1.13.3/src/roadmeet/ui/roadmeet.ui
+-r--r--r--   0 ndf       (1000) ndf       (1000)     8749 2023-07-24 16:07:31.000000 metarace-roadmeet-1.13.3/src/roadmeet/ui/swap_rider.ui
+-rw-r--r--   0 ndf       (1000) ndf       (1000)    45966 2023-07-31 16:58:41.000000 metarace-roadmeet-1.13.3/src/roadmeet/uiutil.py
```

### Comparing `metarace-roadmeet-1.13.2/LICENSE` & `metarace-roadmeet-1.13.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metarace-roadmeet-1.13.2/pyproject.toml` & `metarace-roadmeet-1.13.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metarace-roadmeet"
-version = "1.13.2"
+version = "1.13.3"
 description = "Timing and result application for road cycling events"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "MIT"}
 keywords = ["roadrace", "timetrial", "transponder"]
 authors = [
     {email = "ndf-zz@6-v.org", name = "Nathan Fraser"}
```

### Comparing `metarace-roadmeet-1.13.2/src/metarace_roadmeet.egg-info/SOURCES.txt` & `metarace-roadmeet-1.13.3/src/metarace_roadmeet.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -13,13 +13,10 @@
 src/roadmeet/irtt.py
 src/roadmeet/rms.py
 src/roadmeet/trtt.py
 src/roadmeet/uiutil.py
 src/roadmeet/ui/__init__.py
 src/roadmeet/ui/irtt.ui
 src/roadmeet/ui/new_start.ui
-src/roadmeet/ui/rider_context.ui
 src/roadmeet/ui/rms.ui
-src/roadmeet/ui/rms_context.ui
 src/roadmeet/ui/roadmeet.ui
-src/roadmeet/ui/swap_rider.ui
-src/roadmeet/ui/tod_context.ui
+src/roadmeet/ui/swap_rider.ui
```

### Comparing `metarace-roadmeet-1.13.2/src/roadmeet/__init__.py` & `metarace-roadmeet-1.13.3/src/roadmeet/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from metarace import report
 
 from . import uiutil
 from roadmeet.rms import rms, _CONFIG_SCHEMA as _RMS_SCHEMA
 from roadmeet.irtt import irtt, _CONFIG_SCHEMA as _IRTT_SCHEMA
 from roadmeet.trtt import trtt, _CONFIG_SCHEMA as _TRTT_SCHEMA
 
-VERSION = '1.13.2'
+VERSION = '1.13.3'
 LOGFILE = 'event.log'
 LOGFILE_LEVEL = logging.DEBUG
 CONFIGFILE = 'config.json'
 ROADMEET_ID = 'roadmeet-3.2'  # configuration versioning
 EXPORTPATH = 'export'
 _log = logging.getLogger('roadmeet')
 _log.setLevel(logging.DEBUG)
@@ -305,28 +305,39 @@
         """Return the <= 16 char shortname."""
         return self.shortname
 
     def cat_but_auto_clicked(self, but, entry, data=None):
         """Lookup cats and write them into the supplied entry."""
         entry.set_text(' '.join(self.rdb.listcats()))
 
-    def menu_race_decisions_activate_cb(self, menuitem, data=None):
+    def menu_event_decisions_activate_cb(self, menuitem, data=None):
         """Edit decisions of the commissaires panel."""
         if self.curevent is not None:
             self.curevent.decisions = uiutil.decisions_dlg(
                 self.window, self.curevent.decisions)
 
-    def menu_race_properties_activate_cb(self, menuitem, data=None):
-        """Edit race specific properties."""
+    def menu_event_properties_activate_cb(self, menuitem, data=None):
+        """Edit event specific properties."""
         if self.curevent is not None:
-            _log.debug('Editing race properties')
+            _log.debug('Editing event properties')
             if self.curevent.edit_event_properties(self.window):
                 _log.info('Event re-start required')
                 self.event_reload()
 
+    def menu_event_reset_cb(self, menuitem, data=None):
+        """Reset current event."""
+        if self.curevent is not None:
+            _log.debug('Reset event')
+            if uiutil.questiondlg(
+                    window=self.window,
+                    question='Reset event to idle?',
+                    subtext='Note: All result and timing data will be cleared.',
+                    title='Reset Event?'):
+                self.curevent.resettimer()
+
     def menu_meet_properties_cb(self, menuitem, data=None):
         """Edit meet properties."""
         metarace.sysconf.add_section('export', _EXPORT_SCHEMA)
         metarace.sysconf.add_section('telegraph', _TG_SCHEMA)
         metarace.sysconf.add_section('thbc', _THBC_SCHEMA)
         metarace.sysconf.add_section('rru', _RRU_SCHEMA)
         metarace.sysconf.add_section('rrs', _RRS_SCHEMA)
@@ -533,39 +544,39 @@
 
     def event_reload(self):
         """Open the event handler."""
         self.open_event()
         self.set_title()
         return False
 
-    def menu_race_armstart_activate_cb(self, menuitem, data=None):
+    def menu_event_armstart_activate_cb(self, menuitem, data=None):
         """Default armstart handler."""
         _log.info('Arm Start')
         try:
             self.curevent.armstart()
         except Exception as e:
             _log.error('Arm start %s: %s', e.__class__.__name__, e)
 
-    def menu_race_armlap_activate_cb(self, menuitem, data=None):
+    def menu_event_armlap_activate_cb(self, menuitem, data=None):
         """Default armlap handler."""
         _log.debug('Arm Lap')
         try:
             self.curevent.armlap()
         except Exception as e:
             _log.error('Arm lap %s: %s', e.__class__.__name__, e)
 
-    def menu_race_armfin_activate_cb(self, menuitem, data=None):
+    def menu_event_armfin_activate_cb(self, menuitem, data=None):
         """Default armfin handler."""
         _log.info('Arm Finish')
         try:
             self.curevent.armfinish()
         except Exception as e:
             _log.error('Arm finish %s: %s', e.__class__.__name__, e)
 
-    def menu_race_finished_activate_cb(self, menuitem, data=None):
+    def menu_event_finished_activate_cb(self, menuitem, data=None):
         """Default finished handler."""
         _log.info('Finished')
         try:
             self.curevent.set_finished()
         except Exception as e:
             _log.error('Set finished %s: %s', e.__class__.__name__, e)
 
@@ -578,31 +589,31 @@
             self.curevent = irtt(self, self.etype, True)
         elif self.etype == 'trtt':
             self.curevent = trtt(self, self.etype, True)
         else:
             self.curevent = rms(self, self.etype, True)
 
         self.curevent.loadconfig()
-        self.race_box.add(self.curevent.frame)
+        self.event_box.add(self.curevent.frame)
 
         # re-populate the rider command model.
         cmdo = self.curevent.get_ridercmdorder()
         cmds = self.curevent.get_ridercmds()
         if cmds is not None:
             self.action_model.clear()
             for cmd in cmdo:
                 self.action_model.append([cmd, cmds[cmd]])
             self.action_combo.set_active(0)
         self.curevent.show()
 
     def close_event(self):
-        """Close the currently opened race."""
+        """Close the currently opened event."""
         if self.curevent is not None:
-            if self.curevent.frame in self.race_box.get_children():
-                self.race_box.remove(self.curevent.frame)
+            if self.curevent.frame in self.event_box.get_children():
+                self.event_box.remove(self.curevent.frame)
             self.curevent.destroy()
             self.curevent = None
             self.stat_but.update('idle', 'Closed')
             self.stat_but.set_sensitive(False)
 
     ## Reports menu callbacks.
     def menu_reports_startlist_activate_cb(self, menuitem, data=None):
@@ -642,23 +653,23 @@
     def menu_reports_camera_activate_cb(self, menuitem, data=None):
         """Generate the camera operator report."""
         if self.curevent is not None:
             sections = self.curevent.camera_report()
             if sections:
                 self.print_report(sections)
 
-    def race_results_points_activate_cb(self, menuitem, data=None):
+    def event_results_points_activate_cb(self, menuitem, data=None):
         """Generate the points tally report."""
         if self.curevent is not None:
             sections = self.curevent.points_report()
             if sections:
                 self.print_report(sections)
 
     def menu_reports_result_activate_cb(self, menuitem, data=None):
-        """Generate the race result report."""
+        """Generate the event result report."""
         if self.curevent is not None:
             sections = self.curevent.result_report()
             if sections:
                 self.print_report(sections,
                                   self.curevent.timerstat != 'finished')
 
     def menu_data_replace_activate_cb(self, menuitem, data=None):
@@ -950,15 +961,15 @@
                 _log.info('Decoder disconnected')
         else:
             _log.info('No decoder configured')
         # always call into alt timer
         self._alttimer.status()
 
     def menu_timing_start_activate_cb(self, menuitem, data=None):
-        """Manually set race elapsed time via trigger."""
+        """Manually set event elapsed time via trigger."""
         if self.curevent is None:
             _log.info('No event open to set elapsed time on')
         else:
             self.curevent.elapsed_dlg()
 
     def entry_set_now(self, button, entry=None):
         """Enter the current time in the provided entry."""
@@ -1045,29 +1056,29 @@
 
     ## Help menu callbacks
     def menu_help_about_cb(self, menuitem, data=None):
         """Display metarace about dialog."""
         uiutil.about_dlg(self.window, VERSION)
 
     ## Race Control Elem callbacks
-    def race_stat_but_clicked_cb(self, button, data=None):
+    def event_stat_but_clicked_cb(self, button, data=None):
         """Call through into event if open."""
         if self.curevent is not None:
             self.curevent.stat_but_clicked(button)
 
-    def race_stat_entry_activate_cb(self, entry, data=None):
+    def event_stat_entry_activate_cb(self, entry, data=None):
         """Pass the chosen action and bib list through to curevent."""
         action = self.action_model.get_value(
             self.action_combo.get_active_iter(), 0)
         if self.curevent is not None:
-            if self.curevent.race_ctrl(action, self.action_entry.get_text()):
+            if self.curevent.event_ctrl(action, self.action_entry.get_text()):
                 self.action_entry.set_text('')
 
     ## Menu button callbacks
-    def race_action_combo_changed_cb(self, combo, data=None):
+    def event_action_combo_changed_cb(self, combo, data=None):
         """Notify curevent of change in combo."""
         aiter = self.action_combo.get_active_iter()
         if self.curevent is not None and aiter is not None:
             action = self.action_model.get_value(aiter, 0)
             self.curevent.ctrl_change(action, self.action_entry)
 
     def menu_clock_clicked_cb(self, button, data=None):
@@ -1081,15 +1092,15 @@
             # check for completion in the export thread
             if self.mirror is not None:
                 if not self.mirror.is_alive():
                     self.mirror = None
                     _log.debug('Removing completed export thread.')
 
             if self.running:
-                # call into race timeout handler
+                # call into event timeout handler
                 if self.curevent is not None:
                     self.curevent.timeout()
 
                 # update the menu status button
                 nt = tod.now().meridiem()
                 if self.rfuact:
                     self.rfustat.update('activity', nt)
@@ -1156,15 +1167,15 @@
         if self.loghandler is not None:
             rootlogger.removeHandler(self.loghandler)
         self.running = False
         Gtk.main_quit()
         return False
 
     def key_event(self, widget, event):
-        """Collect key events on main window and send to race."""
+        """Collect key events on main window and send to event."""
         if event.type == Gdk.EventType.KEY_PRESS:
             key = Gdk.keyval_name(event.keyval) or 'None'
             if event.state & Gdk.ModifierType.CONTROL_MASK:
                 key = key.lower()
                 t = tod.now(chan='MAN', refid=str(key))
                 if key in ('0', '1'):
                     # trigger
@@ -1172,14 +1183,18 @@
                     t.chan = strops.id2chan(strops.chan2id(key))
                     self._alttimercb(t)
                     return True
                 elif key in ('2', '3', '4', '5', '6', '7', '8', '9'):
                     # passing
                     self._timercb(t)
                     return True
+                elif key == 'left':
+                    self.notebook.prev_page()
+                elif key == 'right':
+                    self.notebook.next_page()
             if self.curevent is not None:
                 return self.curevent.key_event(widget, event)
         return False
 
     def shutdown(self, msg=''):
         """Shutdown worker threads and close application."""
         self.started = False
@@ -1269,19 +1284,19 @@
         # make sure export path exists
         if not os.path.exists(self.exportpath):
             os.mkdir(self.exportpath)
             _log.info('Created export path: %r', self.exportpath)
 
         # check and warn of config mismatch
         cid = cr.get_value('roadmeet', 'id')
-        if cid != ROADMEET_ID:
+        if cid is not None and cid != ROADMEET_ID:
             _log.warning('Meet config mismatch: %r != %r', cid, ROADMEET_ID)
 
     def get_distance(self):
-        """Return race distance in km."""
+        """Return meet distance in km."""
         return self.distance
 
     ## Announcer methods (replaces old irc/unt telegraph)
     def cmd_announce(self, command, msg):
         """Announce the supplied message to the command topic."""
         if self.anntopic:
             topic = '/'.join((self.anntopic, command))
@@ -1550,17 +1565,25 @@
                     view.grab_focus()
                     view.set_cursor(path, col, False)
                     sel = view.get_selection().get_selected()
                     if sel is not None:
                         i = sel[1]
                         r = Gtk.TreeModelRow(self._cur_model, i)
                         self._cur_rider_sel = r[7]
+                        self._rider_menu_edit.set_sensitive(True)
+                        self._rider_menu_del.set_sensitive(True)
                     else:
                         _log.error('Invalid selection ignored')
                         self._cur_rider_sel = None
+                        self._rider_menu_edit.set_sensitive(False)
+                        self._rider_menu_del.set_sensitive(False)
+                else:
+                    self._cur_rider_sel = None
+                    self._rider_menu_edit.set_sensitive(False)
+                    self._rider_menu_del.set_sensitive(False)
                 self._rider_menu.popup_at_pointer(None)
                 return True
         return False
 
     def rider_add_cb(self, menuitem, data=None):
         """Create a new rider entry and edit the content"""
         nser = ''
@@ -1812,31 +1835,40 @@
         self.status = b.get_object('status')
         self.log_buffer = b.get_object('log_buffer')
         self.log_view = b.get_object('log_view')
         #self.log_view.modify_font(uiutil.LOGVIEWFONT)
         self.log_scroll = b.get_object('log_box').get_vadjustment()
         self.context = self.status.get_context_id('metarace meet')
         self.decoder_configure = b.get_object('menu_timing_configure')
-        self.race_box = b.get_object('race_box')
+        self.event_box = b.get_object('event_box')
         self.stat_but = uiutil.statButton()
-        b.get_object('race_stat_but').add(self.stat_but)
-        self.action_model = b.get_object('race_action_model')
-        self.action_combo = b.get_object('race_action_combo')
-        self.action_entry = b.get_object('race_action_entry')
-        b.get_object('race_stat_hbox').set_focus_chain(
+        b.get_object('event_stat_but').add(self.stat_but)
+        self.action_model = b.get_object('event_action_model')
+        self.action_combo = b.get_object('event_action_combo')
+        self.action_entry = b.get_object('event_action_entry')
+        b.get_object('event_stat_hbox').set_focus_chain(
             [self.action_combo, self.action_entry, self.action_combo])
+        self.notebook = b.get_object('meet_nb')
 
         # prepare local scratch pad ? can these be removed?
         self.an_cur_lap = tod.ZERO
         self.an_cur_split = tod.ZERO
         self.an_cur_bunchid = 0
         self.an_cur_bunchcnt = 0
         self.an_last_time = None
         self.an_cur_start = tod.ZERO
 
+        # setup context menu handles
+        self._rider_menu = b.get_object('rider_context')
+        self._rider_menu_edit = b.get_object('rider_edit')
+        self._rider_menu_lookup = b.get_object('rider_lookup')
+        self._rider_menu_del = b.get_object('rider_del')
+        self._cur_rider_sel = None
+        self._cur_model = None
+
         b.connect_signals(self)
 
         # run state
         self.running = True
         self.started = False
         self.curevent = None
 
@@ -1850,21 +1882,14 @@
         rootlogger.addHandler(self.sh)
         self.lh = uiutil.textViewHandler(self.log_buffer, self.log_view,
                                          self.log_scroll)
         self.lh.setFormatter(f)
         self.lh.setLevel(logging.INFO)  # show info+ in text view
         rootlogger.addHandler(self.lh)
 
-        # create a rider context menu
-        bc = uiutil.builder('rider_context.ui')
-        self._rider_menu = bc.get_object('rider_context')
-        self._cur_rider_sel = None
-        self._cur_model = None
-        bc.connect_signals(self)
-
         # Build a rider list store and view
         self._rlm = Gtk.ListStore(
             str,  # no 0
             str,  # series 1
             str,  # name 2 
             str,  # org 3
             str,  # categories 4
@@ -1938,15 +1963,15 @@
         _log.debug('Add riderdb')
         self.rdb = riderdb.riderdb()
         self.rdb.set_notify(self._rcb)
         self._tagmap = {}
         self._maptag = {}
 
         # select event page in notebook.
-        b.get_object('meet_nb').set_current_page(0)
+        self.notebook.set_current_page(0)
 
         # start timer
         GLib.timeout_add_seconds(1, self.timeout)
 
 
 class fakemeet(roadmeet):
     """Non-interactive meet wrapper"""
```

### Comparing `metarace-roadmeet-1.13.2/src/roadmeet/irtt.py` & `metarace-roadmeet-1.13.3/src/roadmeet/irtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,32 +271,15 @@
             self.inters[COL_INTERB][cat].clear()
             self.inters[COL_INTERC][cat].clear()
             self.inters[COL_INTERD][cat].clear()
             self.inters[COL_INTERE][cat].clear()
         self._dorecalc = True
 
     def key_event(self, widget, event):
-        """Race window key press handler."""
-        if event.type == Gdk.EventType.KEY_PRESS:
-            key = Gdk.keyval_name(event.keyval) or 'None'
-            if event.state & Gdk.ModifierType.CONTROL_MASK:
-                if key == key_abort:  # override ctrl+f5
-                    if uiutil.questiondlg(
-                            window=self.meet.window,
-                            question='Reset event to idle?',
-                            subtext=
-                            'Note: All result and timing data will be cleared.',
-                            title='Reset event?'):
-                        self.resettimer()
-                    return True
-            if key[0] == 'F':
-                if key == key_announce:
-                    self.meet.cmd_announce('clear', 'all')
-                    self._doannounce = True
-                    return True
+        """Ignore keys in irtt"""
         return False
 
     def resetall(self):
         """Reset timers."""
         self.fl.toidle()
         self.fl.disable()
 
@@ -306,16 +289,27 @@
             self.timerstat = 'running'
             self.meet.stat_but.update('ok', 'Running')
             self.meet.stat_but.set_sensitive(True)
         else:
             self.timerstat = 'finished'
             self.meet.stat_but.update('idle', 'Finished')
             self.meet.stat_but.set_sensitive(False)
+            self.hidetimer(True)
+
+    def hidetimer(self, hide=False):
+        if hide:
+            self.timericon.set_from_icon_name('view-reveal-symbolic',
+                                              Gtk.IconSize.SMALL_TOOLBAR)
             self.showtimers = False
             self.timerframe.hide()
+        else:
+            self.timericon.set_from_icon_name('view-conceal-symbolic',
+                                              Gtk.IconSize.SMALL_TOOLBAR)
+            self.showtimers = True
+            self.timerframe.show()
 
     def armfinish(self):
         if self.timerstat == 'running':
             if self.fl.getstatus() != 'finish' and self.fl.getstatus(
             ) != 'armfin':
                 self.fl.toarmfin()
             else:
@@ -371,15 +365,15 @@
             cr.set_property('style', uiutil.STYLE_NORMAL)
         else:
             wt = model.get_value(iter, COL_WALLSTART)
             if wt is not None:
                 cr.set_property('text', wt.rawtime(0))
             else:
                 cr.set_property('text', '')  # no info on start time
-            cr.set_property('style', uiutil.STYLE_OBLIQUE)
+            cr.set_property('style', uiutil.STYLE_ITALIC)
 
     def announce_rider(self,
                        place='',
                        bib='',
                        namestr='',
                        shortname='',
                        cat='',
@@ -436,15 +430,15 @@
                 st = self.riders.get_value(iter, COL_WALLSTART)
             if st is not None:  # still none is error
                 # truncate rolling time
                 ret = (tod.now() - st).truncate(self.precision)
         return ret
 
     def checkplaces(self, rlist='', dnf=True):
-        """Check the proposed places against current race model."""
+        """Check the proposed places against current event model."""
         ret = True
         placeset = set()
         for no in strops.reformat_bibserlist(rlist).split():
             if no != 'x':
                 # repetition? - already in place set?
                 if no in placeset:
                     _log.error('Duplicate no in places: %r', no)
@@ -453,15 +447,15 @@
                 # rider in the model?
                 b, s = strops.bibstr2bibser(no)
                 lr = self.getrider(b, s)
                 if lr is None:
                     _log.error('Non-starter in places: %r', no)
                     ret = False
                 else:
-                    # rider still in the race?
+                    # rider still in the event?
                     if lr[COL_COMMENT]:
                         _log.warning('DNS/DNF rider in places: %r', no)
                         if dnf:
                             ret = False
             else:
                 # placeholder needs to be filled in later or left off
                 _log.info('Placeholder in places')
@@ -479,15 +473,15 @@
                 _log.info('Rider %r returned to event', bib)
             else:
                 _log.warning('Unregistered rider %r unchanged', bib)
         if recalc:
             self.recalculate()
         return False
 
-    def race_ctrl(self, acode='', rlist=''):
+    def event_ctrl(self, acode='', rlist=''):
         """Apply the selected action to the provided bib list."""
         if acode in self.intermeds:
             if acode == 'brk':
                 rlist = ' '.join(strops.riderlist_split(rlist))
                 self.intsprint(acode, rlist)
             else:
                 rlist = strops.reformat_bibserplacelist(rlist)
@@ -549,27 +543,27 @@
     def elapstr(self, col, cr, model, iter, data=None):
         """Format elapsed time into text for listview."""
         ft = model.get_value(iter, COL_TODFINISH)
         if ft is not None:
             st = model.get_value(iter, COL_TODSTART)
             if st is None:  # defer to wall start time
                 st = model.get_value(iter, COL_WALLSTART)
-                cr.set_property('style', uiutil.STYLE_OBLIQUE)
+                cr.set_property('style', uiutil.STYLE_ITALIC)
             else:
                 cr.set_property('style', uiutil.STYLE_NORMAL)
             et = self.getelapsed(iter)
             if et is not None:
                 cr.set_property('text', et.rawtime(self.precision))
             else:
                 cr.set_property('text', '[ERR]')
         else:
             cr.set_property('text', '')
 
     def loadconfig(self):
-        """Load race config from disk."""
+        """Load event config from disk."""
         self.ridernos.clear()
         self.riders.clear()
         self.results = {'': tod.todlist('UNCAT')}
         self.cats = []
 
         cr = jsonconfig.config({
             'irtt': {
@@ -608,15 +602,15 @@
             else:
                 _log.debug('Invalid target lap count (%d) ignored',
                            self.totlaps)
                 self.totlaps = None
 
         # hide timer panes
         if not self.showtimers:
-            self.timerframe.hide()
+            self.hidetimer(True)
 
         # transponder timing options
         if self.startloop is not None or self.finishloop is not None:
             if self.autoimpulse:
                 configok = True
                 if self.startloop is None or self.finishloop is None:
                     _log.error(
@@ -764,15 +758,15 @@
         # After load complete - check config and report.
         eid = cr.get_value('irtt', 'id')
         if eid is not None and eid != EVENT_ID:
             _log.info('Event config mismatch: %r != %r', eid, EVENT_ID)
             self.readonly = True
 
     def saveconfig(self):
-        """Save race to disk."""
+        """Save event to disk."""
         if self.readonly:
             _log.error('Attempt to save readonly event')
             return
         cw = jsonconfig.config()
         cw.add_section('irtt', _CONFIG_SCHEMA)
         cw.import_section('irtt', self)
         cw.set('irtt', 'start', self.start)
@@ -870,15 +864,15 @@
         """Return a list of bibs in the rider model as b.s."""
         ret = []
         for r in self.riders:
             ret.append(strops.bibser2bibstr(r[COL_BIB], r[COL_SERIES]))
         return ' '.join(ret)
 
     def get_starters(self):
-        """Return a list of riders that 'started' the race."""
+        """Return a list of riders that 'started' the event."""
         ret = []
         for r in self.riders:
             if r[COL_COMMENT] != 'dns' or r[COL_INRACE]:
                 ret.append(strops.bibser2bibstr(r[COL_BIB], r[COL_SERIES]))
         return ' '.join(ret)
 
     def reorder_signon(self):
@@ -1335,30 +1329,30 @@
             if hdcount > 0:
                 sec.lines.append([
                     None,
                     'Riders finishing out of time limits: ' + str(hdcount)
                 ])
             if dnfcount > 0:
                 sec.lines.append(
-                    [None, 'Riders abandoning the race: ' + str(dnfcount)])
+                    [None, 'Riders abandoning the event: ' + str(dnfcount)])
             ret.append(sec)
 
             # finish report title manipulation
             if catname:
                 cv = []
                 if rsec.heading:
                     cv.append(rsec.heading)
                 cv.append(catname)
                 rsec.heading = ': '.join(cv)
                 rsec.subheading = subhead
             ret.append(report.pagebreak())
         return ret
 
     def result_report(self):
-        """Return a race result report."""
+        """Return event result report."""
         ret = []
         self.recalculate()
 
         # show arrivals if running
         if self.timerstat == 'running':
             # until final, show last few
             arvls = self.arrival_report()
@@ -1914,15 +1908,15 @@
                     _log.info('Load starter: ' + repr(bib))
                     self.sl.setrider(bib, ser)
                     self.sl.toarmstart()
                     self.start_unload = ws + tod.tod('5')
                     break
 
     def timeout(self):
-        """Update slow changing aspects of race."""
+        """Update slow changing aspects of event."""
         if not self.winopen:
             return False
         if self._dorecalc:
             self.recalculate()
             if self.autoexport:
                 GLib.idle_add(self.meet.menu_data_results_cb, None)
 
@@ -2037,24 +2031,24 @@
         if r is not None:
             r[COL_WALLSTART] = start
             _log.debug('Set start time for %s: %s',
                        strops.bibser2bibstr(bib, series), start.rawtime(0))
             #self.unstart(bib, series, wst=start)
 
     def delrider(self, bib='', series=''):
-        """Delete the specified rider from the race model."""
+        """Delete the specified rider from the event model."""
         i = self.getiter(bib, series)
         if i is not None:
             self.settimes(i)
             self.riders.remove(i)
         if (bib, series) in self.ridernos:
             self.ridernos.remove((bib, series))
 
     def addrider(self, bib='', series=''):
-        """Add specified rider to race model."""
+        """Add specified rider to event model."""
         if bib and (bib, series) in self.ridernos:
             return None
 
         if bib:
             nr = [
                 bib, '', '', '', '', True, '', 0, 0, None, None, None,
                 tod.ZERO, None, None, None, None, None, None, None, None, None,
@@ -2105,19 +2099,15 @@
         """Update the local record lr with data from riderdb handle r"""
         lr[COL_NAMESTR] = r.listname()
         lr[COL_CAT] = r['cat']
         lr[COL_SHORTNAME] = r.fitname(24)
 
     def info_time_edit_clicked_cb(self, button, data=None):
         """Toggle the visibility of timer panes"""
-        self.showtimers = not self.showtimers
-        if self.showtimers:
-            self.timerframe.show()
-        else:
-            self.timerframe.hide()
+        self.hidetimer(self.showtimers)
 
     def editcol_cb(self, cell, path, new_text, col):
         """Update value in edited cell."""
         new_text = new_text.strip()
         if col == COL_PASS:
             if new_text.isdigit():
                 self.riders[path][COL_PASS] = int(new_text)
@@ -2319,15 +2309,15 @@
                                      COL_BIB) == bib and self.riders.get_value(
                                          i, COL_SERIES) == series:
                 break
             i = self.riders.iter_next(i)
         return i
 
     def dnfriders(self, biblist='', code='dnf'):
-        """Remove each rider from the race with supplied code."""
+        """Remove each rider from the event with supplied code."""
         recalc = False
         for bibstr in biblist.split():
             bib, ser = strops.bibstr2bibser(bibstr)
             r = self.getrider(bib, ser)
             if r is not None:
                 r[COL_COMMENT] = code
                 nri = r.iter
@@ -2379,15 +2369,15 @@
     def settimes(self,
                  iter,
                  wst=None,
                  tst=None,
                  tft=None,
                  pt=None,
                  doplaces=True):
-        """Transfer race times into rider model."""
+        """Transfer event times into rider model."""
         bib = self.riders.get_value(iter, COL_BIB)
         series = self.riders.get_value(iter, COL_SERIES)
         cs = self.riders.get_value(iter, COL_CAT)
         cat = self.ridercat(riderdb.primary_cat(cs))
         #_log.debug('Check: ' + repr(bib) + ', ' + repr(series)
         #+ ', ' + repr(cat))
 
@@ -2472,76 +2462,76 @@
                 path, col, cellx, celly = pathinfo
                 treeview.grab_focus()
                 treeview.set_cursor(path, col, False)
                 self.context_menu.popup_at_pointer(None)
                 return True
         return False
 
-    def tod_context_print_activate_cb(self, menuitem, data=None):
+    def rider_context_print_activate_cb(self, menuitem, data=None):
         """Print times for selected rider."""
         _log.info('Print times not implemented.')
         pass
 
-    def tod_context_dns_activate_cb(self, menuitem, data=None):
+    def rider_context_dns_activate_cb(self, menuitem, data=None):
         """Register rider as non-starter."""
         sel = self.view.get_selection().get_selected()
         if sel is not None:
             i = sel[1]  # grab off row iter
             bib = self.riders.get_value(i, COL_BIB)
             series = self.riders.get_value(i, COL_SERIES)
             self.dnfriders(strops.bibser2bibstr(bib, series), 'dns')
 
-    def tod_context_dnf_activate_cb(self, menuitem, data=None):
+    def rider_context_dnf_activate_cb(self, menuitem, data=None):
         """Register rider as non-finisher."""
         sel = self.view.get_selection().get_selected()
         if sel is not None:
             i = sel[1]  # grab off row iter
             bib = self.riders.get_value(i, COL_BIB)
             series = self.riders.get_value(i, COL_SERIES)
             self.dnfriders(strops.bibser2bibstr(bib, series), 'dnf')
 
-    def tod_context_dsq_activate_cb(self, menuitem, data=None):
+    def rider_context_dsq_activate_cb(self, menuitem, data=None):
         """Disqualify rider."""
         sel = self.view.get_selection().get_selected()
         if sel is not None:
             i = sel[1]  # grab off row iter
             bib = self.riders.get_value(i, COL_BIB)
             series = self.riders.get_value(i, COL_SERIES)
             self.dnfriders(strops.bibser2bibstr(bib, series), 'dsq')
 
-    def tod_context_rel_activate_cb(self, menuitem, data=None):
+    def rider_context_rel_activate_cb(self, menuitem, data=None):
         """Relegate rider."""
         _log.info('Relegate not implemented for time trial.')
         pass
 
-    def tod_context_ntr_activate_cb(self, menuitem, data=None):
+    def rider_context_ntr_activate_cb(self, menuitem, data=None):
         """Register no time recorded for rider and place last."""
         sel = self.view.get_selection().get_selected()
         if sel is not None:
             i = sel[1]  # grab off row iter
             bib = self.riders.get_value(i, COL_BIB)
             series = self.riders.get_value(i, COL_SERIES)
             self.dnfriders(strops.bibser2bibstr(bib, series), 'ntr')
 
-    def tod_context_clear_activate_cb(self, menuitem, data=None):
+    def rider_context_clear_activate_cb(self, menuitem, data=None):
         """Clear times for selected rider."""
         sel = self.view.get_selection().get_selected()
         if sel is not None:
             self.riders.set_value(sel[1], COL_COMMENT, '')
             self.riders.set_value(sel[1], COL_PASS, 0)
             self.settimes(sel[1])  # clear iter to empty vals
             self.log_clear(self.riders.get_value(sel[1], COL_BIB),
                            self.riders.get_value(sel[1], COL_SERIES))
 
     def now_button_clicked_cb(self, button, entry=None):
         """Set specified entry to the current time."""
         if entry is not None:
             entry.set_text(tod.now().timestr())
 
-    def tod_context_edit_activate_cb(self, menuitem, data=None):
+    def rider_context_edit_activate_cb(self, menuitem, data=None):
         """Edit rider start/finish/etc."""
         sel = self.view.get_selection().get_selected()
         if sel is None:
             return False
 
         lr = Gtk.TreeModelRow(self.riders, sel[1])
         bibstr = strops.bibser2bibstr(lr[COL_BIB], lr[COL_SERIES])
@@ -2686,16 +2676,16 @@
             self.settimes(lr.iter,
                           tst=lr[COL_TODSTART],
                           tft=lr[COL_TODFINISH],
                           pt=lr[COL_TODPENALTY])
         if changed:
             self.recalculate()
 
-    def tod_context_del_activate_cb(self, menuitem, data=None):
-        """Delete selected row from race model."""
+    def rider_context_del_activate_cb(self, menuitem, data=None):
+        """Delete selected row from event model."""
         sel = self.view.get_selection().get_selected()
         if sel is not None:
             i = sel[1]  # grab off row iter
             bib = self.riders.get_value(i, COL_BIB)
             series = self.riders.get_value(i, COL_SERIES)
             self.settimes(i)  # clear times
             if self.riders.remove(i):
@@ -2741,15 +2731,15 @@
         self.clubmode = False
         self.allowspares = False
         self.minlap = STARTFUDGE
         self.arrivaltimeout = ARRIVALTIMEOUT
         self.timelimit = None
         self.gapthresh = GAPTHRESH
 
-        # race run time attributes
+        # event run time attributes
         self.live_announce = False
         self.curlap = -1
         self.onlap = 1
         self.lapstart = None
         self.lapfin = None
         self.onestart = False
         self.winopen = True
@@ -2822,36 +2812,37 @@
             object,  # eta 21
             int,  # pass count 22
             int,  # distance 23
             str,  # series 24
         )
 
         b = uiutil.builder('irtt.ui')
-        self.frame = b.get_object('race_vbox')
+        self.frame = b.get_object('event_vbox')
         self.frame.connect('destroy', self.shutdown)
 
         # meta info pane
         self.title_namestr = b.get_object('title_namestr')
         self.set_titlestr()
 
         # Timer Panes
-        mf = b.get_object('race_timer_pane')
+        mf = b.get_object('event_timer_pane')
         self.sl = uiutil.timerpane('Start Line', doser=True)
         self.sl.disable()
         self.sl.bibent.connect('activate', self.bibent_cb, self.sl)
         self.sl.serent.connect('activate', self.bibent_cb, self.sl)
         self.fl = uiutil.timerpane('Finish Line', doser=True)
         self.fl.disable()
         self.fl.bibent.connect('activate', self.bibent_cb, self.fl)
         self.fl.serent.connect('activate', self.bibent_cb, self.fl)
         self.fl.tment.connect('activate', self.tment_cb, self.fl)
         mf.pack_start(self.sl.frame, True, True, 0)
         mf.pack_start(self.fl.frame, True, True, 0)
         mf.set_focus_chain([self.sl.frame, self.fl.frame, self.sl.frame])
         self.timerframe = mf
+        self.timericon = b.get_object('info_time_icon')
         self.lapentry = Gtk.Label()
         self.totlapentry = Gtk.Label()
 
         # Result Pane
         t = Gtk.TreeView(self.riders)
         self.view = t
         t.set_reorderable(True)
@@ -2871,17 +2862,14 @@
             uiutil.mkviewcoltod(t,
                                 'Start',
                                 cb=self.startstr,
                                 editcb=self.editstart)
             uiutil.mkviewcoltod(t, 'Time', cb=self.elapstr)
             uiutil.mkviewcoltxt(t, 'Rank', COL_PLACE, halign=0.5, calign=0.5)
             t.show()
-            b.get_object('race_result_win').add(t)
-            b.connect_signals(self)
-
-            b = uiutil.builder('tod_context.ui')
-            self.context_menu = b.get_object('tod_context')
+            b.get_object('event_result_win').add(t)
+            self.context_menu = b.get_object('rider_context')
             b.connect_signals(self)
 
             # connect timer callback functions
             self.meet.timercb = self.timertrig  # transponders
             self.meet.alttimercb = self.alttimertrig  # chronometer
```

### Comparing `metarace-roadmeet-1.13.2/src/roadmeet/rms.py` & `metarace-roadmeet-1.13.3/src/roadmeet/rms.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 
 # basic infos
 COL_BIB = 0
 COL_NAMESTR = 1
 COL_SHORTNAME = 2
 COL_CAT = 3
 COL_COMMENT = 4
-COL_INRACE = 5  # boolean in the race
+COL_INRACE = 5  # boolean in the event
 COL_PLACE = 6  # Place assigned in result
-COL_LAPS = 7  # Incremented if inrace and not finished
+COL_LAPS = 7  # Incremented if COL_INRACE and not finished
 COL_SEED = 8  # Seeding number (overrides startlist ordering)
 
 # timing infos
 COL_RFTIME = 9  # one-off finish time by rfid
 COL_CBUNCH = 10  # computed bunch time   -> derived from rftime
 COL_MBUNCH = 11  # manual bunch time     -> manual overrive
 COL_STOFT = 12  # start time 'offset' - only reported in result
@@ -81,18 +81,25 @@
     'wd': 'Withdraw',
     'dsq': 'Disqualify',
     'add': 'Add starters',
     'del': 'Remove starters',
     'que': 'Query riders',
     'fin': 'Final places',
     'dec': 'Add decision',
-    'ret': 'Return to race',
+    'ret': 'Return to event',
     'man': 'Manual passing',
     '': '',
 }
+_DNFLABELS = {
+    'did not start': 'dns',
+    'did not finish': 'dnf',
+    'withdrawn': 'wd',
+    'outside time limit': 'otl',
+    'disqualify': 'dsq',
+}
 
 RESERVED_SOURCES = [
     'fin',  # finished stage
     'reg',  # registered to stage
     'start',  # started stage
 ]
 
@@ -578,15 +585,15 @@
         """Return a list of all rider numbers registered to event."""
         ret = []
         for r in self.riders:
             ret.append(r[COL_BIB])
         return ' '.join(ret)
 
     def get_starters(self):
-        """Return a list of riders that 'started' the race."""
+        """Return a list of riders that 'started' the event."""
         ret = []
         for r in self.riders:
             if r[COL_COMMENT] != 'dns' or r[COL_INRACE]:
                 ret.append(r[COL_BIB])
         return ' '.join(ret)
 
     def get_catlist(self):
@@ -725,28 +732,28 @@
         self.frame.show()
 
     def hide(self):
         """Hide event container."""
         self.frame.hide()
 
     def title_close_clicked_cb(self, button, entry=None):
-        """Close and save the race."""
+        """Close and save the event."""
         self.meet.close_event()
 
     def set_titlestr(self, titlestr=None):
         """Update the title string label."""
         if titlestr is None or titlestr == '':
             if self.etype in ROADRACE_TYPES:
                 titlestr = '[' + ROADRACE_TYPES[self.etype] + ']'
             else:
                 titlestr = '[Road Event]'
         self.title_namestr.set_text(titlestr)
 
     def destroy(self):
-        """Emit destroy signal to race handler."""
+        """Emit destroy signal to event handler."""
         if self.context_menu is not None:
             self.context_menu.destroy()
         self.frame.destroy()
 
     def points_report(self):
         """Return the points tally report."""
         ret = []
@@ -1221,15 +1228,15 @@
             if len(sec.lines) > 0:
                 ret.append(sec)
         else:
             _log.warning('Event is idle, report not available')
         return ret
 
     def catresult_report(self):
-        """Return a categorised race result report."""
+        """Return a categorised event result report."""
         _log.debug('Categorised result report')
         ret = []
         for cat in self.cats:
             ret.extend(self.single_catresult(cat))
 
         return ret
 
@@ -1722,15 +1729,15 @@
                 bt = self.vbunch(r[COL_CBUNCH], r[COL_MBUNCH])
                 if bt is not None:
                     timed = True
                     fincount += 1  # for accounting, use bunch time
                     if wt is None:  # first finish time
                         wt = bt
                         first = False
-                        # for hcap, first time is always race time
+                        # for hcap, first time is always event time
                         dstr = wt.rawtime(0)
                     else:
                         # for handicap, time gap is always
                         # down on winner's uncorrected time
                         if self.showdowntimes:
                             down = bt - wt
                             if down < MAXELAP:
@@ -1858,29 +1865,29 @@
         elif acode in self.intermeds:
             if entry is not None:
                 entry.set_text(self.intermap[acode]['places'])
         else:
             if entry is not None:
                 entry.set_text('')
 
-    def race_ctrl_add(self, rlist):
+    def event_ctrl_add(self, rlist):
         """Add the supplied riders to event model with lookup"""
         rlist = strops.riderlist_split(rlist, self.meet.rdb, self.series)
         for bib in rlist:
             self.addrider(bib)
         return True
 
-    def race_ctrl_del(self, rlist):
+    def event_ctrl_del(self, rlist):
         """Delete nominated riders from event model"""
         rlist = strops.riderlist_split(rlist, self.meet.rdb, self.series)
         for bib in rlist:
             self.delrider(bib)
         return True
 
-    def race_ctrl(self, acode='', rlist=''):
+    def event_ctrl(self, acode='', rlist=''):
         """Apply the selected action to the provided bib list."""
         if acode in self.intermeds:
             if acode == 'brk':
                 rlist = ' '.join(strops.riderlist_split(rlist))
                 self.intsprint(acode, rlist)
             else:
                 rlist = strops.reformat_placelist(rlist)
@@ -1921,17 +1928,17 @@
             self.retriders(strops.reformat_biblist(rlist))
             return True
         elif acode == 'man':
             # crude hack tool for now
             self.manpassing(strops.reformat_bibserlist(rlist))
             return True
         elif acode == 'del':
-            return self.race_ctrl_del(rlist)
+            return self.event_ctrl_del(rlist)
         elif acode == 'add':
-            return self.race_ctrl_add(rlist)
+            return self.event_ctrl_add(rlist)
         elif acode == 'que':
             rlist = strops.reformat_biblist(rlist)
             if rlist != '':
                 for bib in rlist.split():
                     self.query_rider(bib)
             return True
         elif acode == 'dec':
@@ -2051,15 +2058,15 @@
     def result_gen(self, cat=''):
         """Create and return result list with rows:
 
            ( rank, bib, time, bonus, penalty )
 
         Notes: 
 
-           - Handicap race type includes start offset in bonus time
+           - Handicap event type includes start offset in bonus time
            - Cross type adjusts time to include cat leader's average
              lap time and time down at finish
         """
         self.recalculate()
         mcat = self.ridercat(cat)
         rcount = 0
         lrank = None
@@ -2156,15 +2163,15 @@
         return ret
 
     def clear_results(self):
         """Clear all data from event model."""
         self.resetplaces()
         self.places = ''
         _log.debug('Clear event result')
-        # scan riders to clear any race info
+        # scan riders to clear any event info
         for r in self.riders:
             r[COL_COMMENT] = ''
             r[COL_INRACE] = True
             r[COL_PLACE] = ''
             r[COL_LAPS] = 0
             r[COL_RFSEEN] = []
             r[COL_RFTIME] = None
@@ -2396,24 +2403,15 @@
         return False
 
     def key_event(self, widget, event):
         """Handle global key presses in event."""
         if event.type == Gdk.EventType.KEY_PRESS:
             key = Gdk.keyval_name(event.keyval) or 'None'
             if event.state & Gdk.ModifierType.CONTROL_MASK:
-                if key == key_abort:  # override ctrl+f5
-                    if uiutil.questiondlg(
-                            window=self.meet.window,
-                            question='Reset event to idle?',
-                            subtext=
-                            'Note: All result and timing data will be cleared.',
-                            title='Reset Event?'):
-                        self.resettimer()
-                    return True
-                elif key == key_announce:  # re-send current announce vars
+                if key == key_announce:  # re-send current announce vars
                     self.reannounce_times()
                     return True
                 elif key == key_clearfrom:  # clear all places from selected
                     self.clear_places_from_selection()
                     return True
                 elif key == key_clearplace:  # clear selected rider from places
                     self.clear_selected_place()
@@ -2793,15 +2791,15 @@
                           e.rawtime(2), e.source)
                 return False
 
         # log passing of rider before further processing
         if not lr[COL_INRACE]:
             _log.warning('Withdrawn rider: %s:%s@%s/%s', bib, e.chan,
                          e.rawtime(2), e.source)
-            # but continue as if still in race
+            # but continue as if still in event
         else:
             _log.info('Saw: %s:%s@%s/%s', bib, e.chan, e.rawtime(2), e.source)
 
         # check run state
         if self.timerstat in ('idle', 'armstart', 'finished'):
             return False
 
@@ -2865,15 +2863,15 @@
             else:
                 targetlap = self.totlaps
             if targetlap and lr[COL_LAPS] >= targetlap - 1:
                 lapfinish = True  # arm just this rider
                 if self.etype == 'cross':
                     doarm = True
 
-        # for cross races when targets apply, armfinish is set automatically
+        # for cross events when targets apply, armfinish is set automatically
         if doarm and lapfinish and self.timerstat != 'armfinish':
             self.armfinish()
 
         # finishing rider path
         if self.timerstat == 'armfinish' or lapfinish:
             if self.finish is None:  # implies lr[COL_RFTIME] is None
                 # in case finish is being triggered by a lap target,
@@ -2909,15 +2907,15 @@
                           e.rawtime(2), e.source)
         # end finishing rider path
 
         # lapping rider path
         elif self.timerstat == 'running':
             self._dorecalc = True
             if lr[COL_INRACE] and (lr[COL_PLACE] or lr[COL_CBUNCH] is None):
-                # rider in the race, not yet finished: increment own lap count
+                # rider in the event, not yet finished: increment own lap count
                 lr[COL_LAPS] += 1
                 onlap = False
 
                 # category and target lap counting
                 if self.autofinish:
                     catlap = 0
                     if rcat in self.catonlap:
@@ -3584,15 +3582,15 @@
 
     def showbunch_cb(self, col, cr, model, iter, data=None):
         """Update bunch time on rider view."""
         cb = model.get_value(iter, COL_CBUNCH)
         mb = model.get_value(iter, COL_MBUNCH)
         if mb is not None:
             cr.set_property('text', mb.rawtime(0))
-            cr.set_property('style', uiutil.STYLE_OBLIQUE)
+            cr.set_property('style', uiutil.STYLE_ITALIC)
         else:
             cr.set_property('style', uiutil.STYLE_NORMAL)
             if cb is not None:
                 cr.set_property('text', cb.rawtime(0))
             else:
                 # display last lap time
                 seen = model.get_value(iter, COL_RFSEEN)
@@ -3605,15 +3603,15 @@
                         #et = seen[-1] - seen[-2]
                         #else:
                         # show elapsed
                         et = seen[-1] - self.start
                     else:
                         et = seen[-1]
                     cr.set_property('text', '[' + et.rawtime(1) + ']')
-                    cr.set_property('style', uiutil.STYLE_OBLIQUE)
+                    cr.set_property('style', uiutil.STYLE_ITALIC)
                 else:
                     cr.set_property('text', '')
 
     def editstart_cb(self, cell, path, new_text, col=None):
         """Edit start time on rider view."""
         newst = tod.mktod(new_text)
         if newst:
@@ -3763,15 +3761,15 @@
                 placeset.add(no)
                 # rider in the model?
                 lr = self.getrider(no)
                 if lr is None:
                     _log.error('Non-starter in places: %r', no)
                     ret = False
                 else:
-                    # rider still in the race?
+                    # rider still in the event?
                     if not lr[COL_INRACE]:
                         _log.info('DNF/DNS rider in places: %r', no)
                         if dnf:
                             ret = False
             else:
                 # placeholder needs to be filled in later or left off
                 _log.info('Placeholder in places')
@@ -4064,15 +4062,15 @@
                         # establish elapsed, but allow subsequent override
                         if rtime > self.maxfinish:
                             self.maxfinish = rtime
                         et = rtime - self.start
 
                         # establish bunch time
                         if ft is None and r[COL_RFTIME] is not None:
-                            racefinish = r[COL_RFTIME]  # save race finish
+                            racefinish = r[COL_RFTIME]  # save event finish
                             ft = et.truncate(0)  # compute first time
                             bt = ft
                         else:
                             if lt is not None and (
                                     rtime < lt or rtime - lt < self.gapthresh):
                                 # same time
                                 pass
@@ -4590,30 +4588,30 @@
         bib = None
         if sel is not None:
             i = sel[1]
             selbib = self.riders.get_value(i, COL_BIB)
             if change == 'delete':
                 _log.info('Delete rider: %r', selbib)
                 self.delrider(selbib)
-            elif change == 'clear':
+            elif change == 'clear finish':
                 _log.info('Clear rider %r finish time', selbib)
                 self.riders.set_value(i, COL_RFTIME, None)
                 self.riders.set_value(i, COL_MBUNCH, None)
                 self.recalculate()
             elif change == 'refinish':
                 splits = self.riders.get_value(i, COL_RFSEEN)
                 if splits is not None and len(splits) > 0:
                     nf = splits[-1]
                     _log.info(
                         'Set raw finish for rider %r to last passing: %s',
                         selbib, nf.rawtime(2))
                     self.riders.set_value(i, COL_RFTIME, nf)
                     self.recalculate()
-            elif change in ('dns', 'dnf', 'wd', 'otl', 'dsq'):
-                self.dnfriders(selbib, change)
+            elif change in _DNFLABELS:
+                self.dnfriders(selbib, _DNFLABELS[change])
             elif change == 'return':
                 self.retriders(selbib)
             elif change == 'passing':
                 self.manpassing(selbib)
             else:
                 _log.info('Unknown rider change %r ignored', change)
 
@@ -4708,15 +4706,15 @@
             object,  # gobject.TYPE_PYOBJECT,  # STOFT = 12
             object,  # gobject.TYPE_PYOBJECT,  # BONUS = 13
             object,  # gobject.TYPE_PYOBJECT,  # PENALTY = 14
             object,  # gobject.TYPE_PYOBJECT  # RFSEEN = 15
         )
 
         b = uiutil.builder('rms.ui')
-        self.frame = b.get_object('race_vbox')
+        self.frame = b.get_object('event_vbox')
 
         # meta info pane
         self.shortname = None
         self.title_namestr = b.get_object('title_namestr')
         self.set_titlestr()
         self.elaplbl = b.get_object('time_lbl')
         self.lapentry = b.get_object('lapentry')
@@ -4758,16 +4756,13 @@
             uiutil.mkviewcoltod(t,
                                 'Time',
                                 cb=self.showbunch_cb,
                                 editcb=self.editbunch_cb,
                                 width=50)
             uiutil.mkviewcoltxt(t, 'Place', COL_PLACE, calign=0.5, width=50)
             t.show()
-            b.get_object('race_result_win').add(t)
-            b.connect_signals(self)
-
-            b = uiutil.builder('rms_context.ui')
+            b.get_object('event_result_win').add(t)
             self.context_menu = b.get_object('rms_context')
             self.view.connect('button_press_event', self.treeview_button_press)
             b.connect_signals(self)
             self.meet.timercb = self.timertrig
             self.meet.alttimercb = self.alttimertrig
```

### Comparing `metarace-roadmeet-1.13.2/src/roadmeet/trtt.py` & `metarace-roadmeet-1.13.3/src/roadmeet/trtt.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 # trtt adds team reference to rms model
 # basic infos
 COL_BIB = 0
 COL_NAMESTR = 1
 COL_SHORTNAME = 2
 COL_CAT = 3
 COL_COMMENT = 4
-COL_INRACE = 5  # boolean in the race
+COL_INRACE = 5  # boolean in the event
 COL_PLACE = 6  # Place assigned in result
-COL_LAPS = 7  # Incremented if inrace and not finished
+COL_LAPS = 7  # Incremented if COL_INRACE and not finished
 COL_SEED = 8  # Seeding number (overrides startlist ordering)
 
 # timing infos
 COL_RFTIME = 9  # one-off finish time by rfid
 COL_CBUNCH = 10  # computed bunch time   -> derived from rftime
 COL_MBUNCH = 11  # manual bunch time     -> manual overrive
 COL_STOFT = 12  # start time 'offset' - only reported in result
@@ -564,15 +564,15 @@
 
     def reorder_arrivals(self):
         """Re-order the rider list according to arrival at finish line"""
         self.calcset = False
         aux = []
         cnt = 0
         for r in self.riders:
-            # in the race?
+            # in the event?
             inField = True
             if not r[COL_INRACE]:
                 inField = False
 
             comStr = r[COL_COMMENT]
             if r[COL_PLACE]:
                 comStr = r[COL_PLACE]
@@ -951,15 +951,15 @@
                 cv.append(catname)
                 rsec.heading = ': '.join(cv)
                 rsec.subheading = subhead
             ret.append(report.pagebreak())
         return ret
 
     def result_report(self):
-        """Return a race result report"""
+        """Return event result report"""
         ret = []
         self.recalculate()
 
         # always use cat result for trtt
         ret = self.catresult_report()
 
         # show all intermediates here
@@ -969,23 +969,23 @@
                 ret.extend(self.int_report(i))
 
         # append a decisions section
         ret.append(self.decision_section())
 
         return ret
 
-    def race_ctrl_add(self, rlist):
+    def event_ctrl_add(self, rlist):
         """Add the supplied riders to event model with lookup"""
         rlist = strops.riderlist_split(rlist, self.meet.rdb, self.series)
         for bib in rlist:
             self.addrider(bib)
         self.team_start_times()
         return True
 
-    def race_ctrl_del(self, rlist):
+    def event_ctrl_del(self, rlist):
         """Delete nominated riders from event model"""
         rlist = strops.riderlist_split(rlist, self.meet.rdb, self.series)
         for bib in rlist:
             self.delrider(bib)
         self.team_start_times()
         return True
 
@@ -1124,15 +1124,15 @@
 
     def updateteam(self, team=None):
         """Handle a change in team data"""
         # assume the worst and recalc all riders
         self.team_start_times()
 
     def resettimer(self):
-        """Reset race timer."""
+        """Reset event timer."""
         _log.info('Reset event to idle')
         self.set_start()
         self.clear_results()
         self.teamtimes = {}
         self.timerstat = 'idle'
         self.meet.cmd_announce('timerstat', 'idle')
         self.meet.stat_but.update('idle', 'Idle')
@@ -1223,15 +1223,15 @@
                           e.rawtime(2), e.source)
         # end finishing rider path
 
         # lapping rider path
         elif self.timerstat == 'running':
             self._dorecalc = True
             if lr[COL_INRACE] and (lr[COL_PLACE] or lr[COL_CBUNCH] is None):
-                # rider in the race, not yet finished: increment own lap count
+                # rider in event, not yet finished: increment own lap count
                 lr[COL_LAPS] += 1
 
                 # announce all rider passings
                 self.announce_rider('', bib, lr[COL_NAMESTR], lr[COL_CAT], e)
         return False
 
     def finsprint(self, places):
@@ -1568,15 +1568,15 @@
             object,  # gobject.TYPE_PYOBJECT,  # BONUS = 13
             object,  # gobject.TYPE_PYOBJECT,  # PENALTY = 14
             object,  # gobject.TYPE_PYOBJECT,  # RFSEEN = 15
             str,  # gobject.TYPE_STRING)  # TEAM = 16
         )
 
         b = uiutil.builder('rms.ui')
-        self.frame = b.get_object('race_vbox')
+        self.frame = b.get_object('event_vbox')
         self.frame.connect('destroy', self.shutdown)
 
         # meta info pane
         self.shortname = None
         self.title_namestr = b.get_object('title_namestr')
         self.set_titlestr()
         self.elaplbl = b.get_object('time_lbl')
@@ -1614,16 +1614,13 @@
             uiutil.mkviewcoltod(t,
                                 'Time',
                                 cb=self.showbunch_cb,
                                 editcb=self.editbunch_cb,
                                 width=50)
             uiutil.mkviewcoltxt(t, 'Arvl', COL_PLACE, calign=0.5, width=50)
             t.show()
-            b.get_object('race_result_win').add(t)
-            b.connect_signals(self)
-
-            b = uiutil.builder('rms_context.ui')
+            b.get_object('event_result_win').add(t)
             self.context_menu = b.get_object('rms_context')
-            self.view.connect('button_press_event', self.treeview_button_press)
             b.connect_signals(self)
+            self.view.connect('button_press_event', self.treeview_button_press)
             self.meet.timercb = self.timertrig
             self.meet.alttimercb = self.alttimertrig
```

### Comparing `metarace-roadmeet-1.13.2/src/roadmeet/ui/new_start.ui` & `metarace-roadmeet-1.13.3/src/roadmeet/ui/new_start.ui`

 * *Files identical despite different names*

### Comparing `metarace-roadmeet-1.13.2/src/roadmeet/ui/roadmeet.ui` & `metarace-roadmeet-1.13.3/src/roadmeet/ui/roadmeet.ui`

 * *Files 18% similar despite different names*

```diff
@@ -1,2638 +1,2235 @@
-00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
-00000010: 2e30 223f 3e0a 3c69 6e74 6572 6661 6365  .0"?>.<interface
-00000020: 3e0a 2020 3c72 6571 7569 7265 7320 6c69  >.  <requires li
-00000030: 623d 2267 746b 2b22 2076 6572 7369 6f6e  b="gtk+" version
-00000040: 3d22 322e 3136 222f 3e0a 2020 3c21 2d2d  ="2.16"/>.  <!--
-00000050: 2069 6e74 6572 6661 6365 2d6e 616d 696e   interface-namin
-00000060: 672d 706f 6c69 6379 2070 726f 6a65 6374  g-policy project
-00000070: 2d77 6964 6520 2d2d 3e0a 2020 3c6f 626a  -wide -->.  <obj
-00000080: 6563 7420 636c 6173 733d 2247 746b 5769  ect class="GtkWi
-00000090: 6e64 6f77 2220 6964 3d22 6d65 6574 223e  ndow" id="meet">
-000000a0: 0a20 2020 203c 7072 6f70 6572 7479 206e  .    <property n
-000000b0: 616d 653d 2274 6974 6c65 2220 7472 616e  ame="title" tran
-000000c0: 736c 6174 6162 6c65 3d22 7965 7322 3e4d  slatable="yes">M
-000000d0: 6574 6172 6163 653a 2052 6f61 6420 4d65  etarace: Road Me
-000000e0: 6574 3c2f 7072 6f70 6572 7479 3e0a 2020  et</property>.  
-000000f0: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00000100: 3d22 6465 6661 756c 745f 7769 6474 6822  ="default_width"
-00000110: 3e38 3030 3c2f 7072 6f70 6572 7479 3e0a  >800</property>.
-00000120: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00000130: 6d65 3d22 6465 6661 756c 745f 6865 6967  me="default_heig
-00000140: 6874 223e 3630 303c 2f70 726f 7065 7274  ht">600</propert
-00000150: 793e 0a20 2020 203c 7369 676e 616c 206e  y>.    <signal n
-00000160: 616d 653d 2264 6573 7472 6f79 2220 6861  ame="destroy" ha
-00000170: 6e64 6c65 723d 226d 6565 745f 6465 7374  ndler="meet_dest
-00000180: 726f 795f 6362 222f 3e0a 2020 2020 3c63  roy_cb"/>.    <c
-00000190: 6869 6c64 3e0a 2020 2020 2020 3c6f 626a  hild>.      <obj
-000001a0: 6563 7420 636c 6173 733d 2247 746b 5642  ect class="GtkVB
-000001b0: 6f78 2220 6964 3d22 6d65 6574 5f76 626f  ox" id="meet_vbo
-000001c0: 7822 3e0a 2020 2020 2020 2020 3c70 726f  x">.        <pro
-000001d0: 7065 7274 7920 6e61 6d65 3d22 7669 7369  perty name="visi
-000001e0: 626c 6522 3e54 7275 653c 2f70 726f 7065  ble">True</prope
-000001f0: 7274 793e 0a20 2020 2020 2020 203c 7072  rty>.        <pr
-00000200: 6f70 6572 7479 206e 616d 653d 226f 7269  operty name="ori
-00000210: 656e 7461 7469 6f6e 223e 7665 7274 6963  entation">vertic
-00000220: 616c 3c2f 7072 6f70 6572 7479 3e0a 2020  al</property>.  
-00000230: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
-00000240: 6e61 6d65 3d22 7370 6163 696e 6722 3e35  name="spacing">5
-00000250: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-00000260: 2020 2020 3c63 6869 6c64 3e0a 2020 2020      <child>.    
-00000270: 2020 2020 2020 3c6f 626a 6563 7420 636c        <object cl
-00000280: 6173 733d 2247 746b 4842 6f78 2220 6964  ass="GtkHBox" id
-00000290: 3d22 746f 705f 626f 7822 3e0a 2020 2020  ="top_box">.    
-000002a0: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-000002b0: 7920 6e61 6d65 3d22 7669 7369 626c 6522  y name="visible"
-000002c0: 3e54 7275 653c 2f70 726f 7065 7274 793e  >True</property>
-000002d0: 0a20 2020 2020 2020 2020 2020 203c 7072  .            <pr
-000002e0: 6f70 6572 7479 206e 616d 653d 2273 7061  operty name="spa
-000002f0: 6369 6e67 223e 313c 2f70 726f 7065 7274  cing">1</propert
+00000000: 3c21 2d2d 2072 6f61 646d 6565 7420 6170  <!-- roadmeet ap
+00000010: 706c 6963 6174 696f 6e20 7569 202d 2d3e  plication ui -->
+00000020: 0a3c 696e 7465 7266 6163 653e 0a20 203c  .<interface>.  <
+00000030: 7265 7175 6972 6573 206c 6962 3d22 6774  requires lib="gt
+00000040: 6b2b 2220 7665 7273 696f 6e3d 2233 2e30  k+" version="3.0
+00000050: 222f 3e0a 0a20 203c 212d 2d20 6d65 6574  "/>..  <!-- meet
+00000060: 206d 6169 6e20 7769 6e64 6f77 202d 2d3e   main window -->
+00000070: 0a20 203c 6f62 6a65 6374 2063 6c61 7373  .  <object class
+00000080: 3d22 4774 6b57 696e 646f 7722 2069 643d  ="GtkWindow" id=
+00000090: 226d 6565 7422 3e0a 2020 2020 3c70 726f  "meet">.    <pro
+000000a0: 7065 7274 7920 6e61 6d65 3d22 7469 746c  perty name="titl
+000000b0: 6522 3e52 6f61 6420 4d65 6574 3c2f 7072  e">Road Meet</pr
+000000c0: 6f70 6572 7479 3e0a 2020 2020 3c70 726f  operty>.    <pro
+000000d0: 7065 7274 7920 6e61 6d65 3d22 6465 6661  perty name="defa
+000000e0: 756c 745f 7769 6474 6822 3e38 3030 3c2f  ult_width">800</
+000000f0: 7072 6f70 6572 7479 3e0a 2020 2020 3c70  property>.    <p
+00000100: 726f 7065 7274 7920 6e61 6d65 3d22 6465  roperty name="de
+00000110: 6661 756c 745f 6865 6967 6874 223e 3630  fault_height">60
+00000120: 303c 2f70 726f 7065 7274 793e 0a20 2020  0</property>.   
+00000130: 203c 7369 676e 616c 206e 616d 653d 2264   <signal name="d
+00000140: 6573 7472 6f79 2220 6861 6e64 6c65 723d  estroy" handler=
+00000150: 226d 6565 745f 6465 7374 726f 795f 6362  "meet_destroy_cb
+00000160: 222f 3e0a 2020 2020 3c63 6869 6c64 3e0a  "/>.    <child>.
+00000170: 2020 2020 2020 3c6f 626a 6563 7420 636c        <object cl
+00000180: 6173 733d 2247 746b 426f 7822 2069 643d  ass="GtkBox" id=
+00000190: 226d 6565 745f 7662 6f78 223e 0a20 2020  "meet_vbox">.   
+000001a0: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+000001b0: 616d 653d 226f 7269 656e 7461 7469 6f6e  ame="orientation
+000001c0: 223e 7665 7274 6963 616c 3c2f 7072 6f70  ">vertical</prop
+000001d0: 6572 7479 3e0a 2020 2020 2020 2020 3c70  erty>.        <p
+000001e0: 726f 7065 7274 7920 6e61 6d65 3d22 7669  roperty name="vi
+000001f0: 7369 626c 6522 3e54 7275 653c 2f70 726f  sible">True</pro
+00000200: 7065 7274 793e 0a20 2020 2020 2020 203c  perty>.        <
+00000210: 7072 6f70 6572 7479 206e 616d 653d 2273  property name="s
+00000220: 7061 6369 6e67 223e 353c 2f70 726f 7065  pacing">5</prope
+00000230: 7274 793e 0a0a 2020 2020 2020 2020 3c21  rty>..        <!
+00000240: 2d2d 206d 656e 7520 6261 7220 2d2d 3e0a  -- menu bar -->.
+00000250: 2020 2020 2020 2020 3c63 6869 6c64 3e0a          <child>.
+00000260: 2020 2020 2020 2020 2020 3c6f 626a 6563            <objec
+00000270: 7420 636c 6173 733d 2247 746b 426f 7822  t class="GtkBox"
+00000280: 2069 643d 2274 6f70 5f62 6f78 223e 0a20   id="top_box">. 
+00000290: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
+000002a0: 6572 7479 206e 616d 653d 226f 7269 656e  erty name="orien
+000002b0: 7461 7469 6f6e 223e 686f 7269 7a6f 6e74  tation">horizont
+000002c0: 616c 3c2f 7072 6f70 6572 7479 3e0a 2020  al</property>.  
+000002d0: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
+000002e0: 7274 7920 6e61 6d65 3d22 7669 7369 626c  rty name="visibl
+000002f0: 6522 3e54 7275 653c 2f70 726f 7065 7274  e">True</propert
 00000300: 793e 0a20 2020 2020 2020 2020 2020 203c  y>.            <
-00000310: 6368 696c 643e 0a20 2020 2020 2020 2020  child>.         
-00000320: 2020 2020 203c 6f62 6a65 6374 2063 6c61       <object cla
-00000330: 7373 3d22 4774 6b4d 656e 7542 6172 2220  ss="GtkMenuBar" 
-00000340: 6964 3d22 6d65 6e75 5f62 6172 223e 0a20  id="menu_bar">. 
-00000350: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000360: 7072 6f70 6572 7479 206e 616d 653d 2276  property name="v
-00000370: 6973 6962 6c65 223e 5472 7565 3c2f 7072  isible">True</pr
-00000380: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
-00000390: 2020 2020 2020 2020 3c63 6869 6c64 3e0a          <child>.
-000003a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003b0: 2020 3c6f 626a 6563 7420 636c 6173 733d    <object class=
-000003c0: 2247 746b 4d65 6e75 4974 656d 2220 6964  "GtkMenuItem" id
-000003d0: 3d22 6d65 6e75 5f6d 6565 7422 3e0a 2020  ="menu_meet">.  
-000003e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003f0: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00000400: 3d22 7669 7369 626c 6522 3e54 7275 653c  ="visible">True<
-00000410: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
-00000420: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000430: 7072 6f70 6572 7479 206e 616d 653d 226c  property name="l
-00000440: 6162 656c 2220 7472 616e 736c 6174 6162  abel" translatab
-00000450: 6c65 3d22 7965 7322 3e5f 4d65 6574 3c2f  le="yes">_Meet</
-00000460: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
-00000470: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-00000480: 726f 7065 7274 7920 6e61 6d65 3d22 7573  roperty name="us
-00000490: 655f 756e 6465 726c 696e 6522 3e54 7275  e_underline">Tru
-000004a0: 653c 2f70 726f 7065 7274 793e 0a20 2020  e</property>.   
+00000310: 7072 6f70 6572 7479 206e 616d 653d 2273  property name="s
+00000320: 7061 6369 6e67 223e 313c 2f70 726f 7065  pacing">1</prope
+00000330: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
+00000340: 203c 6368 696c 643e 0a20 2020 2020 2020   <child>.       
+00000350: 2020 2020 2020 203c 6f62 6a65 6374 2063         <object c
+00000360: 6c61 7373 3d22 4774 6b4d 656e 7542 6172  lass="GtkMenuBar
+00000370: 2220 6964 3d22 6d65 6e75 5f62 6172 223e  " id="menu_bar">
+00000380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000390: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+000003a0: 2276 6973 6962 6c65 223e 5472 7565 3c2f  "visible">True</
+000003b0: 7072 6f70 6572 7479 3e0a 0a20 2020 2020  property>..     
+000003c0: 2020 2020 2020 2020 2020 203c 212d 2d20             <!-- 
+000003d0: 6d65 6574 206d 656e 7520 2d2d 3e0a 2020  meet menu -->.  
+000003e0: 2020 2020 2020 2020 2020 2020 2020 3c63                <c
+000003f0: 6869 6c64 3e0a 2020 2020 2020 2020 2020  hild>.          
+00000400: 2020 2020 2020 2020 3c6f 626a 6563 7420          <object 
+00000410: 636c 6173 733d 2247 746b 4d65 6e75 4974  class="GtkMenuIt
+00000420: 656d 2220 6964 3d22 6d65 6e75 5f6d 6565  em" id="menu_mee
+00000430: 7422 3e0a 2020 2020 2020 2020 2020 2020  t">.            
+00000440: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
+00000450: 7920 6e61 6d65 3d22 7669 7369 626c 6522  y name="visible"
+00000460: 3e54 7275 653c 2f70 726f 7065 7274 793e  >True</property>
+00000470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000480: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+00000490: 616d 653d 226c 6162 656c 223e 5f4d 6565  ame="label">_Mee
+000004a0: 743c 2f70 726f 7065 7274 793e 0a20 2020  t</property>.   
 000004b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000004c0: 203c 6368 696c 6420 7479 7065 3d22 7375   <child type="su
-000004d0: 626d 656e 7522 3e0a 2020 2020 2020 2020  bmenu">.        
-000004e0: 2020 2020 2020 2020 2020 2020 2020 3c6f                <o
-000004f0: 626a 6563 7420 636c 6173 733d 2247 746b  bject class="Gtk
-00000500: 4d65 6e75 2220 6964 3d22 6d65 6e75 3122  Menu" id="menu1"
-00000510: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000520: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00000530: 7274 7920 6e61 6d65 3d22 7669 7369 626c  rty name="visibl
-00000540: 6522 3e54 7275 653c 2f70 726f 7065 7274  e">True</propert
-00000550: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
-00000560: 2020 2020 2020 2020 2020 203c 6368 696c             <chil
-00000570: 643e 0a20 2020 2020 2020 2020 2020 2020  d>.             
-00000580: 2020 2020 2020 2020 2020 2020 203c 6f62               <ob
-00000590: 6a65 6374 2063 6c61 7373 3d22 4774 6b49  ject class="GtkI
-000005a0: 6d61 6765 4d65 6e75 4974 656d 2220 6964  mageMenuItem" id
-000005b0: 3d22 6d65 6e75 5f6d 6565 745f 7361 7665  ="menu_meet_save
-000005c0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-000005d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000005e0: 7072 6f70 6572 7479 206e 616d 653d 226c  property name="l
-000005f0: 6162 656c 223e 6774 6b2d 7361 7665 3c2f  abel">gtk-save</
-00000600: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
-00000610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000620: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
-00000630: 6e61 6d65 3d22 7669 7369 626c 6522 3e54  name="visible">T
-00000640: 7275 653c 2f70 726f 7065 7274 793e 0a20  rue</property>. 
+000004c0: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+000004d0: 2275 7365 5f75 6e64 6572 6c69 6e65 223e  "use_underline">
+000004e0: 5472 7565 3c2f 7072 6f70 6572 7479 3e0a  True</property>.
+000004f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000500: 2020 2020 3c63 6869 6c64 2074 7970 653d      <child type=
+00000510: 2273 7562 6d65 6e75 223e 0a20 2020 2020  "submenu">.     
+00000520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000530: 203c 6f62 6a65 6374 2063 6c61 7373 3d22   <object class="
+00000540: 4774 6b4d 656e 7522 2069 643d 226d 656e  GtkMenu" id="men
+00000550: 7531 223e 0a20 2020 2020 2020 2020 2020  u1">.           
+00000560: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
+00000570: 6f70 6572 7479 206e 616d 653d 2276 6973  operty name="vis
+00000580: 6962 6c65 223e 5472 7565 3c2f 7072 6f70  ible">True</prop
+00000590: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
+000005a0: 2020 2020 2020 2020 2020 2020 2020 3c63                <c
+000005b0: 6869 6c64 3e0a 2020 2020 2020 2020 2020  hild>.          
+000005c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005d0: 3c6f 626a 6563 7420 636c 6173 733d 2247  <object class="G
+000005e0: 746b 4d65 6e75 4974 656d 2220 6964 3d22  tkMenuItem" id="
+000005f0: 6d65 6e75 5f6d 6565 745f 7361 7665 223e  menu_meet_save">
+00000600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000610: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
+00000620: 6f70 6572 7479 206e 616d 653d 226c 6162  operty name="lab
+00000630: 656c 223e 5f53 6176 653c 2f70 726f 7065  el">_Save</prope
+00000640: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
 00000650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000660: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
-00000670: 6572 7479 206e 616d 653d 2274 6f6f 6c74  erty name="toolt
-00000680: 6970 5f74 6578 7422 2074 7261 6e73 6c61  ip_text" transla
-00000690: 7461 626c 653d 2279 6573 223e 5361 7665  table="yes">Save
-000006a0: 2074 6865 2063 7572 7265 6e74 206d 6565   the current mee
-000006b0: 743c 2f70 726f 7065 7274 793e 0a20 2020  t</property>.   
-000006c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006d0: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-000006e0: 7479 206e 616d 653d 2275 7365 5f75 6e64  ty name="use_und
-000006f0: 6572 6c69 6e65 223e 5472 7565 3c2f 7072  erline">True</pr
-00000700: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
-00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000720: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00000730: 6d65 3d22 7573 655f 7374 6f63 6b22 3e54  me="use_stock">T
-00000740: 7275 653c 2f70 726f 7065 7274 793e 0a20  rue</property>. 
-00000750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000760: 2020 2020 2020 2020 2020 203c 6163 6365             <acce
-00000770: 6c65 7261 746f 7220 6b65 793d 2273 2220  lerator key="s" 
-00000780: 7369 676e 616c 3d22 6163 7469 7661 7465  signal="activate
-00000790: 2220 6d6f 6469 6669 6572 733d 2247 444b  " modifiers="GDK
-000007a0: 5f43 4f4e 5452 4f4c 5f4d 4153 4b22 2f3e  _CONTROL_MASK"/>
-000007b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000007c0: 2020 2020 2020 2020 2020 2020 203c 7369               <si
-000007d0: 676e 616c 206e 616d 653d 2261 6374 6976  gnal name="activ
-000007e0: 6174 6522 2068 616e 646c 6572 3d22 6d65  ate" handler="me
-000007f0: 6e75 5f6d 6565 745f 7361 7665 5f63 6222  nu_meet_save_cb"
-00000800: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00000810: 2020 2020 2020 2020 2020 2020 203c 2f6f               </o
-00000820: 626a 6563 743e 0a20 2020 2020 2020 2020  bject>.         
-00000830: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000840: 2f63 6869 6c64 3e0a 2020 2020 2020 2020  /child>.        
-00000850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000860: 3c63 6869 6c64 3e0a 2020 2020 2020 2020  <child>.        
-00000870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000880: 2020 3c6f 626a 6563 7420 636c 6173 733d    <object class=
-00000890: 2247 746b 5365 7061 7261 746f 724d 656e  "GtkSeparatorMen
-000008a0: 7549 7465 6d22 2069 643d 226d 656e 755f  uItem" id="menu_
-000008b0: 6d65 6574 5f73 6570 3122 3e0a 2020 2020  meet_sep1">.    
-000008c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008d0: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-000008e0: 7920 6e61 6d65 3d22 7669 7369 626c 6522  y name="visible"
-000008f0: 3e54 7275 653c 2f70 726f 7065 7274 793e  >True</property>
-00000900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000910: 2020 2020 2020 2020 2020 203c 2f6f 626a             </obj
-00000920: 6563 743e 0a20 2020 2020 2020 2020 2020  ect>.           
-00000930: 2020 2020 2020 2020 2020 2020 203c 2f63               </c
-00000940: 6869 6c64 3e0a 2020 2020 2020 2020 2020  hild>.          
-00000950: 2020 2020 2020 2020 2020 2020 2020 3c63                <c
-00000960: 6869 6c64 3e0a 2020 2020 2020 2020 2020  hild>.          
-00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000980: 3c6f 626a 6563 7420 636c 6173 733d 2247  <object class="G
-00000990: 746b 496d 6167 654d 656e 7549 7465 6d22  tkImageMenuItem"
-000009a0: 2069 643d 226d 656e 755f 6d65 6574 5f70   id="menu_meet_p
-000009b0: 726f 7065 7274 6965 7322 3e0a 2020 2020  roperties">.    
-000009c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009d0: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-000009e0: 7920 6e61 6d65 3d22 6c61 6265 6c22 3e67  y name="label">g
-000009f0: 746b 2d70 726f 7065 7274 6965 733c 2f70  tk-properties</p
-00000a00: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
-00000a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a20: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00000a30: 616d 653d 2276 6973 6962 6c65 223e 5472  ame="visible">Tr
-00000a40: 7565 3c2f 7072 6f70 6572 7479 3e0a 2020  ue</property>.  
-00000a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a60: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00000a70: 7274 7920 6e61 6d65 3d22 746f 6f6c 7469  rty name="toolti
-00000a80: 705f 7465 7874 2220 7472 616e 736c 6174  p_text" translat
-00000a90: 6162 6c65 3d22 7965 7322 3e45 6469 7420  able="yes">Edit 
-00000aa0: 6d65 6574 2070 726f 7065 7274 6965 733c  meet properties<
-00000ab0: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
-00000ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ad0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00000ae0: 206e 616d 653d 2275 7365 5f73 746f 636b   name="use_stock
-00000af0: 223e 5472 7565 3c2f 7072 6f70 6572 7479  ">True</property
-00000b00: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000b10: 2020 2020 2020 2020 2020 2020 2020 3c61                <a
-00000b20: 6363 656c 6572 6174 6f72 206b 6579 3d22  ccelerator key="
-00000b30: 7022 2073 6967 6e61 6c3d 2261 6374 6976  p" signal="activ
-00000b40: 6174 6522 206d 6f64 6966 6965 7273 3d22  ate" modifiers="
-00000b50: 4744 4b5f 434f 4e54 524f 4c5f 4d41 534b  GDK_CONTROL_MASK
-00000b60: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00000b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b80: 3c73 6967 6e61 6c20 6e61 6d65 3d22 6163  <signal name="ac
-00000b90: 7469 7661 7465 2220 6861 6e64 6c65 723d  tivate" handler=
-00000ba0: 226d 656e 755f 6d65 6574 5f70 726f 7065  "menu_meet_prope
-00000bb0: 7274 6965 735f 6362 222f 3e0a 2020 2020  rties_cb"/>.    
-00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bd0: 2020 2020 2020 3c2f 6f62 6a65 6374 3e0a        </object>.
-00000be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bf0: 2020 2020 2020 2020 3c2f 6368 696c 643e          </child>
-00000c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c10: 2020 2020 2020 2020 203c 6368 696c 643e           <child>
-00000c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c30: 2020 2020 2020 2020 2020 203c 6f62 6a65             <obje
-00000c40: 6374 2063 6c61 7373 3d22 4774 6b53 6570  ct class="GtkSep
-00000c50: 6172 6174 6f72 4d65 6e75 4974 656d 2220  aratorMenuItem" 
-00000c60: 6964 3d22 6d65 6e75 5f6d 6565 745f 7365  id="menu_meet_se
-00000c70: 7072 223e 0a20 2020 2020 2020 2020 2020  pr">.           
-00000c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c90: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-00000ca0: 2276 6973 6962 6c65 223e 5472 7565 3c2f  "visible">True</
-00000cb0: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
+00000660: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00000670: 2276 6973 6962 6c65 223e 5472 7565 3c2f  "visible">True</
+00000680: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
+00000690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006a0: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+000006b0: 6e61 6d65 3d22 7573 655f 756e 6465 726c  name="use_underl
+000006c0: 696e 6522 3e54 7275 653c 2f70 726f 7065  ine">True</prope
+000006d0: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
+000006e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006f0: 203c 6163 6365 6c65 7261 746f 7220 6b65   <accelerator ke
+00000700: 793d 2273 2220 7369 676e 616c 3d22 6163  y="s" signal="ac
+00000710: 7469 7661 7465 2220 6d6f 6469 6669 6572  tivate" modifier
+00000720: 733d 2247 444b 5f43 4f4e 5452 4f4c 5f4d  s="GDK_CONTROL_M
+00000730: 4153 4b22 2f3e 0a20 2020 2020 2020 2020  ASK"/>.         
+00000740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000750: 2020 203c 7369 676e 616c 206e 616d 653d     <signal name=
+00000760: 2261 6374 6976 6174 6522 2068 616e 646c  "activate" handl
+00000770: 6572 3d22 6d65 6e75 5f6d 6565 745f 7361  er="menu_meet_sa
+00000780: 7665 5f63 6222 2f3e 0a20 2020 2020 2020  ve_cb"/>.       
+00000790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007a0: 2020 203c 2f6f 626a 6563 743e 0a20 2020     </object>.   
+000007b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007c0: 2020 2020 203c 2f63 6869 6c64 3e0a 2020       </child>.  
+000007d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007e0: 2020 2020 2020 3c63 6869 6c64 3e0a 2020        <child>.  
+000007f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000800: 2020 2020 2020 2020 3c6f 626a 6563 7420          <object 
+00000810: 636c 6173 733d 2247 746b 4d65 6e75 4974  class="GtkMenuIt
+00000820: 656d 2220 6964 3d22 6d65 6e75 5f6d 6565  em" id="menu_mee
+00000830: 745f 7072 6f70 6572 7469 6573 223e 0a20  t_properties">. 
+00000840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000850: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
+00000860: 6572 7479 206e 616d 653d 226c 6162 656c  erty name="label
+00000870: 223e 5f50 726f 7065 7274 6965 733c 2f70  ">_Properties</p
+00000880: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
+00000890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008a0: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+000008b0: 616d 653d 2276 6973 6962 6c65 223e 5472  ame="visible">Tr
+000008c0: 7565 3c2f 7072 6f70 6572 7479 3e0a 2020  ue</property>.  
+000008d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008e0: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
+000008f0: 7274 7920 6e61 6d65 3d22 7573 655f 756e  rty name="use_un
+00000900: 6465 726c 696e 6522 3e54 7275 653c 2f70  derline">True</p
+00000910: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
+00000920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000930: 2020 2020 203c 6163 6365 6c65 7261 746f       <accelerato
+00000940: 7220 6b65 793d 2270 2220 7369 676e 616c  r key="p" signal
+00000950: 3d22 6163 7469 7661 7465 2220 6d6f 6469  ="activate" modi
+00000960: 6669 6572 733d 2247 444b 5f43 4f4e 5452  fiers="GDK_CONTR
+00000970: 4f4c 5f4d 4153 4b22 2f3e 0a20 2020 2020  OL_MASK"/>.     
+00000980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000990: 2020 2020 2020 203c 7369 676e 616c 206e         <signal n
+000009a0: 616d 653d 2261 6374 6976 6174 6522 2068  ame="activate" h
+000009b0: 616e 646c 6572 3d22 6d65 6e75 5f6d 6565  andler="menu_mee
+000009c0: 745f 7072 6f70 6572 7469 6573 5f63 6222  t_properties_cb"
+000009d0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+000009e0: 2020 2020 2020 2020 2020 2020 203c 2f6f               </o
+000009f0: 626a 6563 743e 0a20 2020 2020 2020 2020  bject>.         
+00000a00: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000a10: 2f63 6869 6c64 3e0a 2020 2020 2020 2020  /child>.        
+00000a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a30: 3c63 6869 6c64 3e0a 2020 2020 2020 2020  <child>.        
+00000a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a50: 2020 3c6f 626a 6563 7420 636c 6173 733d    <object class=
+00000a60: 2247 746b 5365 7061 7261 746f 724d 656e  "GtkSeparatorMen
+00000a70: 7549 7465 6d22 2069 643d 226d 656e 755f  uItem" id="menu_
+00000a80: 6d65 6574 5f73 6570 7222 3e0a 2020 2020  meet_sepr">.    
+00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000aa0: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
+00000ab0: 7920 6e61 6d65 3d22 7669 7369 626c 6522  y name="visible"
+00000ac0: 3e54 7275 653c 2f70 726f 7065 7274 793e  >True</property>
+00000ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000ae0: 2020 2020 2020 2020 2020 203c 2f6f 626a             </obj
+00000af0: 6563 743e 0a20 2020 2020 2020 2020 2020  ect>.           
+00000b00: 2020 2020 2020 2020 2020 2020 203c 2f63               </c
+00000b10: 6869 6c64 3e0a 2020 2020 2020 2020 2020  hild>.          
+00000b20: 2020 2020 2020 2020 2020 2020 2020 3c63                <c
+00000b30: 6869 6c64 3e0a 2020 2020 2020 2020 2020  hild>.          
+00000b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b50: 3c6f 626a 6563 7420 636c 6173 733d 2247  <object class="G
+00000b60: 746b 4d65 6e75 4974 656d 2220 6964 3d22  tkMenuItem" id="
+00000b70: 6d65 6e75 5f6d 6565 745f 7175 6974 223e  menu_meet_quit">
+00000b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000b90: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
+00000ba0: 6f70 6572 7479 206e 616d 653d 226c 6162  operty name="lab
+00000bb0: 656c 223e 5f51 7569 743c 2f70 726f 7065  el">_Quit</prope
+00000bc0: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
+00000bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000be0: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00000bf0: 2276 6973 6962 6c65 223e 5472 7565 3c2f  "visible">True</
+00000c00: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
+00000c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c20: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+00000c30: 6e61 6d65 3d22 7573 655f 756e 6465 726c  name="use_underl
+00000c40: 696e 6522 3e54 7275 653c 2f70 726f 7065  ine">True</prope
+00000c50: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
+00000c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c70: 203c 6163 6365 6c65 7261 746f 7220 6b65   <accelerator ke
+00000c80: 793d 2271 2220 7369 676e 616c 3d22 6163  y="q" signal="ac
+00000c90: 7469 7661 7465 2220 6d6f 6469 6669 6572  tivate" modifier
+00000ca0: 733d 2247 444b 5f43 4f4e 5452 4f4c 5f4d  s="GDK_CONTROL_M
+00000cb0: 4153 4b22 2f3e 0a20 2020 2020 2020 2020  ASK"/>.         
 00000cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cd0: 2020 2020 3c2f 6f62 6a65 6374 3e0a 2020      </object>.  
-00000ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cf0: 2020 2020 2020 3c2f 6368 696c 643e 0a20        </child>. 
-00000d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d10: 2020 2020 2020 203c 6368 696c 643e 0a20         <child>. 
-00000d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d30: 2020 2020 2020 2020 203c 6f62 6a65 6374           <object
-00000d40: 2063 6c61 7373 3d22 4774 6b49 6d61 6765   class="GtkImage
-00000d50: 4d65 6e75 4974 656d 2220 6964 3d22 6d65  MenuItem" id="me
-00000d60: 6e75 5f6d 6565 745f 7175 6974 223e 0a20  nu_meet_quit">. 
+00000cd0: 2020 203c 7369 676e 616c 206e 616d 653d     <signal name=
+00000ce0: 2261 6374 6976 6174 6522 2068 616e 646c  "activate" handl
+00000cf0: 6572 3d22 6d65 6e75 5f6d 6565 745f 7175  er="menu_meet_qu
+00000d00: 6974 5f63 6222 2f3e 0a20 2020 2020 2020  it_cb"/>.       
+00000d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d20: 2020 203c 2f6f 626a 6563 743e 0a20 2020     </object>.   
+00000d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d40: 2020 2020 203c 2f63 6869 6c64 3e0a 2020       </child>.  
+00000d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d60: 2020 2020 3c2f 6f62 6a65 6374 3e0a 2020      </object>.  
 00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d80: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
-00000d90: 6572 7479 206e 616d 653d 226c 6162 656c  erty name="label
-00000da0: 223e 6774 6b2d 7175 6974 3c2f 7072 6f70  ">gtk-quit</prop
-00000db0: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
-00000dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000dd0: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00000de0: 3d22 7669 7369 626c 6522 3e54 7275 653c  ="visible">True<
-00000df0: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
-00000e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e10: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00000e20: 206e 616d 653d 2274 6f6f 6c74 6970 5f74   name="tooltip_t
-00000e30: 6578 7422 2074 7261 6e73 6c61 7461 626c  ext" translatabl
-00000e40: 653d 2279 6573 223e 4578 6974 2072 6f61  e="yes">Exit roa
-00000e50: 646d 6565 743c 2f70 726f 7065 7274 793e  dmeet</property>
-00000e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000e70: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
-00000e80: 6f70 6572 7479 206e 616d 653d 2275 7365  operty name="use
-00000e90: 5f75 6e64 6572 6c69 6e65 223e 5472 7565  _underline">True
-00000ea0: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-00000eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ec0: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-00000ed0: 7920 6e61 6d65 3d22 7573 655f 7374 6f63  y name="use_stoc
-00000ee0: 6b22 3e54 7275 653c 2f70 726f 7065 7274  k">True</propert
-00000ef0: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
-00000f00: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000f10: 6163 6365 6c65 7261 746f 7220 6b65 793d  accelerator key=
-00000f20: 2271 2220 7369 676e 616c 3d22 6163 7469  "q" signal="acti
-00000f30: 7661 7465 2220 6d6f 6469 6669 6572 733d  vate" modifiers=
-00000f40: 2247 444b 5f43 4f4e 5452 4f4c 5f4d 4153  "GDK_CONTROL_MAS
-00000f50: 4b22 2f3e 0a20 2020 2020 2020 2020 2020  K"/>.           
+00000d80: 2020 3c2f 6368 696c 643e 0a20 2020 2020    </child>.     
+00000d90: 2020 2020 2020 2020 2020 2020 203c 2f6f               </o
+00000da0: 626a 6563 743e 0a20 2020 2020 2020 2020  bject>.         
+00000db0: 2020 2020 2020 203c 2f63 6869 6c64 3e0a         </child>.
+00000dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000dd0: 203c 212d 2d20 6576 656e 7420 6d65 6e75   <!-- event menu
+00000de0: 202d 2d3e 0a20 2020 2020 2020 2020 2020   -->.           
+00000df0: 2020 2020 203c 6368 696c 643e 0a20 2020       <child>.   
+00000e00: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000e10: 6f62 6a65 6374 2063 6c61 7373 3d22 4774  object class="Gt
+00000e20: 6b4d 656e 7549 7465 6d22 2069 643d 226d  kMenuItem" id="m
+00000e30: 656e 755f 6576 656e 7422 3e0a 2020 2020  enu_event">.    
+00000e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e50: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+00000e60: 7669 7369 626c 6522 3e54 7275 653c 2f70  visible">True</p
+00000e70: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
+00000e80: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
+00000e90: 6f70 6572 7479 206e 616d 653d 226c 6162  operty name="lab
+00000ea0: 656c 223e 5f45 7665 6e74 3c2f 7072 6f70  el">_Event</prop
+00000eb0: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
+00000ec0: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
+00000ed0: 7274 7920 6e61 6d65 3d22 7573 655f 756e  rty name="use_un
+00000ee0: 6465 726c 696e 6522 3e54 7275 653c 2f70  derline">True</p
+00000ef0: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
+00000f00: 2020 2020 2020 2020 2020 2020 203c 6368               <ch
+00000f10: 696c 6420 7479 7065 3d22 7375 626d 656e  ild type="submen
+00000f20: 7522 3e0a 2020 2020 2020 2020 2020 2020  u">.            
+00000f30: 2020 2020 2020 2020 2020 3c6f 626a 6563            <objec
+00000f40: 7420 636c 6173 733d 2247 746b 4d65 6e75  t class="GtkMenu
+00000f50: 2220 6964 3d22 6d65 6e75 3622 3e0a 2020  " id="menu6">.  
 00000f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f70: 203c 7369 676e 616c 206e 616d 653d 2261   <signal name="a
-00000f80: 6374 6976 6174 6522 2068 616e 646c 6572  ctivate" handler
-00000f90: 3d22 6d65 6e75 5f6d 6565 745f 7175 6974  ="menu_meet_quit
-00000fa0: 5f63 6222 2f3e 0a20 2020 2020 2020 2020  _cb"/>.         
-00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fc0: 203c 2f6f 626a 6563 743e 0a20 2020 2020   </object>.     
-00000fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fe0: 2020 203c 2f63 6869 6c64 3e0a 2020 2020     </child>.    
-00000ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001000: 2020 3c2f 6f62 6a65 6374 3e0a 2020 2020    </object>.    
-00001010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001020: 3c2f 6368 696c 643e 0a20 2020 2020 2020  </child>.       
-00001030: 2020 2020 2020 2020 2020 203c 2f6f 626a             </obj
-00001040: 6563 743e 0a20 2020 2020 2020 2020 2020  ect>.           
-00001050: 2020 2020 203c 2f63 6869 6c64 3e0a 2020       </child>.  
-00001060: 2020 2020 2020 2020 2020 2020 2020 3c63                <c
-00001070: 6869 6c64 3e0a 2020 2020 2020 2020 2020  hild>.          
-00001080: 2020 2020 2020 2020 3c6f 626a 6563 7420          <object 
-00001090: 636c 6173 733d 2247 746b 4d65 6e75 4974  class="GtkMenuIt
-000010a0: 656d 2220 6964 3d22 6d65 6e75 5f72 6163  em" id="menu_rac
-000010b0: 6522 3e0a 2020 2020 2020 2020 2020 2020  e">.            
-000010c0: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-000010d0: 7920 6e61 6d65 3d22 7669 7369 626c 6522  y name="visible"
-000010e0: 3e54 7275 653c 2f70 726f 7065 7274 793e  >True</property>
-000010f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001100: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00001110: 616d 653d 226c 6162 656c 2220 7472 616e  ame="label" tran
-00001120: 736c 6174 6162 6c65 3d22 7965 7322 3e5f  slatable="yes">_
-00001130: 4576 656e 743c 2f70 726f 7065 7274 793e  Event</property>
-00001140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001150: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00001160: 616d 653d 2275 7365 5f75 6e64 6572 6c69  ame="use_underli
-00001170: 6e65 223e 5472 7565 3c2f 7072 6f70 6572  ne">True</proper
-00001180: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
-00001190: 2020 2020 2020 2020 3c63 6869 6c64 2074          <child t
-000011a0: 7970 653d 2273 7562 6d65 6e75 223e 0a20  ype="submenu">. 
-000011b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011c0: 2020 2020 203c 6f62 6a65 6374 2063 6c61       <object cla
-000011d0: 7373 3d22 4774 6b4d 656e 7522 2069 643d  ss="GtkMenu" id=
-000011e0: 226d 656e 7536 223e 0a20 2020 2020 2020  "menu6">.       
-000011f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001200: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-00001210: 2276 6973 6962 6c65 223e 5472 7565 3c2f  "visible">True</
-00001220: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
-00001230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001240: 2020 3c63 6869 6c64 3e0a 2020 2020 2020    <child>.      
+00000f70: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+00000f80: 6e61 6d65 3d22 7669 7369 626c 6522 3e54  name="visible">T
+00000f90: 7275 653c 2f70 726f 7065 7274 793e 0a20  rue</property>. 
+00000fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fb0: 2020 2020 2020 203c 6368 696c 643e 0a20         <child>. 
+00000fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fd0: 2020 2020 2020 2020 203c 6f62 6a65 6374           <object
+00000fe0: 2063 6c61 7373 3d22 4774 6b4d 656e 7549   class="GtkMenuI
+00000ff0: 7465 6d22 2069 643d 226d 656e 755f 6576  tem" id="menu_ev
+00001000: 656e 745f 7072 6f70 6572 7469 6573 223e  ent_properties">
+00001010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001020: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
+00001030: 6f70 6572 7479 206e 616d 653d 226c 6162  operty name="lab
+00001040: 656c 223e 5f50 726f 7065 7274 6965 733c  el">_Properties<
+00001050: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
+00001060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001070: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+00001080: 206e 616d 653d 2276 6973 6962 6c65 223e   name="visible">
+00001090: 5472 7565 3c2f 7072 6f70 6572 7479 3e0a  True</property>.
+000010a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010b0: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
+000010c0: 7065 7274 7920 6e61 6d65 3d22 7573 655f  perty name="use_
+000010d0: 756e 6465 726c 696e 6522 3e54 7275 653c  underline">True<
+000010e0: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
+000010f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001100: 2020 2020 2020 203c 7369 676e 616c 206e         <signal n
+00001110: 616d 653d 2261 6374 6976 6174 6522 2068  ame="activate" h
+00001120: 616e 646c 6572 3d22 6d65 6e75 5f65 7665  andler="menu_eve
+00001130: 6e74 5f70 726f 7065 7274 6965 735f 6163  nt_properties_ac
+00001140: 7469 7661 7465 5f63 6222 2f3e 0a20 2020  tivate_cb"/>.   
+00001150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001160: 2020 2020 2020 203c 2f6f 626a 6563 743e         </object>
+00001170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001180: 2020 2020 2020 2020 203c 2f63 6869 6c64           </child
+00001190: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000011a0: 2020 2020 2020 2020 2020 3c63 6869 6c64            <child
+000011b0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000011c0: 2020 2020 2020 2020 2020 2020 3c6f 626a              <obj
+000011d0: 6563 7420 636c 6173 733d 2247 746b 5365  ect class="GtkSe
+000011e0: 7061 7261 746f 724d 656e 7549 7465 6d22  paratorMenuItem"
+000011f0: 2069 643d 226d 656e 755f 6576 656e 745f   id="menu_event_
+00001200: 7365 7032 223e 0a20 2020 2020 2020 2020  sep2">.         
+00001210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001220: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+00001230: 653d 2276 6973 6962 6c65 223e 5472 7565  e="visible">True
+00001240: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
 00001250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001260: 2020 2020 3c6f 626a 6563 7420 636c 6173      <object clas
-00001270: 733d 2247 746b 496d 6167 654d 656e 7549  s="GtkImageMenuI
-00001280: 7465 6d22 2069 643d 226d 656e 755f 7261  tem" id="menu_ra
-00001290: 6365 5f70 726f 7065 7274 6965 7322 3e0a  ce_properties">.
-000012a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012b0: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
-000012c0: 7065 7274 7920 6e61 6d65 3d22 6c61 6265  perty name="labe
-000012d0: 6c22 3e67 746b 2d70 726f 7065 7274 6965  l">gtk-propertie
-000012e0: 733c 2f70 726f 7065 7274 793e 0a20 2020  s</property>.   
-000012f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001300: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-00001310: 7479 206e 616d 653d 2276 6973 6962 6c65  ty name="visible
-00001320: 223e 5472 7565 3c2f 7072 6f70 6572 7479  ">True</property
-00001330: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00001340: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-00001350: 726f 7065 7274 7920 6e61 6d65 3d22 746f  roperty name="to
-00001360: 6f6c 7469 705f 7465 7874 2220 7472 616e  oltip_text" tran
-00001370: 736c 6174 6162 6c65 3d22 7965 7322 3e45  slatable="yes">E
-00001380: 6469 7420 6576 656e 7420 7370 6563 6966  dit event specif
-00001390: 6963 2070 6172 616d 6574 6572 733c 2f70  ic parameters</p
-000013a0: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
-000013b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013c0: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-000013d0: 616d 653d 2275 7365 5f75 6e64 6572 6c69  ame="use_underli
-000013e0: 6e65 223e 5472 7565 3c2f 7072 6f70 6572  ne">True</proper
-000013f0: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
-00001400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001410: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00001420: 7573 655f 7374 6f63 6b22 3e54 7275 653c  use_stock">True<
-00001430: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
-00001440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001450: 2020 2020 2020 203c 7369 676e 616c 206e         <signal n
-00001460: 616d 653d 2261 6374 6976 6174 6522 2068  ame="activate" h
-00001470: 616e 646c 6572 3d22 6d65 6e75 5f72 6163  andler="menu_rac
-00001480: 655f 7072 6f70 6572 7469 6573 5f61 6374  e_properties_act
-00001490: 6976 6174 655f 6362 222f 3e0a 2020 2020  ivate_cb"/>.    
-000014a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014b0: 2020 2020 2020 3c2f 6f62 6a65 6374 3e0a        </object>.
-000014c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014d0: 2020 2020 2020 2020 3c2f 6368 696c 643e          </child>
-000014e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000014f0: 2020 2020 2020 2020 203c 6368 696c 643e           <child>
-00001500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001510: 2020 2020 2020 2020 2020 203c 6f62 6a65             <obje
-00001520: 6374 2063 6c61 7373 3d22 4774 6b53 6570  ct class="GtkSep
-00001530: 6172 6174 6f72 4d65 6e75 4974 656d 2220  aratorMenuItem" 
-00001540: 6964 3d22 6d65 6e75 5f72 6163 655f 7365  id="menu_race_se
-00001550: 7032 223e 0a20 2020 2020 2020 2020 2020  p2">.           
-00001560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001570: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-00001580: 2276 6973 6962 6c65 223e 5472 7565 3c2f  "visible">True</
-00001590: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
-000015a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015b0: 2020 2020 3c2f 6f62 6a65 6374 3e0a 2020      </object>.  
+00001260: 2020 2020 2020 3c2f 6f62 6a65 6374 3e0a        </object>.
+00001270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001280: 2020 2020 2020 2020 3c2f 6368 696c 643e          </child>
+00001290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000012a0: 2020 2020 2020 2020 203c 6368 696c 643e           <child>
+000012b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000012c0: 2020 2020 2020 2020 2020 203c 6f62 6a65             <obje
+000012d0: 6374 2063 6c61 7373 3d22 4774 6b4d 656e  ct class="GtkMen
+000012e0: 7549 7465 6d22 2069 643d 226d 656e 755f  uItem" id="menu_
+000012f0: 6576 656e 745f 6172 6d73 7461 7274 223e  event_armstart">
+00001300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001310: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
+00001320: 6f70 6572 7479 206e 616d 653d 2276 6973  operty name="vis
+00001330: 6962 6c65 223e 5472 7565 3c2f 7072 6f70  ible">True</prop
+00001340: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
+00001350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001360: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+00001370: 3d22 6c61 6265 6c22 3e41 726d 205f 5374  ="label">Arm _St
+00001380: 6172 743c 2f70 726f 7065 7274 793e 0a20  art</property>. 
+00001390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013a0: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
+000013b0: 6572 7479 206e 616d 653d 2275 7365 5f75  erty name="use_u
+000013c0: 6e64 6572 6c69 6e65 223e 5472 7565 3c2f  nderline">True</
+000013d0: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
+000013e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013f0: 2020 2020 2020 3c61 6363 656c 6572 6174        <accelerat
+00001400: 6f72 206b 6579 3d22 4635 2220 7369 676e  or key="F5" sign
+00001410: 616c 3d22 6163 7469 7661 7465 222f 3e0a  al="activate"/>.
+00001420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001430: 2020 2020 2020 2020 2020 2020 3c73 6967              <sig
+00001440: 6e61 6c20 6e61 6d65 3d22 6163 7469 7661  nal name="activa
+00001450: 7465 2220 6861 6e64 6c65 723d 226d 656e  te" handler="men
+00001460: 755f 6576 656e 745f 6172 6d73 7461 7274  u_event_armstart
+00001470: 5f61 6374 6976 6174 655f 6362 222f 3e0a  _activate_cb"/>.
+00001480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001490: 2020 2020 2020 2020 2020 3c2f 6f62 6a65            </obje
+000014a0: 6374 3e0a 2020 2020 2020 2020 2020 2020  ct>.            
+000014b0: 2020 2020 2020 2020 2020 2020 3c2f 6368              </ch
+000014c0: 696c 643e 0a20 2020 2020 2020 2020 2020  ild>.           
+000014d0: 2020 2020 2020 2020 2020 2020 203c 6368               <ch
+000014e0: 696c 643e 0a20 2020 2020 2020 2020 2020  ild>.           
+000014f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001500: 6f62 6a65 6374 2063 6c61 7373 3d22 4774  object class="Gt
+00001510: 6b4d 656e 7549 7465 6d22 2069 643d 226d  kMenuItem" id="m
+00001520: 656e 755f 6576 656e 745f 6172 6d6c 6170  enu_event_armlap
+00001530: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00001540: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001550: 7072 6f70 6572 7479 206e 616d 653d 2276  property name="v
+00001560: 6973 6962 6c65 223e 5472 7565 3c2f 7072  isible">True</pr
+00001570: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
+00001580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001590: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+000015a0: 6d65 3d22 6c61 6265 6c22 3e41 726d 205f  me="label">Arm _
+000015b0: 4c61 703c 2f70 726f 7065 7274 793e 0a20  Lap</property>. 
 000015c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015d0: 2020 2020 2020 3c2f 6368 696c 643e 0a20        </child>. 
-000015e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015f0: 2020 2020 2020 203c 6368 696c 643e 0a20         <child>. 
-00001600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001610: 2020 2020 2020 2020 203c 6f62 6a65 6374           <object
-00001620: 2063 6c61 7373 3d22 4774 6b4d 656e 7549   class="GtkMenuI
-00001630: 7465 6d22 2069 643d 226d 656e 755f 7261  tem" id="menu_ra
-00001640: 6365 5f61 726d 7374 6172 7422 3e0a 2020  ce_armstart">.  
+000015d0: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
+000015e0: 6572 7479 206e 616d 653d 2275 7365 5f75  erty name="use_u
+000015f0: 6e64 6572 6c69 6e65 223e 5472 7565 3c2f  nderline">True</
+00001600: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
+00001610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001620: 2020 2020 2020 3c61 6363 656c 6572 6174        <accelerat
+00001630: 6f72 206b 6579 3d22 4636 2220 7369 676e  or key="F6" sign
+00001640: 616c 3d22 6163 7469 7661 7465 222f 3e0a  al="activate"/>.
 00001650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001660: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00001670: 7274 7920 6e61 6d65 3d22 7669 7369 626c  rty name="visibl
-00001680: 6522 3e54 7275 653c 2f70 726f 7065 7274  e">True</propert
-00001690: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
-000016a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000016b0: 7072 6f70 6572 7479 206e 616d 653d 226c  property name="l
-000016c0: 6162 656c 2220 7472 616e 736c 6174 6162  abel" translatab
-000016d0: 6c65 3d22 7965 7322 3e41 726d 2053 7461  le="yes">Arm Sta
-000016e0: 7274 3c2f 7072 6f70 6572 7479 3e0a 2020  rt</property>.  
-000016f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001700: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00001710: 7274 7920 6e61 6d65 3d22 746f 6f6c 7469  rty name="toolti
-00001720: 705f 7465 7874 2220 7472 616e 736c 6174  p_text" translat
-00001730: 6162 6c65 3d22 7965 7322 3e41 726d 2065  able="yes">Arm e
-00001740: 7665 6e74 2066 6f72 2061 2073 7461 7274  vent for a start
-00001750: 2074 7269 6767 6572 3c2f 7072 6f70 6572   trigger</proper
-00001760: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
-00001770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001780: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00001790: 7573 655f 756e 6465 726c 696e 6522 3e54  use_underline">T
-000017a0: 7275 653c 2f70 726f 7065 7274 793e 0a20  rue</property>. 
+00001660: 2020 2020 2020 2020 2020 2020 3c73 6967              <sig
+00001670: 6e61 6c20 6e61 6d65 3d22 6163 7469 7661  nal name="activa
+00001680: 7465 2220 6861 6e64 6c65 723d 226d 656e  te" handler="men
+00001690: 755f 6576 656e 745f 6172 6d6c 6170 5f61  u_event_armlap_a
+000016a0: 6374 6976 6174 655f 6362 222f 3e0a 2020  ctivate_cb"/>.  
+000016b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016c0: 2020 2020 2020 2020 3c2f 6f62 6a65 6374          </object
+000016d0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000016e0: 2020 2020 2020 2020 2020 3c2f 6368 696c            </chil
+000016f0: 643e 0a20 2020 2020 2020 2020 2020 2020  d>.             
+00001700: 2020 2020 2020 2020 2020 203c 6368 696c             <chil
+00001710: 643e 0a20 2020 2020 2020 2020 2020 2020  d>.             
+00001720: 2020 2020 2020 2020 2020 2020 203c 6f62               <ob
+00001730: 6a65 6374 2063 6c61 7373 3d22 4774 6b4d  ject class="GtkM
+00001740: 656e 7549 7465 6d22 2069 643d 226d 656e  enuItem" id="men
+00001750: 755f 6576 656e 745f 6172 6d66 696e 223e  u_event_armfin">
+00001760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001770: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
+00001780: 6f70 6572 7479 206e 616d 653d 2276 6973  operty name="vis
+00001790: 6962 6c65 223e 5472 7565 3c2f 7072 6f70  ible">True</prop
+000017a0: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
 000017b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017c0: 2020 2020 2020 2020 2020 203c 6163 6365             <acce
-000017d0: 6c65 7261 746f 7220 6b65 793d 2246 3522  lerator key="F5"
-000017e0: 2073 6967 6e61 6c3d 2261 6374 6976 6174   signal="activat
-000017f0: 6522 2f3e 0a20 2020 2020 2020 2020 2020  e"/>.           
-00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001810: 203c 7369 676e 616c 206e 616d 653d 2261   <signal name="a
-00001820: 6374 6976 6174 6522 2068 616e 646c 6572  ctivate" handler
-00001830: 3d22 6d65 6e75 5f72 6163 655f 6172 6d73  ="menu_race_arms
-00001840: 7461 7274 5f61 6374 6976 6174 655f 6362  tart_activate_cb
-00001850: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00001860: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00001870: 6f62 6a65 6374 3e0a 2020 2020 2020 2020  object>.        
+000017c0: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+000017d0: 3d22 6c61 6265 6c22 3e41 726d 2046 696e  ="label">Arm Fin
+000017e0: 6973 683c 2f70 726f 7065 7274 793e 0a20  ish</property>. 
+000017f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001800: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
+00001810: 6572 7479 206e 616d 653d 2275 7365 5f75  erty name="use_u
+00001820: 6e64 6572 6c69 6e65 223e 5472 7565 3c2f  nderline">True</
+00001830: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
+00001840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001850: 2020 2020 2020 3c61 6363 656c 6572 6174        <accelerat
+00001860: 6f72 206b 6579 3d22 4639 2220 7369 676e  or key="F9" sign
+00001870: 616c 3d22 6163 7469 7661 7465 222f 3e0a  al="activate"/>.
 00001880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001890: 3c2f 6368 696c 643e 0a20 2020 2020 2020  </child>.       
-000018a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018b0: 203c 6368 696c 643e 0a20 2020 2020 2020   <child>.       
-000018c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018d0: 2020 203c 6f62 6a65 6374 2063 6c61 7373     <object class
-000018e0: 3d22 4774 6b4d 656e 7549 7465 6d22 2069  ="GtkMenuItem" i
-000018f0: 643d 226d 656e 755f 7261 6365 5f61 726d  d="menu_race_arm
-00001900: 6c61 7022 3e0a 2020 2020 2020 2020 2020  lap">.          
-00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001920: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00001930: 3d22 7669 7369 626c 6522 3e54 7275 653c  ="visible">True<
-00001940: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
-00001950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001960: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00001970: 206e 616d 653d 226c 6162 656c 2220 7472   name="label" tr
-00001980: 616e 736c 6174 6162 6c65 3d22 7965 7322  anslatable="yes"
-00001990: 3e41 726d 204c 6170 3c2f 7072 6f70 6572  >Arm Lap</proper
-000019a0: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
-000019b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019c0: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-000019d0: 746f 6f6c 7469 705f 7465 7874 2220 7472  tooltip_text" tr
-000019e0: 616e 736c 6174 6162 6c65 3d22 7965 7322  anslatable="yes"
-000019f0: 3e41 726d 2065 7665 6e74 2066 6f72 2061  >Arm event for a
-00001a00: 206e 6577 206c 6170 3c2f 7072 6f70 6572   new lap</proper
-00001a10: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
+00001890: 2020 2020 2020 2020 2020 2020 3c73 6967              <sig
+000018a0: 6e61 6c20 6e61 6d65 3d22 6163 7469 7661  nal name="activa
+000018b0: 7465 2220 6861 6e64 6c65 723d 226d 656e  te" handler="men
+000018c0: 755f 6576 656e 745f 6172 6d66 696e 5f61  u_event_armfin_a
+000018d0: 6374 6976 6174 655f 6362 222f 3e0a 2020  ctivate_cb"/>.  
+000018e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018f0: 2020 2020 2020 2020 3c2f 6f62 6a65 6374          </object
+00001900: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001910: 2020 2020 2020 2020 2020 3c2f 6368 696c            </chil
+00001920: 643e 0a20 2020 2020 2020 2020 2020 2020  d>.             
+00001930: 2020 2020 2020 2020 2020 203c 6368 696c             <chil
+00001940: 643e 0a20 2020 2020 2020 2020 2020 2020  d>.             
+00001950: 2020 2020 2020 2020 2020 2020 203c 6f62               <ob
+00001960: 6a65 6374 2063 6c61 7373 3d22 4774 6b4d  ject class="GtkM
+00001970: 656e 7549 7465 6d22 2069 643d 226d 656e  enuItem" id="men
+00001980: 755f 6576 656e 745f 6669 6e69 7368 6564  u_event_finished
+00001990: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+000019a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000019b0: 7072 6f70 6572 7479 206e 616d 653d 2276  property name="v
+000019c0: 6973 6962 6c65 223e 5472 7565 3c2f 7072  isible">True</pr
+000019d0: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
+000019e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019f0: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00001a00: 6d65 3d22 6c61 6265 6c22 3e46 696e 6973  me="label">Finis
+00001a10: 6865 643c 2f70 726f 7065 7274 793e 0a20  hed</property>. 
 00001a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a30: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00001a40: 7573 655f 756e 6465 726c 696e 6522 3e54  use_underline">T
-00001a50: 7275 653c 2f70 726f 7065 7274 793e 0a20  rue</property>. 
-00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a70: 2020 2020 2020 2020 2020 203c 6163 6365             <acce
-00001a80: 6c65 7261 746f 7220 6b65 793d 2246 3622  lerator key="F6"
-00001a90: 2073 6967 6e61 6c3d 2261 6374 6976 6174   signal="activat
-00001aa0: 6522 2f3e 0a20 2020 2020 2020 2020 2020  e"/>.           
-00001ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ac0: 203c 7369 676e 616c 206e 616d 653d 2261   <signal name="a
-00001ad0: 6374 6976 6174 6522 2068 616e 646c 6572  ctivate" handler
-00001ae0: 3d22 6d65 6e75 5f72 6163 655f 6172 6d6c  ="menu_race_arml
-00001af0: 6170 5f61 6374 6976 6174 655f 6362 222f  ap_activate_cb"/
-00001b00: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00001b10: 2020 2020 2020 2020 2020 2020 3c2f 6f62              </ob
-00001b20: 6a65 6374 3e0a 2020 2020 2020 2020 2020  ject>.          
-00001b30: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00001b40: 6368 696c 643e 0a20 2020 2020 2020 2020  child>.         
-00001b50: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001b60: 6368 696c 643e 0a20 2020 2020 2020 2020  child>.         
-00001b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b80: 203c 6f62 6a65 6374 2063 6c61 7373 3d22   <object class="
-00001b90: 4774 6b4d 656e 7549 7465 6d22 2069 643d  GtkMenuItem" id=
-00001ba0: 226d 656e 755f 7261 6365 5f61 726d 6669  "menu_race_armfi
-00001bb0: 6e22 3e0a 2020 2020 2020 2020 2020 2020  n">.            
-00001bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bd0: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00001be0: 7669 7369 626c 6522 3e54 7275 653c 2f70  visible">True</p
-00001bf0: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
-00001c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c10: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00001c20: 616d 653d 226c 6162 656c 2220 7472 616e  ame="label" tran
-00001c30: 736c 6174 6162 6c65 3d22 7965 7322 3e41  slatable="yes">A
-00001c40: 726d 2046 696e 6973 683c 2f70 726f 7065  rm Finish</prope
-00001c50: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
-00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c70: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-00001c80: 2274 6f6f 6c74 6970 5f74 6578 7422 2074  "tooltip_text" t
-00001c90: 7261 6e73 6c61 7461 626c 653d 2279 6573  ranslatable="yes
-00001ca0: 223e 4172 6d20 6576 656e 7420 666f 7220  ">Arm event for 
-00001cb0: 6669 6e69 7368 696e 6720 7269 6465 7273  finishing riders
-00001cc0: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-00001cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ce0: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-00001cf0: 7920 6e61 6d65 3d22 7573 655f 756e 6465  y name="use_unde
-00001d00: 726c 696e 6522 3e54 7275 653c 2f70 726f  rline">True</pro
-00001d10: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
-00001d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d30: 2020 203c 6163 6365 6c65 7261 746f 7220     <accelerator 
-00001d40: 6b65 793d 2246 3922 2073 6967 6e61 6c3d  key="F9" signal=
-00001d50: 2261 6374 6976 6174 6522 2f3e 0a20 2020  "activate"/>.   
-00001d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d70: 2020 2020 2020 2020 203c 7369 676e 616c           <signal
-00001d80: 206e 616d 653d 2261 6374 6976 6174 6522   name="activate"
-00001d90: 2068 616e 646c 6572 3d22 6d65 6e75 5f72   handler="menu_r
-00001da0: 6163 655f 6172 6d66 696e 5f61 6374 6976  ace_armfin_activ
-00001db0: 6174 655f 6362 222f 3e0a 2020 2020 2020  ate_cb"/>.      
+00001a30: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
+00001a40: 6572 7479 206e 616d 653d 2275 7365 5f75  erty name="use_u
+00001a50: 6e64 6572 6c69 6e65 223e 5472 7565 3c2f  nderline">True</
+00001a60: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
+00001a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a80: 2020 2020 2020 3c61 6363 656c 6572 6174        <accelerat
+00001a90: 6f72 206b 6579 3d22 4631 3022 2073 6967  or key="F10" sig
+00001aa0: 6e61 6c3d 2261 6374 6976 6174 6522 2f3e  nal="activate"/>
+00001ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001ac0: 2020 2020 2020 2020 2020 2020 203c 7369               <si
+00001ad0: 676e 616c 206e 616d 653d 2261 6374 6976  gnal name="activ
+00001ae0: 6174 6522 2068 616e 646c 6572 3d22 6d65  ate" handler="me
+00001af0: 6e75 5f65 7665 6e74 5f66 696e 6973 6865  nu_event_finishe
+00001b00: 645f 6163 7469 7661 7465 5f63 6222 2f3e  d_activate_cb"/>
+00001b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001b20: 2020 2020 2020 2020 2020 203c 2f6f 626a             </obj
+00001b30: 6563 743e 0a20 2020 2020 2020 2020 2020  ect>.           
+00001b40: 2020 2020 2020 2020 2020 2020 203c 2f63               </c
+00001b50: 6869 6c64 3e0a 2020 2020 2020 2020 2020  hild>.          
+00001b60: 2020 2020 2020 2020 2020 2020 2020 3c63                <c
+00001b70: 6869 6c64 3e0a 2020 2020 2020 2020 2020  hild>.          
+00001b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b90: 3c6f 626a 6563 7420 636c 6173 733d 2247  <object class="G
+00001ba0: 746b 4d65 6e75 4974 656d 2220 6964 3d22  tkMenuItem" id="
+00001bb0: 6d65 6e75 5f65 7665 6e74 5f72 6573 6574  menu_event_reset
+00001bc0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00001bd0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001be0: 7072 6f70 6572 7479 206e 616d 653d 2276  property name="v
+00001bf0: 6973 6962 6c65 223e 5472 7565 3c2f 7072  isible">True</pr
+00001c00: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
+00001c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c20: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00001c30: 6d65 3d22 6c61 6265 6c22 3e52 6573 6574  me="label">Reset
+00001c40: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+00001c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c60: 2020 2020 2020 2020 3c61 6363 656c 6572          <acceler
+00001c70: 6174 6f72 206b 6579 3d22 4635 2220 7369  ator key="F5" si
+00001c80: 676e 616c 3d22 6163 7469 7661 7465 2220  gnal="activate" 
+00001c90: 6d6f 6469 6669 6572 733d 2247 444b 5f43  modifiers="GDK_C
+00001ca0: 4f4e 5452 4f4c 5f4d 4153 4b22 2f3e 0a20  ONTROL_MASK"/>. 
+00001cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cc0: 2020 2020 2020 2020 2020 203c 7369 676e             <sign
+00001cd0: 616c 206e 616d 653d 2261 6374 6976 6174  al name="activat
+00001ce0: 6522 2068 616e 646c 6572 3d22 6d65 6e75  e" handler="menu
+00001cf0: 5f65 7665 6e74 5f72 6573 6574 5f63 6222  _event_reset_cb"
+00001d00: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+00001d10: 2020 2020 2020 2020 2020 2020 203c 2f6f               </o
+00001d20: 626a 6563 743e 0a20 2020 2020 2020 2020  bject>.         
+00001d30: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001d40: 2f63 6869 6c64 3e0a 2020 2020 2020 2020  /child>.        
+00001d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d60: 3c63 6869 6c64 3e0a 2020 2020 2020 2020  <child>.        
+00001d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d80: 2020 3c6f 626a 6563 7420 636c 6173 733d    <object class=
+00001d90: 2247 746b 5365 7061 7261 746f 724d 656e  "GtkSeparatorMen
+00001da0: 7549 7465 6d22 2069 643d 226d 656e 755f  uItem" id="menu_
+00001db0: 6576 656e 745f 7365 7032 3122 3e0a 2020  event_sep21">.  
 00001dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001dd0: 2020 2020 3c2f 6f62 6a65 6374 3e0a 2020      </object>.  
-00001de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001df0: 2020 2020 2020 3c2f 6368 696c 643e 0a20        </child>. 
-00001e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e10: 2020 2020 2020 203c 6368 696c 643e 0a20         <child>. 
-00001e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e30: 2020 2020 2020 2020 203c 6f62 6a65 6374           <object
-00001e40: 2063 6c61 7373 3d22 4774 6b4d 656e 7549   class="GtkMenuI
-00001e50: 7465 6d22 2069 643d 226d 656e 755f 7261  tem" id="menu_ra
-00001e60: 6365 5f66 696e 6973 6865 6422 3e0a 2020  ce_finished">.  
+00001dd0: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
+00001de0: 7274 7920 6e61 6d65 3d22 7669 7369 626c  rty name="visibl
+00001df0: 6522 3e54 7275 653c 2f70 726f 7065 7274  e">True</propert
+00001e00: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
+00001e10: 2020 2020 2020 2020 2020 2020 203c 2f6f               </o
+00001e20: 626a 6563 743e 0a20 2020 2020 2020 2020  bject>.         
+00001e30: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001e40: 2f63 6869 6c64 3e0a 2020 2020 2020 2020  /child>.        
+00001e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e60: 3c63 6869 6c64 3e0a 2020 2020 2020 2020  <child>.        
 00001e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e80: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00001e90: 7274 7920 6e61 6d65 3d22 7669 7369 626c  rty name="visibl
-00001ea0: 6522 3e54 7275 653c 2f70 726f 7065 7274  e">True</propert
-00001eb0: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
-00001ec0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001ed0: 7072 6f70 6572 7479 206e 616d 653d 226c  property name="l
-00001ee0: 6162 656c 2220 7472 616e 736c 6174 6162  abel" translatab
-00001ef0: 6c65 3d22 7965 7322 3e46 696e 6973 6865  le="yes">Finishe
-00001f00: 643c 2f70 726f 7065 7274 793e 0a20 2020  d</property>.   
-00001f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f20: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-00001f30: 7479 206e 616d 653d 2274 6f6f 6c74 6970  ty name="tooltip
-00001f40: 5f74 6578 7422 2074 7261 6e73 6c61 7461  _text" translata
-00001f50: 626c 653d 2279 6573 223e 4d61 726b 2065  ble="yes">Mark e
-00001f60: 7665 6e74 2061 7320 6669 6e69 7368 6564  vent as finished
-00001f70: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-00001f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f90: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-00001fa0: 7920 6e61 6d65 3d22 7573 655f 756e 6465  y name="use_unde
-00001fb0: 726c 696e 6522 3e54 7275 653c 2f70 726f  rline">True</pro
-00001fc0: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
+00001e80: 2020 3c6f 626a 6563 7420 636c 6173 733d    <object class=
+00001e90: 2247 746b 4d65 6e75 4974 656d 2220 6964  "GtkMenuItem" id
+00001ea0: 3d22 6d65 6e75 5f65 7665 6e74 5f64 6563  ="menu_event_dec
+00001eb0: 6973 696f 6e73 223e 0a20 2020 2020 2020  isions">.       
+00001ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ed0: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+00001ee0: 616d 653d 2276 6973 6962 6c65 223e 5472  ame="visible">Tr
+00001ef0: 7565 3c2f 7072 6f70 6572 7479 3e0a 2020  ue</property>.  
+00001f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f10: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
+00001f20: 7274 7920 6e61 6d65 3d22 6c61 6265 6c22  rty name="label"
+00001f30: 3e44 6563 6973 696f 6e73 3c2f 7072 6f70  >Decisions</prop
+00001f40: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
+00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f60: 2020 3c73 6967 6e61 6c20 6e61 6d65 3d22    <signal name="
+00001f70: 6163 7469 7661 7465 2220 6861 6e64 6c65  activate" handle
+00001f80: 723d 226d 656e 755f 6576 656e 745f 6465  r="menu_event_de
+00001f90: 6369 7369 6f6e 735f 6163 7469 7661 7465  cisions_activate
+00001fa0: 5f63 6222 2f3e 0a20 2020 2020 2020 2020  _cb"/>.         
+00001fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fc0: 203c 2f6f 626a 6563 743e 0a20 2020 2020   </object>.     
 00001fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fe0: 2020 203c 6163 6365 6c65 7261 746f 7220     <accelerator 
-00001ff0: 6b65 793d 2246 3130 2220 7369 676e 616c  key="F10" signal
-00002000: 3d22 6163 7469 7661 7465 222f 3e0a 2020  ="activate"/>.  
+00001fe0: 2020 203c 2f63 6869 6c64 3e0a 2020 2020     </child>.    
+00001ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002000: 2020 3c2f 6f62 6a65 6374 3e0a 2020 2020    </object>.    
 00002010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002020: 2020 2020 2020 2020 2020 3c73 6967 6e61            <signa
-00002030: 6c20 6e61 6d65 3d22 6163 7469 7661 7465  l name="activate
-00002040: 2220 6861 6e64 6c65 723d 226d 656e 755f  " handler="menu_
-00002050: 7261 6365 5f66 696e 6973 6865 645f 6163  race_finished_ac
-00002060: 7469 7661 7465 5f63 6222 2f3e 0a20 2020  tivate_cb"/>.   
-00002070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002080: 2020 2020 2020 203c 2f6f 626a 6563 743e         </object>
-00002090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000020a0: 2020 2020 2020 2020 203c 2f63 6869 6c64           </child
-000020b0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000020c0: 2020 2020 2020 2020 2020 3c63 6869 6c64            <child
-000020d0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000020e0: 2020 2020 2020 2020 2020 2020 3c6f 626a              <obj
-000020f0: 6563 7420 636c 6173 733d 2247 746b 5365  ect class="GtkSe
-00002100: 7061 7261 746f 724d 656e 7549 7465 6d22  paratorMenuItem"
-00002110: 2069 643d 226d 656e 755f 7261 6365 5f73   id="menu_race_s
-00002120: 6570 3231 223e 0a20 2020 2020 2020 2020  ep21">.         
-00002130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002140: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00002150: 653d 2276 6973 6962 6c65 223e 5472 7565  e="visible">True
-00002160: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-00002170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002180: 2020 2020 2020 3c2f 6f62 6a65 6374 3e0a        </object>.
-00002190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021a0: 2020 2020 2020 2020 3c2f 6368 696c 643e          </child>
-000021b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000021c0: 2020 2020 2020 2020 203c 6368 696c 643e           <child>
-000021d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000021e0: 2020 2020 2020 2020 2020 203c 6f62 6a65             <obje
-000021f0: 6374 2063 6c61 7373 3d22 4774 6b4d 656e  ct class="GtkMen
-00002200: 7549 7465 6d22 2069 643d 226d 656e 755f  uItem" id="menu_
-00002210: 7261 6365 5f64 6563 6973 696f 6e73 223e  race_decisions">
-00002220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002230: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
-00002240: 6f70 6572 7479 206e 616d 653d 2276 6973  operty name="vis
-00002250: 6962 6c65 223e 5472 7565 3c2f 7072 6f70  ible">True</prop
-00002260: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
-00002270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002280: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00002290: 3d22 6c61 6265 6c22 2074 7261 6e73 6c61  ="label" transla
-000022a0: 7461 626c 653d 2279 6573 223e 4465 6369  table="yes">Deci
-000022b0: 7369 6f6e 733c 2f70 726f 7065 7274 793e  sions</property>
-000022c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000022d0: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
-000022e0: 6f70 6572 7479 206e 616d 653d 2274 6f6f  operty name="too
-000022f0: 6c74 6970 5f74 6578 7422 2074 7261 6e73  ltip_text" trans
-00002300: 6c61 7461 626c 653d 2279 6573 223e 4564  latable="yes">Ed
-00002310: 6974 2064 6563 6973 696f 6e73 206f 6620  it decisions of 
-00002320: 7468 6520 636f 6d6d 6973 7361 6972 6573  the commissaires
-00002330: 2070 616e 656c 3c2f 7072 6f70 6572 7479   panel</property
-00002340: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00002350: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
-00002360: 6967 6e61 6c20 6e61 6d65 3d22 6163 7469  ignal name="acti
-00002370: 7661 7465 2220 6861 6e64 6c65 723d 226d  vate" handler="m
-00002380: 656e 755f 7261 6365 5f64 6563 6973 696f  enu_race_decisio
-00002390: 6e73 5f61 6374 6976 6174 655f 6362 222f  ns_activate_cb"/
-000023a0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000023b0: 2020 2020 2020 2020 2020 2020 3c2f 6f62              </ob
-000023c0: 6a65 6374 3e0a 2020 2020 2020 2020 2020  ject>.          
-000023d0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-000023e0: 6368 696c 643e 0a20 2020 2020 2020 2020  child>.         
-000023f0: 2020 2020 2020 2020 2020 2020 203c 2f6f               </o
-00002400: 626a 6563 743e 0a20 2020 2020 2020 2020  bject>.         
-00002410: 2020 2020 2020 2020 2020 203c 2f63 6869             </chi
-00002420: 6c64 3e0a 2020 2020 2020 2020 2020 2020  ld>.            
-00002430: 2020 2020 2020 3c2f 6f62 6a65 6374 3e0a        </object>.
-00002440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002450: 3c2f 6368 696c 643e 0a20 2020 2020 2020  </child>.       
-00002460: 2020 2020 2020 2020 203c 6368 696c 643e           <child>
-00002470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002480: 2020 203c 6f62 6a65 6374 2063 6c61 7373     <object class
-00002490: 3d22 4774 6b4d 656e 7549 7465 6d22 2069  ="GtkMenuItem" i
-000024a0: 643d 226d 656e 755f 7265 706f 7274 7322  d="menu_reports"
-000024b0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000024c0: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
-000024d0: 6e61 6d65 3d22 7669 7369 626c 6522 3e54  name="visible">T
-000024e0: 7275 653c 2f70 726f 7065 7274 793e 0a20  rue</property>. 
-000024f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002500: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00002510: 653d 226c 6162 656c 2220 7472 616e 736c  e="label" transl
-00002520: 6174 6162 6c65 3d22 7965 7322 3e52 5f65  atable="yes">R_e
-00002530: 706f 7274 733c 2f70 726f 7065 7274 793e  ports</property>
-00002540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002550: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00002560: 616d 653d 2275 7365 5f75 6e64 6572 6c69  ame="use_underli
-00002570: 6e65 223e 5472 7565 3c2f 7072 6f70 6572  ne">True</proper
-00002580: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
-00002590: 2020 2020 2020 2020 3c63 6869 6c64 2074          <child t
-000025a0: 7970 653d 2273 7562 6d65 6e75 223e 0a20  ype="submenu">. 
-000025b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025c0: 2020 2020 203c 6f62 6a65 6374 2063 6c61       <object cla
-000025d0: 7373 3d22 4774 6b4d 656e 7522 2069 643d  ss="GtkMenu" id=
-000025e0: 226d 656e 7535 223e 0a20 2020 2020 2020  "menu5">.       
-000025f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002600: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-00002610: 2276 6973 6962 6c65 223e 5472 7565 3c2f  "visible">True</
-00002620: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
-00002630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002640: 2020 3c63 6869 6c64 3e0a 2020 2020 2020    <child>.      
-00002650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002660: 2020 2020 3c6f 626a 6563 7420 636c 6173      <object clas
-00002670: 733d 2247 746b 496d 6167 654d 656e 7549  s="GtkImageMenuI
-00002680: 7465 6d22 2069 643d 226d 656e 755f 7265  tem" id="menu_re
-00002690: 706f 7274 735f 7374 6172 746c 6973 7422  ports_startlist"
-000026a0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000026b0: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-000026c0: 726f 7065 7274 7920 6e61 6d65 3d22 6c61  roperty name="la
-000026d0: 6265 6c22 2074 7261 6e73 6c61 7461 626c  bel" translatabl
-000026e0: 653d 2279 6573 223e 5f53 7461 7274 6c69  e="yes">_Startli
-000026f0: 7374 3c2f 7072 6f70 6572 7479 3e0a 2020  st</property>.  
-00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002710: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00002720: 7274 7920 6e61 6d65 3d22 7669 7369 626c  rty name="visibl
-00002730: 6522 3e54 7275 653c 2f70 726f 7065 7274  e">True</propert
-00002740: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
-00002750: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002760: 7072 6f70 6572 7479 206e 616d 653d 2274  property name="t
-00002770: 6f6f 6c74 6970 5f74 6578 7422 2074 7261  ooltip_text" tra
-00002780: 6e73 6c61 7461 626c 653d 2279 6573 223e  nslatable="yes">
-00002790: 4576 656e 7420 7374 6172 746c 6973 7420  Event startlist 
-000027a0: 7265 706f 7274 3c2f 7072 6f70 6572 7479  report</property
-000027b0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000027c0: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-000027d0: 726f 7065 7274 7920 6e61 6d65 3d22 7573  roperty name="us
-000027e0: 655f 756e 6465 726c 696e 6522 3e54 7275  e_underline">Tru
-000027f0: 653c 2f70 726f 7065 7274 793e 0a20 2020  e</property>.   
-00002800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002810: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-00002820: 7479 206e 616d 653d 2269 6d61 6765 223e  ty name="image">
-00002830: 696d 6167 6531 303c 2f70 726f 7065 7274  image10</propert
-00002840: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
-00002850: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002860: 7072 6f70 6572 7479 206e 616d 653d 2275  property name="u
-00002870: 7365 5f73 746f 636b 223e 4661 6c73 653c  se_stock">False<
-00002880: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
-00002890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028a0: 2020 2020 2020 203c 6163 6365 6c65 7261         <accelera
-000028b0: 746f 7220 6b65 793d 2246 3322 2073 6967  tor key="F3" sig
-000028c0: 6e61 6c3d 2261 6374 6976 6174 6522 2f3e  nal="activate"/>
-000028d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000028e0: 2020 2020 2020 2020 2020 2020 203c 7369               <si
-000028f0: 676e 616c 206e 616d 653d 2261 6374 6976  gnal name="activ
-00002900: 6174 6522 2068 616e 646c 6572 3d22 6d65  ate" handler="me
-00002910: 6e75 5f72 6570 6f72 7473 5f73 7461 7274  nu_reports_start
-00002920: 6c69 7374 5f61 6374 6976 6174 655f 6362  list_activate_cb
-00002930: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00002940: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00002950: 6f62 6a65 6374 3e0a 2020 2020 2020 2020  object>.        
-00002960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002970: 3c2f 6368 696c 643e 0a20 2020 2020 2020  </child>.       
-00002980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002990: 203c 6368 696c 643e 0a20 2020 2020 2020   <child>.       
-000029a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029b0: 2020 203c 6f62 6a65 6374 2063 6c61 7373     <object class
-000029c0: 3d22 4774 6b4d 656e 7549 7465 6d22 2069  ="GtkMenuItem" i
-000029d0: 643d 226d 656e 755f 7265 706f 7274 735f  d="menu_reports_
-000029e0: 6361 6c6c 7570 223e 0a20 2020 2020 2020  callup">.       
-000029f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a00: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00002a10: 616d 653d 226c 6162 656c 2220 7472 616e  ame="label" tran
-00002a20: 736c 6174 6162 6c65 3d22 7965 7322 3e5f  slatable="yes">_
-00002a30: 4361 6c6c 7570 3c2f 7072 6f70 6572 7479  Callup</property
-00002a40: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00002a50: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-00002a60: 726f 7065 7274 7920 6e61 6d65 3d22 7669  roperty name="vi
-00002a70: 7369 626c 6522 3e54 7275 653c 2f70 726f  sible">True</pro
-00002a80: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
+00002020: 3c2f 6368 696c 643e 0a20 2020 2020 2020  </child>.       
+00002030: 2020 2020 2020 2020 2020 203c 2f6f 626a             </obj
+00002040: 6563 743e 0a20 2020 2020 2020 2020 2020  ect>.           
+00002050: 2020 2020 203c 2f63 6869 6c64 3e0a 2020       </child>.  
+00002060: 2020 2020 2020 2020 2020 2020 2020 3c63                <c
+00002070: 6869 6c64 3e0a 2020 2020 2020 2020 2020  hild>.          
+00002080: 2020 2020 2020 2020 3c6f 626a 6563 7420          <object 
+00002090: 636c 6173 733d 2247 746b 4d65 6e75 4974  class="GtkMenuIt
+000020a0: 656d 2220 6964 3d22 6d65 6e75 5f72 6570  em" id="menu_rep
+000020b0: 6f72 7473 223e 0a20 2020 2020 2020 2020  orts">.         
+000020c0: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
+000020d0: 6572 7479 206e 616d 653d 2276 6973 6962  erty name="visib
+000020e0: 6c65 223e 5472 7565 3c2f 7072 6f70 6572  le">True</proper
+000020f0: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
+00002100: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
+00002110: 7920 6e61 6d65 3d22 6c61 6265 6c22 3e52  y name="label">R
+00002120: 5f65 706f 7274 733c 2f70 726f 7065 7274  _eports</propert
+00002130: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
+00002140: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+00002150: 206e 616d 653d 2275 7365 5f75 6e64 6572   name="use_under
+00002160: 6c69 6e65 223e 5472 7565 3c2f 7072 6f70  line">True</prop
+00002170: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
+00002180: 2020 2020 2020 2020 2020 3c63 6869 6c64            <child
+00002190: 2074 7970 653d 2273 7562 6d65 6e75 223e   type="submenu">
+000021a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000021b0: 2020 2020 2020 203c 6f62 6a65 6374 2063         <object c
+000021c0: 6c61 7373 3d22 4774 6b4d 656e 7522 2069  lass="GtkMenu" i
+000021d0: 643d 226d 656e 7535 223e 0a20 2020 2020  d="menu5">.     
+000021e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021f0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+00002200: 653d 2276 6973 6962 6c65 223e 5472 7565  e="visible">True
+00002210: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+00002220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002230: 2020 2020 3c63 6869 6c64 3e0a 2020 2020      <child>.    
+00002240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002250: 2020 2020 2020 3c6f 626a 6563 7420 636c        <object cl
+00002260: 6173 733d 2247 746b 4d65 6e75 4974 656d  ass="GtkMenuItem
+00002270: 2220 6964 3d22 6d65 6e75 5f72 6570 6f72  " id="menu_repor
+00002280: 7473 5f73 7461 7274 6c69 7374 223e 0a20  ts_startlist">. 
+00002290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022a0: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
+000022b0: 6572 7479 206e 616d 653d 226c 6162 656c  erty name="label
+000022c0: 223e 5f53 7461 7274 6c69 7374 3c2f 7072  ">_Startlist</pr
+000022d0: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
+000022e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022f0: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00002300: 6d65 3d22 7669 7369 626c 6522 3e54 7275  me="visible">Tru
+00002310: 653c 2f70 726f 7065 7274 793e 0a20 2020  e</property>.   
+00002320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002330: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+00002340: 7479 206e 616d 653d 2275 7365 5f75 6e64  ty name="use_und
+00002350: 6572 6c69 6e65 223e 5472 7565 3c2f 7072  erline">True</pr
+00002360: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
+00002370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002380: 2020 2020 3c61 6363 656c 6572 6174 6f72      <accelerator
+00002390: 206b 6579 3d22 4633 2220 7369 676e 616c   key="F3" signal
+000023a0: 3d22 6163 7469 7661 7465 222f 3e0a 2020  ="activate"/>.  
+000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023c0: 2020 2020 2020 2020 2020 3c73 6967 6e61            <signa
+000023d0: 6c20 6e61 6d65 3d22 6163 7469 7661 7465  l name="activate
+000023e0: 2220 6861 6e64 6c65 723d 226d 656e 755f  " handler="menu_
+000023f0: 7265 706f 7274 735f 7374 6172 746c 6973  reports_startlis
+00002400: 745f 6163 7469 7661 7465 5f63 6222 2f3e  t_activate_cb"/>
+00002410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002420: 2020 2020 2020 2020 2020 203c 2f6f 626a             </obj
+00002430: 6563 743e 0a20 2020 2020 2020 2020 2020  ect>.           
+00002440: 2020 2020 2020 2020 2020 2020 203c 2f63               </c
+00002450: 6869 6c64 3e0a 2020 2020 2020 2020 2020  hild>.          
+00002460: 2020 2020 2020 2020 2020 2020 2020 3c63                <c
+00002470: 6869 6c64 3e0a 2020 2020 2020 2020 2020  hild>.          
+00002480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002490: 3c6f 626a 6563 7420 636c 6173 733d 2247  <object class="G
+000024a0: 746b 4d65 6e75 4974 656d 2220 6964 3d22  tkMenuItem" id="
+000024b0: 6d65 6e75 5f72 6570 6f72 7473 5f63 616c  menu_reports_cal
+000024c0: 6c75 7022 3e0a 2020 2020 2020 2020 2020  lup">.          
+000024d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024e0: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+000024f0: 3d22 6c61 6265 6c22 3e5f 4361 6c6c 7570  ="label">_Callup
+00002500: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+00002510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002520: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
+00002530: 7920 6e61 6d65 3d22 7669 7369 626c 6522  y name="visible"
+00002540: 3e54 7275 653c 2f70 726f 7065 7274 793e  >True</property>
+00002550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002560: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
+00002570: 6f70 6572 7479 206e 616d 653d 2275 7365  operty name="use
+00002580: 5f75 6e64 6572 6c69 6e65 223e 5472 7565  _underline">True
+00002590: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+000025a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025b0: 2020 2020 2020 2020 3c61 6363 656c 6572          <acceler
+000025c0: 6174 6f72 206b 6579 3d22 4633 2220 7369  ator key="F3" si
+000025d0: 676e 616c 3d22 6163 7469 7661 7465 2220  gnal="activate" 
+000025e0: 6d6f 6469 6669 6572 733d 2247 444b 5f43  modifiers="GDK_C
+000025f0: 4f4e 5452 4f4c 5f4d 4153 4b22 2f3e 0a20  ONTROL_MASK"/>. 
+00002600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002610: 2020 2020 2020 2020 2020 203c 7369 676e             <sign
+00002620: 616c 206e 616d 653d 2261 6374 6976 6174  al name="activat
+00002630: 6522 2068 616e 646c 6572 3d22 6d65 6e75  e" handler="menu
+00002640: 5f72 6570 6f72 7473 5f63 616c 6c75 705f  _reports_callup_
+00002650: 6163 7469 7661 7465 5f63 6222 2f3e 0a20  activate_cb"/>. 
+00002660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002670: 2020 2020 2020 2020 203c 2f6f 626a 6563           </objec
+00002680: 743e 0a20 2020 2020 2020 2020 2020 2020  t>.             
+00002690: 2020 2020 2020 2020 2020 203c 2f63 6869             </chi
+000026a0: 6c64 3e0a 2020 2020 2020 2020 2020 2020  ld>.            
+000026b0: 2020 2020 2020 2020 2020 2020 3c63 6869              <chi
+000026c0: 6c64 3e0a 2020 2020 2020 2020 2020 2020  ld>.            
+000026d0: 2020 2020 2020 2020 2020 2020 2020 3c6f                <o
+000026e0: 626a 6563 7420 636c 6173 733d 2247 746b  bject class="Gtk
+000026f0: 4d65 6e75 4974 656d 2220 6964 3d22 6d65  MenuItem" id="me
+00002700: 6e75 5f72 6570 6f72 7473 5f61 6e61 6c79  nu_reports_analy
+00002710: 7369 7322 3e0a 2020 2020 2020 2020 2020  sis">.          
+00002720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002730: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+00002740: 3d22 6c61 6265 6c22 3e5f 416e 616c 7973  ="label">_Analys
+00002750: 6973 3c2f 7072 6f70 6572 7479 3e0a 2020  is</property>.  
+00002760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002770: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
+00002780: 7274 7920 6e61 6d65 3d22 7669 7369 626c  rty name="visibl
+00002790: 6522 3e54 7275 653c 2f70 726f 7065 7274  e">True</propert
+000027a0: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
+000027b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000027c0: 7072 6f70 6572 7479 206e 616d 653d 2275  property name="u
+000027d0: 7365 5f75 6e64 6572 6c69 6e65 223e 5472  se_underline">Tr
+000027e0: 7565 3c2f 7072 6f70 6572 7479 3e0a 2020  ue</property>.  
+000027f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002800: 2020 2020 2020 2020 2020 3c61 6363 656c            <accel
+00002810: 6572 6174 6f72 206b 6579 3d22 4632 2220  erator key="F2" 
+00002820: 7369 676e 616c 3d22 6163 7469 7661 7465  signal="activate
+00002830: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00002840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002850: 3c73 6967 6e61 6c20 6e61 6d65 3d22 6163  <signal name="ac
+00002860: 7469 7661 7465 2220 6861 6e64 6c65 723d  tivate" handler=
+00002870: 226d 656e 755f 7265 706f 7274 735f 616e  "menu_reports_an
+00002880: 616c 7973 6973 5f61 6374 6976 6174 655f  alysis_activate_
+00002890: 6362 222f 3e0a 2020 2020 2020 2020 2020  cb"/>.          
+000028a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028b0: 3c2f 6f62 6a65 6374 3e0a 2020 2020 2020  </object>.      
+000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028d0: 2020 3c2f 6368 696c 643e 0a20 2020 2020    </child>.     
+000028e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028f0: 2020 203c 6368 696c 643e 0a20 2020 2020     <child>.     
+00002900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002910: 2020 2020 203c 6f62 6a65 6374 2063 6c61       <object cla
+00002920: 7373 3d22 4774 6b4d 656e 7549 7465 6d22  ss="GtkMenuItem"
+00002930: 2069 643d 226d 656e 755f 7265 706f 7274   id="menu_report
+00002940: 735f 7369 676e 6f6e 223e 0a20 2020 2020  s_signon">.     
+00002950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002960: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+00002970: 206e 616d 653d 226c 6162 656c 223e 535f   name="label">S_
+00002980: 6967 6e6f 6e3c 2f70 726f 7065 7274 793e  ignon</property>
+00002990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000029a0: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
+000029b0: 6f70 6572 7479 206e 616d 653d 2276 6973  operty name="vis
+000029c0: 6962 6c65 223e 5472 7565 3c2f 7072 6f70  ible">True</prop
+000029d0: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
+000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029f0: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+00002a00: 3d22 7573 655f 756e 6465 726c 696e 6522  ="use_underline"
+00002a10: 3e54 7275 653c 2f70 726f 7065 7274 793e  >True</property>
+00002a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002a30: 2020 2020 2020 2020 2020 2020 203c 6163               <ac
+00002a40: 6365 6c65 7261 746f 7220 6b65 793d 2246  celerator key="F
+00002a50: 3222 2073 6967 6e61 6c3d 2261 6374 6976  2" signal="activ
+00002a60: 6174 6522 206d 6f64 6966 6965 7273 3d22  ate" modifiers="
+00002a70: 4744 4b5f 434f 4e54 524f 4c5f 4d41 534b  GDK_CONTROL_MASK
+00002a80: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
 00002a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002aa0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00002ab0: 653d 2274 6f6f 6c74 6970 5f74 6578 7422  e="tooltip_text"
-00002ac0: 2074 7261 6e73 6c61 7461 626c 653d 2279   translatable="y
-00002ad0: 6573 223e 5374 6172 7420 6c69 6e65 2063  es">Start line c
-00002ae0: 616c 6c2d 7570 2072 6570 6f72 743c 2f70  all-up report</p
-00002af0: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
-00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b10: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00002b20: 616d 653d 2275 7365 5f75 6e64 6572 6c69  ame="use_underli
-00002b30: 6e65 223e 5472 7565 3c2f 7072 6f70 6572  ne">True</proper
-00002b40: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
+00002aa0: 3c73 6967 6e61 6c20 6e61 6d65 3d22 6163  <signal name="ac
+00002ab0: 7469 7661 7465 2220 6861 6e64 6c65 723d  tivate" handler=
+00002ac0: 226d 656e 755f 7265 706f 7274 735f 7369  "menu_reports_si
+00002ad0: 676e 6f6e 5f61 6374 6976 6174 655f 6362  gnon_activate_cb
+00002ae0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00002af0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00002b00: 6f62 6a65 6374 3e0a 2020 2020 2020 2020  object>.        
+00002b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b20: 3c2f 6368 696c 643e 0a20 2020 2020 2020  </child>.       
+00002b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b40: 203c 6368 696c 643e 0a20 2020 2020 2020   <child>.       
 00002b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b60: 3c61 6363 656c 6572 6174 6f72 206b 6579  <accelerator key
-00002b70: 3d22 4633 2220 7369 676e 616c 3d22 6163  ="F3" signal="ac
-00002b80: 7469 7661 7465 2220 6d6f 6469 6669 6572  tivate" modifier
-00002b90: 733d 2247 444b 5f43 4f4e 5452 4f4c 5f4d  s="GDK_CONTROL_M
-00002ba0: 4153 4b22 2f3e 0a20 2020 2020 2020 2020  ASK"/>.         
-00002bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bc0: 2020 203c 7369 676e 616c 206e 616d 653d     <signal name=
-00002bd0: 2261 6374 6976 6174 6522 2068 616e 646c  "activate" handl
-00002be0: 6572 3d22 6d65 6e75 5f72 6570 6f72 7473  er="menu_reports
-00002bf0: 5f63 616c 6c75 705f 6163 7469 7661 7465  _callup_activate
-00002c00: 5f63 6222 2f3e 0a20 2020 2020 2020 2020  _cb"/>.         
-00002c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c20: 203c 2f6f 626a 6563 743e 0a20 2020 2020   </object>.     
+00002b60: 2020 203c 6f62 6a65 6374 2063 6c61 7373     <object class
+00002b70: 3d22 4774 6b4d 656e 7549 7465 6d22 2069  ="GtkMenuItem" i
+00002b80: 643d 226d 656e 755f 7265 706f 7274 735f  d="menu_reports_
+00002b90: 6361 6d65 7261 223e 0a20 2020 2020 2020  camera">.       
+00002ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bb0: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+00002bc0: 616d 653d 226c 6162 656c 223e 5f4a 7564  ame="label">_Jud
+00002bd0: 6765 7320 466f 726d 3c2f 7072 6f70 6572  ges Form</proper
+00002be0: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
+00002bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c00: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+00002c10: 7669 7369 626c 6522 3e54 7275 653c 2f70  visible">True</p
+00002c20: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
 00002c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c40: 2020 203c 2f63 6869 6c64 3e0a 2020 2020     </child>.    
-00002c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c60: 2020 2020 3c63 6869 6c64 3e0a 2020 2020      <child>.    
-00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c80: 2020 2020 2020 3c6f 626a 6563 7420 636c        <object cl
-00002c90: 6173 733d 2247 746b 4d65 6e75 4974 656d  ass="GtkMenuItem
-00002ca0: 2220 6964 3d22 6d65 6e75 5f72 6570 6f72  " id="menu_repor
-00002cb0: 7473 5f61 6e61 6c79 7369 7322 3e0a 2020  ts_analysis">.  
+00002c40: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+00002c50: 616d 653d 2275 7365 5f75 6e64 6572 6c69  ame="use_underli
+00002c60: 6e65 223e 5472 7565 3c2f 7072 6f70 6572  ne">True</proper
+00002c70: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
+00002c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c90: 3c61 6363 656c 6572 6174 6f72 206b 6579  <accelerator key
+00002ca0: 3d22 4631 3122 2073 6967 6e61 6c3d 2261  ="F11" signal="a
+00002cb0: 6374 6976 6174 6522 2f3e 0a20 2020 2020  ctivate"/>.     
 00002cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cd0: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00002ce0: 7274 7920 6e61 6d65 3d22 6c61 6265 6c22  rty name="label"
-00002cf0: 2074 7261 6e73 6c61 7461 626c 653d 2279   translatable="y
-00002d00: 6573 223e 5f41 6e61 6c79 7369 733c 2f70  es">_Analysis</p
-00002d10: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
+00002cd0: 2020 2020 2020 203c 7369 676e 616c 206e         <signal n
+00002ce0: 616d 653d 2261 6374 6976 6174 6522 2068  ame="activate" h
+00002cf0: 616e 646c 6572 3d22 6d65 6e75 5f72 6570  andler="menu_rep
+00002d00: 6f72 7473 5f63 616d 6572 615f 6163 7469  orts_camera_acti
+00002d10: 7661 7465 5f63 6222 2f3e 0a20 2020 2020  vate_cb"/>.     
 00002d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d30: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00002d40: 616d 653d 2276 6973 6962 6c65 223e 5472  ame="visible">Tr
-00002d50: 7565 3c2f 7072 6f70 6572 7479 3e0a 2020  ue</property>.  
+00002d30: 2020 2020 203c 2f6f 626a 6563 743e 0a20       </object>. 
+00002d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d50: 2020 2020 2020 203c 2f63 6869 6c64 3e0a         </child>.
 00002d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d70: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00002d80: 7274 7920 6e61 6d65 3d22 746f 6f6c 7469  rty name="toolti
-00002d90: 705f 7465 7874 2220 7472 616e 736c 6174  p_text" translat
-00002da0: 6162 6c65 3d22 7965 7322 3e45 7665 6e74  able="yes">Event
-00002db0: 2061 6e61 6c79 7369 7320 7265 706f 7274   analysis report
-00002dc0: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-00002dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002de0: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-00002df0: 7920 6e61 6d65 3d22 7573 655f 756e 6465  y name="use_unde
-00002e00: 726c 696e 6522 3e54 7275 653c 2f70 726f  rline">True</pro
-00002e10: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
+00002d70: 2020 2020 2020 2020 3c63 6869 6c64 3e0a          <child>.
+00002d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d90: 2020 2020 2020 2020 2020 3c6f 626a 6563            <objec
+00002da0: 7420 636c 6173 733d 2247 746b 4d65 6e75  t class="GtkMenu
+00002db0: 4974 656d 2220 6964 3d22 6576 656e 745f  Item" id="event_
+00002dc0: 7265 7375 6c74 735f 706f 696e 7473 223e  results_points">
+00002dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002de0: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
+00002df0: 6f70 6572 7479 206e 616d 653d 226c 6162  operty name="lab
+00002e00: 656c 223e 5f50 6f69 6e74 7320 5461 6c6c  el">_Points Tall
+00002e10: 793c 2f70 726f 7065 7274 793e 0a20 2020  y</property>.   
 00002e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e30: 2020 203c 6163 6365 6c65 7261 746f 7220     <accelerator 
-00002e40: 6b65 793d 2246 3222 2073 6967 6e61 6c3d  key="F2" signal=
-00002e50: 2261 6374 6976 6174 6522 2f3e 0a20 2020  "activate"/>.   
-00002e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e70: 2020 2020 2020 2020 203c 7369 676e 616c           <signal
-00002e80: 206e 616d 653d 2261 6374 6976 6174 6522   name="activate"
-00002e90: 2068 616e 646c 6572 3d22 6d65 6e75 5f72   handler="menu_r
-00002ea0: 6570 6f72 7473 5f61 6e61 6c79 7369 735f  eports_analysis_
-00002eb0: 6163 7469 7661 7465 5f63 6222 2f3e 0a20  activate_cb"/>. 
-00002ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ed0: 2020 2020 2020 2020 203c 2f6f 626a 6563           </objec
-00002ee0: 743e 0a20 2020 2020 2020 2020 2020 2020  t>.             
-00002ef0: 2020 2020 2020 2020 2020 203c 2f63 6869             </chi
-00002f00: 6c64 3e0a 2020 2020 2020 2020 2020 2020  ld>.            
-00002f10: 2020 2020 2020 2020 2020 2020 3c63 6869              <chi
-00002f20: 6c64 3e0a 2020 2020 2020 2020 2020 2020  ld>.            
-00002f30: 2020 2020 2020 2020 2020 2020 2020 3c6f                <o
-00002f40: 626a 6563 7420 636c 6173 733d 2247 746b  bject class="Gtk
-00002f50: 496d 6167 654d 656e 7549 7465 6d22 2069  ImageMenuItem" i
-00002f60: 643d 226d 656e 755f 7265 706f 7274 735f  d="menu_reports_
-00002f70: 7369 676e 6f6e 223e 0a20 2020 2020 2020  signon">.       
-00002f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f90: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00002fa0: 616d 653d 226c 6162 656c 2220 7472 616e  ame="label" tran
-00002fb0: 736c 6174 6162 6c65 3d22 7965 7322 3e53  slatable="yes">S
-00002fc0: 5f69 676e 6f6e 3c2f 7072 6f70 6572 7479  _ignon</property
-00002fd0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00002fe0: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-00002ff0: 726f 7065 7274 7920 6e61 6d65 3d22 7669  roperty name="vi
-00003000: 7369 626c 6522 3e54 7275 653c 2f70 726f  sible">True</pro
-00003010: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
-00003020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003030: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00003040: 653d 2274 6f6f 6c74 6970 5f74 6578 7422  e="tooltip_text"
-00003050: 2074 7261 6e73 6c61 7461 626c 653d 2279   translatable="y
-00003060: 6573 223e 4576 656e 7420 7369 676e 2d6f  es">Event sign-o
-00003070: 6e20 7265 706f 7274 3c2f 7072 6f70 6572  n report</proper
-00003080: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
-00003090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030a0: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-000030b0: 7573 655f 756e 6465 726c 696e 6522 3e54  use_underline">T
-000030c0: 7275 653c 2f70 726f 7065 7274 793e 0a20  rue</property>. 
-000030d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030e0: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
-000030f0: 6572 7479 206e 616d 653d 2269 6d61 6765  erty name="image
-00003100: 223e 696d 6167 6532 323c 2f70 726f 7065  ">image22</prope
-00003110: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
-00003120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003130: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-00003140: 2275 7365 5f73 746f 636b 223e 4661 6c73  "use_stock">Fals
-00003150: 653c 2f70 726f 7065 7274 793e 0a20 2020  e</property>.   
-00003160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003170: 2020 2020 2020 2020 203c 6163 6365 6c65           <accele
-00003180: 7261 746f 7220 6b65 793d 2246 3222 2073  rator key="F2" s
-00003190: 6967 6e61 6c3d 2261 6374 6976 6174 6522  ignal="activate"
-000031a0: 206d 6f64 6966 6965 7273 3d22 4744 4b5f   modifiers="GDK_
-000031b0: 434f 4e54 524f 4c5f 4d41 534b 222f 3e0a  CONTROL_MASK"/>.
-000031c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031d0: 2020 2020 2020 2020 2020 2020 3c73 6967              <sig
-000031e0: 6e61 6c20 6e61 6d65 3d22 6163 7469 7661  nal name="activa
-000031f0: 7465 2220 6861 6e64 6c65 723d 226d 656e  te" handler="men
-00003200: 755f 7265 706f 7274 735f 7369 676e 6f6e  u_reports_signon
-00003210: 5f61 6374 6976 6174 655f 6362 222f 3e0a  _activate_cb"/>.
-00003220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003230: 2020 2020 2020 2020 2020 3c2f 6f62 6a65            </obje
-00003240: 6374 3e0a 2020 2020 2020 2020 2020 2020  ct>.            
-00003250: 2020 2020 2020 2020 2020 2020 3c2f 6368              </ch
-00003260: 696c 643e 0a20 2020 2020 2020 2020 2020  ild>.           
-00003270: 2020 2020 2020 2020 2020 2020 203c 6368               <ch
-00003280: 696c 643e 0a20 2020 2020 2020 2020 2020  ild>.           
-00003290: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000032a0: 6f62 6a65 6374 2063 6c61 7373 3d22 4774  object class="Gt
-000032b0: 6b49 6d61 6765 4d65 6e75 4974 656d 2220  kImageMenuItem" 
-000032c0: 6964 3d22 6d65 6e75 5f72 6570 6f72 7473  id="menu_reports
-000032d0: 5f63 616d 6572 6122 3e0a 2020 2020 2020  _camera">.      
-000032e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032f0: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
-00003300: 6e61 6d65 3d22 6c61 6265 6c22 2074 7261  name="label" tra
-00003310: 6e73 6c61 7461 626c 653d 2279 6573 223e  nslatable="yes">
-00003320: 5f4a 7564 6765 7320 466f 726d 3c2f 7072  _Judges Form</pr
-00003330: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
-00003340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003350: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00003360: 6d65 3d22 7669 7369 626c 6522 3e54 7275  me="visible">Tru
-00003370: 653c 2f70 726f 7065 7274 793e 0a20 2020  e</property>.   
-00003380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003390: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-000033a0: 7479 206e 616d 653d 2274 6f6f 6c74 6970  ty name="tooltip
-000033b0: 5f74 6578 7422 2074 7261 6e73 6c61 7461  _text" translata
-000033c0: 626c 653d 2279 6573 223e 4576 656e 7420  ble="yes">Event 
-000033d0: 6a75 6467 6573 2072 6570 6f72 743c 2f70  judges report</p
-000033e0: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
-000033f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003400: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00003410: 616d 653d 2275 7365 5f75 6e64 6572 6c69  ame="use_underli
-00003420: 6e65 223e 5472 7565 3c2f 7072 6f70 6572  ne">True</proper
-00003430: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
-00003440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003450: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00003460: 696d 6167 6522 3e69 6d61 6765 3133 3c2f  image">image13</
-00003470: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
-00003480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003490: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
-000034a0: 6e61 6d65 3d22 7573 655f 7374 6f63 6b22  name="use_stock"
-000034b0: 3e46 616c 7365 3c2f 7072 6f70 6572 7479  >False</property
-000034c0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000034d0: 2020 2020 2020 2020 2020 2020 2020 3c61                <a
-000034e0: 6363 656c 6572 6174 6f72 206b 6579 3d22  ccelerator key="
-000034f0: 4631 3122 2073 6967 6e61 6c3d 2261 6374  F11" signal="act
-00003500: 6976 6174 6522 2f3e 0a20 2020 2020 2020  ivate"/>.       
-00003510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003520: 2020 2020 203c 7369 676e 616c 206e 616d       <signal nam
-00003530: 653d 2261 6374 6976 6174 6522 2068 616e  e="activate" han
-00003540: 646c 6572 3d22 6d65 6e75 5f72 6570 6f72  dler="menu_repor
-00003550: 7473 5f63 616d 6572 615f 6163 7469 7661  ts_camera_activa
-00003560: 7465 5f63 6222 2f3e 0a20 2020 2020 2020  te_cb"/>.       
+00002e30: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+00002e40: 7479 206e 616d 653d 2276 6973 6962 6c65  ty name="visible
+00002e50: 223e 5472 7565 3c2f 7072 6f70 6572 7479  ">True</property
+00002e60: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00002e70: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
+00002e80: 726f 7065 7274 7920 6e61 6d65 3d22 7573  roperty name="us
+00002e90: 655f 756e 6465 726c 696e 6522 3e54 7275  e_underline">Tru
+00002ea0: 653c 2f70 726f 7065 7274 793e 0a20 2020  e</property>.   
+00002eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ec0: 2020 2020 2020 2020 203c 6163 6365 6c65           <accele
+00002ed0: 7261 746f 7220 6b65 793d 2246 3131 2220  rator key="F11" 
+00002ee0: 7369 676e 616c 3d22 6163 7469 7661 7465  signal="activate
+00002ef0: 2220 6d6f 6469 6669 6572 733d 2247 444b  " modifiers="GDK
+00002f00: 5f43 4f4e 5452 4f4c 5f4d 4153 4b22 2f3e  _CONTROL_MASK"/>
+00002f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002f20: 2020 2020 2020 2020 2020 2020 203c 7369               <si
+00002f30: 676e 616c 206e 616d 653d 2261 6374 6976  gnal name="activ
+00002f40: 6174 6522 2068 616e 646c 6572 3d22 6576  ate" handler="ev
+00002f50: 656e 745f 7265 7375 6c74 735f 706f 696e  ent_results_poin
+00002f60: 7473 5f61 6374 6976 6174 655f 6362 222f  ts_activate_cb"/
+00002f70: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00002f80: 2020 2020 2020 2020 2020 2020 3c2f 6f62              </ob
+00002f90: 6a65 6374 3e0a 2020 2020 2020 2020 2020  ject>.          
+00002fa0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00002fb0: 6368 696c 643e 0a20 2020 2020 2020 2020  child>.         
+00002fc0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00002fd0: 6368 696c 643e 0a20 2020 2020 2020 2020  child>.         
+00002fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ff0: 203c 6f62 6a65 6374 2063 6c61 7373 3d22   <object class="
+00003000: 4774 6b4d 656e 7549 7465 6d22 2069 643d  GtkMenuItem" id=
+00003010: 226d 656e 755f 7265 706f 7274 735f 7265  "menu_reports_re
+00003020: 7375 6c74 223e 0a20 2020 2020 2020 2020  sult">.         
+00003030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003040: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+00003050: 653d 226c 6162 656c 223e 5f52 6573 756c  e="label">_Resul
+00003060: 743c 2f70 726f 7065 7274 793e 0a20 2020  t</property>.   
+00003070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003080: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+00003090: 7479 206e 616d 653d 2276 6973 6962 6c65  ty name="visible
+000030a0: 223e 5472 7565 3c2f 7072 6f70 6572 7479  ">True</property
+000030b0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000030c0: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
+000030d0: 726f 7065 7274 7920 6e61 6d65 3d22 7573  roperty name="us
+000030e0: 655f 756e 6465 726c 696e 6522 3e54 7275  e_underline">Tru
+000030f0: 653c 2f70 726f 7065 7274 793e 0a20 2020  e</property>.   
+00003100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003110: 2020 2020 2020 2020 203c 6163 6365 6c65           <accele
+00003120: 7261 746f 7220 6b65 793d 2246 3132 2220  rator key="F12" 
+00003130: 7369 676e 616c 3d22 6163 7469 7661 7465  signal="activate
+00003140: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00003150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003160: 3c73 6967 6e61 6c20 6e61 6d65 3d22 6163  <signal name="ac
+00003170: 7469 7661 7465 2220 6861 6e64 6c65 723d  tivate" handler=
+00003180: 226d 656e 755f 7265 706f 7274 735f 7265  "menu_reports_re
+00003190: 7375 6c74 5f61 6374 6976 6174 655f 6362  sult_activate_cb
+000031a0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+000031b0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+000031c0: 6f62 6a65 6374 3e0a 2020 2020 2020 2020  object>.        
+000031d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031e0: 3c2f 6368 696c 643e 0a20 2020 2020 2020  </child>.       
+000031f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003200: 203c 6368 696c 643e 0a20 2020 2020 2020   <child>.       
+00003210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003220: 2020 203c 6f62 6a65 6374 2063 6c61 7373     <object class
+00003230: 3d22 4774 6b53 6570 6172 6174 6f72 4d65  ="GtkSeparatorMe
+00003240: 6e75 4974 656d 2220 6964 3d22 6d65 6e75  nuItem" id="menu
+00003250: 5f72 6570 6f72 7473 5f73 6570 222f 3e0a  _reports_sep"/>.
+00003260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003270: 2020 2020 2020 2020 3c2f 6368 696c 643e          </child>
+00003280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003290: 2020 2020 2020 203c 2f6f 626a 6563 743e         </object>
+000032a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000032b0: 2020 2020 203c 2f63 6869 6c64 3e0a 2020       </child>.  
+000032c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032d0: 3c2f 6f62 6a65 6374 3e0a 2020 2020 2020  </object>.      
+000032e0: 2020 2020 2020 2020 2020 3c2f 6368 696c            </chil
+000032f0: 643e 0a20 2020 2020 2020 2020 2020 2020  d>.             
+00003300: 2020 203c 6368 696c 643e 0a20 2020 2020     <child>.     
+00003310: 2020 2020 2020 2020 2020 2020 203c 6f62               <ob
+00003320: 6a65 6374 2063 6c61 7373 3d22 4774 6b4d  ject class="GtkM
+00003330: 656e 7549 7465 6d22 2069 643d 226d 656e  enuItem" id="men
+00003340: 755f 6461 7461 223e 0a20 2020 2020 2020  u_data">.       
+00003350: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
+00003360: 6f70 6572 7479 206e 616d 653d 2276 6973  operty name="vis
+00003370: 6962 6c65 223e 5472 7565 3c2f 7072 6f70  ible">True</prop
+00003380: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
+00003390: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
+000033a0: 7274 7920 6e61 6d65 3d22 6c61 6265 6c22  rty name="label"
+000033b0: 3e5f 4461 7461 3c2f 7072 6f70 6572 7479  >_Data</property
+000033c0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000033d0: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+000033e0: 6e61 6d65 3d22 7573 655f 756e 6465 726c  name="use_underl
+000033f0: 696e 6522 3e54 7275 653c 2f70 726f 7065  ine">True</prope
+00003400: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
+00003410: 2020 2020 2020 2020 203c 6368 696c 6420           <child 
+00003420: 7479 7065 3d22 7375 626d 656e 7522 3e0a  type="submenu">.
+00003430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003440: 2020 2020 2020 3c6f 626a 6563 7420 636c        <object cl
+00003450: 6173 733d 2247 746b 4d65 6e75 2220 6964  ass="GtkMenu" id
+00003460: 3d22 6d65 6e75 3222 3e0a 2020 2020 2020  ="menu2">.      
+00003470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003480: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+00003490: 3d22 7669 7369 626c 6522 3e54 7275 653c  ="visible">True<
+000034a0: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
+000034b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034c0: 2020 203c 6368 696c 643e 0a20 2020 2020     <child>.     
+000034d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034e0: 2020 2020 203c 6f62 6a65 6374 2063 6c61       <object cla
+000034f0: 7373 3d22 4774 6b4d 656e 7549 7465 6d22  ss="GtkMenuItem"
+00003500: 2069 643d 226d 656e 755f 6461 7461 5f72   id="menu_data_r
+00003510: 6570 6c61 6365 223e 0a20 2020 2020 2020  eplace">.       
+00003520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003530: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+00003540: 616d 653d 226c 6162 656c 223e 5265 5f70  ame="label">Re_p
+00003550: 6c61 6365 2052 6964 6572 733c 2f70 726f  lace Riders</pro
+00003560: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
 00003570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003580: 2020 203c 2f6f 626a 6563 743e 0a20 2020     </object>.   
-00003590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035a0: 2020 2020 203c 2f63 6869 6c64 3e0a 2020       </child>.  
+00003580: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+00003590: 653d 2276 6973 6962 6c65 223e 5472 7565  e="visible">True
+000035a0: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
 000035b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035c0: 2020 2020 2020 3c63 6869 6c64 3e0a 2020        <child>.  
-000035d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035e0: 2020 2020 2020 2020 3c6f 626a 6563 7420          <object 
-000035f0: 636c 6173 733d 2247 746b 496d 6167 654d  class="GtkImageM
-00003600: 656e 7549 7465 6d22 2069 643d 2272 6163  enuItem" id="rac
-00003610: 655f 7265 7375 6c74 735f 706f 696e 7473  e_results_points
-00003620: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00003630: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00003640: 7072 6f70 6572 7479 206e 616d 653d 226c  property name="l
-00003650: 6162 656c 2220 7472 616e 736c 6174 6162  abel" translatab
-00003660: 6c65 3d22 7965 7322 3e5f 506f 696e 7473  le="yes">_Points
-00003670: 2054 616c 6c79 3c2f 7072 6f70 6572 7479   Tally</property
-00003680: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00003690: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-000036a0: 726f 7065 7274 7920 6e61 6d65 3d22 7669  roperty name="vi
-000036b0: 7369 626c 6522 3e54 7275 653c 2f70 726f  sible">True</pro
-000036c0: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
-000036d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036e0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-000036f0: 653d 2274 6f6f 6c74 6970 5f74 6578 7422  e="tooltip_text"
-00003700: 2074 7261 6e73 6c61 7461 626c 653d 2279   translatable="y
-00003710: 6573 223e 506f 696e 7473 2074 616c 6c79  es">Points tally
-00003720: 2072 6570 6f72 743c 2f70 726f 7065 7274   report</propert
-00003730: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
-00003740: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00003750: 7072 6f70 6572 7479 206e 616d 653d 2275  property name="u
-00003760: 7365 5f75 6e64 6572 6c69 6e65 223e 5472  se_underline">Tr
-00003770: 7565 3c2f 7072 6f70 6572 7479 3e0a 2020  ue</property>.  
-00003780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003790: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-000037a0: 7274 7920 6e61 6d65 3d22 696d 6167 6522  rty name="image"
-000037b0: 3e69 6d61 6765 3137 3c2f 7072 6f70 6572  >image17</proper
-000037c0: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
-000037d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037e0: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-000037f0: 7573 655f 7374 6f63 6b22 3e46 616c 7365  use_stock">False
-00003800: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-00003810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003820: 2020 2020 2020 2020 3c61 6363 656c 6572          <acceler
-00003830: 6174 6f72 206b 6579 3d22 4631 3122 2073  ator key="F11" s
-00003840: 6967 6e61 6c3d 2261 6374 6976 6174 6522  ignal="activate"
-00003850: 206d 6f64 6966 6965 7273 3d22 4744 4b5f   modifiers="GDK_
-00003860: 434f 4e54 524f 4c5f 4d41 534b 222f 3e0a  CONTROL_MASK"/>.
-00003870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003880: 2020 2020 2020 2020 2020 2020 3c73 6967              <sig
-00003890: 6e61 6c20 6e61 6d65 3d22 6163 7469 7661  nal name="activa
-000038a0: 7465 2220 6861 6e64 6c65 723d 2272 6163  te" handler="rac
-000038b0: 655f 7265 7375 6c74 735f 706f 696e 7473  e_results_points
-000038c0: 5f61 6374 6976 6174 655f 6362 222f 3e0a  _activate_cb"/>.
-000038d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038e0: 2020 2020 2020 2020 2020 3c2f 6f62 6a65            </obje
-000038f0: 6374 3e0a 2020 2020 2020 2020 2020 2020  ct>.            
-00003900: 2020 2020 2020 2020 2020 2020 3c2f 6368              </ch
-00003910: 696c 643e 0a20 2020 2020 2020 2020 2020  ild>.           
-00003920: 2020 2020 2020 2020 2020 2020 203c 6368               <ch
-00003930: 696c 643e 0a20 2020 2020 2020 2020 2020  ild>.           
-00003940: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00003950: 6f62 6a65 6374 2063 6c61 7373 3d22 4774  object class="Gt
-00003960: 6b49 6d61 6765 4d65 6e75 4974 656d 2220  kImageMenuItem" 
-00003970: 6964 3d22 6d65 6e75 5f72 6570 6f72 7473  id="menu_reports
-00003980: 5f72 6573 756c 7422 3e0a 2020 2020 2020  _result">.      
-00003990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039a0: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
-000039b0: 6e61 6d65 3d22 6c61 6265 6c22 2074 7261  name="label" tra
-000039c0: 6e73 6c61 7461 626c 653d 2279 6573 223e  nslatable="yes">
-000039d0: 5f52 6573 756c 743c 2f70 726f 7065 7274  _Result</propert
-000039e0: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
-000039f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00003a00: 7072 6f70 6572 7479 206e 616d 653d 2276  property name="v
-00003a10: 6973 6962 6c65 223e 5472 7565 3c2f 7072  isible">True</pr
-00003a20: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
-00003a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a40: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00003a50: 6d65 3d22 746f 6f6c 7469 705f 7465 7874  me="tooltip_text
-00003a60: 2220 7472 616e 736c 6174 6162 6c65 3d22  " translatable="
-00003a70: 7965 7322 3e45 7665 6e74 2072 6573 756c  yes">Event resul
-00003a80: 7420 7265 706f 7274 3c2f 7072 6f70 6572  t report</proper
-00003a90: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
-00003aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ab0: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00003ac0: 7573 655f 756e 6465 726c 696e 6522 3e54  use_underline">T
-00003ad0: 7275 653c 2f70 726f 7065 7274 793e 0a20  rue</property>. 
-00003ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003af0: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
-00003b00: 6572 7479 206e 616d 653d 2269 6d61 6765  erty name="image
-00003b10: 223e 696d 6167 6531 343c 2f70 726f 7065  ">image14</prope
-00003b20: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
-00003b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b40: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-00003b50: 2275 7365 5f73 746f 636b 223e 4661 6c73  "use_stock">Fals
-00003b60: 653c 2f70 726f 7065 7274 793e 0a20 2020  e</property>.   
-00003b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b80: 2020 2020 2020 2020 203c 6163 6365 6c65           <accele
-00003b90: 7261 746f 7220 6b65 793d 2246 3132 2220  rator key="F12" 
-00003ba0: 7369 676e 616c 3d22 6163 7469 7661 7465  signal="activate
-00003bb0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00003bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bd0: 3c73 6967 6e61 6c20 6e61 6d65 3d22 6163  <signal name="ac
-00003be0: 7469 7661 7465 2220 6861 6e64 6c65 723d  tivate" handler=
-00003bf0: 226d 656e 755f 7265 706f 7274 735f 7265  "menu_reports_re
-00003c00: 7375 6c74 5f61 6374 6976 6174 655f 6362  sult_activate_cb
-00003c10: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00003c20: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00003c30: 6f62 6a65 6374 3e0a 2020 2020 2020 2020  object>.        
-00003c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c50: 3c2f 6368 696c 643e 0a20 2020 2020 2020  </child>.       
+000035c0: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
+000035d0: 7920 6e61 6d65 3d22 7573 655f 756e 6465  y name="use_unde
+000035e0: 726c 696e 6522 3e54 7275 653c 2f70 726f  rline">True</pro
+000035f0: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
+00003600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003610: 2020 203c 7369 676e 616c 206e 616d 653d     <signal name=
+00003620: 2261 6374 6976 6174 6522 2068 616e 646c  "activate" handl
+00003630: 6572 3d22 6d65 6e75 5f64 6174 615f 7265  er="menu_data_re
+00003640: 706c 6163 655f 6163 7469 7661 7465 5f63  place_activate_c
+00003650: 6222 2f3e 0a20 2020 2020 2020 2020 2020  b"/>.           
+00003660: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00003670: 2f6f 626a 6563 743e 0a20 2020 2020 2020  /object>.       
+00003680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003690: 203c 2f63 6869 6c64 3e0a 2020 2020 2020   </child>.      
+000036a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036b0: 2020 3c63 6869 6c64 3e0a 2020 2020 2020    <child>.      
+000036c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036d0: 2020 2020 3c6f 626a 6563 7420 636c 6173      <object clas
+000036e0: 733d 2247 746b 4d65 6e75 4974 656d 2220  s="GtkMenuItem" 
+000036f0: 6964 3d22 6d65 6e75 5f64 6174 615f 6164  id="menu_data_ad
+00003700: 6422 3e0a 2020 2020 2020 2020 2020 2020  d">.            
+00003710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003720: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+00003730: 6c61 6265 6c22 3e5f 436c 6561 7220 5269  label">_Clear Ri
+00003740: 6465 7273 3c2f 7072 6f70 6572 7479 3e0a  ders</property>.
+00003750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003760: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
+00003770: 7065 7274 7920 6e61 6d65 3d22 7669 7369  perty name="visi
+00003780: 626c 6522 3e54 7275 653c 2f70 726f 7065  ble">True</prope
+00003790: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
+000037a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000037b0: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+000037c0: 2275 7365 5f75 6e64 6572 6c69 6e65 223e  "use_underline">
+000037d0: 5472 7565 3c2f 7072 6f70 6572 7479 3e0a  True</property>.
+000037e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000037f0: 2020 2020 2020 2020 2020 2020 3c73 6967              <sig
+00003800: 6e61 6c20 6e61 6d65 3d22 6163 7469 7661  nal name="activa
+00003810: 7465 2220 6861 6e64 6c65 723d 226d 656e  te" handler="men
+00003820: 755f 6461 7461 5f63 6c65 6172 5f61 6374  u_data_clear_act
+00003830: 6976 6174 655f 6362 222f 3e0a 2020 2020  ivate_cb"/>.    
+00003840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003850: 2020 2020 2020 3c2f 6f62 6a65 6374 3e0a        </object>.
+00003860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003870: 2020 2020 2020 2020 3c2f 6368 696c 643e          </child>
+00003880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003890: 2020 2020 2020 2020 203c 6368 696c 643e           <child>
+000038a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000038b0: 2020 2020 2020 2020 2020 203c 6f62 6a65             <obje
+000038c0: 6374 2063 6c61 7373 3d22 4774 6b53 6570  ct class="GtkSep
+000038d0: 6172 6174 6f72 4d65 6e75 4974 656d 2220  aratorMenuItem" 
+000038e0: 6964 3d22 6d65 6e75 5f64 6174 615f 7365  id="menu_data_se
+000038f0: 7061 223e 0a20 2020 2020 2020 2020 2020  pa">.           
+00003900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003910: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00003920: 2276 6973 6962 6c65 223e 5472 7565 3c2f  "visible">True</
+00003930: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
+00003940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003950: 2020 2020 3c2f 6f62 6a65 6374 3e0a 2020      </object>.  
+00003960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003970: 2020 2020 2020 3c2f 6368 696c 643e 0a20        </child>. 
+00003980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003990: 2020 2020 2020 203c 6368 696c 643e 0a20         <child>. 
+000039a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039b0: 2020 2020 2020 2020 203c 6f62 6a65 6374           <object
+000039c0: 2063 6c61 7373 3d22 4774 6b4d 656e 7549   class="GtkMenuI
+000039d0: 7465 6d22 2069 643d 226d 656e 755f 6461  tem" id="menu_da
+000039e0: 7461 5f69 6d70 6f72 7422 3e0a 2020 2020  ta_import">.    
+000039f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a00: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
+00003a10: 7920 6e61 6d65 3d22 7669 7369 626c 6522  y name="visible"
+00003a20: 3e54 7275 653c 2f70 726f 7065 7274 793e  >True</property>
+00003a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003a40: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
+00003a50: 6f70 6572 7479 206e 616d 653d 226c 6162  operty name="lab
+00003a60: 656c 223e 5f49 6d70 6f72 743c 2f70 726f  el">_Import</pro
+00003a70: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
+00003a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a90: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+00003aa0: 653d 2275 7365 5f75 6e64 6572 6c69 6e65  e="use_underline
+00003ab0: 223e 5472 7565 3c2f 7072 6f70 6572 7479  ">True</property
+00003ac0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00003ad0: 2020 2020 2020 2020 2020 2020 2020 3c63                <c
+00003ae0: 6869 6c64 2074 7970 653d 2273 7562 6d65  hild type="subme
+00003af0: 6e75 223e 0a20 2020 2020 2020 2020 2020  nu">.           
+00003b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b10: 2020 203c 6f62 6a65 6374 2063 6c61 7373     <object class
+00003b20: 3d22 4774 6b4d 656e 7522 2069 643d 226d  ="GtkMenu" id="m
+00003b30: 656e 7537 223e 0a20 2020 2020 2020 2020  enu7">.         
+00003b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b50: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+00003b60: 206e 616d 653d 2276 6973 6962 6c65 223e   name="visible">
+00003b70: 5472 7565 3c2f 7072 6f70 6572 7479 3e0a  True</property>.
+00003b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ba0: 3c63 6869 6c64 3e0a 2020 2020 2020 2020  <child>.        
+00003bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bc0: 2020 2020 2020 2020 2020 3c6f 626a 6563            <objec
+00003bd0: 7420 636c 6173 733d 2247 746b 4d65 6e75  t class="GtkMenu
+00003be0: 4974 656d 2220 6964 3d22 6d65 6e75 5f69  Item" id="menu_i
+00003bf0: 6d70 6f72 745f 7269 6465 7273 223e 0a20  mport_riders">. 
+00003c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c20: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+00003c30: 653d 2276 6973 6962 6c65 223e 5472 7565  e="visible">True
+00003c40: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+00003c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c70: 203c 6368 696c 643e 0a20 2020 2020 2020   <child>.       
-00003c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c90: 2020 203c 6f62 6a65 6374 2063 6c61 7373     <object class
-00003ca0: 3d22 4774 6b53 6570 6172 6174 6f72 4d65  ="GtkSeparatorMe
-00003cb0: 6e75 4974 656d 2220 6964 3d22 6d65 6e75  nuItem" id="menu
-00003cc0: 5f72 6570 6f72 7473 5f73 6570 222f 3e0a  _reports_sep"/>.
-00003cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ce0: 2020 2020 2020 2020 3c2f 6368 696c 643e          </child>
-00003cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003d00: 2020 2020 2020 203c 2f6f 626a 6563 743e         </object>
-00003d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003d20: 2020 2020 203c 2f63 6869 6c64 3e0a 2020       </child>.  
-00003d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d40: 3c2f 6f62 6a65 6374 3e0a 2020 2020 2020  </object>.      
-00003d50: 2020 2020 2020 2020 2020 3c2f 6368 696c            </chil
-00003d60: 643e 0a20 2020 2020 2020 2020 2020 2020  d>.             
-00003d70: 2020 203c 6368 696c 643e 0a20 2020 2020     <child>.     
-00003d80: 2020 2020 2020 2020 2020 2020 203c 6f62               <ob
-00003d90: 6a65 6374 2063 6c61 7373 3d22 4774 6b4d  ject class="GtkM
-00003da0: 656e 7549 7465 6d22 2069 643d 226d 656e  enuItem" id="men
-00003db0: 755f 6461 7461 223e 0a20 2020 2020 2020  u_data">.       
-00003dc0: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
-00003dd0: 6f70 6572 7479 206e 616d 653d 2276 6973  operty name="vis
-00003de0: 6962 6c65 223e 5472 7565 3c2f 7072 6f70  ible">True</prop
-00003df0: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
-00003e00: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00003e10: 7274 7920 6e61 6d65 3d22 6c61 6265 6c22  rty name="label"
-00003e20: 2074 7261 6e73 6c61 7461 626c 653d 2279   translatable="y
-00003e30: 6573 223e 5f44 6174 613c 2f70 726f 7065  es">_Data</prope
-00003e40: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
-00003e50: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-00003e60: 7479 206e 616d 653d 2275 7365 5f75 6e64  ty name="use_und
-00003e70: 6572 6c69 6e65 223e 5472 7565 3c2f 7072  erline">True</pr
-00003e80: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
-00003e90: 2020 2020 2020 2020 2020 2020 3c63 6869              <chi
-00003ea0: 6c64 2074 7970 653d 2273 7562 6d65 6e75  ld type="submenu
-00003eb0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00003ec0: 2020 2020 2020 2020 203c 6f62 6a65 6374           <object
-00003ed0: 2063 6c61 7373 3d22 4774 6b4d 656e 7522   class="GtkMenu"
-00003ee0: 2069 643d 226d 656e 7532 223e 0a20 2020   id="menu2">.   
-00003ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f00: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00003f10: 616d 653d 2276 6973 6962 6c65 223e 5472  ame="visible">Tr
-00003f20: 7565 3c2f 7072 6f70 6572 7479 3e0a 2020  ue</property>.  
-00003f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f40: 2020 2020 2020 3c63 6869 6c64 3e0a 2020        <child>.  
-00003f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f60: 2020 2020 2020 2020 3c6f 626a 6563 7420          <object 
-00003f70: 636c 6173 733d 2247 746b 496d 6167 654d  class="GtkImageM
-00003f80: 656e 7549 7465 6d22 2069 643d 226d 656e  enuItem" id="men
-00003f90: 755f 6461 7461 5f72 6570 6c61 6365 223e  u_data_replace">
-00003fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003fb0: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
-00003fc0: 6f70 6572 7479 206e 616d 653d 226c 6162  operty name="lab
-00003fd0: 656c 2220 7472 616e 736c 6174 6162 6c65  el" translatable
-00003fe0: 3d22 7965 7322 3e52 655f 706c 6163 6520  ="yes">Re_place 
-00003ff0: 5269 6465 7273 3c2f 7072 6f70 6572 7479  Riders</property
-00004000: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00004010: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-00004020: 726f 7065 7274 7920 6e61 6d65 3d22 7669  roperty name="vi
-00004030: 7369 626c 6522 3e54 7275 653c 2f70 726f  sible">True</pro
-00004040: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
-00004050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004060: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00004070: 653d 2274 6f6f 6c74 6970 5f74 6578 7422  e="tooltip_text"
-00004080: 2074 7261 6e73 6c61 7461 626c 653d 2279   translatable="y
-00004090: 6573 223e 5265 706c 6163 6520 6578 6973  es">Replace exis
-000040a0: 7469 6e67 2072 6964 6572 7320 6672 6f6d  ting riders from
-000040b0: 2063 7376 2066 696c 653c 2f70 726f 7065   csv file</prope
-000040c0: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
-000040d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040e0: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-000040f0: 2275 7365 5f75 6e64 6572 6c69 6e65 223e  "use_underline">
-00004100: 5472 7565 3c2f 7072 6f70 6572 7479 3e0a  True</property>.
-00004110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004120: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
-00004130: 7065 7274 7920 6e61 6d65 3d22 696d 6167  perty name="imag
-00004140: 6522 3e69 6d61 6765 3234 3c2f 7072 6f70  e">image24</prop
-00004150: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
-00004160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004170: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00004180: 3d22 7573 655f 7374 6f63 6b22 3e46 616c  ="use_stock">Fal
-00004190: 7365 3c2f 7072 6f70 6572 7479 3e0a 2020  se</property>.  
-000041a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041b0: 2020 2020 2020 2020 2020 3c73 6967 6e61            <signa
-000041c0: 6c20 6e61 6d65 3d22 6163 7469 7661 7465  l name="activate
-000041d0: 2220 6861 6e64 6c65 723d 226d 656e 755f  " handler="menu_
-000041e0: 6461 7461 5f72 6570 6c61 6365 5f61 6374  data_replace_act
-000041f0: 6976 6174 655f 6362 222f 3e0a 2020 2020  ivate_cb"/>.    
-00004200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004210: 2020 2020 2020 3c2f 6f62 6a65 6374 3e0a        </object>.
-00004220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004230: 2020 2020 2020 2020 3c2f 6368 696c 643e          </child>
-00004240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004250: 2020 2020 2020 2020 203c 6368 696c 643e           <child>
-00004260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004270: 2020 2020 2020 2020 2020 203c 6f62 6a65             <obje
-00004280: 6374 2063 6c61 7373 3d22 4774 6b4d 656e  ct class="GtkMen
-00004290: 7549 7465 6d22 2069 643d 226d 656e 755f  uItem" id="menu_
-000042a0: 6461 7461 5f61 6464 223e 0a20 2020 2020  data_add">.     
-000042b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042c0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-000042d0: 206e 616d 653d 226c 6162 656c 2220 7472   name="label" tr
-000042e0: 616e 736c 6174 6162 6c65 3d22 7965 7322  anslatable="yes"
-000042f0: 3e43 6c65 6172 2052 6964 6572 733c 2f70  >Clear Riders</p
-00004300: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
+00003c70: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+00003c80: 6c61 6265 6c22 3e5f 5269 6465 7273 3c2f  label">_Riders</
+00003c90: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
+00003ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003cb0: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
+00003cc0: 726f 7065 7274 7920 6e61 6d65 3d22 7573  roperty name="us
+00003cd0: 655f 756e 6465 726c 696e 6522 3e54 7275  e_underline">Tru
+00003ce0: 653c 2f70 726f 7065 7274 793e 0a20 2020  e</property>.   
+00003cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d10: 203c 7369 676e 616c 206e 616d 653d 2261   <signal name="a
+00003d20: 6374 6976 6174 6522 2068 616e 646c 6572  ctivate" handler
+00003d30: 3d22 6d65 6e75 5f69 6d70 6f72 745f 7269  ="menu_import_ri
+00003d40: 6465 7273 5f61 6374 6976 6174 655f 6362  ders_activate_cb
+00003d50: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00003d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d70: 2020 2020 2020 3c2f 6f62 6a65 6374 3e0a        </object>.
+00003d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003da0: 3c2f 6368 696c 643e 0a20 2020 2020 2020  </child>.       
+00003db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003dc0: 2020 2020 2020 2020 203c 6368 696c 643e           <child>
+00003dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003df0: 2020 203c 6f62 6a65 6374 2063 6c61 7373     <object class
+00003e00: 3d22 4774 6b4d 656e 7549 7465 6d22 2069  ="GtkMenuItem" i
+00003e10: 643d 226d 656e 755f 696d 706f 7274 5f63  d="menu_import_c
+00003e20: 6869 7066 696c 6522 3e0a 2020 2020 2020  hipfile">.      
+00003e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e40: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
+00003e50: 726f 7065 7274 7920 6e61 6d65 3d22 7669  roperty name="vi
+00003e60: 7369 626c 6522 3e54 7275 653c 2f70 726f  sible">True</pro
+00003e70: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
+00003e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e90: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
+00003ea0: 6572 7479 206e 616d 653d 226c 6162 656c  erty name="label
+00003eb0: 223e 5f43 6869 7066 696c 653c 2f70 726f  ">_Chipfile</pro
+00003ec0: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
+00003ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ee0: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
+00003ef0: 6572 7479 206e 616d 653d 2275 7365 5f75  erty name="use_u
+00003f00: 6e64 6572 6c69 6e65 223e 5472 7565 3c2f  nderline">True</
+00003f10: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
+00003f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f30: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
+00003f40: 6967 6e61 6c20 6e61 6d65 3d22 6163 7469  ignal name="acti
+00003f50: 7661 7465 2220 6861 6e64 6c65 723d 226d  vate" handler="m
+00003f60: 656e 755f 696d 706f 7274 5f63 6869 7066  enu_import_chipf
+00003f70: 696c 655f 6163 7469 7661 7465 5f63 6222  ile_activate_cb"
+00003f80: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+00003f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fa0: 2020 2020 203c 2f6f 626a 6563 743e 0a20       </object>. 
+00003fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fc0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00003fd0: 2f63 6869 6c64 3e0a 2020 2020 2020 2020  /child>.        
+00003fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ff0: 2020 2020 2020 2020 3c63 6869 6c64 3e0a          <child>.
+00004000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004020: 2020 3c6f 626a 6563 7420 636c 6173 733d    <object class=
+00004030: 2247 746b 4d65 6e75 4974 656d 2220 6964  "GtkMenuItem" id
+00004040: 3d22 6d65 6e75 5f69 6d70 6f72 745f 7374  ="menu_import_st
+00004050: 6172 746c 6973 7422 3e0a 2020 2020 2020  artlist">.      
+00004060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004070: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
+00004080: 726f 7065 7274 7920 6e61 6d65 3d22 7669  roperty name="vi
+00004090: 7369 626c 6522 3e54 7275 653c 2f70 726f  sible">True</pro
+000040a0: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
+000040b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040c0: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
+000040d0: 6572 7479 206e 616d 653d 226c 6162 656c  erty name="label
+000040e0: 223e 5f53 7461 7274 6c69 7374 3c2f 7072  ">_Startlist</pr
+000040f0: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
+00004100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004110: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
+00004120: 7065 7274 7920 6e61 6d65 3d22 7573 655f  perty name="use_
+00004130: 756e 6465 726c 696e 6522 3e54 7275 653c  underline">True<
+00004140: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
+00004150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004160: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00004170: 7369 676e 616c 206e 616d 653d 2261 6374  signal name="act
+00004180: 6976 6174 6522 2068 616e 646c 6572 3d22  ivate" handler="
+00004190: 6d65 6e75 5f69 6d70 6f72 745f 7374 6172  menu_import_star
+000041a0: 746c 6973 745f 6163 7469 7661 7465 5f63  tlist_activate_c
+000041b0: 6222 2f3e 0a20 2020 2020 2020 2020 2020  b"/>.           
+000041c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000041d0: 2020 2020 2020 203c 2f6f 626a 6563 743e         </object>
+000041e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000041f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004200: 203c 2f63 6869 6c64 3e0a 2020 2020 2020   </child>.      
+00004210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004220: 2020 2020 2020 2020 3c2f 6f62 6a65 6374          </object
+00004230: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00004240: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00004250: 6368 696c 643e 0a20 2020 2020 2020 2020  child>.         
+00004260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004270: 203c 2f6f 626a 6563 743e 0a20 2020 2020   </object>.     
+00004280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004290: 2020 203c 2f63 6869 6c64 3e0a 2020 2020     </child>.    
+000042a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000042b0: 2020 2020 3c63 6869 6c64 3e0a 2020 2020      <child>.    
+000042c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000042d0: 2020 2020 2020 3c6f 626a 6563 7420 636c        <object cl
+000042e0: 6173 733d 2247 746b 4d65 6e75 4974 656d  ass="GtkMenuItem
+000042f0: 2220 6964 3d22 6d65 6e75 5f64 6174 615f  " id="menu_data_
+00004300: 6578 706f 7274 223e 0a20 2020 2020 2020  export">.       
 00004310: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004320: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
 00004330: 616d 653d 2276 6973 6962 6c65 223e 5472  ame="visible">Tr
 00004340: 7565 3c2f 7072 6f70 6572 7479 3e0a 2020  ue</property>.  
 00004350: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004360: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00004370: 7274 7920 6e61 6d65 3d22 746f 6f6c 7469  rty name="toolti
-00004380: 705f 7465 7874 2220 7472 616e 736c 6174  p_text" translat
-00004390: 6162 6c65 3d22 7965 7322 3e43 6c65 6172  able="yes">Clear
-000043a0: 2061 6c6c 2072 6964 6572 2064 6174 613c   all rider data<
-000043b0: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
-000043c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043d0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-000043e0: 206e 616d 653d 2275 7365 5f75 6e64 6572   name="use_under
-000043f0: 6c69 6e65 223e 5472 7565 3c2f 7072 6f70  line">True</prop
-00004400: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
-00004410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004420: 2020 3c73 6967 6e61 6c20 6e61 6d65 3d22    <signal name="
-00004430: 6163 7469 7661 7465 2220 6861 6e64 6c65  activate" handle
-00004440: 723d 226d 656e 755f 6461 7461 5f63 6c65  r="menu_data_cle
-00004450: 6172 5f61 6374 6976 6174 655f 6362 222f  ar_activate_cb"/
-00004460: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00004470: 2020 2020 2020 2020 2020 2020 3c2f 6f62              </ob
-00004480: 6a65 6374 3e0a 2020 2020 2020 2020 2020  ject>.          
-00004490: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-000044a0: 6368 696c 643e 0a20 2020 2020 2020 2020  child>.         
-000044b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000044c0: 6368 696c 643e 0a20 2020 2020 2020 2020  child>.         
+00004370: 7274 7920 6e61 6d65 3d22 6c61 6265 6c22  rty name="label"
+00004380: 3e45 5f78 706f 7274 3c2f 7072 6f70 6572  >E_xport</proper
+00004390: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
+000043a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043b0: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+000043c0: 7573 655f 756e 6465 726c 696e 6522 3e54  use_underline">T
+000043d0: 7275 653c 2f70 726f 7065 7274 793e 0a20  rue</property>. 
+000043e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043f0: 2020 2020 2020 2020 2020 203c 6368 696c             <chil
+00004400: 6420 7479 7065 3d22 7375 626d 656e 7522  d type="submenu"
+00004410: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00004420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004430: 3c6f 626a 6563 7420 636c 6173 733d 2247  <object class="G
+00004440: 746b 4d65 6e75 2220 6964 3d22 6d65 6e75  tkMenu" id="menu
+00004450: 3822 3e0a 2020 2020 2020 2020 2020 2020  8">.            
+00004460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004470: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00004480: 6d65 3d22 7669 7369 626c 6522 3e54 7275  me="visible">Tru
+00004490: 653c 2f70 726f 7065 7274 793e 0a20 2020  e</property>.   
+000044a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044b0: 2020 2020 2020 2020 2020 2020 203c 6368               <ch
+000044c0: 696c 643e 0a20 2020 2020 2020 2020 2020  ild>.           
 000044d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044e0: 203c 6f62 6a65 6374 2063 6c61 7373 3d22   <object class="
-000044f0: 4774 6b53 6570 6172 6174 6f72 4d65 6e75  GtkSeparatorMenu
-00004500: 4974 656d 2220 6964 3d22 6d65 6e75 5f64  Item" id="menu_d
-00004510: 6174 615f 7365 7061 223e 0a20 2020 2020  ata_sepa">.     
+000044e0: 2020 2020 2020 203c 6f62 6a65 6374 2063         <object c
+000044f0: 6c61 7373 3d22 4774 6b4d 656e 7549 7465  lass="GtkMenuIte
+00004500: 6d22 2069 643d 226d 656e 755f 6578 706f  m" id="menu_expo
+00004510: 7274 5f72 6573 756c 7422 3e0a 2020 2020  rt_result">.    
 00004520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004530: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00004540: 206e 616d 653d 2276 6973 6962 6c65 223e   name="visible">
-00004550: 5472 7565 3c2f 7072 6f70 6572 7479 3e0a  True</property>.
-00004560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004570: 2020 2020 2020 2020 2020 3c2f 6f62 6a65            </obje
-00004580: 6374 3e0a 2020 2020 2020 2020 2020 2020  ct>.            
-00004590: 2020 2020 2020 2020 2020 2020 3c2f 6368              </ch
-000045a0: 696c 643e 0a20 2020 2020 2020 2020 2020  ild>.           
-000045b0: 2020 2020 2020 2020 2020 2020 203c 6368               <ch
-000045c0: 696c 643e 0a20 2020 2020 2020 2020 2020  ild>.           
-000045d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000045e0: 6f62 6a65 6374 2063 6c61 7373 3d22 4774  object class="Gt
-000045f0: 6b4d 656e 7549 7465 6d22 2069 643d 226d  kMenuItem" id="m
-00004600: 656e 755f 6461 7461 5f69 6d70 6f72 7422  enu_data_import"
-00004610: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00004620: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-00004630: 726f 7065 7274 7920 6e61 6d65 3d22 7669  roperty name="vi
-00004640: 7369 626c 6522 3e54 7275 653c 2f70 726f  sible">True</pro
-00004650: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
-00004660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004670: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00004680: 653d 226c 6162 656c 2220 7472 616e 736c  e="label" transl
-00004690: 6174 6162 6c65 3d22 7965 7322 3e5f 496d  atable="yes">_Im
-000046a0: 706f 7274 3c2f 7072 6f70 6572 7479 3e0a  port</property>.
-000046b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046c0: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
-000046d0: 7065 7274 7920 6e61 6d65 3d22 7573 655f  perty name="use_
-000046e0: 756e 6465 726c 696e 6522 3e54 7275 653c  underline">True<
-000046f0: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
+00004530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004540: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+00004550: 7669 7369 626c 6522 3e54 7275 653c 2f70  visible">True</p
+00004560: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
+00004570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004580: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
+00004590: 6f70 6572 7479 206e 616d 653d 226c 6162  operty name="lab
+000045a0: 656c 223e 525f 6573 756c 743c 2f70 726f  el">R_esult</pro
+000045b0: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
+000045c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045d0: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
+000045e0: 6572 7479 206e 616d 653d 2275 7365 5f75  erty name="use_u
+000045f0: 6e64 6572 6c69 6e65 223e 5472 7565 3c2f  nderline">True</
+00004600: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
+00004610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004620: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
+00004630: 6967 6e61 6c20 6e61 6d65 3d22 6163 7469  ignal name="acti
+00004640: 7661 7465 2220 6861 6e64 6c65 723d 226d  vate" handler="m
+00004650: 656e 755f 6578 706f 7274 5f72 6573 756c  enu_export_resul
+00004660: 745f 6163 7469 7661 7465 5f63 6222 2f3e  t_activate_cb"/>
+00004670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004690: 2020 203c 2f6f 626a 6563 743e 0a20 2020     </object>.   
+000046a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046b0: 2020 2020 2020 2020 2020 2020 203c 2f63               </c
+000046c0: 6869 6c64 3e0a 2020 2020 2020 2020 2020  hild>.          
+000046d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046e0: 2020 2020 2020 3c63 6869 6c64 3e0a 2020        <child>.  
+000046f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004710: 2020 2020 2020 203c 6368 696c 6420 7479         <child ty
-00004720: 7065 3d22 7375 626d 656e 7522 3e0a 2020  pe="submenu">.  
-00004730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004740: 2020 2020 2020 2020 2020 2020 3c6f 626a              <obj
-00004750: 6563 7420 636c 6173 733d 2247 746b 4d65  ect class="GtkMe
-00004760: 6e75 2220 6964 3d22 6d65 6e75 3722 3e0a  nu" id="menu7">.
-00004770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004790: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-000047a0: 7669 7369 626c 6522 3e54 7275 653c 2f70  visible">True</p
-000047b0: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
-000047c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047d0: 2020 2020 2020 2020 203c 6368 696c 643e           <child>
-000047e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004710: 3c6f 626a 6563 7420 636c 6173 733d 2247  <object class="G
+00004720: 746b 4d65 6e75 4974 656d 2220 6964 3d22  tkMenuItem" id="
+00004730: 6d65 6e75 5f65 7870 6f72 745f 7269 6465  menu_export_ride
+00004740: 7273 223e 0a20 2020 2020 2020 2020 2020  rs">.           
+00004750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004760: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+00004770: 7479 206e 616d 653d 2276 6973 6962 6c65  ty name="visible
+00004780: 223e 5472 7565 3c2f 7072 6f70 6572 7479  ">True</property
+00004790: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000047a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047b0: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+000047c0: 6e61 6d65 3d22 6c61 6265 6c22 3e5f 5269  name="label">_Ri
+000047d0: 6465 7273 3c2f 7072 6f70 6572 7479 3e0a  ders</property>.
+000047e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000047f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004800: 2020 203c 6f62 6a65 6374 2063 6c61 7373     <object class
-00004810: 3d22 4774 6b4d 656e 7549 7465 6d22 2069  ="GtkMenuItem" i
-00004820: 643d 226d 656e 755f 696d 706f 7274 5f72  d="menu_import_r
-00004830: 6964 6572 7322 3e0a 2020 2020 2020 2020  iders">.        
+00004800: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00004810: 6d65 3d22 7573 655f 756e 6465 726c 696e  me="use_underlin
+00004820: 6522 3e54 7275 653c 2f70 726f 7065 7274  e">True</propert
+00004830: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
 00004840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004850: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
-00004860: 7065 7274 7920 6e61 6d65 3d22 7669 7369  perty name="visi
-00004870: 626c 6522 3e54 7275 653c 2f70 726f 7065  ble">True</prope
-00004880: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
-00004890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048a0: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-000048b0: 7479 206e 616d 653d 2274 6f6f 6c74 6970  ty name="tooltip
-000048c0: 5f74 6578 7422 2074 7261 6e73 6c61 7461  _text" translata
-000048d0: 626c 653d 2279 6573 223e 496d 706f 7274  ble="yes">Import
-000048e0: 2072 6964 6572 2064 6174 613c 2f70 726f   rider data</pro
-000048f0: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
-00004900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004910: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
-00004920: 6572 7479 206e 616d 653d 226c 6162 656c  erty name="label
-00004930: 2220 7472 616e 736c 6174 6162 6c65 3d22  " translatable="
-00004940: 7965 7322 3e5f 5269 6465 7273 3c2f 7072  yes">_Riders</pr
-00004950: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
-00004960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004970: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
-00004980: 7065 7274 7920 6e61 6d65 3d22 7573 655f  perty name="use_
-00004990: 756e 6465 726c 696e 6522 3e54 7275 653c  underline">True<
-000049a0: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
-000049b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000049d0: 7369 676e 616c 206e 616d 653d 2261 6374  signal name="act
-000049e0: 6976 6174 6522 2068 616e 646c 6572 3d22  ivate" handler="
-000049f0: 6d65 6e75 5f69 6d70 6f72 745f 7269 6465  menu_import_ride
-00004a00: 7273 5f61 6374 6976 6174 655f 6362 222f  rs_activate_cb"/
-00004a10: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00004850: 2020 2020 2020 203c 7369 676e 616c 206e         <signal n
+00004860: 616d 653d 2261 6374 6976 6174 6522 2068  ame="activate" h
+00004870: 616e 646c 6572 3d22 6d65 6e75 5f65 7870  andler="menu_exp
+00004880: 6f72 745f 7269 6465 7273 5f61 6374 6976  ort_riders_activ
+00004890: 6174 655f 6362 222f 3e0a 2020 2020 2020  ate_cb"/>.      
+000048a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048b0: 2020 2020 2020 2020 2020 2020 3c2f 6f62              </ob
+000048c0: 6a65 6374 3e0a 2020 2020 2020 2020 2020  ject>.          
+000048d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048e0: 2020 2020 2020 3c2f 6368 696c 643e 0a20        </child>. 
+000048f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004900: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00004910: 6368 696c 643e 0a20 2020 2020 2020 2020  child>.         
+00004920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004930: 2020 2020 2020 2020 203c 6f62 6a65 6374           <object
+00004940: 2063 6c61 7373 3d22 4774 6b4d 656e 7549   class="GtkMenuI
+00004950: 7465 6d22 2069 643d 226d 656e 755f 6578  tem" id="menu_ex
+00004960: 706f 7274 5f63 6869 7066 696c 6522 3e0a  port_chipfile">.
+00004970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004990: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+000049a0: 6d65 3d22 7669 7369 626c 6522 3e54 7275  me="visible">Tru
+000049b0: 653c 2f70 726f 7065 7274 793e 0a20 2020  e</property>.   
+000049c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049e0: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+000049f0: 226c 6162 656c 223e 5f43 6869 7066 696c  "label">_Chipfil
+00004a00: 653c 2f70 726f 7065 7274 793e 0a20 2020  e</property>.   
+00004a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a30: 2020 2020 3c2f 6f62 6a65 6374 3e0a 2020      </object>.  
-00004a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a50: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00004a60: 6368 696c 643e 0a20 2020 2020 2020 2020  child>.         
+00004a30: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00004a40: 2275 7365 5f75 6e64 6572 6c69 6e65 223e  "use_underline">
+00004a50: 5472 7565 3c2f 7072 6f70 6572 7479 3e0a  True</property>.
+00004a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a80: 2020 2020 2020 203c 6368 696c 643e 0a20         <child>. 
-00004a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ab0: 203c 6f62 6a65 6374 2063 6c61 7373 3d22   <object class="
-00004ac0: 4774 6b4d 656e 7549 7465 6d22 2069 643d  GtkMenuItem" id=
-00004ad0: 226d 656e 755f 696d 706f 7274 5f63 6869  "menu_import_chi
-00004ae0: 7066 696c 6522 3e0a 2020 2020 2020 2020  pfile">.        
-00004af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b00: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
-00004b10: 7065 7274 7920 6e61 6d65 3d22 7669 7369  perty name="visi
-00004b20: 626c 6522 3e54 7275 653c 2f70 726f 7065  ble">True</prope
-00004b30: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
-00004b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b50: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-00004b60: 7479 206e 616d 653d 2274 6f6f 6c74 6970  ty name="tooltip
-00004b70: 5f74 6578 7422 2074 7261 6e73 6c61 7461  _text" translata
-00004b80: 626c 653d 2279 6573 223e 496d 706f 7274  ble="yes">Import
-00004b90: 2074 7261 6e73 706f 6e64 6572 2069 6420   transponder id 
-00004ba0: 6461 7461 3c2f 7072 6f70 6572 7479 3e0a  data</property>.
+00004a80: 2020 2020 3c73 6967 6e61 6c20 6e61 6d65      <signal name
+00004a90: 3d22 6163 7469 7661 7465 2220 6861 6e64  ="activate" hand
+00004aa0: 6c65 723d 226d 656e 755f 6578 706f 7274  ler="menu_export
+00004ab0: 5f63 6869 7066 696c 655f 6163 7469 7661  _chipfile_activa
+00004ac0: 7465 5f63 6222 2f3e 0a20 2020 2020 2020  te_cb"/>.       
+00004ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ae0: 2020 2020 2020 2020 2020 203c 2f6f 626a             </obj
+00004af0: 6563 743e 0a20 2020 2020 2020 2020 2020  ect>.           
+00004b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b10: 2020 2020 203c 2f63 6869 6c64 3e0a 2020       </child>.  
+00004b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b30: 2020 2020 2020 2020 2020 2020 2020 3c63                <c
+00004b40: 6869 6c64 3e0a 2020 2020 2020 2020 2020  hild>.          
+00004b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b60: 2020 2020 2020 2020 3c6f 626a 6563 7420          <object 
+00004b70: 636c 6173 733d 2247 746b 4d65 6e75 4974  class="GtkMenuIt
+00004b80: 656d 2220 6964 3d22 6d65 6e75 5f65 7870  em" id="menu_exp
+00004b90: 6f72 745f 7374 6172 746c 6973 7422 3e0a  ort_startlist">.
+00004ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bd0: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00004be0: 6d65 3d22 6c61 6265 6c22 2074 7261 6e73  me="label" trans
-00004bf0: 6c61 7461 626c 653d 2279 6573 223e 5f43  latable="yes">_C
-00004c00: 6869 7066 696c 653c 2f70 726f 7065 7274  hipfile</propert
-00004c10: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
-00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c30: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00004c40: 206e 616d 653d 2275 7365 5f75 6e64 6572   name="use_under
-00004c50: 6c69 6e65 223e 5472 7565 3c2f 7072 6f70  line">True</prop
-00004c60: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
-00004c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c80: 2020 2020 2020 2020 2020 3c73 6967 6e61            <signa
-00004c90: 6c20 6e61 6d65 3d22 6163 7469 7661 7465  l name="activate
-00004ca0: 2220 6861 6e64 6c65 723d 226d 656e 755f  " handler="menu_
-00004cb0: 696d 706f 7274 5f63 6869 7066 696c 655f  import_chipfile_
-00004cc0: 6163 7469 7661 7465 5f63 6222 2f3e 0a20  activate_cb"/>. 
-00004cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cf0: 203c 2f6f 626a 6563 743e 0a20 2020 2020   </object>.     
+00004bc0: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00004bd0: 6d65 3d22 7669 7369 626c 6522 3e54 7275  me="visible">Tru
+00004be0: 653c 2f70 726f 7065 7274 793e 0a20 2020  e</property>.   
+00004bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c10: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00004c20: 226c 6162 656c 223e 5f53 7461 7274 6c69  "label">_Startli
+00004c30: 7374 3c2f 7072 6f70 6572 7479 3e0a 2020  st</property>.  
+00004c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c60: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+00004c70: 3d22 7573 655f 756e 6465 726c 696e 6522  ="use_underline"
+00004c80: 3e54 7275 653c 2f70 726f 7065 7274 793e  >True</property>
+00004c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cb0: 2020 2020 203c 7369 676e 616c 206e 616d       <signal nam
+00004cc0: 653d 2261 6374 6976 6174 6522 2068 616e  e="activate" han
+00004cd0: 646c 6572 3d22 6d65 6e75 5f65 7870 6f72  dler="menu_expor
+00004ce0: 745f 7374 6172 746c 6973 745f 6163 7469  t_startlist_acti
+00004cf0: 7661 7465 5f63 6222 2f3e 0a20 2020 2020  vate_cb"/>.     
 00004d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d10: 2020 2020 2020 2020 2020 203c 2f63 6869             </chi
-00004d20: 6c64 3e0a 2020 2020 2020 2020 2020 2020  ld>.            
+00004d10: 2020 2020 2020 2020 2020 2020 203c 2f6f               </o
+00004d20: 626a 6563 743e 0a20 2020 2020 2020 2020  bject>.         
 00004d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d40: 2020 2020 3c63 6869 6c64 3e0a 2020 2020      <child>.    
+00004d40: 2020 2020 2020 203c 2f63 6869 6c64 3e0a         </child>.
 00004d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d60: 2020 2020 2020 2020 2020 2020 2020 3c6f                <o
-00004d70: 626a 6563 7420 636c 6173 733d 2247 746b  bject class="Gtk
-00004d80: 4d65 6e75 4974 656d 2220 6964 3d22 6d65  MenuItem" id="me
-00004d90: 6e75 5f69 6d70 6f72 745f 7374 6172 746c  nu_import_startl
-00004da0: 6973 7422 3e0a 2020 2020 2020 2020 2020  ist">.          
-00004db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004dc0: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00004dd0: 7274 7920 6e61 6d65 3d22 7669 7369 626c  rty name="visibl
-00004de0: 6522 3e54 7275 653c 2f70 726f 7065 7274  e">True</propert
-00004df0: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
-00004e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e10: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00004e20: 206e 616d 653d 2274 6f6f 6c74 6970 5f74   name="tooltip_t
-00004e30: 6578 7422 2074 7261 6e73 6c61 7461 626c  ext" translatabl
-00004e40: 653d 2279 6573 223e 496d 706f 7274 2065  e="yes">Import e
-00004e50: 7665 6e74 2073 7461 7274 6c69 7374 2061  vent startlist a
-00004e60: 6e64 2073 7461 7274 2074 696d 6573 3c2f  nd start times</
-00004e70: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
-00004e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e90: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-00004ea0: 726f 7065 7274 7920 6e61 6d65 3d22 6c61  roperty name="la
-00004eb0: 6265 6c22 2074 7261 6e73 6c61 7461 626c  bel" translatabl
-00004ec0: 653d 2279 6573 223e 5f53 7461 7274 6c69  e="yes">_Startli
-00004ed0: 7374 3c2f 7072 6f70 6572 7479 3e0a 2020  st</property>.  
+00004d60: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00004d70: 6f62 6a65 6374 3e0a 2020 2020 2020 2020  object>.        
+00004d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d90: 2020 2020 3c2f 6368 696c 643e 0a20 2020      </child>.   
+00004da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004db0: 2020 2020 2020 203c 2f6f 626a 6563 743e         </object>
+00004dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004dd0: 2020 2020 2020 2020 203c 2f63 6869 6c64           </child
+00004de0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00004df0: 2020 2020 2020 2020 2020 3c63 6869 6c64            <child
+00004e00: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00004e10: 2020 2020 2020 2020 2020 2020 3c6f 626a              <obj
+00004e20: 6563 7420 636c 6173 733d 2247 746b 5365  ect class="GtkSe
+00004e30: 7061 7261 746f 724d 656e 7549 7465 6d22  paratorMenuItem"
+00004e40: 2069 643d 226d 656e 755f 6461 7461 5f73   id="menu_data_s
+00004e50: 6570 223e 0a20 2020 2020 2020 2020 2020  ep">.           
+00004e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e70: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00004e80: 2276 6973 6962 6c65 223e 5472 7565 3c2f  "visible">True</
+00004e90: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
+00004ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004eb0: 2020 2020 3c2f 6f62 6a65 6374 3e0a 2020      </object>.  
+00004ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ed0: 2020 2020 2020 3c2f 6368 696c 643e 0a20        </child>. 
 00004ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f00: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00004f10: 3d22 7573 655f 756e 6465 726c 696e 6522  ="use_underline"
-00004f20: 3e54 7275 653c 2f70 726f 7065 7274 793e  >True</property>
-00004f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f50: 2020 2020 203c 7369 676e 616c 206e 616d       <signal nam
-00004f60: 653d 2261 6374 6976 6174 6522 2068 616e  e="activate" han
-00004f70: 646c 6572 3d22 6d65 6e75 5f69 6d70 6f72  dler="menu_impor
-00004f80: 745f 7374 6172 746c 6973 745f 6163 7469  t_startlist_acti
-00004f90: 7661 7465 5f63 6222 2f3e 0a20 2020 2020  vate_cb"/>.     
-00004fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fb0: 2020 2020 2020 2020 2020 2020 203c 2f6f               </o
-00004fc0: 626a 6563 743e 0a20 2020 2020 2020 2020  bject>.         
-00004fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fe0: 2020 2020 2020 203c 2f63 6869 6c64 3e0a         </child>.
-00004ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005000: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00005010: 6f62 6a65 6374 3e0a 2020 2020 2020 2020  object>.        
-00005020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005030: 2020 2020 3c2f 6368 696c 643e 0a20 2020      </child>.   
-00005040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005050: 2020 2020 2020 203c 2f6f 626a 6563 743e         </object>
-00005060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005070: 2020 2020 2020 2020 203c 2f63 6869 6c64           </child
-00005080: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00005090: 2020 2020 2020 2020 2020 3c63 6869 6c64            <child
-000050a0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000050b0: 2020 2020 2020 2020 2020 2020 3c6f 626a              <obj
-000050c0: 6563 7420 636c 6173 733d 2247 746b 4d65  ect class="GtkMe
-000050d0: 6e75 4974 656d 2220 6964 3d22 6d65 6e75  nuItem" id="menu
-000050e0: 5f64 6174 615f 6578 706f 7274 223e 0a20  _data_export">. 
-000050f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005100: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
-00005110: 6572 7479 206e 616d 653d 2276 6973 6962  erty name="visib
-00005120: 6c65 223e 5472 7565 3c2f 7072 6f70 6572  le">True</proper
-00005130: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
+00004ef0: 2020 2020 2020 203c 6368 696c 643e 0a20         <child>. 
+00004f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f10: 2020 2020 2020 2020 203c 6f62 6a65 6374           <object
+00004f20: 2063 6c61 7373 3d22 4774 6b4d 656e 7549   class="GtkMenuI
+00004f30: 7465 6d22 2069 643d 226d 656e 755f 6461  tem" id="menu_da
+00004f40: 7461 5f72 6573 756c 7473 223e 0a20 2020  ta_results">.   
+00004f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f60: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+00004f70: 7479 206e 616d 653d 226c 6162 656c 223e  ty name="label">
+00004f80: 525f 6573 756c 743c 2f70 726f 7065 7274  R_esult</propert
+00004f90: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
+00004fa0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00004fb0: 7072 6f70 6572 7479 206e 616d 653d 2276  property name="v
+00004fc0: 6973 6962 6c65 223e 5472 7565 3c2f 7072  isible">True</pr
+00004fd0: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
+00004fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ff0: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00005000: 6d65 3d22 7573 655f 756e 6465 726c 696e  me="use_underlin
+00005010: 6522 3e54 7275 653c 2f70 726f 7065 7274  e">True</propert
+00005020: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
+00005030: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00005040: 6163 6365 6c65 7261 746f 7220 6b65 793d  accelerator key=
+00005050: 2265 2220 7369 676e 616c 3d22 6163 7469  "e" signal="acti
+00005060: 7661 7465 2220 6d6f 6469 6669 6572 733d  vate" modifiers=
+00005070: 2247 444b 5f43 4f4e 5452 4f4c 5f4d 4153  "GDK_CONTROL_MAS
+00005080: 4b22 2f3e 0a20 2020 2020 2020 2020 2020  K"/>.           
+00005090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050a0: 203c 7369 676e 616c 206e 616d 653d 2261   <signal name="a
+000050b0: 6374 6976 6174 6522 2068 616e 646c 6572  ctivate" handler
+000050c0: 3d22 6d65 6e75 5f64 6174 615f 7265 7375  ="menu_data_resu
+000050d0: 6c74 735f 6362 222f 3e0a 2020 2020 2020  lts_cb"/>.      
+000050e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050f0: 2020 2020 3c2f 6f62 6a65 6374 3e0a 2020      </object>.  
+00005100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005110: 2020 2020 2020 3c2f 6368 696c 643e 0a20        </child>. 
+00005120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005130: 2020 2020 203c 2f6f 626a 6563 743e 0a20       </object>. 
 00005140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005150: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00005160: 6c61 6265 6c22 2074 7261 6e73 6c61 7461  label" translata
-00005170: 626c 653d 2279 6573 223e 455f 7870 6f72  ble="yes">E_xpor
-00005180: 743c 2f70 726f 7065 7274 793e 0a20 2020  t</property>.   
-00005190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051a0: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-000051b0: 7479 206e 616d 653d 2275 7365 5f75 6e64  ty name="use_und
-000051c0: 6572 6c69 6e65 223e 5472 7565 3c2f 7072  erline">True</pr
-000051d0: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
-000051e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051f0: 2020 2020 3c63 6869 6c64 2074 7970 653d      <child type=
-00005200: 2273 7562 6d65 6e75 223e 0a20 2020 2020  "submenu">.     
-00005210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005220: 2020 2020 2020 2020 203c 6f62 6a65 6374           <object
-00005230: 2063 6c61 7373 3d22 4774 6b4d 656e 7522   class="GtkMenu"
-00005240: 2069 643d 226d 656e 7538 223e 0a20 2020   id="menu8">.   
-00005250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005260: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
-00005270: 6f70 6572 7479 206e 616d 653d 2276 6973  operty name="vis
-00005280: 6962 6c65 223e 5472 7565 3c2f 7072 6f70  ible">True</prop
-00005290: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
-000052a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052b0: 2020 2020 2020 3c63 6869 6c64 3e0a 2020        <child>.  
-000052c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005150: 2020 203c 2f63 6869 6c64 3e0a 2020 2020     </child>.    
+00005160: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00005170: 6f62 6a65 6374 3e0a 2020 2020 2020 2020  object>.        
+00005180: 2020 2020 2020 2020 3c2f 6368 696c 643e          </child>
+00005190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000051a0: 203c 6368 696c 643e 0a20 2020 2020 2020   <child>.       
+000051b0: 2020 2020 2020 2020 2020 203c 6f62 6a65             <obje
+000051c0: 6374 2063 6c61 7373 3d22 4774 6b4d 656e  ct class="GtkMen
+000051d0: 7549 7465 6d22 2069 643d 226d 656e 755f  uItem" id="menu_
+000051e0: 7469 6d79 223e 0a20 2020 2020 2020 2020  timy">.         
+000051f0: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
+00005200: 6572 7479 206e 616d 653d 2276 6973 6962  erty name="visib
+00005210: 6c65 223e 5472 7565 3c2f 7072 6f70 6572  le">True</proper
+00005220: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
+00005230: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
+00005240: 7920 6e61 6d65 3d22 6c61 6265 6c22 3e5f  y name="label">_
+00005250: 5469 6d69 6e67 3c2f 7072 6f70 6572 7479  Timing</property
+00005260: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00005270: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+00005280: 6e61 6d65 3d22 7573 655f 756e 6465 726c  name="use_underl
+00005290: 696e 6522 3e54 7275 653c 2f70 726f 7065  ine">True</prope
+000052a0: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
+000052b0: 2020 2020 2020 2020 203c 6368 696c 6420           <child 
+000052c0: 7479 7065 3d22 7375 626d 656e 7522 3e0a  type="submenu">.
 000052d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052e0: 3c6f 626a 6563 7420 636c 6173 733d 2247  <object class="G
-000052f0: 746b 4d65 6e75 4974 656d 2220 6964 3d22  tkMenuItem" id="
-00005300: 6d65 6e75 5f65 7870 6f72 745f 7265 7375  menu_export_resu
-00005310: 6c74 223e 0a20 2020 2020 2020 2020 2020  lt">.           
-00005320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005330: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-00005340: 7479 206e 616d 653d 2276 6973 6962 6c65  ty name="visible
-00005350: 223e 5472 7565 3c2f 7072 6f70 6572 7479  ">True</property
-00005360: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000052e0: 2020 2020 2020 3c6f 626a 6563 7420 636c        <object cl
+000052f0: 6173 733d 2247 746b 4d65 6e75 2220 6964  ass="GtkMenu" id
+00005300: 3d22 6d65 6e75 3422 3e0a 2020 2020 2020  ="menu4">.      
+00005310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005320: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+00005330: 3d22 7669 7369 626c 6522 3e54 7275 653c  ="visible">True<
+00005340: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
+00005350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005360: 2020 203c 6368 696c 643e 0a20 2020 2020     <child>.     
 00005370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005380: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
-00005390: 6e61 6d65 3d22 746f 6f6c 7469 705f 7465  name="tooltip_te
-000053a0: 7874 2220 7472 616e 736c 6174 6162 6c65  xt" translatable
-000053b0: 3d22 7965 7322 3e45 7870 6f72 7420 6576  ="yes">Export ev
-000053c0: 656e 7420 7265 7375 6c74 2074 6f20 7370  ent result to sp
-000053d0: 7265 6164 7368 6565 743c 2f70 726f 7065  readsheet</prope
-000053e0: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
-000053f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005400: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-00005410: 7479 206e 616d 653d 226c 6162 656c 2220  ty name="label" 
-00005420: 7472 616e 736c 6174 6162 6c65 3d22 7965  translatable="ye
-00005430: 7322 3e52 5f65 7375 6c74 3c2f 7072 6f70  s">R_esult</prop
-00005440: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
+00005380: 2020 2020 203c 6f62 6a65 6374 2063 6c61       <object cla
+00005390: 7373 3d22 4774 6b4d 656e 7549 7465 6d22  ss="GtkMenuItem"
+000053a0: 2069 643d 226d 656e 755f 7469 6d69 6e67   id="menu_timing
+000053b0: 5f73 7461 7274 223e 0a20 2020 2020 2020  _start">.       
+000053c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053d0: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+000053e0: 616d 653d 226c 6162 656c 223e 5365 7420  ame="label">Set 
+000053f0: 5f45 6c61 7073 6564 3c2f 7072 6f70 6572  _Elapsed</proper
+00005400: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
+00005410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005420: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+00005430: 7669 7369 626c 6522 3e54 7275 653c 2f70  visible">True</p
+00005440: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
 00005450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005460: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00005470: 7274 7920 6e61 6d65 3d22 7573 655f 756e  rty name="use_un
-00005480: 6465 726c 696e 6522 3e54 7275 653c 2f70  derline">True</p
-00005490: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
+00005460: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+00005470: 616d 653d 2275 7365 5f75 6e64 6572 6c69  ame="use_underli
+00005480: 6e65 223e 5472 7565 3c2f 7072 6f70 6572  ne">True</proper
+00005490: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
 000054a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054b0: 2020 2020 2020 2020 2020 2020 203c 7369               <si
-000054c0: 676e 616c 206e 616d 653d 2261 6374 6976  gnal name="activ
-000054d0: 6174 6522 2068 616e 646c 6572 3d22 6d65  ate" handler="me
-000054e0: 6e75 5f65 7870 6f72 745f 7265 7375 6c74  nu_export_result
-000054f0: 5f61 6374 6976 6174 655f 6362 222f 3e0a  _activate_cb"/>.
-00005500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005520: 2020 3c2f 6f62 6a65 6374 3e0a 2020 2020    </object>.    
-00005530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005540: 2020 2020 2020 2020 2020 2020 3c2f 6368              </ch
-00005550: 696c 643e 0a20 2020 2020 2020 2020 2020  ild>.           
+000054b0: 3c73 6967 6e61 6c20 6e61 6d65 3d22 6163  <signal name="ac
+000054c0: 7469 7661 7465 2220 6861 6e64 6c65 723d  tivate" handler=
+000054d0: 226d 656e 755f 7469 6d69 6e67 5f73 7461  "menu_timing_sta
+000054e0: 7274 5f61 6374 6976 6174 655f 6362 222f  rt_activate_cb"/
+000054f0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00005500: 2020 2020 2020 2020 2020 2020 3c2f 6f62              </ob
+00005510: 6a65 6374 3e0a 2020 2020 2020 2020 2020  ject>.          
+00005520: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00005530: 6368 696c 643e 0a20 2020 2020 2020 2020  child>.         
+00005540: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00005550: 6368 696c 643e 0a20 2020 2020 2020 2020  child>.         
 00005560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005570: 2020 2020 203c 6368 696c 643e 0a20 2020       <child>.   
-00005580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005590: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000055a0: 6f62 6a65 6374 2063 6c61 7373 3d22 4774  object class="Gt
-000055b0: 6b4d 656e 7549 7465 6d22 2069 643d 226d  kMenuItem" id="m
-000055c0: 656e 755f 6578 706f 7274 5f72 6964 6572  enu_export_rider
-000055d0: 7322 3e0a 2020 2020 2020 2020 2020 2020  s">.            
-000055e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055f0: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-00005600: 7920 6e61 6d65 3d22 7669 7369 626c 6522  y name="visible"
-00005610: 3e54 7275 653c 2f70 726f 7065 7274 793e  >True</property>
-00005620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005640: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00005650: 616d 653d 2274 6f6f 6c74 6970 5f74 6578  ame="tooltip_tex
-00005660: 7422 2074 7261 6e73 6c61 7461 626c 653d  t" translatable=
-00005670: 2279 6573 223e 4578 706f 7274 2072 6964  "yes">Export rid
-00005680: 6572 2064 6174 613c 2f70 726f 7065 7274  er data</propert
-00005690: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
-000056a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056b0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-000056c0: 206e 616d 653d 226c 6162 656c 2220 7472   name="label" tr
-000056d0: 616e 736c 6174 6162 6c65 3d22 7965 7322  anslatable="yes"
-000056e0: 3e5f 5269 6465 7273 3c2f 7072 6f70 6572  >_Riders</proper
-000056f0: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
-00005700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005710: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-00005720: 7920 6e61 6d65 3d22 7573 655f 756e 6465  y name="use_unde
-00005730: 726c 696e 6522 3e54 7275 653c 2f70 726f  rline">True</pro
-00005740: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
-00005750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005760: 2020 2020 2020 2020 2020 203c 7369 676e             <sign
-00005770: 616c 206e 616d 653d 2261 6374 6976 6174  al name="activat
-00005780: 6522 2068 616e 646c 6572 3d22 6d65 6e75  e" handler="menu
-00005790: 5f65 7870 6f72 745f 7269 6465 7273 5f61  _export_riders_a
-000057a0: 6374 6976 6174 655f 6362 222f 3e0a 2020  ctivate_cb"/>.  
-000057b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057d0: 3c2f 6f62 6a65 6374 3e0a 2020 2020 2020  </object>.      
-000057e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057f0: 2020 2020 2020 2020 2020 3c2f 6368 696c            </chil
-00005800: 643e 0a20 2020 2020 2020 2020 2020 2020  d>.             
-00005810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005820: 2020 203c 6368 696c 643e 0a20 2020 2020     <child>.     
-00005830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005840: 2020 2020 2020 2020 2020 2020 203c 6f62               <ob
-00005850: 6a65 6374 2063 6c61 7373 3d22 4774 6b4d  ject class="GtkM
-00005860: 656e 7549 7465 6d22 2069 643d 226d 656e  enuItem" id="men
-00005870: 755f 6578 706f 7274 5f63 6869 7066 696c  u_export_chipfil
-00005880: 6522 3e0a 2020 2020 2020 2020 2020 2020  e">.            
+00005570: 203c 6f62 6a65 6374 2063 6c61 7373 3d22   <object class="
+00005580: 4774 6b53 6570 6172 6174 6f72 4d65 6e75  GtkSeparatorMenu
+00005590: 4974 656d 2220 6964 3d22 6d65 6e75 5f74  Item" id="menu_t
+000055a0: 696d 696e 675f 7365 7031 223e 0a20 2020  iming_sep1">.   
+000055b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055c0: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+000055d0: 7479 206e 616d 653d 2276 6973 6962 6c65  ty name="visible
+000055e0: 223e 5472 7565 3c2f 7072 6f70 6572 7479  ">True</property
+000055f0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00005600: 2020 2020 2020 2020 2020 2020 3c2f 6f62              </ob
+00005610: 6a65 6374 3e0a 2020 2020 2020 2020 2020  ject>.          
+00005620: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00005630: 6368 696c 643e 0a20 2020 2020 2020 2020  child>.         
+00005640: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00005650: 6368 696c 643e 0a20 2020 2020 2020 2020  child>.         
+00005660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005670: 203c 6f62 6a65 6374 2063 6c61 7373 3d22   <object class="
+00005680: 4774 6b4d 656e 7549 7465 6d22 2069 643d  GtkMenuItem" id=
+00005690: 226d 656e 755f 7469 6d69 6e67 5f63 6c65  "menu_timing_cle
+000056a0: 6172 223e 0a20 2020 2020 2020 2020 2020  ar">.           
+000056b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056c0: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+000056d0: 226c 6162 656c 223e 5f4e 6577 2053 6573  "label">_New Ses
+000056e0: 7369 6f6e 3c2f 7072 6f70 6572 7479 3e0a  sion</property>.
+000056f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005700: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
+00005710: 7065 7274 7920 6e61 6d65 3d22 7669 7369  perty name="visi
+00005720: 626c 6522 3e54 7275 653c 2f70 726f 7065  ble">True</prope
+00005730: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
+00005740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005750: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00005760: 2273 656e 7369 7469 7665 223e 5472 7565  "sensitive">True
+00005770: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+00005780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005790: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
+000057a0: 7920 6e61 6d65 3d22 7573 655f 756e 6465  y name="use_unde
+000057b0: 726c 696e 6522 3e54 7275 653c 2f70 726f  rline">True</pro
+000057c0: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
+000057d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057e0: 2020 203c 7369 676e 616c 206e 616d 653d     <signal name=
+000057f0: 2261 6374 6976 6174 6522 2068 616e 646c  "activate" handl
+00005800: 6572 3d22 6d65 6e75 5f74 696d 696e 675f  er="menu_timing_
+00005810: 636c 6561 725f 6163 7469 7661 7465 5f63  clear_activate_c
+00005820: 6222 2f3e 0a20 2020 2020 2020 2020 2020  b"/>.           
+00005830: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00005840: 2f6f 626a 6563 743e 0a20 2020 2020 2020  /object>.       
+00005850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005860: 203c 2f63 6869 6c64 3e0a 2020 2020 2020   </child>.      
+00005870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005880: 2020 3c63 6869 6c64 3e0a 2020 2020 2020    <child>.      
 00005890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058a0: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-000058b0: 7920 6e61 6d65 3d22 7669 7369 626c 6522  y name="visible"
-000058c0: 3e54 7275 653c 2f70 726f 7065 7274 793e  >True</property>
-000058d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000058a0: 2020 2020 3c6f 626a 6563 7420 636c 6173      <object clas
+000058b0: 733d 2247 746b 4d65 6e75 4974 656d 2220  s="GtkMenuItem" 
+000058c0: 6964 3d22 6d65 6e75 5f74 696d 696e 675f  id="menu_timing_
+000058d0: 7374 6174 7573 223e 0a20 2020 2020 2020  status">.       
 000058e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000058f0: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00005900: 616d 653d 2274 6f6f 6c74 6970 5f74 6578  ame="tooltip_tex
-00005910: 7422 2074 7261 6e73 6c61 7461 626c 653d  t" translatable=
-00005920: 2279 6573 223e 4578 706f 7274 2074 7261  "yes">Export tra
-00005930: 6e73 706f 6e64 6572 2069 6420 6461 7461  nsponder id data
-00005940: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-00005950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005970: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00005980: 6c61 6265 6c22 2074 7261 6e73 6c61 7461  label" translata
-00005990: 626c 653d 2279 6573 223e 5f43 6869 7066  ble="yes">_Chipf
-000059a0: 696c 653c 2f70 726f 7065 7274 793e 0a20  ile</property>. 
+00005900: 616d 653d 2276 6973 6962 6c65 223e 5472  ame="visible">Tr
+00005910: 7565 3c2f 7072 6f70 6572 7479 3e0a 2020  ue</property>.  
+00005920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005930: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
+00005940: 7274 7920 6e61 6d65 3d22 6c61 6265 6c22  rty name="label"
+00005950: 3e5f 5374 6174 7573 3c2f 7072 6f70 6572  >_Status</proper
+00005960: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
+00005970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005980: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+00005990: 7573 655f 756e 6465 726c 696e 6522 3e54  use_underline">T
+000059a0: 7275 653c 2f70 726f 7065 7274 793e 0a20  rue</property>. 
 000059b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059d0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-000059e0: 653d 2275 7365 5f75 6e64 6572 6c69 6e65  e="use_underline
-000059f0: 223e 5472 7565 3c2f 7072 6f70 6572 7479  ">True</property
-00005a00: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00005a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a20: 2020 2020 2020 3c73 6967 6e61 6c20 6e61        <signal na
-00005a30: 6d65 3d22 6163 7469 7661 7465 2220 6861  me="activate" ha
-00005a40: 6e64 6c65 723d 226d 656e 755f 6578 706f  ndler="menu_expo
-00005a50: 7274 5f63 6869 7066 696c 655f 6163 7469  rt_chipfile_acti
-00005a60: 7661 7465 5f63 6222 2f3e 0a20 2020 2020  vate_cb"/>.     
+000059c0: 2020 2020 2020 2020 2020 203c 7369 676e             <sign
+000059d0: 616c 206e 616d 653d 2261 6374 6976 6174  al name="activat
+000059e0: 6522 2068 616e 646c 6572 3d22 6d65 6e75  e" handler="menu
+000059f0: 5f74 696d 696e 675f 7374 6174 7573 5f63  _timing_status_c
+00005a00: 6222 2f3e 0a20 2020 2020 2020 2020 2020  b"/>.           
+00005a10: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00005a20: 2f6f 626a 6563 743e 0a20 2020 2020 2020  /object>.       
+00005a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a40: 203c 2f63 6869 6c64 3e0a 2020 2020 2020   </child>.      
+00005a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a60: 2020 3c63 6869 6c64 3e0a 2020 2020 2020    <child>.      
 00005a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a80: 2020 2020 2020 2020 2020 2020 203c 2f6f               </o
-00005a90: 626a 6563 743e 0a20 2020 2020 2020 2020  bject>.         
-00005aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ab0: 2020 2020 2020 203c 2f63 6869 6c64 3e0a         </child>.
+00005a80: 2020 2020 3c6f 626a 6563 7420 636c 6173      <object clas
+00005a90: 733d 2247 746b 4d65 6e75 4974 656d 2220  s="GtkMenuItem" 
+00005aa0: 6964 3d22 6d65 6e75 5f74 696d 696e 675f  id="menu_timing_
+00005ab0: 7265 636f 6e6e 6563 7422 3e0a 2020 2020  reconnect">.    
 00005ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ae0: 3c63 6869 6c64 3e0a 2020 2020 2020 2020  <child>.        
-00005af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b00: 2020 2020 2020 2020 2020 3c6f 626a 6563            <objec
-00005b10: 7420 636c 6173 733d 2247 746b 4d65 6e75  t class="GtkMenu
-00005b20: 4974 656d 2220 6964 3d22 6d65 6e75 5f65  Item" id="menu_e
-00005b30: 7870 6f72 745f 7374 6172 746c 6973 7422  xport_startlist"
-00005b40: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00005ad0: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
+00005ae0: 7920 6e61 6d65 3d22 6c61 6265 6c22 3e5f  y name="label">_
+00005af0: 5265 636f 6e6e 6563 743c 2f70 726f 7065  Reconnect</prope
+00005b00: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
+00005b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b20: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00005b30: 2276 6973 6962 6c65 223e 5472 7565 3c2f  "visible">True</
+00005b40: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
 00005b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005b60: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
-00005b70: 6e61 6d65 3d22 7669 7369 626c 6522 3e54  name="visible">T
-00005b80: 7275 653c 2f70 726f 7065 7274 793e 0a20  rue</property>. 
-00005b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b70: 6e61 6d65 3d22 7573 655f 756e 6465 726c  name="use_underl
+00005b80: 696e 6522 3e54 7275 653c 2f70 726f 7065  ine">True</prope
+00005b90: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
 00005ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bb0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00005bc0: 653d 2274 6f6f 6c74 6970 5f74 6578 7422  e="tooltip_text"
-00005bd0: 2074 7261 6e73 6c61 7461 626c 653d 2279   translatable="y
-00005be0: 6573 223e 4578 706f 7274 2061 2073 7461  es">Export a sta
-00005bf0: 7274 6c69 7374 3c2f 7072 6f70 6572 7479  rtlist</property
-00005c00: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00005c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c20: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
-00005c30: 6e61 6d65 3d22 6c61 6265 6c22 2074 7261  name="label" tra
-00005c40: 6e73 6c61 7461 626c 653d 2279 6573 223e  nslatable="yes">
-00005c50: 5f53 7461 7274 6c69 7374 3c2f 7072 6f70  _Startlist</prop
-00005c60: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
-00005c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c80: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00005c90: 7274 7920 6e61 6d65 3d22 7573 655f 756e  rty name="use_un
-00005ca0: 6465 726c 696e 6522 3e54 7275 653c 2f70  derline">True</p
-00005cb0: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
-00005cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cd0: 2020 2020 2020 2020 2020 2020 203c 7369               <si
-00005ce0: 676e 616c 206e 616d 653d 2261 6374 6976  gnal name="activ
-00005cf0: 6174 6522 2068 616e 646c 6572 3d22 6d65  ate" handler="me
-00005d00: 6e75 5f65 7870 6f72 745f 7374 6172 746c  nu_export_startl
-00005d10: 6973 745f 6163 7469 7661 7465 5f63 6222  ist_activate_cb"
-00005d20: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00005d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d40: 2020 2020 203c 2f6f 626a 6563 743e 0a20       </object>. 
-00005d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d60: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00005d70: 2f63 6869 6c64 3e0a 2020 2020 2020 2020  /child>.        
-00005d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d90: 2020 2020 2020 3c2f 6f62 6a65 6374 3e0a        </object>.
-00005da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005db0: 2020 2020 2020 2020 2020 2020 3c2f 6368              </ch
-00005dc0: 696c 643e 0a20 2020 2020 2020 2020 2020  ild>.           
-00005dd0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00005de0: 2f6f 626a 6563 743e 0a20 2020 2020 2020  /object>.       
+00005bb0: 203c 7369 676e 616c 206e 616d 653d 2261   <signal name="a
+00005bc0: 6374 6976 6174 6522 2068 616e 646c 6572  ctivate" handler
+00005bd0: 3d22 6d65 6e75 5f74 696d 696e 675f 7265  ="menu_timing_re
+00005be0: 636f 6e6e 6563 745f 6163 7469 7661 7465  connect_activate
+00005bf0: 5f63 6222 2f3e 0a20 2020 2020 2020 2020  _cb"/>.         
+00005c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c10: 203c 2f6f 626a 6563 743e 0a20 2020 2020   </object>.     
+00005c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c30: 2020 203c 2f63 6869 6c64 3e0a 2020 2020     </child>.    
+00005c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c50: 2020 2020 3c63 6869 6c64 3e0a 2020 2020      <child>.    
+00005c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c70: 2020 2020 2020 3c6f 626a 6563 7420 636c        <object cl
+00005c80: 6173 733d 2247 746b 4d65 6e75 4974 656d  ass="GtkMenuItem
+00005c90: 2220 6964 3d22 6d65 6e75 5f74 696d 696e  " id="menu_timin
+00005ca0: 675f 636f 6e66 6967 7572 6522 3e0a 2020  g_configure">.  
+00005cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cc0: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
+00005cd0: 7274 7920 6e61 6d65 3d22 7669 7369 626c  rty name="visibl
+00005ce0: 6522 3e54 7275 653c 2f70 726f 7065 7274  e">True</propert
+00005cf0: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
+00005d00: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00005d10: 7072 6f70 6572 7479 206e 616d 653d 226c  property name="l
+00005d20: 6162 656c 223e 435f 6f6e 6669 6775 7265  abel">C_onfigure
+00005d30: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+00005d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d50: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
+00005d60: 7920 6e61 6d65 3d22 7573 655f 756e 6465  y name="use_unde
+00005d70: 726c 696e 6522 3e54 7275 653c 2f70 726f  rline">True</pro
+00005d80: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
+00005d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005da0: 2020 203c 7369 676e 616c 206e 616d 653d     <signal name=
+00005db0: 2261 6374 6976 6174 6522 2068 616e 646c  "activate" handl
+00005dc0: 6572 3d22 6d65 6e75 5f74 696d 696e 675f  er="menu_timing_
+00005dd0: 636f 6e66 6967 7572 655f 6163 7469 7661  configure_activa
+00005de0: 7465 5f63 6222 2f3e 0a20 2020 2020 2020  te_cb"/>.       
 00005df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e00: 203c 2f63 6869 6c64 3e0a 2020 2020 2020   </child>.      
+00005e00: 2020 203c 2f6f 626a 6563 743e 0a20 2020     </object>.   
 00005e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e20: 2020 3c63 6869 6c64 3e0a 2020 2020 2020    <child>.      
+00005e20: 2020 2020 203c 2f63 6869 6c64 3e0a 2020       </child>.  
 00005e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e40: 2020 2020 3c6f 626a 6563 7420 636c 6173      <object clas
-00005e50: 733d 2247 746b 5365 7061 7261 746f 724d  s="GtkSeparatorM
-00005e60: 656e 7549 7465 6d22 2069 643d 226d 656e  enuItem" id="men
-00005e70: 755f 6461 7461 5f73 6570 223e 0a20 2020  u_data_sep">.   
-00005e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e90: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-00005ea0: 7479 206e 616d 653d 2276 6973 6962 6c65  ty name="visible
-00005eb0: 223e 5472 7565 3c2f 7072 6f70 6572 7479  ">True</property
-00005ec0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00005ed0: 2020 2020 2020 2020 2020 2020 3c2f 6f62              </ob
-00005ee0: 6a65 6374 3e0a 2020 2020 2020 2020 2020  ject>.          
-00005ef0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00005f00: 6368 696c 643e 0a20 2020 2020 2020 2020  child>.         
-00005f10: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00005f20: 6368 696c 643e 0a20 2020 2020 2020 2020  child>.         
-00005f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f40: 203c 6f62 6a65 6374 2063 6c61 7373 3d22   <object class="
-00005f50: 4774 6b49 6d61 6765 4d65 6e75 4974 656d  GtkImageMenuItem
-00005f60: 2220 6964 3d22 6d65 6e75 5f64 6174 615f  " id="menu_data_
-00005f70: 7265 7375 6c74 7322 3e0a 2020 2020 2020  results">.      
-00005f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f90: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
-00005fa0: 6e61 6d65 3d22 6c61 6265 6c22 2074 7261  name="label" tra
-00005fb0: 6e73 6c61 7461 626c 653d 2279 6573 223e  nslatable="yes">
-00005fc0: 525f 6573 756c 743c 2f70 726f 7065 7274  R_esult</propert
-00005fd0: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
-00005fe0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00005ff0: 7072 6f70 6572 7479 206e 616d 653d 2276  property name="v
-00006000: 6973 6962 6c65 223e 5472 7565 3c2f 7072  isible">True</pr
-00006010: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
-00006020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006030: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00006040: 6d65 3d22 746f 6f6c 7469 705f 7465 7874  me="tooltip_text
-00006050: 2220 7472 616e 736c 6174 6162 6c65 3d22  " translatable="
-00006060: 7965 7322 3e50 7265 7061 7265 2072 6570  yes">Prepare rep
-00006070: 6f72 7473 2061 6e64 2065 7870 6f72 743c  orts and export<
-00006080: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
-00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060a0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-000060b0: 206e 616d 653d 2275 7365 5f75 6e64 6572   name="use_under
-000060c0: 6c69 6e65 223e 5472 7565 3c2f 7072 6f70  line">True</prop
-000060d0: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
-000060e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060f0: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00006100: 3d22 696d 6167 6522 3e69 6d61 6765 3135  ="image">image15
-00006110: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-00006120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006130: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-00006140: 7920 6e61 6d65 3d22 7573 655f 7374 6f63  y name="use_stoc
-00006150: 6b22 3e46 616c 7365 3c2f 7072 6f70 6572  k">False</proper
-00006160: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
-00006170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006180: 3c61 6363 656c 6572 6174 6f72 206b 6579  <accelerator key
-00006190: 3d22 6522 2073 6967 6e61 6c3d 2261 6374  ="e" signal="act
-000061a0: 6976 6174 6522 206d 6f64 6966 6965 7273  ivate" modifiers
-000061b0: 3d22 4744 4b5f 434f 4e54 524f 4c5f 4d41  ="GDK_CONTROL_MA
-000061c0: 534b 222f 3e0a 2020 2020 2020 2020 2020  SK"/>.          
-000061d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061e0: 2020 3c73 6967 6e61 6c20 6e61 6d65 3d22    <signal name="
-000061f0: 6163 7469 7661 7465 2220 6861 6e64 6c65  activate" handle
-00006200: 723d 226d 656e 755f 6461 7461 5f72 6573  r="menu_data_res
-00006210: 756c 7473 5f63 6222 2f3e 0a20 2020 2020  ults_cb"/>.     
-00006220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006230: 2020 2020 203c 2f6f 626a 6563 743e 0a20       </object>. 
-00006240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006250: 2020 2020 2020 203c 2f63 6869 6c64 3e0a         </child>.
-00006260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006270: 2020 2020 2020 3c2f 6f62 6a65 6374 3e0a        </object>.
-00006280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006290: 2020 2020 3c2f 6368 696c 643e 0a20 2020      </child>.   
-000062a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000062b0: 2f6f 626a 6563 743e 0a20 2020 2020 2020  /object>.       
-000062c0: 2020 2020 2020 2020 203c 2f63 6869 6c64           </child
-000062d0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000062e0: 2020 3c63 6869 6c64 3e0a 2020 2020 2020    <child>.      
-000062f0: 2020 2020 2020 2020 2020 2020 3c6f 626a              <obj
-00006300: 6563 7420 636c 6173 733d 2247 746b 4d65  ect class="GtkMe
-00006310: 6e75 4974 656d 2220 6964 3d22 6d65 6e75  nuItem" id="menu
-00006320: 5f74 696d 7922 3e0a 2020 2020 2020 2020  _timy">.        
-00006330: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
-00006340: 7065 7274 7920 6e61 6d65 3d22 7669 7369  perty name="visi
-00006350: 626c 6522 3e54 7275 653c 2f70 726f 7065  ble">True</prope
-00006360: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
-00006370: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-00006380: 7479 206e 616d 653d 226c 6162 656c 2220  ty name="label" 
-00006390: 7472 616e 736c 6174 6162 6c65 3d22 7965  translatable="ye
-000063a0: 7322 3e5f 5469 6d69 6e67 3c2f 7072 6f70  s">_Timing</prop
-000063b0: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
-000063c0: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-000063d0: 7274 7920 6e61 6d65 3d22 7573 655f 756e  rty name="use_un
-000063e0: 6465 726c 696e 6522 3e54 7275 653c 2f70  derline">True</p
-000063f0: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
-00006400: 2020 2020 2020 2020 2020 2020 203c 6368               <ch
-00006410: 696c 6420 7479 7065 3d22 7375 626d 656e  ild type="submen
-00006420: 7522 3e0a 2020 2020 2020 2020 2020 2020  u">.            
-00006430: 2020 2020 2020 2020 2020 3c6f 626a 6563            <objec
-00006440: 7420 636c 6173 733d 2247 746b 4d65 6e75  t class="GtkMenu
-00006450: 2220 6964 3d22 6d65 6e75 3422 3e0a 2020  " id="menu4">.  
-00006460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006470: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
-00006480: 6e61 6d65 3d22 7669 7369 626c 6522 3e54  name="visible">T
-00006490: 7275 653c 2f70 726f 7065 7274 793e 0a20  rue</property>. 
-000064a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064b0: 2020 2020 2020 203c 6368 696c 643e 0a20         <child>. 
-000064c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064d0: 2020 2020 2020 2020 203c 6f62 6a65 6374           <object
-000064e0: 2063 6c61 7373 3d22 4774 6b4d 656e 7549   class="GtkMenuI
-000064f0: 7465 6d22 2069 643d 226d 656e 755f 7469  tem" id="menu_ti
-00006500: 6d69 6e67 5f73 7461 7274 223e 0a20 2020  ming_start">.   
-00006510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006520: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-00006530: 7479 206e 616d 653d 226c 6162 656c 2220  ty name="label" 
-00006540: 7472 616e 736c 6174 6162 6c65 3d22 7965  translatable="ye
-00006550: 7322 3e53 6574 205f 456c 6170 7365 643c  s">Set _Elapsed<
-00006560: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
-00006570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006580: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00006590: 206e 616d 653d 2276 6973 6962 6c65 223e   name="visible">
-000065a0: 5472 7565 3c2f 7072 6f70 6572 7479 3e0a  True</property>.
-000065b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065c0: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
-000065d0: 7065 7274 7920 6e61 6d65 3d22 746f 6f6c  perty name="tool
-000065e0: 7469 705f 7465 7874 2220 7472 616e 736c  tip_text" transl
-000065f0: 6174 6162 6c65 3d22 7965 7322 3e41 646a  atable="yes">Adj
-00006600: 7573 7420 6576 656e 7420 7275 6e20 7469  ust event run ti
-00006610: 6d65 3c2f 7072 6f70 6572 7479 3e0a 2020  me</property>.  
-00006620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006630: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00006640: 7274 7920 6e61 6d65 3d22 7573 655f 756e  rty name="use_un
-00006650: 6465 726c 696e 6522 3e54 7275 653c 2f70  derline">True</p
-00006660: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
-00006670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006680: 2020 2020 203c 7369 676e 616c 206e 616d       <signal nam
-00006690: 653d 2261 6374 6976 6174 6522 2068 616e  e="activate" han
-000066a0: 646c 6572 3d22 6d65 6e75 5f74 696d 696e  dler="menu_timin
-000066b0: 675f 7374 6172 745f 6163 7469 7661 7465  g_start_activate
-000066c0: 5f63 6222 2f3e 0a20 2020 2020 2020 2020  _cb"/>.         
-000066d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066e0: 203c 2f6f 626a 6563 743e 0a20 2020 2020   </object>.     
-000066f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006700: 2020 203c 2f63 6869 6c64 3e0a 2020 2020     </child>.    
-00006710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006720: 2020 2020 3c63 6869 6c64 3e0a 2020 2020      <child>.    
-00006730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006740: 2020 2020 2020 3c6f 626a 6563 7420 636c        <object cl
-00006750: 6173 733d 2247 746b 5365 7061 7261 746f  ass="GtkSeparato
-00006760: 724d 656e 7549 7465 6d22 2069 643d 226d  rMenuItem" id="m
-00006770: 656e 755f 7469 6d69 6e67 5f73 6570 3122  enu_timing_sep1"
-00006780: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00006790: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-000067a0: 726f 7065 7274 7920 6e61 6d65 3d22 7669  roperty name="vi
-000067b0: 7369 626c 6522 3e54 7275 653c 2f70 726f  sible">True</pro
-000067c0: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
-000067d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067e0: 203c 2f6f 626a 6563 743e 0a20 2020 2020   </object>.     
-000067f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006800: 2020 203c 2f63 6869 6c64 3e0a 2020 2020     </child>.    
-00006810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006820: 2020 2020 3c63 6869 6c64 3e0a 2020 2020      <child>.    
-00006830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006840: 2020 2020 2020 3c6f 626a 6563 7420 636c        <object cl
-00006850: 6173 733d 2247 746b 4d65 6e75 4974 656d  ass="GtkMenuItem
-00006860: 2220 6964 3d22 6d65 6e75 5f74 696d 696e  " id="menu_timin
-00006870: 675f 636c 6561 7222 3e0a 2020 2020 2020  g_clear">.      
-00006880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006890: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
-000068a0: 6e61 6d65 3d22 6c61 6265 6c22 2074 7261  name="label" tra
-000068b0: 6e73 6c61 7461 626c 653d 2279 6573 223e  nslatable="yes">
-000068c0: 5f4e 6577 2053 6573 7369 6f6e 3c2f 7072  _New Session</pr
-000068d0: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
-000068e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068f0: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00006900: 6d65 3d22 7669 7369 626c 6522 3e54 7275  me="visible">Tru
-00006910: 653c 2f70 726f 7065 7274 793e 0a20 2020  e</property>.   
-00006920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006930: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-00006940: 7479 206e 616d 653d 2273 656e 7369 7469  ty name="sensiti
-00006950: 7665 223e 5472 7565 3c2f 7072 6f70 6572  ve">True</proper
-00006960: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
-00006970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006980: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00006990: 746f 6f6c 7469 705f 7465 7874 2220 7472  tooltip_text" tr
-000069a0: 616e 736c 6174 6162 6c65 3d22 7965 7322  anslatable="yes"
-000069b0: 3e53 7461 7274 2061 206e 6577 2074 696d  >Start a new tim
-000069c0: 696e 6720 7365 7373 696f 6e20 6f6e 2074  ing session on t
-000069d0: 6865 2061 7474 6163 6865 6420 6465 636f  he attached deco
-000069e0: 6465 723c 2f70 726f 7065 7274 793e 0a20  der</property>. 
-000069f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a00: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
-00006a10: 6572 7479 206e 616d 653d 2275 7365 5f75  erty name="use_u
-00006a20: 6e64 6572 6c69 6e65 223e 5472 7565 3c2f  nderline">True</
-00006a30: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
-00006a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a50: 2020 2020 2020 3c73 6967 6e61 6c20 6e61        <signal na
-00006a60: 6d65 3d22 6163 7469 7661 7465 2220 6861  me="activate" ha
-00006a70: 6e64 6c65 723d 226d 656e 755f 7469 6d69  ndler="menu_timi
-00006a80: 6e67 5f63 6c65 6172 5f61 6374 6976 6174  ng_clear_activat
-00006a90: 655f 6362 222f 3e0a 2020 2020 2020 2020  e_cb"/>.        
-00006aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ab0: 2020 3c2f 6f62 6a65 6374 3e0a 2020 2020    </object>.    
-00006ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ad0: 2020 2020 3c2f 6368 696c 643e 0a20 2020      </child>.   
-00006ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006af0: 2020 2020 203c 6368 696c 643e 0a20 2020       <child>.   
-00006b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b10: 2020 2020 2020 203c 6f62 6a65 6374 2063         <object c
-00006b20: 6c61 7373 3d22 4774 6b4d 656e 7549 7465  lass="GtkMenuIte
-00006b30: 6d22 2069 643d 226d 656e 755f 7469 6d69  m" id="menu_timi
-00006b40: 6e67 5f73 7461 7475 7322 3e0a 2020 2020  ng_status">.    
-00006b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b60: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-00006b70: 7920 6e61 6d65 3d22 7669 7369 626c 6522  y name="visible"
-00006b80: 3e54 7275 653c 2f70 726f 7065 7274 793e  >True</property>
-00006b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006ba0: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
-00006bb0: 6f70 6572 7479 206e 616d 653d 2274 6f6f  operty name="too
-00006bc0: 6c74 6970 5f74 6578 7422 2074 7261 6e73  ltip_text" trans
-00006bd0: 6c61 7461 626c 653d 2279 6573 223e 5265  latable="yes">Re
-00006be0: 7175 6573 7420 7374 6174 7573 2066 726f  quest status fro
-00006bf0: 6d20 6174 7461 6368 6564 2064 6563 6f64  m attached decod
-00006c00: 6572 3c2f 7072 6f70 6572 7479 3e0a 2020  er</property>.  
-00006c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c20: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00006c30: 7274 7920 6e61 6d65 3d22 6c61 6265 6c22  rty name="label"
-00006c40: 2074 7261 6e73 6c61 7461 626c 653d 2279   translatable="y
-00006c50: 6573 223e 5f53 7461 7475 733c 2f70 726f  es">_Status</pro
-00006c60: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
-00006c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c80: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00006c90: 653d 2275 7365 5f75 6e64 6572 6c69 6e65  e="use_underline
-00006ca0: 223e 5472 7565 3c2f 7072 6f70 6572 7479  ">True</property
+00005e40: 2020 2020 3c2f 6f62 6a65 6374 3e0a 2020      </object>.  
+00005e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e60: 2020 3c2f 6368 696c 643e 0a20 2020 2020    </child>.     
+00005e70: 2020 2020 2020 2020 2020 2020 203c 2f6f               </o
+00005e80: 626a 6563 743e 0a20 2020 2020 2020 2020  bject>.         
+00005e90: 2020 2020 2020 203c 2f63 6869 6c64 3e0a         </child>.
+00005ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005eb0: 3c63 6869 6c64 3e0a 2020 2020 2020 2020  <child>.        
+00005ec0: 2020 2020 2020 2020 2020 3c6f 626a 6563            <objec
+00005ed0: 7420 636c 6173 733d 2247 746b 4d65 6e75  t class="GtkMenu
+00005ee0: 4974 656d 2220 6964 3d22 6d65 6e75 5f68  Item" id="menu_h
+00005ef0: 656c 7022 3e0a 2020 2020 2020 2020 2020  elp">.          
+00005f00: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
+00005f10: 7274 7920 6e61 6d65 3d22 7669 7369 626c  rty name="visibl
+00005f20: 6522 3e54 7275 653c 2f70 726f 7065 7274  e">True</propert
+00005f30: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
+00005f40: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+00005f50: 206e 616d 653d 226c 6162 656c 223e 5f48   name="label">_H
+00005f60: 656c 703c 2f70 726f 7065 7274 793e 0a20  elp</property>. 
+00005f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f80: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+00005f90: 653d 2275 7365 5f75 6e64 6572 6c69 6e65  e="use_underline
+00005fa0: 223e 5472 7565 3c2f 7072 6f70 6572 7479  ">True</property
+00005fb0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00005fc0: 2020 2020 2020 3c63 6869 6c64 2074 7970        <child typ
+00005fd0: 653d 2273 7562 6d65 6e75 223e 0a20 2020  e="submenu">.   
+00005fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ff0: 2020 203c 6f62 6a65 6374 2063 6c61 7373     <object class
+00006000: 3d22 4774 6b4d 656e 7522 2069 643d 226d  ="GtkMenu" id="m
+00006010: 656e 7533 223e 0a20 2020 2020 2020 2020  enu3">.         
+00006020: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00006030: 7072 6f70 6572 7479 206e 616d 653d 2276  property name="v
+00006040: 6973 6962 6c65 223e 5472 7565 3c2f 7072  isible">True</pr
+00006050: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
+00006060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006070: 3c63 6869 6c64 3e0a 2020 2020 2020 2020  <child>.        
+00006080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006090: 2020 3c6f 626a 6563 7420 636c 6173 733d    <object class=
+000060a0: 2247 746b 4d65 6e75 4974 656d 2220 6964  "GtkMenuItem" id
+000060b0: 3d22 6d65 6e75 5f68 656c 705f 6162 6f75  ="menu_help_abou
+000060c0: 7422 3e0a 2020 2020 2020 2020 2020 2020  t">.            
+000060d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060e0: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+000060f0: 6c61 6265 6c22 3e5f 4162 6f75 743c 2f70  label">_About</p
+00006100: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
+00006110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006120: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+00006130: 616d 653d 2276 6973 6962 6c65 223e 5472  ame="visible">Tr
+00006140: 7565 3c2f 7072 6f70 6572 7479 3e0a 2020  ue</property>.  
+00006150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006160: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
+00006170: 7274 7920 6e61 6d65 3d22 7573 655f 756e  rty name="use_un
+00006180: 6465 726c 696e 6522 3e54 7275 653c 2f70  derline">True</p
+00006190: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
+000061a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061b0: 2020 2020 203c 7369 676e 616c 206e 616d       <signal nam
+000061c0: 653d 2261 6374 6976 6174 6522 2068 616e  e="activate" han
+000061d0: 646c 6572 3d22 6d65 6e75 5f68 656c 705f  dler="menu_help_
+000061e0: 6162 6f75 745f 6362 222f 3e0a 2020 2020  about_cb"/>.    
+000061f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006200: 2020 2020 2020 3c2f 6f62 6a65 6374 3e0a        </object>.
+00006210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006220: 2020 2020 2020 2020 3c2f 6368 696c 643e          </child>
+00006230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006240: 2020 2020 2020 203c 2f6f 626a 6563 743e         </object>
+00006250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006260: 2020 2020 203c 2f63 6869 6c64 3e0a 2020       </child>.  
+00006270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006280: 3c2f 6f62 6a65 6374 3e0a 2020 2020 2020  </object>.      
+00006290: 2020 2020 2020 2020 2020 3c2f 6368 696c            </chil
+000062a0: 643e 0a20 2020 2020 2020 2020 2020 2020  d>.             
+000062b0: 203c 2f6f 626a 6563 743e 0a20 2020 2020   </object>.     
+000062c0: 2020 2020 2020 2020 203c 7061 636b 696e           <packin
+000062d0: 673e 0a20 2020 2020 2020 2020 2020 2020  g>.             
+000062e0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+000062f0: 653d 2270 6163 6b2d 7479 7065 223e 7374  e="pack-type">st
+00006300: 6172 743c 2f70 726f 7065 7274 793e 0a20  art</property>. 
+00006310: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00006320: 7072 6f70 6572 7479 206e 616d 653d 2265  property name="e
+00006330: 7870 616e 6422 3e54 7275 653c 2f70 726f  xpand">True</pro
+00006340: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
+00006350: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+00006360: 206e 616d 653d 2266 696c 6c22 3e54 7275   name="fill">Tru
+00006370: 653c 2f70 726f 7065 7274 793e 0a20 2020  e</property>.   
+00006380: 2020 2020 2020 2020 2020 203c 2f70 6163             </pac
+00006390: 6b69 6e67 3e0a 2020 2020 2020 2020 2020  king>.          
+000063a0: 2020 3c2f 6368 696c 643e 0a20 2020 2020    </child>.     
+000063b0: 2020 2020 2020 203c 6368 696c 643e 0a20         <child>. 
+000063c0: 2020 2020 2020 2020 2020 2020 203c 6f62               <ob
+000063d0: 6a65 6374 2063 6c61 7373 3d22 4774 6b42  ject class="GtkB
+000063e0: 7574 746f 6e22 2069 643d 226d 656e 755f  utton" id="menu_
+000063f0: 636c 6f63 6b22 3e0a 2020 2020 2020 2020  clock">.        
+00006400: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
+00006410: 7920 6e61 6d65 3d22 7669 7369 626c 6522  y name="visible"
+00006420: 3e54 7275 653c 2f70 726f 7065 7274 793e  >True</property>
+00006430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006440: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00006450: 2263 616e 5f66 6f63 7573 223e 4661 6c73  "can_focus">Fals
+00006460: 653c 2f70 726f 7065 7274 793e 0a20 2020  e</property>.   
+00006470: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
+00006480: 6f70 6572 7479 206e 616d 653d 2273 656e  operty name="sen
+00006490: 7369 7469 7665 223e 5472 7565 3c2f 7072  sitive">True</pr
+000064a0: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
+000064b0: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
+000064c0: 7920 6e61 6d65 3d22 7265 6365 6976 6573  y name="receives
+000064d0: 5f64 6566 6175 6c74 223e 4661 6c73 653c  _default">False<
+000064e0: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
+000064f0: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
+00006500: 6572 7479 206e 616d 653d 2266 6f63 7573  erty name="focus
+00006510: 5f6f 6e5f 636c 6963 6b22 3e46 616c 7365  _on_click">False
+00006520: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+00006530: 2020 2020 2020 2020 2020 2020 3c73 6967              <sig
+00006540: 6e61 6c20 6e61 6d65 3d22 636c 6963 6b65  nal name="clicke
+00006550: 6422 2068 616e 646c 6572 3d22 6d65 6e75  d" handler="menu
+00006560: 5f63 6c6f 636b 5f63 6c69 636b 6564 5f63  _clock_clicked_c
+00006570: 6222 2f3e 0a20 2020 2020 2020 2020 2020  b"/>.           
+00006580: 2020 203c 2f6f 626a 6563 743e 0a20 2020     </object>.   
+00006590: 2020 2020 2020 2020 2020 203c 7061 636b             <pack
+000065a0: 696e 673e 0a20 2020 2020 2020 2020 2020  ing>.           
+000065b0: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+000065c0: 616d 653d 2270 6163 6b2d 7479 7065 223e  ame="pack-type">
+000065d0: 7374 6172 743c 2f70 726f 7065 7274 793e  start</property>
+000065e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000065f0: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00006600: 2265 7870 616e 6422 3e46 616c 7365 3c2f  "expand">False</
+00006610: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
+00006620: 2020 2020 2020 2020 3c2f 7061 636b 696e          </packin
+00006630: 673e 0a20 2020 2020 2020 2020 2020 203c  g>.            <
+00006640: 2f63 6869 6c64 3e0a 2020 2020 2020 2020  /child>.        
+00006650: 2020 3c2f 6f62 6a65 6374 3e0a 2020 2020    </object>.    
+00006660: 2020 2020 2020 3c70 6163 6b69 6e67 3e0a        <packing>.
+00006670: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
+00006680: 7065 7274 7920 6e61 6d65 3d22 6578 7061  perty name="expa
+00006690: 6e64 223e 4661 6c73 653c 2f70 726f 7065  nd">False</prope
+000066a0: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
+000066b0: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+000066c0: 2270 6163 6b2d 7479 7065 223e 7374 6172  "pack-type">star
+000066d0: 743c 2f70 726f 7065 7274 793e 0a20 2020  t</property>.   
+000066e0: 2020 2020 2020 203c 2f70 6163 6b69 6e67         </packing
+000066f0: 3e0a 2020 2020 2020 2020 3c2f 6368 696c  >.        </chil
+00006700: 643e 0a20 2020 2020 2020 203c 212d 2d20  d>.        <!-- 
+00006710: 656e 6420 6f66 206d 656e 7520 6261 7220  end of menu bar 
+00006720: 2d2d 3e0a 0a20 2020 2020 2020 203c 212d  -->..        <!-
+00006730: 2d20 6576 656e 7420 7374 6174 7573 2061  - event status a
+00006740: 6e64 2063 6f6e 7472 6f6c 2062 6f78 202d  nd control box -
+00006750: 2d3e 0a20 2020 2020 2020 203c 6368 696c  ->.        <chil
+00006760: 643e 0a20 2020 2020 2020 2020 203c 6f62  d>.          <ob
+00006770: 6a65 6374 2063 6c61 7373 3d22 4774 6b42  ject class="GtkB
+00006780: 6f78 2220 6964 3d22 6576 656e 745f 7374  ox" id="event_st
+00006790: 6174 5f68 626f 7822 3e0a 2020 2020 2020  at_hbox">.      
+000067a0: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+000067b0: 6e61 6d65 3d22 6f72 6965 6e74 6174 696f  name="orientatio
+000067c0: 6e22 3e68 6f72 697a 6f6e 7461 6c3c 2f70  n">horizontal</p
+000067d0: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
+000067e0: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+000067f0: 616d 653d 2276 6973 6962 6c65 223e 5472  ame="visible">Tr
+00006800: 7565 3c2f 7072 6f70 6572 7479 3e0a 2020  ue</property>.  
+00006810: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
+00006820: 7274 7920 6e61 6d65 3d22 626f 7264 6572  rty name="border
+00006830: 5f77 6964 7468 223e 323c 2f70 726f 7065  _width">2</prope
+00006840: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
+00006850: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00006860: 2273 7061 6369 6e67 223e 343c 2f70 726f  "spacing">4</pro
+00006870: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
+00006880: 2020 203c 6368 696c 643e 0a20 2020 2020     <child>.     
+00006890: 2020 2020 2020 2020 203c 6f62 6a65 6374           <object
+000068a0: 2063 6c61 7373 3d22 4774 6b42 7574 746f   class="GtkButto
+000068b0: 6e22 2069 643d 2265 7665 6e74 5f73 7461  n" id="event_sta
+000068c0: 745f 6275 7422 3e0a 2020 2020 2020 2020  t_but">.        
+000068d0: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
+000068e0: 7920 6e61 6d65 3d22 7769 6474 685f 7265  y name="width_re
+000068f0: 7175 6573 7422 3e31 3630 3c2f 7072 6f70  quest">160</prop
+00006900: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
+00006910: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+00006920: 6e61 6d65 3d22 7669 7369 626c 6522 3e54  name="visible">T
+00006930: 7275 653c 2f70 726f 7065 7274 793e 0a20  rue</property>. 
+00006940: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00006950: 7369 676e 616c 206e 616d 653d 2263 6c69  signal name="cli
+00006960: 636b 6564 2220 6861 6e64 6c65 723d 2265  cked" handler="e
+00006970: 7665 6e74 5f73 7461 745f 6275 745f 636c  vent_stat_but_cl
+00006980: 6963 6b65 645f 6362 222f 3e0a 2020 2020  icked_cb"/>.    
+00006990: 2020 2020 2020 2020 2020 3c2f 6f62 6a65            </obje
+000069a0: 6374 3e0a 2020 2020 2020 2020 2020 2020  ct>.            
+000069b0: 2020 3c70 6163 6b69 6e67 3e0a 2020 2020    <packing>.    
+000069c0: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
+000069d0: 7065 7274 7920 6e61 6d65 3d22 6578 7061  perty name="expa
+000069e0: 6e64 223e 4661 6c73 653c 2f70 726f 7065  nd">False</prope
+000069f0: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
+00006a00: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+00006a10: 616d 653d 2270 6163 6b2d 7479 7065 223e  ame="pack-type">
+00006a20: 7374 6172 743c 2f70 726f 7065 7274 793e  start</property>
+00006a30: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00006a40: 2f70 6163 6b69 6e67 3e0a 2020 2020 2020  /packing>.      
+00006a50: 2020 2020 2020 3c2f 6368 696c 643e 0a20        </child>. 
+00006a60: 2020 2020 2020 2020 2020 203c 6368 696c             <chil
+00006a70: 643e 0a20 2020 2020 2020 2020 2020 2020  d>.             
+00006a80: 203c 6f62 6a65 6374 2063 6c61 7373 3d22   <object class="
+00006a90: 4774 6b43 6f6d 626f 426f 7822 2069 643d  GtkComboBox" id=
+00006aa0: 2265 7665 6e74 5f61 6374 696f 6e5f 636f  "event_action_co
+00006ab0: 6d62 6f22 3e0a 2020 2020 2020 2020 2020  mbo">.          
+00006ac0: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+00006ad0: 6e61 6d65 3d22 7669 7369 626c 6522 3e54  name="visible">T
+00006ae0: 7275 653c 2f70 726f 7065 7274 793e 0a20  rue</property>. 
+00006af0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00006b00: 7072 6f70 6572 7479 206e 616d 653d 226d  property name="m
+00006b10: 6f64 656c 223e 6576 656e 745f 6163 7469  odel">event_acti
+00006b20: 6f6e 5f6d 6f64 656c 3c2f 7072 6f70 6572  on_model</proper
+00006b30: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
+00006b40: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00006b50: 6d65 3d22 6163 7469 7665 223e 303c 2f70  me="active">0</p
+00006b60: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
+00006b70: 2020 2020 2020 2020 203c 7369 676e 616c           <signal
+00006b80: 206e 616d 653d 2263 6861 6e67 6564 2220   name="changed" 
+00006b90: 6861 6e64 6c65 723d 2265 7665 6e74 5f61  handler="event_a
+00006ba0: 6374 696f 6e5f 636f 6d62 6f5f 6368 616e  ction_combo_chan
+00006bb0: 6765 645f 6362 222f 3e0a 2020 2020 2020  ged_cb"/>.      
+00006bc0: 2020 2020 2020 2020 2020 3c63 6869 6c64            <child
+00006bd0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00006be0: 2020 2020 3c6f 626a 6563 7420 636c 6173      <object clas
+00006bf0: 733d 2247 746b 4365 6c6c 5265 6e64 6572  s="GtkCellRender
+00006c00: 6572 5465 7874 2220 6964 3d22 6365 6c6c  erText" id="cell
+00006c10: 7265 6e64 6572 6572 7465 7874 3122 2f3e  renderertext1"/>
+00006c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006c30: 2020 203c 6174 7472 6962 7574 6573 3e0a     <attributes>.
+00006c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c50: 2020 2020 3c61 7474 7269 6275 7465 206e      <attribute n
+00006c60: 616d 653d 2274 6578 7422 3e31 3c2f 6174  ame="text">1</at
+00006c70: 7472 6962 7574 653e 0a20 2020 2020 2020  tribute>.       
+00006c80: 2020 2020 2020 2020 2020 203c 2f61 7474             </att
+00006c90: 7269 6275 7465 733e 0a20 2020 2020 2020  ributes>.       
+00006ca0: 2020 2020 2020 2020 203c 2f63 6869 6c64           </child
 00006cb0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00006cc0: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
-00006cd0: 6967 6e61 6c20 6e61 6d65 3d22 6163 7469  ignal name="acti
-00006ce0: 7661 7465 2220 6861 6e64 6c65 723d 226d  vate" handler="m
-00006cf0: 656e 755f 7469 6d69 6e67 5f73 7461 7475  enu_timing_statu
-00006d00: 735f 6362 222f 3e0a 2020 2020 2020 2020  s_cb"/>.        
-00006d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d20: 2020 3c2f 6f62 6a65 6374 3e0a 2020 2020    </object>.    
-00006d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d40: 2020 2020 3c2f 6368 696c 643e 0a20 2020      </child>.   
-00006d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d60: 2020 2020 203c 6368 696c 643e 0a20 2020       <child>.   
-00006d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d80: 2020 2020 2020 203c 6f62 6a65 6374 2063         <object c
-00006d90: 6c61 7373 3d22 4774 6b53 6570 6172 6174  lass="GtkSeparat
-00006da0: 6f72 4d65 6e75 4974 656d 2220 6964 3d22  orMenuItem" id="
-00006db0: 6d65 6e75 6974 656d 3122 3e0a 2020 2020  menuitem1">.    
-00006dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006dd0: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-00006de0: 7920 6e61 6d65 3d22 7669 7369 626c 6522  y name="visible"
-00006df0: 3e54 7275 653c 2f70 726f 7065 7274 793e  >True</property>
-00006e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006e10: 2020 2020 2020 2020 2020 203c 2f6f 626a             </obj
-00006e20: 6563 743e 0a20 2020 2020 2020 2020 2020  ect>.           
-00006e30: 2020 2020 2020 2020 2020 2020 203c 2f63               </c
-00006e40: 6869 6c64 3e0a 2020 2020 2020 2020 2020  hild>.          
-00006e50: 2020 2020 2020 2020 2020 2020 2020 3c63                <c
-00006e60: 6869 6c64 3e0a 2020 2020 2020 2020 2020  hild>.          
-00006e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e80: 3c6f 626a 6563 7420 636c 6173 733d 2247  <object class="G
-00006e90: 746b 4d65 6e75 4974 656d 2220 6964 3d22  tkMenuItem" id="
-00006ea0: 6d65 6e75 5f74 696d 696e 675f 7265 636f  menu_timing_reco
-00006eb0: 6e6e 6563 7422 3e0a 2020 2020 2020 2020  nnect">.        
-00006ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ed0: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00006ee0: 6d65 3d22 6c61 6265 6c22 2074 7261 6e73  me="label" trans
-00006ef0: 6c61 7461 626c 653d 2279 6573 223e 5f52  latable="yes">_R
-00006f00: 6563 6f6e 6e65 6374 3c2f 7072 6f70 6572  econnect</proper
-00006f10: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
-00006f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f30: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00006f40: 7669 7369 626c 6522 3e54 7275 653c 2f70  visible">True</p
-00006f50: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
-00006f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f70: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00006f80: 616d 653d 2274 6f6f 6c74 6970 5f74 6578  ame="tooltip_tex
-00006f90: 7422 2074 7261 6e73 6c61 7461 626c 653d  t" translatable=
-00006fa0: 2279 6573 223e 5265 636f 6e6e 6563 7420  "yes">Reconnect 
-00006fb0: 7469 6d69 6e67 2064 6576 6963 6573 3c2f  timing devices</
-00006fc0: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
-00006fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fe0: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
-00006ff0: 6e61 6d65 3d22 7573 655f 756e 6465 726c  name="use_underl
-00007000: 696e 6522 3e54 7275 653c 2f70 726f 7065  ine">True</prope
-00007010: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
-00007020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007030: 203c 7369 676e 616c 206e 616d 653d 2261   <signal name="a
-00007040: 6374 6976 6174 6522 2068 616e 646c 6572  ctivate" handler
-00007050: 3d22 6d65 6e75 5f74 696d 696e 675f 7265  ="menu_timing_re
-00007060: 636f 6e6e 6563 745f 6163 7469 7661 7465  connect_activate
-00007070: 5f63 6222 2f3e 0a20 2020 2020 2020 2020  _cb"/>.         
-00007080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007090: 203c 2f6f 626a 6563 743e 0a20 2020 2020   </object>.     
-000070a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070b0: 2020 203c 2f63 6869 6c64 3e0a 2020 2020     </child>.    
-000070c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070d0: 2020 2020 3c63 6869 6c64 3e0a 2020 2020      <child>.    
-000070e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070f0: 2020 2020 2020 3c6f 626a 6563 7420 636c        <object cl
-00007100: 6173 733d 2247 746b 4d65 6e75 4974 656d  ass="GtkMenuItem
-00007110: 2220 6964 3d22 6d65 6e75 5f74 696d 696e  " id="menu_timin
-00007120: 675f 636f 6e66 6967 7572 6522 3e0a 2020  g_configure">.  
-00007130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007140: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00007150: 7274 7920 6e61 6d65 3d22 7669 7369 626c  rty name="visibl
-00007160: 6522 3e54 7275 653c 2f70 726f 7065 7274  e">True</propert
-00007170: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
-00007180: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00007190: 7072 6f70 6572 7479 206e 616d 653d 2274  property name="t
-000071a0: 6f6f 6c74 6970 5f74 6578 7422 2074 7261  ooltip_text" tra
-000071b0: 6e73 6c61 7461 626c 653d 2279 6573 223e  nslatable="yes">
-000071c0: 436f 6e66 6967 7572 6520 6174 7461 6368  Configure attach
-000071d0: 6564 2064 6563 6f64 6572 3c2f 7072 6f70  ed decoder</prop
-000071e0: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
-000071f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007200: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00007210: 3d22 6c61 6265 6c22 2074 7261 6e73 6c61  ="label" transla
-00007220: 7461 626c 653d 2279 6573 223e 436f 6e66  table="yes">Conf
-00007230: 6967 7572 653c 2f70 726f 7065 7274 793e  igure</property>
-00007240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007250: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
-00007260: 6f70 6572 7479 206e 616d 653d 2275 7365  operty name="use
-00007270: 5f75 6e64 6572 6c69 6e65 223e 5472 7565  _underline">True
-00007280: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-00007290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072a0: 2020 2020 2020 2020 3c73 6967 6e61 6c20          <signal 
-000072b0: 6e61 6d65 3d22 6163 7469 7661 7465 2220  name="activate" 
-000072c0: 6861 6e64 6c65 723d 226d 656e 755f 7469  handler="menu_ti
-000072d0: 6d69 6e67 5f63 6f6e 6669 6775 7265 5f61  ming_configure_a
-000072e0: 6374 6976 6174 655f 6362 222f 3e0a 2020  ctivate_cb"/>.  
-000072f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007300: 2020 2020 2020 2020 3c2f 6f62 6a65 6374          </object
-00007310: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00007320: 2020 2020 2020 2020 2020 3c2f 6368 696c            </chil
-00007330: 643e 0a20 2020 2020 2020 2020 2020 2020  d>.             
-00007340: 2020 2020 2020 2020 203c 2f6f 626a 6563           </objec
-00007350: 743e 0a20 2020 2020 2020 2020 2020 2020  t>.             
-00007360: 2020 2020 2020 203c 2f63 6869 6c64 3e0a         </child>.
-00007370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007380: 2020 3c2f 6f62 6a65 6374 3e0a 2020 2020    </object>.    
-00007390: 2020 2020 2020 2020 2020 2020 3c2f 6368              </ch
-000073a0: 696c 643e 0a20 2020 2020 2020 2020 2020  ild>.           
-000073b0: 2020 2020 203c 6368 696c 643e 0a20 2020       <child>.   
-000073c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000073d0: 6f62 6a65 6374 2063 6c61 7373 3d22 4774  object class="Gt
-000073e0: 6b4d 656e 7549 7465 6d22 2069 643d 226d  kMenuItem" id="m
-000073f0: 656e 755f 6865 6c70 223e 0a20 2020 2020  enu_help">.     
-00007400: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00007410: 7072 6f70 6572 7479 206e 616d 653d 2276  property name="v
-00007420: 6973 6962 6c65 223e 5472 7565 3c2f 7072  isible">True</pr
-00007430: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
-00007440: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
-00007450: 7065 7274 7920 6e61 6d65 3d22 6c61 6265  perty name="labe
-00007460: 6c22 2074 7261 6e73 6c61 7461 626c 653d  l" translatable=
-00007470: 2279 6573 223e 5f48 656c 703c 2f70 726f  "yes">_Help</pro
-00007480: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
-00007490: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
-000074a0: 6572 7479 206e 616d 653d 2275 7365 5f75  erty name="use_u
-000074b0: 6e64 6572 6c69 6e65 223e 5472 7565 3c2f  nderline">True</
-000074c0: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
-000074d0: 2020 2020 2020 2020 2020 2020 2020 3c63                <c
-000074e0: 6869 6c64 2074 7970 653d 2273 7562 6d65  hild type="subme
-000074f0: 6e75 223e 0a20 2020 2020 2020 2020 2020  nu">.           
-00007500: 2020 2020 2020 2020 2020 203c 6f62 6a65             <obje
-00007510: 6374 2063 6c61 7373 3d22 4774 6b4d 656e  ct class="GtkMen
-00007520: 7522 2069 643d 226d 656e 7533 223e 0a20  u" id="menu3">. 
-00007530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007540: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00007550: 206e 616d 653d 2276 6973 6962 6c65 223e   name="visible">
-00007560: 5472 7565 3c2f 7072 6f70 6572 7479 3e0a  True</property>.
-00007570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007580: 2020 2020 2020 2020 3c63 6869 6c64 3e0a          <child>.
-00007590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075a0: 2020 2020 2020 2020 2020 3c6f 626a 6563            <objec
-000075b0: 7420 636c 6173 733d 2247 746b 496d 6167  t class="GtkImag
-000075c0: 654d 656e 7549 7465 6d22 2069 643d 226d  eMenuItem" id="m
-000075d0: 656e 755f 6865 6c70 5f61 626f 7574 223e  enu_help_about">
-000075e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000075f0: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
-00007600: 6f70 6572 7479 206e 616d 653d 226c 6162  operty name="lab
-00007610: 656c 223e 6774 6b2d 6162 6f75 743c 2f70  el">gtk-about</p
-00007620: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
-00007630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007640: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00007650: 616d 653d 2276 6973 6962 6c65 223e 5472  ame="visible">Tr
-00007660: 7565 3c2f 7072 6f70 6572 7479 3e0a 2020  ue</property>.  
-00007670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007680: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00007690: 7274 7920 6e61 6d65 3d22 746f 6f6c 7469  rty name="toolti
-000076a0: 705f 7465 7874 2220 7472 616e 736c 6174  p_text" translat
-000076b0: 6162 6c65 3d22 7965 7322 3e41 626f 7574  able="yes">About
-000076c0: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-000076d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076e0: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-000076f0: 7920 6e61 6d65 3d22 7573 655f 756e 6465  y name="use_unde
-00007700: 726c 696e 6522 3e54 7275 653c 2f70 726f  rline">True</pro
-00007710: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
-00007720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007730: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00007740: 653d 2275 7365 5f73 746f 636b 223e 5472  e="use_stock">Tr
-00007750: 7565 3c2f 7072 6f70 6572 7479 3e0a 2020  ue</property>.  
-00007760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007770: 2020 2020 2020 2020 2020 3c73 6967 6e61            <signa
-00007780: 6c20 6e61 6d65 3d22 6163 7469 7661 7465  l name="activate
-00007790: 2220 6861 6e64 6c65 723d 226d 656e 755f  " handler="menu_
-000077a0: 6865 6c70 5f61 626f 7574 5f63 6222 2f3e  help_about_cb"/>
-000077b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000077c0: 2020 2020 2020 2020 2020 203c 2f6f 626a             </obj
-000077d0: 6563 743e 0a20 2020 2020 2020 2020 2020  ect>.           
-000077e0: 2020 2020 2020 2020 2020 2020 203c 2f63               </c
-000077f0: 6869 6c64 3e0a 2020 2020 2020 2020 2020  hild>.          
-00007800: 2020 2020 2020 2020 2020 2020 3c2f 6f62              </ob
-00007810: 6a65 6374 3e0a 2020 2020 2020 2020 2020  ject>.          
-00007820: 2020 2020 2020 2020 2020 3c2f 6368 696c            </chil
-00007830: 643e 0a20 2020 2020 2020 2020 2020 2020  d>.             
-00007840: 2020 2020 203c 2f6f 626a 6563 743e 0a20       </object>. 
-00007850: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00007860: 2f63 6869 6c64 3e0a 2020 2020 2020 2020  /child>.        
-00007870: 2020 2020 2020 3c2f 6f62 6a65 6374 3e0a        </object>.
-00007880: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-00007890: 6163 6b69 6e67 3e0a 2020 2020 2020 2020  acking>.        
-000078a0: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-000078b0: 7920 6e61 6d65 3d22 706f 7369 7469 6f6e  y name="position
-000078c0: 223e 303c 2f70 726f 7065 7274 793e 0a20  ">0</property>. 
-000078d0: 2020 2020 2020 2020 2020 2020 203c 2f70               </p
-000078e0: 6163 6b69 6e67 3e0a 2020 2020 2020 2020  acking>.        
-000078f0: 2020 2020 3c2f 6368 696c 643e 0a20 2020      </child>.   
-00007900: 2020 2020 2020 2020 203c 6368 696c 643e           <child>
-00007910: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00007920: 6f62 6a65 6374 2063 6c61 7373 3d22 4774  object class="Gt
-00007930: 6b42 7574 746f 6e22 2069 643d 226d 656e  kButton" id="men
-00007940: 755f 636c 6f63 6b22 3e0a 2020 2020 2020  u_clock">.      
-00007950: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00007960: 7274 7920 6e61 6d65 3d22 7669 7369 626c  rty name="visibl
-00007970: 6522 3e54 7275 653c 2f70 726f 7065 7274  e">True</propert
-00007980: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
-00007990: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-000079a0: 653d 2263 616e 5f66 6f63 7573 223e 4661  e="can_focus">Fa
-000079b0: 6c73 653c 2f70 726f 7065 7274 793e 0a20  lse</property>. 
-000079c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000079d0: 7072 6f70 6572 7479 206e 616d 653d 2273  property name="s
-000079e0: 656e 7369 7469 7665 223e 5472 7565 3c2f  ensitive">True</
-000079f0: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
-00007a00: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00007a10: 7274 7920 6e61 6d65 3d22 7265 6365 6976  rty name="receiv
-00007a20: 6573 5f64 6566 6175 6c74 223e 4661 6c73  es_default">Fals
-00007a30: 653c 2f70 726f 7065 7274 793e 0a20 2020  e</property>.   
-00007a40: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
-00007a50: 6f70 6572 7479 206e 616d 653d 2266 6f63  operty name="foc
-00007a60: 7573 5f6f 6e5f 636c 6963 6b22 3e46 616c  us_on_click">Fal
-00007a70: 7365 3c2f 7072 6f70 6572 7479 3e0a 2020  se</property>.  
-00007a80: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
-00007a90: 6967 6e61 6c20 6e61 6d65 3d22 636c 6963  ignal name="clic
-00007aa0: 6b65 6422 2068 616e 646c 6572 3d22 6d65  ked" handler="me
-00007ab0: 6e75 5f63 6c6f 636b 5f63 6c69 636b 6564  nu_clock_clicked
-00007ac0: 5f63 6222 2f3e 0a20 2020 2020 2020 2020  _cb"/>.         
-00007ad0: 2020 2020 203c 2f6f 626a 6563 743e 0a20       </object>. 
-00007ae0: 2020 2020 2020 2020 2020 2020 203c 7061               <pa
-00007af0: 636b 696e 673e 0a20 2020 2020 2020 2020  cking>.         
-00007b00: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00007b10: 206e 616d 653d 2265 7870 616e 6422 3e46   name="expand">F
-00007b20: 616c 7365 3c2f 7072 6f70 6572 7479 3e0a  alse</property>.
-00007b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b40: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00007b50: 706f 7369 7469 6f6e 223e 323c 2f70 726f  position">2</pro
-00007b60: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
-00007b70: 2020 2020 203c 2f70 6163 6b69 6e67 3e0a       </packing>.
-00007b80: 2020 2020 2020 2020 2020 2020 3c2f 6368              </ch
-00007b90: 696c 643e 0a20 2020 2020 2020 2020 203c  ild>.          <
-00007ba0: 2f6f 626a 6563 743e 0a20 2020 2020 2020  /object>.       
-00007bb0: 2020 203c 7061 636b 696e 673e 0a20 2020     <packing>.   
-00007bc0: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-00007bd0: 7479 206e 616d 653d 2265 7870 616e 6422  ty name="expand"
-00007be0: 3e46 616c 7365 3c2f 7072 6f70 6572 7479  >False</property
-00007bf0: 3e0a 2020 2020 2020 2020 2020 2020 3c70  >.            <p
-00007c00: 726f 7065 7274 7920 6e61 6d65 3d22 706f  roperty name="po
-00007c10: 7369 7469 6f6e 223e 303c 2f70 726f 7065  sition">0</prope
-00007c20: 7274 793e 0a20 2020 2020 2020 2020 203c  rty>.          <
-00007c30: 2f70 6163 6b69 6e67 3e0a 2020 2020 2020  /packing>.      
-00007c40: 2020 3c2f 6368 696c 643e 0a20 2020 2020    </child>.     
-00007c50: 2020 203c 6368 696c 643e 0a20 2020 2020     <child>.     
-00007c60: 2020 2020 203c 6f62 6a65 6374 2063 6c61       <object cla
-00007c70: 7373 3d22 4774 6b48 426f 7822 2069 643d  ss="GtkHBox" id=
-00007c80: 2272 6163 655f 7374 6174 5f68 626f 7822  "race_stat_hbox"
-00007c90: 3e0a 2020 2020 2020 2020 2020 2020 3c70  >.            <p
-00007ca0: 726f 7065 7274 7920 6e61 6d65 3d22 7669  roperty name="vi
-00007cb0: 7369 626c 6522 3e54 7275 653c 2f70 726f  sible">True</pro
-00007cc0: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
-00007cd0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00007ce0: 653d 2262 6f72 6465 725f 7769 6474 6822  e="border_width"
-00007cf0: 3e32 3c2f 7072 6f70 6572 7479 3e0a 2020  >2</property>.  
-00007d00: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00007d10: 7274 7920 6e61 6d65 3d22 7370 6163 696e  rty name="spacin
-00007d20: 6722 3e34 3c2f 7072 6f70 6572 7479 3e0a  g">4</property>.
-00007d30: 2020 2020 2020 2020 2020 2020 3c63 6869              <chi
-00007d40: 6c64 3e0a 2020 2020 2020 2020 2020 2020  ld>.            
-00007d50: 2020 3c6f 626a 6563 7420 636c 6173 733d    <object class=
-00007d60: 2247 746b 4275 7474 6f6e 2220 6964 3d22  "GtkButton" id="
-00007d70: 7261 6365 5f73 7461 745f 6275 7422 3e0a  race_stat_but">.
-00007d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d90: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00007da0: 7769 6474 685f 7265 7175 6573 7422 3e31  width_request">1
-00007db0: 3630 3c2f 7072 6f70 6572 7479 3e0a 2020  60</property>.  
-00007dc0: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-00007dd0: 726f 7065 7274 7920 6e61 6d65 3d22 7669  roperty name="vi
-00007de0: 7369 626c 6522 3e54 7275 653c 2f70 726f  sible">True</pro
-00007df0: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
-00007e00: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00007e10: 206e 616d 653d 2273 656e 7369 7469 7665   name="sensitive
-00007e20: 223e 5472 7565 3c2f 7072 6f70 6572 7479  ">True</property
-00007e30: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00007e40: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00007e50: 3d22 6361 6e5f 666f 6375 7322 3e46 616c  ="can_focus">Fal
-00007e60: 7365 3c2f 7072 6f70 6572 7479 3e0a 2020  se</property>.  
-00007e70: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-00007e80: 726f 7065 7274 7920 6e61 6d65 3d22 7265  roperty name="re
-00007e90: 6365 6976 6573 5f64 6566 6175 6c74 223e  ceives_default">
-00007ea0: 5472 7565 3c2f 7072 6f70 6572 7479 3e0a  True</property>.
-00007eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ec0: 3c73 6967 6e61 6c20 6e61 6d65 3d22 636c  <signal name="cl
-00007ed0: 6963 6b65 6422 2068 616e 646c 6572 3d22  icked" handler="
-00007ee0: 7261 6365 5f73 7461 745f 6275 745f 636c  race_stat_but_cl
-00007ef0: 6963 6b65 645f 6362 222f 3e0a 2020 2020  icked_cb"/>.    
-00007f00: 2020 2020 2020 2020 2020 3c2f 6f62 6a65            </obje
-00007f10: 6374 3e0a 2020 2020 2020 2020 2020 2020  ct>.            
-00007f20: 2020 3c70 6163 6b69 6e67 3e0a 2020 2020    <packing>.    
-00007f30: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
-00007f40: 7065 7274 7920 6e61 6d65 3d22 6578 7061  perty name="expa
-00007f50: 6e64 223e 4661 6c73 653c 2f70 726f 7065  nd">False</prope
-00007f60: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
-00007f70: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00007f80: 616d 653d 2270 6f73 6974 696f 6e22 3e30  ame="position">0
-00007f90: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-00007fa0: 2020 2020 2020 2020 2020 3c2f 7061 636b            </pack
-00007fb0: 696e 673e 0a20 2020 2020 2020 2020 2020  ing>.           
-00007fc0: 203c 2f63 6869 6c64 3e0a 2020 2020 2020   </child>.      
-00007fd0: 2020 2020 2020 3c63 6869 6c64 3e0a 2020        <child>.  
-00007fe0: 2020 2020 2020 2020 2020 2020 3c6f 626a              <obj
-00007ff0: 6563 7420 636c 6173 733d 2247 746b 436f  ect class="GtkCo
-00008000: 6d62 6f42 6f78 2220 6964 3d22 7261 6365  mboBox" id="race
-00008010: 5f61 6374 696f 6e5f 636f 6d62 6f22 3e0a  _action_combo">.
-00008020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008030: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00008040: 7669 7369 626c 6522 3e54 7275 653c 2f70  visible">True</p
-00008050: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
-00008060: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-00008070: 7479 206e 616d 653d 226d 6f64 656c 223e  ty name="model">
-00008080: 7261 6365 5f61 6374 696f 6e5f 6d6f 6465  race_action_mode
-00008090: 6c3c 2f70 726f 7065 7274 793e 0a20 2020  l</property>.   
-000080a0: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
-000080b0: 6f70 6572 7479 206e 616d 653d 2261 6374  operty name="act
-000080c0: 6976 6522 3e30 3c2f 7072 6f70 6572 7479  ive">0</property
-000080d0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000080e0: 2020 3c73 6967 6e61 6c20 6e61 6d65 3d22    <signal name="
-000080f0: 6368 616e 6765 6422 2068 616e 646c 6572  changed" handler
-00008100: 3d22 7261 6365 5f61 6374 696f 6e5f 636f  ="race_action_co
-00008110: 6d62 6f5f 6368 616e 6765 645f 6362 222f  mbo_changed_cb"/
-00008120: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00008130: 2020 3c63 6869 6c64 3e0a 2020 2020 2020    <child>.      
-00008140: 2020 2020 2020 2020 2020 2020 3c6f 626a              <obj
-00008150: 6563 7420 636c 6173 733d 2247 746b 4365  ect class="GtkCe
-00008160: 6c6c 5265 6e64 6572 6572 5465 7874 2220  llRendererText" 
-00008170: 6964 3d22 6365 6c6c 7265 6e64 6572 6572  id="cellrenderer
-00008180: 7465 7874 3122 2f3e 0a20 2020 2020 2020  text1"/>.       
-00008190: 2020 2020 2020 2020 2020 203c 6174 7472             <attr
-000081a0: 6962 7574 6573 3e0a 2020 2020 2020 2020  ibutes>.        
-000081b0: 2020 2020 2020 2020 2020 2020 3c61 7474              <att
-000081c0: 7269 6275 7465 206e 616d 653d 2274 6578  ribute name="tex
-000081d0: 7422 3e31 3c2f 6174 7472 6962 7574 653e  t">1</attribute>
-000081e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000081f0: 2020 203c 2f61 7474 7269 6275 7465 733e     </attributes>
-00008200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008210: 203c 2f63 6869 6c64 3e0a 2020 2020 2020   </child>.      
-00008220: 2020 2020 2020 2020 3c2f 6f62 6a65 6374          </object
-00008230: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00008240: 3c70 6163 6b69 6e67 3e0a 2020 2020 2020  <packing>.      
-00008250: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00008260: 7274 7920 6e61 6d65 3d22 6578 7061 6e64  rty name="expand
-00008270: 223e 4661 6c73 653c 2f70 726f 7065 7274  ">False</propert
-00008280: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
-00008290: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-000082a0: 653d 2270 6f73 6974 696f 6e22 3e31 3c2f  e="position">1</
-000082b0: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
-000082c0: 2020 2020 2020 2020 3c2f 7061 636b 696e          </packin
-000082d0: 673e 0a20 2020 2020 2020 2020 2020 203c  g>.            <
-000082e0: 2f63 6869 6c64 3e0a 2020 2020 2020 2020  /child>.        
-000082f0: 2020 2020 3c63 6869 6c64 3e0a 2020 2020      <child>.    
-00008300: 2020 2020 2020 2020 2020 3c6f 626a 6563            <objec
-00008310: 7420 636c 6173 733d 2247 746b 456e 7472  t class="GtkEntr
-00008320: 7922 2069 643d 2272 6163 655f 6163 7469  y" id="race_acti
-00008330: 6f6e 5f65 6e74 7279 223e 0a20 2020 2020  on_entry">.     
-00008340: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
-00008350: 6572 7479 206e 616d 653d 2276 6973 6962  erty name="visib
-00008360: 6c65 223e 5472 7565 3c2f 7072 6f70 6572  le">True</proper
-00008370: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
-00008380: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00008390: 6d65 3d22 6361 6e5f 666f 6375 7322 3e54  me="can_focus">T
-000083a0: 7275 653c 2f70 726f 7065 7274 793e 0a20  rue</property>. 
-000083b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000083c0: 7072 6f70 6572 7479 206e 616d 653d 2269  property name="i
-000083d0: 6e76 6973 6962 6c65 5f63 6861 7222 3e26  nvisible_char">&
-000083e0: 2378 3235 4346 3b3c 2f70 726f 7065 7274  #x25CF;</propert
-000083f0: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
-00008400: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00008410: 653d 2263 6170 735f 6c6f 636b 5f77 6172  e="caps_lock_war
-00008420: 6e69 6e67 223e 4661 6c73 653c 2f70 726f  ning">False</pro
-00008430: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
-00008440: 2020 2020 2020 203c 7369 676e 616c 206e         <signal n
-00008450: 616d 653d 2261 6374 6976 6174 6522 2068  ame="activate" h
-00008460: 616e 646c 6572 3d22 7261 6365 5f73 7461  andler="race_sta
-00008470: 745f 656e 7472 795f 6163 7469 7661 7465  t_entry_activate
-00008480: 5f63 6222 2f3e 0a20 2020 2020 2020 2020  _cb"/>.         
-00008490: 2020 2020 203c 2f6f 626a 6563 743e 0a20       </object>. 
-000084a0: 2020 2020 2020 2020 2020 2020 203c 7061               <pa
-000084b0: 636b 696e 673e 0a20 2020 2020 2020 2020  cking>.         
-000084c0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-000084d0: 206e 616d 653d 2270 6f73 6974 696f 6e22   name="position"
-000084e0: 3e32 3c2f 7072 6f70 6572 7479 3e0a 2020  >2</property>.  
-000084f0: 2020 2020 2020 2020 2020 2020 3c2f 7061              </pa
-00008500: 636b 696e 673e 0a20 2020 2020 2020 2020  cking>.         
-00008510: 2020 203c 2f63 6869 6c64 3e0a 2020 2020     </child>.    
-00008520: 2020 2020 2020 3c2f 6f62 6a65 6374 3e0a        </object>.
-00008530: 2020 2020 2020 2020 2020 3c70 6163 6b69            <packi
-00008540: 6e67 3e0a 2020 2020 2020 2020 2020 2020  ng>.            
-00008550: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00008560: 6578 7061 6e64 223e 4661 6c73 653c 2f70  expand">False</p
-00008570: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
-00008580: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00008590: 616d 653d 2270 6f73 6974 696f 6e22 3e31  ame="position">1
-000085a0: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-000085b0: 2020 2020 2020 3c2f 7061 636b 696e 673e        </packing>
-000085c0: 0a20 2020 2020 2020 203c 2f63 6869 6c64  .        </child
-000085d0: 3e0a 2020 2020 2020 2020 3c63 6869 6c64  >.        <child
-000085e0: 3e0a 2020 2020 2020 2020 2020 3c6f 626a  >.          <obj
-000085f0: 6563 7420 636c 6173 733d 2247 746b 4e6f  ect class="GtkNo
-00008600: 7465 626f 6f6b 2220 6964 3d22 6d65 6574  tebook" id="meet
-00008610: 5f6e 6222 3e0a 2020 2020 2020 2020 2020  _nb">.          
-00008620: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00008630: 3d22 7669 7369 626c 6522 3e54 7275 653c  ="visible">True<
-00008640: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
-00008650: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00008660: 206e 616d 653d 2263 616e 5f66 6f63 7573   name="can_focus
-00008670: 223e 5472 7565 3c2f 7072 6f70 6572 7479  ">True</property
-00008680: 3e0a 2020 2020 2020 2020 2020 2020 3c70  >.            <p
-00008690: 726f 7065 7274 7920 6e61 6d65 3d22 626f  roperty name="bo
-000086a0: 7264 6572 5f77 6964 7468 223e 343c 2f70  rder_width">4</p
-000086b0: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
-000086c0: 2020 2020 203c 6368 696c 643e 0a20 2020       <child>.   
-000086d0: 2020 2020 2020 2020 2020 203c 6f62 6a65             <obje
-000086e0: 6374 2063 6c61 7373 3d22 4774 6b46 7261  ct class="GtkFra
-000086f0: 6d65 2220 6964 3d22 7261 6365 5f62 6f78  me" id="race_box
-00008700: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00008710: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00008720: 653d 2276 6973 6962 6c65 223e 5472 7565  e="visible">True
-00008730: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-00008740: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
-00008750: 7065 7274 7920 6e61 6d65 3d22 626f 7264  perty name="bord
-00008760: 6572 5f77 6964 7468 223e 353c 2f70 726f  er_width">5</pro
-00008770: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
-00008780: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00008790: 206e 616d 653d 226c 6162 656c 5f78 616c   name="label_xal
-000087a0: 6967 6e22 3e30 3c2f 7072 6f70 6572 7479  ign">0</property
-000087b0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000087c0: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-000087d0: 3d22 7368 6164 6f77 5f74 7970 6522 3e6e  ="shadow_type">n
-000087e0: 6f6e 653c 2f70 726f 7065 7274 793e 0a20  one</property>. 
-000087f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00008800: 6368 696c 643e 0a20 2020 2020 2020 2020  child>.         
-00008810: 2020 2020 2020 2020 203c 706c 6163 6568           <placeh
-00008820: 6f6c 6465 722f 3e0a 2020 2020 2020 2020  older/>.        
-00008830: 2020 2020 2020 2020 3c2f 6368 696c 643e          </child>
-00008840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008850: 203c 6368 696c 6420 7479 7065 3d22 6c61   <child type="la
-00008860: 6265 6c5f 6974 656d 223e 0a20 2020 2020  bel_item">.     
-00008870: 2020 2020 2020 2020 2020 2020 203c 706c               <pl
-00008880: 6163 6568 6f6c 6465 722f 3e0a 2020 2020  aceholder/>.    
-00008890: 2020 2020 2020 2020 2020 2020 3c2f 6368              </ch
-000088a0: 696c 643e 0a20 2020 2020 2020 2020 2020  ild>.           
-000088b0: 2020 203c 2f6f 626a 6563 743e 0a20 2020     </object>.   
-000088c0: 2020 2020 2020 2020 2020 203c 7061 636b             <pack
-000088d0: 696e 673e 0a20 2020 2020 2020 2020 2020  ing>.           
-000088e0: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-000088f0: 616d 653d 2270 6f73 6974 696f 6e22 3e31  ame="position">1
-00008900: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-00008910: 2020 2020 2020 2020 2020 3c2f 7061 636b            </pack
-00008920: 696e 673e 0a20 2020 2020 2020 2020 2020  ing>.           
-00008930: 203c 2f63 6869 6c64 3e0a 2020 2020 2020   </child>.      
-00008940: 2020 2020 2020 3c63 6869 6c64 2074 7970        <child typ
-00008950: 653d 2274 6162 223e 0a20 2020 2020 2020  e="tab">.       
-00008960: 2020 2020 2020 203c 6f62 6a65 6374 2063         <object c
-00008970: 6c61 7373 3d22 4774 6b4c 6162 656c 2220  lass="GtkLabel" 
-00008980: 6964 3d22 7261 6365 5f62 6f78 5f74 6162  id="race_box_tab
-00008990: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-000089a0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-000089b0: 653d 226c 6162 656c 223e 4576 656e 743c  e="label">Event<
-000089c0: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
-000089d0: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
-000089e0: 6572 7479 206e 616d 653d 2277 6964 7468  erty name="width
-000089f0: 5f63 6861 7273 223e 3136 3c2f 7072 6f70  _chars">16</prop
-00008a00: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
-00008a10: 2020 2020 3c2f 6f62 6a65 6374 3e0a 2020      </object>.  
-00008a20: 2020 2020 2020 2020 2020 3c2f 6368 696c            </chil
-00008a30: 643e 0a20 2020 2020 2020 2020 2020 203c  d>.            <
-00008a40: 6368 696c 643e 0a20 2020 2020 2020 2020  child>.         
-00008a50: 2020 2020 203c 6f62 6a65 6374 2063 6c61       <object cla
-00008a60: 7373 3d22 4774 6b53 6372 6f6c 6c65 6457  ss="GtkScrolledW
-00008a70: 696e 646f 7722 2069 643d 2272 6964 6572  indow" id="rider
-00008a80: 735f 626f 7822 3e0a 2020 2020 2020 2020  s_box">.        
-00008a90: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-00008aa0: 7920 6e61 6d65 3d22 7669 7369 626c 6522  y name="visible"
-00008ab0: 3e54 7275 653c 2f70 726f 7065 7274 793e  >True</property>
-00008ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008ad0: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-00008ae0: 2263 616e 5f66 6f63 7573 223e 5472 7565  "can_focus">True
+00006cc0: 3c2f 6f62 6a65 6374 3e0a 2020 2020 2020  </object>.      
+00006cd0: 2020 2020 2020 2020 3c70 6163 6b69 6e67          <packing
+00006ce0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00006cf0: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+00006d00: 3d22 6578 7061 6e64 223e 4661 6c73 653c  ="expand">False<
+00006d10: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
+00006d20: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
+00006d30: 6572 7479 206e 616d 653d 2270 6163 6b2d  erty name="pack-
+00006d40: 7479 7065 223e 7374 6172 743c 2f70 726f  type">start</pro
+00006d50: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
+00006d60: 2020 2020 203c 2f70 6163 6b69 6e67 3e0a       </packing>.
+00006d70: 2020 2020 2020 2020 2020 2020 3c2f 6368              </ch
+00006d80: 696c 643e 0a20 2020 2020 2020 2020 2020  ild>.           
+00006d90: 203c 6368 696c 643e 0a20 2020 2020 2020   <child>.       
+00006da0: 2020 2020 2020 203c 6f62 6a65 6374 2063         <object c
+00006db0: 6c61 7373 3d22 4774 6b45 6e74 7279 2220  lass="GtkEntry" 
+00006dc0: 6964 3d22 6576 656e 745f 6163 7469 6f6e  id="event_action
+00006dd0: 5f65 6e74 7279 223e 0a20 2020 2020 2020  _entry">.       
+00006de0: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+00006df0: 7479 206e 616d 653d 2276 6973 6962 6c65  ty name="visible
+00006e00: 223e 5472 7565 3c2f 7072 6f70 6572 7479  ">True</property
+00006e10: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00006e20: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+00006e30: 3d22 6361 6e5f 666f 6375 7322 3e54 7275  ="can_focus">Tru
+00006e40: 653c 2f70 726f 7065 7274 793e 0a20 2020  e</property>.   
+00006e50: 2020 2020 2020 2020 2020 2020 203c 7369               <si
+00006e60: 676e 616c 206e 616d 653d 2261 6374 6976  gnal name="activ
+00006e70: 6174 6522 2068 616e 646c 6572 3d22 6576  ate" handler="ev
+00006e80: 656e 745f 7374 6174 5f65 6e74 7279 5f61  ent_stat_entry_a
+00006e90: 6374 6976 6174 655f 6362 222f 3e0a 2020  ctivate_cb"/>.  
+00006ea0: 2020 2020 2020 2020 2020 2020 3c2f 6f62              </ob
+00006eb0: 6a65 6374 3e0a 2020 2020 2020 2020 2020  ject>.          
+00006ec0: 2020 2020 3c70 6163 6b69 6e67 3e0a 2020      <packing>.  
+00006ed0: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
+00006ee0: 726f 7065 7274 7920 6e61 6d65 3d22 7061  roperty name="pa
+00006ef0: 636b 2d74 7970 6522 3e73 7461 7274 3c2f  ck-type">start</
+00006f00: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
+00006f10: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
+00006f20: 7274 7920 6e61 6d65 3d22 6578 7061 6e64  rty name="expand
+00006f30: 223e 5472 7565 3c2f 7072 6f70 6572 7479  ">True</property
+00006f40: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00006f50: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+00006f60: 3d22 6669 6c6c 223e 5472 7565 3c2f 7072  ="fill">True</pr
+00006f70: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
+00006f80: 2020 2020 2020 3c2f 7061 636b 696e 673e        </packing>
+00006f90: 0a20 2020 2020 2020 2020 2020 203c 2f63  .            </c
+00006fa0: 6869 6c64 3e0a 2020 2020 2020 2020 2020  hild>.          
+00006fb0: 3c2f 6f62 6a65 6374 3e0a 2020 2020 2020  </object>.      
+00006fc0: 2020 2020 3c70 6163 6b69 6e67 3e0a 2020      <packing>.  
+00006fd0: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
+00006fe0: 7274 7920 6e61 6d65 3d22 6578 7061 6e64  rty name="expand
+00006ff0: 223e 4661 6c73 653c 2f70 726f 7065 7274  ">False</propert
+00007000: 793e 0a20 2020 2020 2020 2020 2020 203c  y>.            <
+00007010: 7072 6f70 6572 7479 206e 616d 653d 2270  property name="p
+00007020: 6163 6b2d 7479 7065 223e 7374 6172 743c  ack-type">start<
+00007030: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
+00007040: 2020 2020 203c 2f70 6163 6b69 6e67 3e0a       </packing>.
+00007050: 2020 2020 2020 2020 3c2f 6368 696c 643e          </child>
+00007060: 0a20 2020 2020 2020 203c 212d 2d20 656e  .        <!-- en
+00007070: 6420 6f66 2065 7665 6e74 2073 7461 7475  d of event statu
+00007080: 7320 616e 6420 636f 6e74 726f 6c20 626f  s and control bo
+00007090: 7820 2d2d 3e0a 0a20 2020 2020 2020 203c  x -->..        <
+000070a0: 212d 2d20 6d65 6574 206e 6f74 6562 6f6f  !-- meet noteboo
+000070b0: 6b20 2d2d 3e0a 2020 2020 2020 2020 3c63  k -->.        <c
+000070c0: 6869 6c64 3e0a 2020 2020 2020 2020 2020  hild>.          
+000070d0: 3c6f 626a 6563 7420 636c 6173 733d 2247  <object class="G
+000070e0: 746b 4e6f 7465 626f 6f6b 2220 6964 3d22  tkNotebook" id="
+000070f0: 6d65 6574 5f6e 6222 3e0a 2020 2020 2020  meet_nb">.      
+00007100: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+00007110: 6e61 6d65 3d22 7669 7369 626c 6522 3e54  name="visible">T
+00007120: 7275 653c 2f70 726f 7065 7274 793e 0a20  rue</property>. 
+00007130: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
+00007140: 6572 7479 206e 616d 653d 2263 616e 5f66  erty name="can_f
+00007150: 6f63 7573 223e 5472 7565 3c2f 7072 6f70  ocus">True</prop
+00007160: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
+00007170: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+00007180: 3d22 626f 7264 6572 5f77 6964 7468 223e  ="border_width">
+00007190: 343c 2f70 726f 7065 7274 793e 0a0a 2020  4</property>..  
+000071a0: 2020 2020 2020 2020 2020 3c21 2d2d 2065            <!-- e
+000071b0: 7665 6e74 2070 6167 6520 2d2d 3e0a 2020  vent page -->.  
+000071c0: 2020 2020 2020 2020 2020 3c63 6869 6c64            <child
+000071d0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000071e0: 3c6f 626a 6563 7420 636c 6173 733d 2247  <object class="G
+000071f0: 746b 4672 616d 6522 2069 643d 2265 7665  tkFrame" id="eve
+00007200: 6e74 5f62 6f78 223e 0a20 2020 2020 2020  nt_box">.       
+00007210: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+00007220: 7479 206e 616d 653d 2276 6973 6962 6c65  ty name="visible
+00007230: 223e 5472 7565 3c2f 7072 6f70 6572 7479  ">True</property
+00007240: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00007250: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+00007260: 3d22 626f 7264 6572 5f77 6964 7468 223e  ="border_width">
+00007270: 353c 2f70 726f 7065 7274 793e 0a20 2020  5</property>.   
+00007280: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
+00007290: 6f70 6572 7479 206e 616d 653d 2273 6861  operty name="sha
+000072a0: 646f 775f 7479 7065 223e 6e6f 6e65 3c2f  dow_type">none</
+000072b0: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
+000072c0: 2020 2020 2020 2020 3c2f 6f62 6a65 6374          </object
+000072d0: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
+000072e0: 6368 696c 643e 0a20 2020 2020 2020 2020  child>.         
+000072f0: 2020 203c 6368 696c 6420 7479 7065 3d22     <child type="
+00007300: 7461 6222 3e0a 2020 2020 2020 2020 2020  tab">.          
+00007310: 2020 2020 3c6f 626a 6563 7420 636c 6173      <object clas
+00007320: 733d 2247 746b 4c61 6265 6c22 2069 643d  s="GtkLabel" id=
+00007330: 2265 7665 6e74 5f62 6f78 5f74 6162 223e  "event_box_tab">
+00007340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007350: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00007360: 226c 6162 656c 223e 4576 656e 743c 2f70  "label">Event</p
+00007370: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
+00007380: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+00007390: 7479 206e 616d 653d 2277 6964 7468 5f63  ty name="width_c
+000073a0: 6861 7273 223e 3136 3c2f 7072 6f70 6572  hars">16</proper
+000073b0: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
+000073c0: 2020 3c2f 6f62 6a65 6374 3e0a 2020 2020    </object>.    
+000073d0: 2020 2020 2020 2020 3c2f 6368 696c 643e          </child>
+000073e0: 0a0a 2020 2020 2020 2020 2020 2020 3c21  ..            <!
+000073f0: 2d2d 2072 6964 6572 7320 7061 6765 202d  -- riders page -
+00007400: 2d3e 0a20 2020 2020 2020 2020 2020 203c  ->.            <
+00007410: 6368 696c 643e 0a20 2020 2020 2020 2020  child>.         
+00007420: 2020 2020 203c 6f62 6a65 6374 2063 6c61       <object cla
+00007430: 7373 3d22 4774 6b53 6372 6f6c 6c65 6457  ss="GtkScrolledW
+00007440: 696e 646f 7722 2069 643d 2272 6964 6572  indow" id="rider
+00007450: 735f 626f 7822 3e0a 2020 2020 2020 2020  s_box">.        
+00007460: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
+00007470: 7920 6e61 6d65 3d22 7669 7369 626c 6522  y name="visible"
+00007480: 3e54 7275 653c 2f70 726f 7065 7274 793e  >True</property>
+00007490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000074a0: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+000074b0: 2263 616e 5f66 6f63 7573 223e 5472 7565  "can_focus">True
+000074c0: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+000074d0: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
+000074e0: 7065 7274 7920 6e61 6d65 3d22 626f 7264  perty name="bord
+000074f0: 6572 5f77 6964 7468 223e 353c 2f70 726f  er_width">5</pro
+00007500: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
+00007510: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+00007520: 206e 616d 653d 2268 7363 726f 6c6c 6261   name="hscrollba
+00007530: 725f 706f 6c69 6379 223e 6175 746f 6d61  r_policy">automa
+00007540: 7469 633c 2f70 726f 7065 7274 793e 0a20  tic</property>. 
+00007550: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00007560: 7072 6f70 6572 7479 206e 616d 653d 2276  property name="v
+00007570: 7363 726f 6c6c 6261 725f 706f 6c69 6379  scrollbar_policy
+00007580: 223e 6175 746f 6d61 7469 633c 2f70 726f  ">automatic</pro
+00007590: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
+000075a0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+000075b0: 206e 616d 653d 2273 6861 646f 775f 7479   name="shadow_ty
+000075c0: 7065 223e 696e 3c2f 7072 6f70 6572 7479  pe">in</property
+000075d0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000075e0: 3c2f 6f62 6a65 6374 3e0a 2020 2020 2020  </object>.      
+000075f0: 2020 2020 2020 3c2f 6368 696c 643e 0a20        </child>. 
+00007600: 2020 2020 2020 2020 2020 203c 6368 696c             <chil
+00007610: 6420 7479 7065 3d22 7461 6222 3e0a 2020  d type="tab">.  
+00007620: 2020 2020 2020 2020 2020 2020 3c6f 626a              <obj
+00007630: 6563 7420 636c 6173 733d 2247 746b 4c61  ect class="GtkLa
+00007640: 6265 6c22 2069 643d 2272 6964 6572 735f  bel" id="riders_
+00007650: 626f 785f 7461 6222 3e0a 2020 2020 2020  box_tab">.      
+00007660: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
+00007670: 7274 7920 6e61 6d65 3d22 6c61 6265 6c22  rty name="label"
+00007680: 3e52 6964 6572 2044 6174 613c 2f70 726f  >Rider Data</pro
+00007690: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
+000076a0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+000076b0: 206e 616d 653d 2277 6964 7468 5f63 6861   name="width_cha
+000076c0: 7273 223e 3136 3c2f 7072 6f70 6572 7479  rs">16</property
+000076d0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000076e0: 3c2f 6f62 6a65 6374 3e0a 2020 2020 2020  </object>.      
+000076f0: 2020 2020 2020 3c2f 6368 696c 643e 0a0a        </child>..
+00007700: 2020 2020 2020 2020 2020 2020 3c21 2d2d              <!--
+00007710: 2063 6174 6567 6f72 6965 7320 7061 6765   categories page
+00007720: 202d 2d3e 0a20 2020 2020 2020 2020 2020   -->.           
+00007730: 203c 6368 696c 643e 0a20 2020 2020 2020   <child>.       
+00007740: 2020 2020 2020 203c 6f62 6a65 6374 2063         <object c
+00007750: 6c61 7373 3d22 4774 6b53 6372 6f6c 6c65  lass="GtkScrolle
+00007760: 6457 696e 646f 7722 2069 643d 2263 6174  dWindow" id="cat
+00007770: 5f62 6f78 223e 0a20 2020 2020 2020 2020  _box">.         
+00007780: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+00007790: 206e 616d 653d 2276 6973 6962 6c65 223e   name="visible">
+000077a0: 5472 7565 3c2f 7072 6f70 6572 7479 3e0a  True</property>.
+000077b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077c0: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+000077d0: 6361 6e5f 666f 6375 7322 3e54 7275 653c  can_focus">True<
+000077e0: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
+000077f0: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
+00007800: 6572 7479 206e 616d 653d 2262 6f72 6465  erty name="borde
+00007810: 725f 7769 6474 6822 3e35 3c2f 7072 6f70  r_width">5</prop
+00007820: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
+00007830: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+00007840: 6e61 6d65 3d22 6873 6372 6f6c 6c62 6172  name="hscrollbar
+00007850: 5f70 6f6c 6963 7922 3e61 7574 6f6d 6174  _policy">automat
+00007860: 6963 3c2f 7072 6f70 6572 7479 3e0a 2020  ic</property>.  
+00007870: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
+00007880: 726f 7065 7274 7920 6e61 6d65 3d22 7673  roperty name="vs
+00007890: 6372 6f6c 6c62 6172 5f70 6f6c 6963 7922  crollbar_policy"
+000078a0: 3e61 7574 6f6d 6174 6963 3c2f 7072 6f70  >automatic</prop
+000078b0: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
+000078c0: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+000078d0: 6e61 6d65 3d22 7368 6164 6f77 5f74 7970  name="shadow_typ
+000078e0: 6522 3e69 6e3c 2f70 726f 7065 7274 793e  e">in</property>
+000078f0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00007900: 2f6f 626a 6563 743e 0a20 2020 2020 2020  /object>.       
+00007910: 2020 2020 203c 2f63 6869 6c64 3e0a 2020       </child>.  
+00007920: 2020 2020 2020 2020 2020 3c63 6869 6c64            <child
+00007930: 2074 7970 653d 2274 6162 223e 0a20 2020   type="tab">.   
+00007940: 2020 2020 2020 2020 2020 203c 6f62 6a65             <obje
+00007950: 6374 2063 6c61 7373 3d22 4774 6b4c 6162  ct class="GtkLab
+00007960: 656c 2220 6964 3d22 6361 745f 626f 785f  el" id="cat_box_
+00007970: 7461 6222 3e0a 2020 2020 2020 2020 2020  tab">.          
+00007980: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+00007990: 6e61 6d65 3d22 6c61 6265 6c22 3e43 6174  name="label">Cat
+000079a0: 6567 6f72 6965 733c 2f70 726f 7065 7274  egories</propert
+000079b0: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
+000079c0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+000079d0: 653d 2277 6964 7468 5f63 6861 7273 223e  e="width_chars">
+000079e0: 3136 3c2f 7072 6f70 6572 7479 3e0a 2020  16</property>.  
+000079f0: 2020 2020 2020 2020 2020 2020 3c2f 6f62              </ob
+00007a00: 6a65 6374 3e0a 2020 2020 2020 2020 2020  ject>.          
+00007a10: 2020 3c2f 6368 696c 643e 0a0a 2020 2020    </child>..    
+00007a20: 2020 2020 2020 2020 3c21 2d2d 206c 6f67          <!-- log
+00007a30: 2070 6167 6520 2d2d 3e0a 2020 2020 2020   page -->.      
+00007a40: 2020 2020 2020 3c63 6869 6c64 3e0a 2020        <child>.  
+00007a50: 2020 2020 2020 2020 2020 2020 3c6f 626a              <obj
+00007a60: 6563 7420 636c 6173 733d 2247 746b 5363  ect class="GtkSc
+00007a70: 726f 6c6c 6564 5769 6e64 6f77 2220 6964  rolledWindow" id
+00007a80: 3d22 6c6f 675f 626f 7822 3e0a 2020 2020  ="log_box">.    
+00007a90: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
+00007aa0: 7065 7274 7920 6e61 6d65 3d22 7669 7369  perty name="visi
+00007ab0: 626c 6522 3e54 7275 653c 2f70 726f 7065  ble">True</prope
+00007ac0: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
+00007ad0: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+00007ae0: 616d 653d 2263 616e 5f66 6f63 7573 223e  ame="can_focus">
+00007af0: 5472 7565 3c2f 7072 6f70 6572 7479 3e0a  True</property>.
+00007b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b10: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+00007b20: 626f 7264 6572 5f77 6964 7468 223e 353c  border_width">5<
+00007b30: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
+00007b40: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
+00007b50: 6572 7479 206e 616d 653d 2268 7363 726f  erty name="hscro
+00007b60: 6c6c 6261 725f 706f 6c69 6379 223e 6175  llbar_policy">au
+00007b70: 746f 6d61 7469 633c 2f70 726f 7065 7274  tomatic</propert
+00007b80: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
+00007b90: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+00007ba0: 653d 2276 7363 726f 6c6c 6261 725f 706f  e="vscrollbar_po
+00007bb0: 6c69 6379 223e 6175 746f 6d61 7469 633c  licy">automatic<
+00007bc0: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
+00007bd0: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
+00007be0: 6572 7479 206e 616d 653d 2273 6861 646f  erty name="shado
+00007bf0: 775f 7479 7065 223e 696e 3c2f 7072 6f70  w_type">in</prop
+00007c00: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
+00007c10: 2020 2020 2020 3c63 6869 6c64 3e0a 2020        <child>.  
+00007c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c30: 3c6f 626a 6563 7420 636c 6173 733d 2247  <object class="G
+00007c40: 746b 5465 7874 5669 6577 2220 6964 3d22  tkTextView" id="
+00007c50: 6c6f 675f 7669 6577 223e 0a20 2020 2020  log_view">.     
+00007c60: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00007c70: 7072 6f70 6572 7479 206e 616d 653d 2276  property name="v
+00007c80: 6973 6962 6c65 223e 5472 7565 3c2f 7072  isible">True</pr
+00007c90: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
+00007ca0: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
+00007cb0: 7065 7274 7920 6e61 6d65 3d22 6361 6e5f  perty name="can_
+00007cc0: 666f 6375 7322 3e54 7275 653c 2f70 726f  focus">True</pro
+00007cd0: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
+00007ce0: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
+00007cf0: 6572 7479 206e 616d 653d 2265 6469 7461  erty name="edita
+00007d00: 626c 6522 3e46 616c 7365 3c2f 7072 6f70  ble">False</prop
+00007d10: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
+00007d20: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
+00007d30: 7274 7920 6e61 6d65 3d22 6c65 6674 5f6d  rty name="left_m
+00007d40: 6172 6769 6e22 3e32 3c2f 7072 6f70 6572  argin">2</proper
+00007d50: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
+00007d60: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
+00007d70: 7920 6e61 6d65 3d22 7269 6768 745f 6d61  y name="right_ma
+00007d80: 7267 696e 223e 323c 2f70 726f 7065 7274  rgin">2</propert
+00007d90: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
+00007da0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+00007db0: 206e 616d 653d 2263 7572 736f 725f 7669   name="cursor_vi
+00007dc0: 7369 626c 6522 3e46 616c 7365 3c2f 7072  sible">False</pr
+00007dd0: 6f70 6572 7479 3e0a 2020 2020 2020 2020  operty>.        
+00007de0: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
+00007df0: 7065 7274 7920 6e61 6d65 3d22 6275 6666  perty name="buff
+00007e00: 6572 223e 6c6f 675f 6275 6666 6572 3c2f  er">log_buffer</
+00007e10: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
+00007e20: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
+00007e30: 726f 7065 7274 7920 6e61 6d65 3d22 6163  roperty name="ac
+00007e40: 6365 7074 735f 7461 6222 3e46 616c 7365  cepts_tab">False
+00007e50: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+00007e60: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00007e70: 6f62 6a65 6374 3e0a 2020 2020 2020 2020  object>.        
+00007e80: 2020 2020 2020 2020 3c2f 6368 696c 643e          </child>
+00007e90: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00007ea0: 2f6f 626a 6563 743e 0a20 2020 2020 2020  /object>.       
+00007eb0: 2020 2020 203c 2f63 6869 6c64 3e0a 2020       </child>.  
+00007ec0: 2020 2020 2020 2020 2020 3c63 6869 6c64            <child
+00007ed0: 2074 7970 653d 2274 6162 223e 0a20 2020   type="tab">.   
+00007ee0: 2020 2020 2020 2020 2020 203c 6f62 6a65             <obje
+00007ef0: 6374 2063 6c61 7373 3d22 4774 6b4c 6162  ct class="GtkLab
+00007f00: 656c 2220 6964 3d22 6c6f 675f 626f 785f  el" id="log_box_
+00007f10: 7461 6222 3e0a 2020 2020 2020 2020 2020  tab">.          
+00007f20: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+00007f30: 6e61 6d65 3d22 6c61 6265 6c22 3e41 6374  name="label">Act
+00007f40: 6976 6974 7920 4c6f 673c 2f70 726f 7065  ivity Log</prope
+00007f50: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
+00007f60: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+00007f70: 616d 653d 2277 6964 7468 5f63 6861 7273  ame="width_chars
+00007f80: 223e 3136 3c2f 7072 6f70 6572 7479 3e0a  ">16</property>.
+00007f90: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00007fa0: 6f62 6a65 6374 3e0a 2020 2020 2020 2020  object>.        
+00007fb0: 2020 2020 3c2f 6368 696c 643e 0a20 2020      </child>.   
+00007fc0: 2020 2020 2020 203c 2f6f 626a 6563 743e         </object>
+00007fd0: 0a20 2020 2020 2020 2020 203c 7061 636b  .          <pack
+00007fe0: 696e 673e 0a20 2020 2020 2020 2020 2020  ing>.           
+00007ff0: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00008000: 2270 6163 6b2d 7479 7065 223e 7374 6172  "pack-type">star
+00008010: 743c 2f70 726f 7065 7274 793e 0a20 2020  t</property>.   
+00008020: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
+00008030: 7479 206e 616d 653d 2265 7870 616e 6422  ty name="expand"
+00008040: 3e54 7275 653c 2f70 726f 7065 7274 793e  >True</property>
+00008050: 0a20 2020 2020 2020 2020 2020 203c 7072  .            <pr
+00008060: 6f70 6572 7479 206e 616d 653d 2266 696c  operty name="fil
+00008070: 6c22 3e54 7275 653c 2f70 726f 7065 7274  l">True</propert
+00008080: 793e 0a20 2020 2020 2020 2020 203c 2f70  y>.          </p
+00008090: 6163 6b69 6e67 3e0a 2020 2020 2020 2020  acking>.        
+000080a0: 3c2f 6368 696c 643e 0a0a 2020 2020 2020  </child>..      
+000080b0: 2020 3c21 2d2d 206d 6565 7420 7374 6174    <!-- meet stat
+000080c0: 7573 2062 6172 202d 2d3e 0a20 2020 2020  us bar -->.     
+000080d0: 2020 203c 6368 696c 643e 0a20 2020 2020     <child>.     
+000080e0: 2020 2020 203c 6f62 6a65 6374 2063 6c61       <object cla
+000080f0: 7373 3d22 4774 6b53 7461 7475 7362 6172  ss="GtkStatusbar
+00008100: 2220 6964 3d22 7374 6174 7573 223e 0a20  " id="status">. 
+00008110: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
+00008120: 6572 7479 206e 616d 653d 2276 6973 6962  erty name="visib
+00008130: 6c65 223e 5472 7565 3c2f 7072 6f70 6572  le">True</proper
+00008140: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
+00008150: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
+00008160: 7370 6163 696e 6722 3e32 3c2f 7072 6f70  spacing">2</prop
+00008170: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
+00008180: 3c2f 6f62 6a65 6374 3e0a 2020 2020 2020  </object>.      
+00008190: 2020 2020 3c70 6163 6b69 6e67 3e0a 2020      <packing>.  
+000081a0: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
+000081b0: 7274 7920 6e61 6d65 3d22 6578 7061 6e64  rty name="expand
+000081c0: 223e 4661 6c73 653c 2f70 726f 7065 7274  ">False</propert
+000081d0: 793e 0a20 2020 2020 2020 2020 2020 203c  y>.            <
+000081e0: 7072 6f70 6572 7479 206e 616d 653d 2270  property name="p
+000081f0: 6163 6b2d 7479 7065 223e 7374 6172 743c  ack-type">start<
+00008200: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
+00008210: 2020 2020 203c 2f70 6163 6b69 6e67 3e0a       </packing>.
+00008220: 2020 2020 2020 2020 3c2f 6368 696c 643e          </child>
+00008230: 0a20 2020 2020 203c 2f6f 626a 6563 743e  .      </object>
+00008240: 0a20 2020 203c 2f63 6869 6c64 3e0a 2020  .    </child>.  
+00008250: 3c2f 6f62 6a65 6374 3e0a 0a20 203c 212d  </object>..  <!-
+00008260: 2d20 7465 7874 2062 7566 6665 7220 666f  - text buffer fo
+00008270: 7220 6c6f 6720 7769 6e64 6f77 202d 2d3e  r log window -->
+00008280: 0a20 203c 6f62 6a65 6374 2063 6c61 7373  .  <object class
+00008290: 3d22 4774 6b54 6578 7442 7566 6665 7222  ="GtkTextBuffer"
+000082a0: 2069 643d 226c 6f67 5f62 7566 6665 7222   id="log_buffer"
+000082b0: 2f3e 0a0a 2020 3c21 2d2d 206c 6973 7420  />..  <!-- list 
+000082c0: 6d6f 6465 6c20 666f 7220 6576 656e 7420  model for event 
+000082d0: 6163 7469 6f6e 7320 2d2d 3e0a 2020 3c6f  actions -->.  <o
+000082e0: 626a 6563 7420 636c 6173 733d 2247 746b  bject class="Gtk
+000082f0: 4c69 7374 5374 6f72 6522 2069 643d 2265  ListStore" id="e
+00008300: 7665 6e74 5f61 6374 696f 6e5f 6d6f 6465  vent_action_mode
+00008310: 6c22 3e0a 2020 2020 3c63 6f6c 756d 6e73  l">.    <columns
+00008320: 3e0a 2020 2020 2020 3c63 6f6c 756d 6e20  >.      <column 
+00008330: 7479 7065 3d22 6763 6861 7261 7272 6179  type="gchararray
+00008340: 222f 3e0a 2020 2020 2020 3c63 6f6c 756d  "/>.      <colum
+00008350: 6e20 7479 7065 3d22 6763 6861 7261 7272  n type="gchararr
+00008360: 6179 222f 3e0a 2020 2020 3c2f 636f 6c75  ay"/>.    </colu
+00008370: 6d6e 733e 0a20 2020 203c 6461 7461 3e0a  mns>.    <data>.
+00008380: 2020 2020 2020 3c72 6f77 3e0a 2020 2020        <row>.    
+00008390: 2020 2020 3c63 6f6c 2069 643d 2230 223e      <col id="0">
+000083a0: 613c 2f63 6f6c 3e0a 2020 2020 2020 2020  a</col>.        
+000083b0: 3c63 6f6c 2069 643d 2231 223e 613c 2f63  <col id="1">a</c
+000083c0: 6f6c 3e0a 2020 2020 2020 3c2f 726f 773e  ol>.      </row>
+000083d0: 0a20 2020 203c 2f64 6174 613e 0a20 203c  .    </data>.  <
+000083e0: 2f6f 626a 6563 743e 0a0a 2020 3c21 2d2d  /object>..  <!--
+000083f0: 2072 6964 6572 2063 6f6e 7465 7874 206d   rider context m
+00008400: 656e 7520 2d2d 3e0a 2020 3c6f 626a 6563  enu -->.  <objec
+00008410: 7420 636c 6173 733d 2247 746b 4d65 6e75  t class="GtkMenu
+00008420: 2220 6964 3d22 7269 6465 725f 636f 6e74  " id="rider_cont
+00008430: 6578 7422 3e0a 2020 2020 3c70 726f 7065  ext">.    <prope
+00008440: 7274 7920 6e61 6d65 3d22 7669 7369 626c  rty name="visibl
+00008450: 6522 3e54 7275 653c 2f70 726f 7065 7274  e">True</propert
+00008460: 793e 0a20 2020 203c 6368 696c 643e 0a20  y>.    <child>. 
+00008470: 2020 2020 203c 6f62 6a65 6374 2063 6c61       <object cla
+00008480: 7373 3d22 4774 6b4d 656e 7549 7465 6d22  ss="GtkMenuItem"
+00008490: 2069 643d 2272 6964 6572 5f65 6469 7422   id="rider_edit"
+000084a0: 3e0a 2020 2020 2020 2020 3c70 726f 7065  >.        <prope
+000084b0: 7274 7920 6e61 6d65 3d22 6c61 6265 6c22  rty name="label"
+000084c0: 3e45 6469 743c 2f70 726f 7065 7274 793e  >Edit</property>
+000084d0: 0a20 2020 2020 2020 203c 7072 6f70 6572  .        <proper
+000084e0: 7479 206e 616d 653d 2276 6973 6962 6c65  ty name="visible
+000084f0: 223e 5472 7565 3c2f 7072 6f70 6572 7479  ">True</property
+00008500: 3e0a 2020 2020 2020 2020 3c70 726f 7065  >.        <prope
+00008510: 7274 7920 6e61 6d65 3d22 7365 6e73 6974  rty name="sensit
+00008520: 6976 6522 3e46 616c 7365 3c2f 7072 6f70  ive">False</prop
+00008530: 6572 7479 3e0a 2020 2020 2020 2020 3c73  erty>.        <s
+00008540: 6967 6e61 6c20 6e61 6d65 3d22 6163 7469  ignal name="acti
+00008550: 7661 7465 2220 6861 6e64 6c65 723d 2272  vate" handler="r
+00008560: 6964 6572 5f65 6469 745f 6362 222f 3e0a  ider_edit_cb"/>.
+00008570: 2020 2020 2020 3c2f 6f62 6a65 6374 3e0a        </object>.
+00008580: 2020 2020 3c2f 6368 696c 643e 0a20 2020      </child>.   
+00008590: 203c 6368 696c 643e 0a20 2020 2020 203c   <child>.      <
+000085a0: 6f62 6a65 6374 2063 6c61 7373 3d22 4774  object class="Gt
+000085b0: 6b4d 656e 7549 7465 6d22 2069 643d 2272  kMenuItem" id="r
+000085c0: 6964 6572 5f6c 6f6f 6b75 7022 3e0a 2020  ider_lookup">.  
+000085d0: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+000085e0: 6e61 6d65 3d22 6c61 6265 6c22 3e4c 6f6f  name="label">Loo
+000085f0: 6b75 703c 2f70 726f 7065 7274 793e 0a20  kup</property>. 
+00008600: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
+00008610: 206e 616d 653d 2276 6973 6962 6c65 223e   name="visible">
+00008620: 5472 7565 3c2f 7072 6f70 6572 7479 3e0a  True</property>.
+00008630: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
+00008640: 7920 6e61 6d65 3d22 7365 6e73 6974 6976  y name="sensitiv
+00008650: 6522 3e46 616c 7365 3c2f 7072 6f70 6572  e">False</proper
+00008660: 7479 3e0a 2020 2020 2020 2020 3c73 6967  ty>.        <sig
+00008670: 6e61 6c20 6e61 6d65 3d22 6163 7469 7661  nal name="activa
+00008680: 7465 2220 6861 6e64 6c65 723d 2272 6964  te" handler="rid
+00008690: 6572 5f6c 6f6f 6b75 705f 6362 222f 3e0a  er_lookup_cb"/>.
+000086a0: 2020 2020 2020 3c2f 6f62 6a65 6374 3e0a        </object>.
+000086b0: 2020 2020 3c2f 6368 696c 643e 0a20 2020      </child>.   
+000086c0: 203c 6368 696c 643e 0a20 2020 2020 203c   <child>.      <
+000086d0: 6f62 6a65 6374 2063 6c61 7373 3d22 4774  object class="Gt
+000086e0: 6b4d 656e 7549 7465 6d22 2069 643d 2272  kMenuItem" id="r
+000086f0: 6964 6572 5f64 656c 223e 0a20 2020 2020  ider_del">.     
+00008700: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
+00008710: 653d 226c 6162 656c 223e 4465 6c65 7465  e="label">Delete
+00008720: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+00008730: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00008740: 6d65 3d22 7669 7369 626c 6522 3e54 7275  me="visible">Tru
+00008750: 653c 2f70 726f 7065 7274 793e 0a20 2020  e</property>.   
+00008760: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
+00008770: 616d 653d 2273 656e 7369 7469 7665 223e  ame="sensitive">
+00008780: 4661 6c73 653c 2f70 726f 7065 7274 793e  False</property>
+00008790: 0a20 2020 2020 2020 203c 7369 676e 616c  .        <signal
+000087a0: 206e 616d 653d 2261 6374 6976 6174 6522   name="activate"
+000087b0: 2068 616e 646c 6572 3d22 7269 6465 725f   handler="rider_
+000087c0: 6465 6c65 7465 5f63 6222 2f3e 0a20 2020  delete_cb"/>.   
+000087d0: 2020 203c 2f6f 626a 6563 743e 0a20 2020     </object>.   
+000087e0: 203c 2f63 6869 6c64 3e0a 2020 2020 3c63   </child>.    <c
+000087f0: 6869 6c64 3e0a 2020 2020 2020 3c6f 626a  hild>.      <obj
+00008800: 6563 7420 636c 6173 733d 2247 746b 5365  ect class="GtkSe
+00008810: 7061 7261 746f 724d 656e 7549 7465 6d22  paratorMenuItem"
+00008820: 2069 643d 2272 6964 6572 5f73 6570 3122   id="rider_sep1"
+00008830: 3e0a 2020 2020 2020 2020 3c70 726f 7065  >.        <prope
+00008840: 7274 7920 6e61 6d65 3d22 7669 7369 626c  rty name="visibl
+00008850: 6522 3e54 7275 653c 2f70 726f 7065 7274  e">True</propert
+00008860: 793e 0a20 2020 2020 203c 2f6f 626a 6563  y>.      </objec
+00008870: 743e 0a20 2020 203c 2f63 6869 6c64 3e0a  t>.    </child>.
+00008880: 2020 2020 3c63 6869 6c64 3e0a 2020 2020      <child>.    
+00008890: 2020 3c6f 626a 6563 7420 636c 6173 733d    <object class=
+000088a0: 2247 746b 4d65 6e75 4974 656d 2220 6964  "GtkMenuItem" id
+000088b0: 3d22 7269 6465 725f 6164 6422 3e0a 2020  ="rider_add">.  
+000088c0: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
+000088d0: 6e61 6d65 3d22 6c61 6265 6c22 3e41 6464  name="label">Add
+000088e0: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
+000088f0: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00008900: 6d65 3d22 7669 7369 626c 6522 3e54 7275  me="visible">Tru
+00008910: 653c 2f70 726f 7065 7274 793e 0a20 2020  e</property>.   
+00008920: 2020 2020 203c 7369 676e 616c 206e 616d       <signal nam
+00008930: 653d 2261 6374 6976 6174 6522 2068 616e  e="activate" han
+00008940: 646c 6572 3d22 7269 6465 725f 6164 645f  dler="rider_add_
+00008950: 6362 222f 3e0a 2020 2020 2020 3c2f 6f62  cb"/>.      </ob
+00008960: 6a65 6374 3e0a 2020 2020 3c2f 6368 696c  ject>.    </chil
+00008970: 643e 0a20 2020 203c 6368 696c 643e 0a20  d>.    <child>. 
+00008980: 2020 2020 203c 6f62 6a65 6374 2063 6c61       <object cla
+00008990: 7373 3d22 4774 6b4d 656e 7549 7465 6d22  ss="GtkMenuItem"
+000089a0: 2069 643d 2272 6964 6572 5f69 6d70 6f72   id="rider_impor
+000089b0: 7422 3e0a 2020 2020 2020 2020 3c70 726f  t">.        <pro
+000089c0: 7065 7274 7920 6e61 6d65 3d22 6c61 6265  perty name="labe
+000089d0: 6c22 3e49 6d70 6f72 7420 4353 563c 2f70  l">Import CSV</p
+000089e0: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
+000089f0: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00008a00: 2276 6973 6962 6c65 223e 5472 7565 3c2f  "visible">True</
+00008a10: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
+00008a20: 2020 3c73 6967 6e61 6c20 6e61 6d65 3d22    <signal name="
+00008a30: 6163 7469 7661 7465 2220 6861 6e64 6c65  activate" handle
+00008a40: 723d 226d 656e 755f 696d 706f 7274 5f72  r="menu_import_r
+00008a50: 6964 6572 735f 6163 7469 7661 7465 5f63  iders_activate_c
+00008a60: 6222 2f3e 0a20 2020 2020 203c 2f6f 626a  b"/>.      </obj
+00008a70: 6563 743e 0a20 2020 203c 2f63 6869 6c64  ect>.    </child
+00008a80: 3e0a 2020 2020 3c63 6869 6c64 3e0a 2020  >.    <child>.  
+00008a90: 2020 2020 3c6f 626a 6563 7420 636c 6173      <object clas
+00008aa0: 733d 2247 746b 4d65 6e75 4974 656d 2220  s="GtkMenuItem" 
+00008ab0: 6964 3d22 7269 6465 725f 6368 6970 6669  id="rider_chipfi
+00008ac0: 6c22 3e0a 2020 2020 2020 2020 3c70 726f  l">.        <pro
+00008ad0: 7065 7274 7920 6e61 6d65 3d22 6c61 6265  perty name="labe
+00008ae0: 6c22 3e4c 6f61 6420 4368 6970 6669 6c65  l">Load Chipfile
 00008af0: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-00008b00: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
-00008b10: 7065 7274 7920 6e61 6d65 3d22 626f 7264  perty name="bord
-00008b20: 6572 5f77 6964 7468 223e 353c 2f70 726f  er_width">5</pro
-00008b30: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
-00008b40: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00008b50: 206e 616d 653d 2268 7363 726f 6c6c 6261   name="hscrollba
-00008b60: 725f 706f 6c69 6379 223e 6175 746f 6d61  r_policy">automa
-00008b70: 7469 633c 2f70 726f 7065 7274 793e 0a20  tic</property>. 
-00008b80: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00008b90: 7072 6f70 6572 7479 206e 616d 653d 2276  property name="v
-00008ba0: 7363 726f 6c6c 6261 725f 706f 6c69 6379  scrollbar_policy
-00008bb0: 223e 6175 746f 6d61 7469 633c 2f70 726f  ">automatic</pro
-00008bc0: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
-00008bd0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00008be0: 206e 616d 653d 2273 6861 646f 775f 7479   name="shadow_ty
-00008bf0: 7065 223e 696e 3c2f 7072 6f70 6572 7479  pe">in</property
-00008c00: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00008c10: 2020 3c63 6869 6c64 3e0a 2020 2020 2020    <child>.      
-00008c20: 2020 2020 2020 2020 2020 2020 3c70 6c61              <pla
-00008c30: 6365 686f 6c64 6572 2f3e 0a20 2020 2020  ceholder/>.     
-00008c40: 2020 2020 2020 2020 2020 203c 2f63 6869             </chi
-00008c50: 6c64 3e0a 2020 2020 2020 2020 2020 2020  ld>.            
-00008c60: 2020 3c2f 6f62 6a65 6374 3e0a 2020 2020    </object>.    
-00008c70: 2020 2020 2020 2020 2020 3c70 6163 6b69            <packi
-00008c80: 6e67 3e0a 2020 2020 2020 2020 2020 2020  ng>.            
-00008c90: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00008ca0: 6d65 3d22 706f 7369 7469 6f6e 223e 313c  me="position">1<
-00008cb0: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
-00008cc0: 2020 2020 2020 2020 203c 2f70 6163 6b69           </packi
-00008cd0: 6e67 3e0a 2020 2020 2020 2020 2020 2020  ng>.            
-00008ce0: 3c2f 6368 696c 643e 0a20 2020 2020 2020  </child>.       
-00008cf0: 2020 2020 203c 6368 696c 6420 7479 7065       <child type
-00008d00: 3d22 7461 6222 3e0a 2020 2020 2020 2020  ="tab">.        
-00008d10: 2020 2020 2020 3c6f 626a 6563 7420 636c        <object cl
-00008d20: 6173 733d 2247 746b 4c61 6265 6c22 2069  ass="GtkLabel" i
-00008d30: 643d 2272 6964 6572 735f 626f 785f 7461  d="riders_box_ta
-00008d40: 6222 3e0a 2020 2020 2020 2020 2020 2020  b">.            
-00008d50: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00008d60: 6d65 3d22 6c61 6265 6c22 3e52 6964 6572  me="label">Rider
-00008d70: 2044 6174 613c 2f70 726f 7065 7274 793e   Data</property>
-00008d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008d90: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-00008da0: 2277 6964 7468 5f63 6861 7273 223e 3136  "width_chars">16
-00008db0: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-00008dc0: 2020 2020 2020 2020 2020 3c2f 6f62 6a65            </obje
-00008dd0: 6374 3e0a 2020 2020 2020 2020 2020 2020  ct>.            
-00008de0: 3c2f 6368 696c 643e 0a20 2020 2020 2020  </child>.       
-00008df0: 2020 2020 203c 6368 696c 643e 0a20 2020       <child>.   
-00008e00: 2020 2020 2020 2020 2020 203c 6f62 6a65             <obje
-00008e10: 6374 2063 6c61 7373 3d22 4774 6b53 6372  ct class="GtkScr
-00008e20: 6f6c 6c65 6457 696e 646f 7722 2069 643d  olledWindow" id=
-00008e30: 2263 6174 5f62 6f78 223e 0a20 2020 2020  "cat_box">.     
-00008e40: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
-00008e50: 6572 7479 206e 616d 653d 2276 6973 6962  erty name="visib
-00008e60: 6c65 223e 5472 7565 3c2f 7072 6f70 6572  le">True</proper
-00008e70: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
-00008e80: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00008e90: 6d65 3d22 6361 6e5f 666f 6375 7322 3e54  me="can_focus">T
-00008ea0: 7275 653c 2f70 726f 7065 7274 793e 0a20  rue</property>. 
-00008eb0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00008ec0: 7072 6f70 6572 7479 206e 616d 653d 2262  property name="b
-00008ed0: 6f72 6465 725f 7769 6474 6822 3e35 3c2f  order_width">5</
-00008ee0: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
-00008ef0: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00008f00: 7274 7920 6e61 6d65 3d22 6873 6372 6f6c  rty name="hscrol
-00008f10: 6c62 6172 5f70 6f6c 6963 7922 3e61 7574  lbar_policy">aut
-00008f20: 6f6d 6174 6963 3c2f 7072 6f70 6572 7479  omatic</property
-00008f30: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00008f40: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00008f50: 3d22 7673 6372 6f6c 6c62 6172 5f70 6f6c  ="vscrollbar_pol
-00008f60: 6963 7922 3e61 7574 6f6d 6174 6963 3c2f  icy">automatic</
-00008f70: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
-00008f80: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00008f90: 7274 7920 6e61 6d65 3d22 7368 6164 6f77  rty name="shadow
-00008fa0: 5f74 7970 6522 3e69 6e3c 2f70 726f 7065  _type">in</prope
-00008fb0: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
-00008fc0: 2020 2020 203c 6368 696c 643e 0a20 2020       <child>.   
-00008fd0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00008fe0: 706c 6163 6568 6f6c 6465 722f 3e0a 2020  placeholder/>.  
-00008ff0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00009000: 6368 696c 643e 0a20 2020 2020 2020 2020  child>.         
-00009010: 2020 2020 203c 2f6f 626a 6563 743e 0a20       </object>. 
-00009020: 2020 2020 2020 2020 2020 2020 203c 7061               <pa
-00009030: 636b 696e 673e 0a20 2020 2020 2020 2020  cking>.         
-00009040: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-00009050: 206e 616d 653d 2270 6f73 6974 696f 6e22   name="position"
-00009060: 3e32 3c2f 7072 6f70 6572 7479 3e0a 2020  >2</property>.  
-00009070: 2020 2020 2020 2020 2020 2020 3c2f 7061              </pa
-00009080: 636b 696e 673e 0a20 2020 2020 2020 2020  cking>.         
-00009090: 2020 203c 2f63 6869 6c64 3e0a 2020 2020     </child>.    
-000090a0: 2020 2020 2020 2020 3c63 6869 6c64 2074          <child t
-000090b0: 7970 653d 2274 6162 223e 0a20 2020 2020  ype="tab">.     
-000090c0: 2020 2020 2020 2020 203c 6f62 6a65 6374           <object
-000090d0: 2063 6c61 7373 3d22 4774 6b4c 6162 656c   class="GtkLabel
-000090e0: 2220 6964 3d22 6361 745f 626f 785f 7461  " id="cat_box_ta
-000090f0: 6222 3e0a 2020 2020 2020 2020 2020 2020  b">.            
-00009100: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00009110: 6d65 3d22 6c61 6265 6c22 3e43 6174 6567  me="label">Categ
-00009120: 6f72 6965 733c 2f70 726f 7065 7274 793e  ories</property>
-00009130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009140: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-00009150: 2277 6964 7468 5f63 6861 7273 223e 3136  "width_chars">16
-00009160: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-00009170: 2020 2020 2020 2020 2020 3c2f 6f62 6a65            </obje
-00009180: 6374 3e0a 2020 2020 2020 2020 2020 2020  ct>.            
-00009190: 3c2f 6368 696c 643e 0a20 2020 2020 2020  </child>.       
-000091a0: 2020 2020 203c 6368 696c 643e 0a20 2020       <child>.   
-000091b0: 2020 2020 2020 2020 2020 203c 6f62 6a65             <obje
-000091c0: 6374 2063 6c61 7373 3d22 4774 6b53 6372  ct class="GtkScr
-000091d0: 6f6c 6c65 6457 696e 646f 7722 2069 643d  olledWindow" id=
-000091e0: 226c 6f67 5f62 6f78 223e 0a20 2020 2020  "log_box">.     
-000091f0: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
-00009200: 6572 7479 206e 616d 653d 2276 6973 6962  erty name="visib
-00009210: 6c65 223e 5472 7565 3c2f 7072 6f70 6572  le">True</proper
-00009220: 7479 3e0a 2020 2020 2020 2020 2020 2020  ty>.            
-00009230: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00009240: 6d65 3d22 6361 6e5f 666f 6375 7322 3e54  me="can_focus">T
-00009250: 7275 653c 2f70 726f 7065 7274 793e 0a20  rue</property>. 
-00009260: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00009270: 7072 6f70 6572 7479 206e 616d 653d 2262  property name="b
-00009280: 6f72 6465 725f 7769 6474 6822 3e35 3c2f  order_width">5</
-00009290: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
-000092a0: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-000092b0: 7274 7920 6e61 6d65 3d22 6873 6372 6f6c  rty name="hscrol
-000092c0: 6c62 6172 5f70 6f6c 6963 7922 3e61 7574  lbar_policy">aut
-000092d0: 6f6d 6174 6963 3c2f 7072 6f70 6572 7479  omatic</property
-000092e0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000092f0: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00009300: 3d22 7673 6372 6f6c 6c62 6172 5f70 6f6c  ="vscrollbar_pol
-00009310: 6963 7922 3e61 7574 6f6d 6174 6963 3c2f  icy">automatic</
-00009320: 7072 6f70 6572 7479 3e0a 2020 2020 2020  property>.      
-00009330: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00009340: 7274 7920 6e61 6d65 3d22 7368 6164 6f77  rty name="shadow
-00009350: 5f74 7970 6522 3e69 6e3c 2f70 726f 7065  _type">in</prope
-00009360: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
-00009370: 2020 2020 203c 6368 696c 643e 0a20 2020       <child>.   
-00009380: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00009390: 6f62 6a65 6374 2063 6c61 7373 3d22 4774  object class="Gt
-000093a0: 6b54 6578 7456 6965 7722 2069 643d 226c  kTextView" id="l
-000093b0: 6f67 5f76 6965 7722 3e0a 2020 2020 2020  og_view">.      
-000093c0: 2020 2020 2020 2020 2020 2020 2020 3c70                <p
-000093d0: 726f 7065 7274 7920 6e61 6d65 3d22 7669  roperty name="vi
-000093e0: 7369 626c 6522 3e54 7275 653c 2f70 726f  sible">True</pro
-000093f0: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
-00009400: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
-00009410: 6572 7479 206e 616d 653d 2263 616e 5f66  erty name="can_f
-00009420: 6f63 7573 223e 5472 7565 3c2f 7072 6f70  ocus">True</prop
-00009430: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
-00009440: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00009450: 7274 7920 6e61 6d65 3d22 6564 6974 6162  rty name="editab
-00009460: 6c65 223e 4661 6c73 653c 2f70 726f 7065  le">False</prope
-00009470: 7274 793e 0a20 2020 2020 2020 2020 2020  rty>.           
-00009480: 2020 2020 2020 2020 203c 7072 6f70 6572           <proper
-00009490: 7479 206e 616d 653d 226c 6566 745f 6d61  ty name="left_ma
-000094a0: 7267 696e 223e 323c 2f70 726f 7065 7274  rgin">2</propert
-000094b0: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
-000094c0: 2020 2020 2020 203c 7072 6f70 6572 7479         <property
-000094d0: 206e 616d 653d 2272 6967 6874 5f6d 6172   name="right_mar
-000094e0: 6769 6e22 3e32 3c2f 7072 6f70 6572 7479  gin">2</property
-000094f0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00009500: 2020 2020 2020 3c70 726f 7065 7274 7920        <property 
-00009510: 6e61 6d65 3d22 6375 7273 6f72 5f76 6973  name="cursor_vis
-00009520: 6962 6c65 223e 4661 6c73 653c 2f70 726f  ible">False</pro
-00009530: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
-00009540: 2020 2020 2020 2020 2020 203c 7072 6f70             <prop
-00009550: 6572 7479 206e 616d 653d 2262 7566 6665  erty name="buffe
-00009560: 7222 3e6c 6f67 5f62 7566 6665 723c 2f70  r">log_buffer</p
-00009570: 726f 7065 7274 793e 0a20 2020 2020 2020  roperty>.       
-00009580: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
-00009590: 6f70 6572 7479 206e 616d 653d 2261 6363  operty name="acc
-000095a0: 6570 7473 5f74 6162 223e 4661 6c73 653c  epts_tab">False<
-000095b0: 2f70 726f 7065 7274 793e 0a20 2020 2020  /property>.     
-000095c0: 2020 2020 2020 2020 2020 2020 203c 2f6f               </o
-000095d0: 626a 6563 743e 0a20 2020 2020 2020 2020  bject>.         
-000095e0: 2020 2020 2020 203c 2f63 6869 6c64 3e0a         </child>.
-000095f0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00009600: 6f62 6a65 6374 3e0a 2020 2020 2020 2020  object>.        
-00009610: 2020 2020 2020 3c70 6163 6b69 6e67 3e0a        <packing>.
-00009620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009630: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-00009640: 706f 7369 7469 6f6e 223e 333c 2f70 726f  position">3</pro
-00009650: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
-00009660: 2020 2020 203c 2f70 6163 6b69 6e67 3e0a       </packing>.
-00009670: 2020 2020 2020 2020 2020 2020 3c2f 6368              </ch
-00009680: 696c 643e 0a20 2020 2020 2020 2020 2020  ild>.           
-00009690: 203c 6368 696c 6420 7479 7065 3d22 7461   <child type="ta
-000096a0: 6222 3e0a 2020 2020 2020 2020 2020 2020  b">.            
-000096b0: 2020 3c6f 626a 6563 7420 636c 6173 733d    <object class=
-000096c0: 2247 746b 4c61 6265 6c22 2069 643d 226c  "GtkLabel" id="l
-000096d0: 6f67 5f62 6f78 5f74 6162 223e 0a20 2020  og_box_tab">.   
-000096e0: 2020 2020 2020 2020 2020 2020 203c 7072               <pr
-000096f0: 6f70 6572 7479 206e 616d 653d 226c 6162  operty name="lab
-00009700: 656c 223e 4163 7469 7669 7479 204c 6f67  el">Activity Log
-00009710: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-00009720: 2020 2020 2020 2020 2020 2020 3c70 726f              <pro
-00009730: 7065 7274 7920 6e61 6d65 3d22 7769 6474  perty name="widt
-00009740: 685f 6368 6172 7322 3e31 363c 2f70 726f  h_chars">16</pro
-00009750: 7065 7274 793e 0a20 2020 2020 2020 2020  perty>.         
-00009760: 2020 2020 203c 2f6f 626a 6563 743e 0a20       </object>. 
-00009770: 2020 2020 2020 2020 2020 203c 2f63 6869             </chi
-00009780: 6c64 3e0a 2020 2020 2020 2020 2020 3c2f  ld>.          </
-00009790: 6f62 6a65 6374 3e0a 2020 2020 2020 2020  object>.        
-000097a0: 2020 3c70 6163 6b69 6e67 3e0a 2020 2020    <packing>.    
-000097b0: 2020 2020 2020 2020 3c70 726f 7065 7274          <propert
-000097c0: 7920 6e61 6d65 3d22 706f 7369 7469 6f6e  y name="position
-000097d0: 223e 323c 2f70 726f 7065 7274 793e 0a20  ">2</property>. 
-000097e0: 2020 2020 2020 2020 203c 2f70 6163 6b69           </packi
-000097f0: 6e67 3e0a 2020 2020 2020 2020 3c2f 6368  ng>.        </ch
-00009800: 696c 643e 0a20 2020 2020 2020 203c 6368  ild>.        <ch
-00009810: 696c 643e 0a20 2020 2020 2020 2020 203c  ild>.          <
-00009820: 6f62 6a65 6374 2063 6c61 7373 3d22 4774  object class="Gt
-00009830: 6b53 7461 7475 7362 6172 2220 6964 3d22  kStatusbar" id="
-00009840: 7374 6174 7573 223e 0a20 2020 2020 2020  status">.       
-00009850: 2020 2020 203c 7072 6f70 6572 7479 206e       <property n
-00009860: 616d 653d 2276 6973 6962 6c65 223e 5472  ame="visible">Tr
-00009870: 7565 3c2f 7072 6f70 6572 7479 3e0a 2020  ue</property>.  
-00009880: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00009890: 7274 7920 6e61 6d65 3d22 7370 6163 696e  rty name="spacin
-000098a0: 6722 3e32 3c2f 7072 6f70 6572 7479 3e0a  g">2</property>.
-000098b0: 2020 2020 2020 2020 2020 2020 3c63 6869              <chi
-000098c0: 6c64 3e0a 2020 2020 2020 2020 2020 2020  ld>.            
-000098d0: 2020 3c70 6c61 6365 686f 6c64 6572 2f3e    <placeholder/>
-000098e0: 0a20 2020 2020 2020 2020 2020 203c 2f63  .            </c
-000098f0: 6869 6c64 3e0a 2020 2020 2020 2020 2020  hild>.          
-00009900: 3c2f 6f62 6a65 6374 3e0a 2020 2020 2020  </object>.      
-00009910: 2020 2020 3c70 6163 6b69 6e67 3e0a 2020      <packing>.  
-00009920: 2020 2020 2020 2020 2020 3c70 726f 7065            <prope
-00009930: 7274 7920 6e61 6d65 3d22 6578 7061 6e64  rty name="expand
-00009940: 223e 4661 6c73 653c 2f70 726f 7065 7274  ">False</propert
-00009950: 793e 0a20 2020 2020 2020 2020 2020 203c  y>.            <
-00009960: 7072 6f70 6572 7479 206e 616d 653d 2270  property name="p
-00009970: 6f73 6974 696f 6e22 3e33 3c2f 7072 6f70  osition">3</prop
-00009980: 6572 7479 3e0a 2020 2020 2020 2020 2020  erty>.          
-00009990: 3c2f 7061 636b 696e 673e 0a20 2020 2020  </packing>.     
-000099a0: 2020 203c 2f63 6869 6c64 3e0a 2020 2020     </child>.    
-000099b0: 2020 3c2f 6f62 6a65 6374 3e0a 2020 2020    </object>.    
-000099c0: 3c2f 6368 696c 643e 0a20 203c 2f6f 626a  </child>.  </obj
-000099d0: 6563 743e 0a20 203c 6f62 6a65 6374 2063  ect>.  <object c
-000099e0: 6c61 7373 3d22 4774 6b49 6d61 6765 2220  lass="GtkImage" 
-000099f0: 6964 3d22 696d 6167 6531 223e 0a20 2020  id="image1">.   
-00009a00: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-00009a10: 2276 6973 6962 6c65 223e 5472 7565 3c2f  "visible">True</
-00009a20: 7072 6f70 6572 7479 3e0a 2020 2020 3c70  property>.    <p
-00009a30: 726f 7065 7274 7920 6e61 6d65 3d22 7374  roperty name="st
-00009a40: 6f63 6b22 3e67 746b 2d72 6576 6572 742d  ock">gtk-revert-
-00009a50: 746f 2d73 6176 6564 3c2f 7072 6f70 6572  to-saved</proper
-00009a60: 7479 3e0a 2020 3c2f 6f62 6a65 6374 3e0a  ty>.  </object>.
-00009a70: 2020 3c6f 626a 6563 7420 636c 6173 733d    <object class=
-00009a80: 2247 746b 496d 6167 6522 2069 643d 2269  "GtkImage" id="i
-00009a90: 6d61 6765 3222 3e0a 2020 2020 3c70 726f  mage2">.    <pro
-00009aa0: 7065 7274 7920 6e61 6d65 3d22 7669 7369  perty name="visi
-00009ab0: 626c 6522 3e54 7275 653c 2f70 726f 7065  ble">True</prope
-00009ac0: 7274 793e 0a20 2020 203c 7072 6f70 6572  rty>.    <proper
-00009ad0: 7479 206e 616d 653d 2273 746f 636b 223e  ty name="stock">
-00009ae0: 6774 6b2d 676f 2d66 6f72 7761 7264 3c2f  gtk-go-forward</
-00009af0: 7072 6f70 6572 7479 3e0a 2020 3c2f 6f62  property>.  </ob
-00009b00: 6a65 6374 3e0a 2020 3c6f 626a 6563 7420  ject>.  <object 
-00009b10: 636c 6173 733d 2247 746b 496d 6167 6522  class="GtkImage"
-00009b20: 2069 643d 2269 6d61 6765 3322 3e0a 2020   id="image3">.  
-00009b30: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00009b40: 3d22 7669 7369 626c 6522 3e54 7275 653c  ="visible">True<
-00009b50: 2f70 726f 7065 7274 793e 0a20 2020 203c  /property>.    <
-00009b60: 7072 6f70 6572 7479 206e 616d 653d 2273  property name="s
-00009b70: 746f 636b 223e 6774 6b2d 676f 2d62 6163  tock">gtk-go-bac
-00009b80: 6b3c 2f70 726f 7065 7274 793e 0a20 203c  k</property>.  <
-00009b90: 2f6f 626a 6563 743e 0a20 203c 6f62 6a65  /object>.  <obje
-00009ba0: 6374 2063 6c61 7373 3d22 4774 6b49 6d61  ct class="GtkIma
-00009bb0: 6765 2220 6964 3d22 696d 6167 6534 223e  ge" id="image4">
-00009bc0: 0a20 2020 203c 7072 6f70 6572 7479 206e  .    <property n
-00009bd0: 616d 653d 2276 6973 6962 6c65 223e 5472  ame="visible">Tr
-00009be0: 7565 3c2f 7072 6f70 6572 7479 3e0a 2020  ue</property>.  
-00009bf0: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
-00009c00: 3d22 7374 6f63 6b22 3e67 746b 2d6e 6574  ="stock">gtk-net
-00009c10: 776f 726b 3c2f 7072 6f70 6572 7479 3e0a  work</property>.
-00009c20: 2020 3c2f 6f62 6a65 6374 3e0a 2020 3c6f    </object>.  <o
-00009c30: 626a 6563 7420 636c 6173 733d 2247 746b  bject class="Gtk
-00009c40: 5465 7874 4275 6666 6572 2220 6964 3d22  TextBuffer" id="
-00009c50: 6c6f 675f 6275 6666 6572 222f 3e0a 2020  log_buffer"/>.  
-00009c60: 3c6f 626a 6563 7420 636c 6173 733d 2247  <object class="G
-00009c70: 746b 496d 6167 6522 2069 643d 2269 6d61  tkImage" id="ima
-00009c80: 6765 3522 3e0a 2020 2020 3c70 726f 7065  ge5">.    <prope
-00009c90: 7274 7920 6e61 6d65 3d22 7669 7369 626c  rty name="visibl
-00009ca0: 6522 3e54 7275 653c 2f70 726f 7065 7274  e">True</propert
-00009cb0: 793e 0a20 2020 203c 7072 6f70 6572 7479  y>.    <property
-00009cc0: 206e 616d 653d 2273 746f 636b 223e 6774   name="stock">gt
-00009cd0: 6b2d 6d65 6469 612d 706c 6179 3c2f 7072  k-media-play</pr
-00009ce0: 6f70 6572 7479 3e0a 2020 3c2f 6f62 6a65  operty>.  </obje
-00009cf0: 6374 3e0a 2020 3c6f 626a 6563 7420 636c  ct>.  <object cl
-00009d00: 6173 733d 2247 746b 496d 6167 6522 2069  ass="GtkImage" i
-00009d10: 643d 2269 6d61 6765 3135 223e 0a20 2020  d="image15">.   
-00009d20: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-00009d30: 2276 6973 6962 6c65 223e 5472 7565 3c2f  "visible">True</
-00009d40: 7072 6f70 6572 7479 3e0a 2020 2020 3c70  property>.    <p
-00009d50: 726f 7065 7274 7920 6e61 6d65 3d22 7374  roperty name="st
-00009d60: 6f63 6b22 3e67 746b 2d67 6f2d 6261 636b  ock">gtk-go-back
-00009d70: 3c2f 7072 6f70 6572 7479 3e0a 2020 3c2f  </property>.  </
-00009d80: 6f62 6a65 6374 3e0a 2020 3c6f 626a 6563  object>.  <objec
-00009d90: 7420 636c 6173 733d 2247 746b 496d 6167  t class="GtkImag
-00009da0: 6522 2069 643d 2269 6d61 6765 3622 3e0a  e" id="image6">.
-00009db0: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00009dc0: 6d65 3d22 7669 7369 626c 6522 3e54 7275  me="visible">Tru
-00009dd0: 653c 2f70 726f 7065 7274 793e 0a20 2020  e</property>.   
-00009de0: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
-00009df0: 2273 746f 636b 223e 6774 6b2d 636c 6f73  "stock">gtk-clos
-00009e00: 653c 2f70 726f 7065 7274 793e 0a20 203c  e</property>.  <
-00009e10: 2f6f 626a 6563 743e 0a20 203c 6f62 6a65  /object>.  <obje
-00009e20: 6374 2063 6c61 7373 3d22 4774 6b49 6d61  ct class="GtkIma
-00009e30: 6765 2220 6964 3d22 696d 6167 6531 3822  ge" id="image18"
-00009e40: 3e0a 2020 2020 3c70 726f 7065 7274 7920  >.    <property 
-00009e50: 6e61 6d65 3d22 7669 7369 626c 6522 3e54  name="visible">T
-00009e60: 7275 653c 2f70 726f 7065 7274 793e 0a20  rue</property>. 
-00009e70: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00009e80: 653d 2273 746f 636b 223e 6774 6b2d 6564  e="stock">gtk-ed
-00009e90: 6974 3c2f 7072 6f70 6572 7479 3e0a 2020  it</property>.  
-00009ea0: 3c2f 6f62 6a65 6374 3e0a 2020 3c6f 626a  </object>.  <obj
-00009eb0: 6563 7420 636c 6173 733d 2247 746b 496d  ect class="GtkIm
-00009ec0: 6167 6522 2069 643d 2269 6d61 6765 3922  age" id="image9"
-00009ed0: 3e0a 2020 2020 3c70 726f 7065 7274 7920  >.    <property 
-00009ee0: 6e61 6d65 3d22 7669 7369 626c 6522 3e54  name="visible">T
-00009ef0: 7275 653c 2f70 726f 7065 7274 793e 0a20  rue</property>. 
-00009f00: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-00009f10: 653d 2273 746f 636b 223e 6774 6b2d 6865  e="stock">gtk-he
-00009f20: 6c70 3c2f 7072 6f70 6572 7479 3e0a 2020  lp</property>.  
-00009f30: 3c2f 6f62 6a65 6374 3e0a 2020 3c6f 626a  </object>.  <obj
-00009f40: 6563 7420 636c 6173 733d 2247 746b 496d  ect class="GtkIm
-00009f50: 6167 6522 2069 643d 2269 6d61 6765 3130  age" id="image10
-00009f60: 223e 0a20 2020 203c 7072 6f70 6572 7479  ">.    <property
-00009f70: 206e 616d 653d 2276 6973 6962 6c65 223e   name="visible">
-00009f80: 5472 7565 3c2f 7072 6f70 6572 7479 3e0a  True</property>.
-00009f90: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
-00009fa0: 6d65 3d22 7374 6f63 6b22 3e67 746b 2d6f  me="stock">gtk-o
-00009fb0: 7269 656e 7461 7469 6f6e 2d70 6f72 7472  rientation-portr
-00009fc0: 6169 743c 2f70 726f 7065 7274 793e 0a20  ait</property>. 
-00009fd0: 203c 2f6f 626a 6563 743e 0a20 203c 6f62   </object>.  <ob
-00009fe0: 6a65 6374 2063 6c61 7373 3d22 4774 6b49  ject class="GtkI
-00009ff0: 6d61 6765 2220 6964 3d22 696d 6167 6531  mage" id="image1
-0000a000: 3322 3e0a 2020 2020 3c70 726f 7065 7274  3">.    <propert
-0000a010: 7920 6e61 6d65 3d22 7669 7369 626c 6522  y name="visible"
-0000a020: 3e54 7275 653c 2f70 726f 7065 7274 793e  >True</property>
-0000a030: 0a20 2020 203c 7072 6f70 6572 7479 206e  .    <property n
-0000a040: 616d 653d 2273 746f 636b 223e 6774 6b2d  ame="stock">gtk-
-0000a050: 6564 6974 3c2f 7072 6f70 6572 7479 3e0a  edit</property>.
-0000a060: 2020 3c2f 6f62 6a65 6374 3e0a 2020 3c6f    </object>.  <o
-0000a070: 626a 6563 7420 636c 6173 733d 2247 746b  bject class="Gtk
-0000a080: 496d 6167 6522 2069 643d 2269 6d61 6765  Image" id="image
-0000a090: 3134 223e 0a20 2020 203c 7072 6f70 6572  14">.    <proper
-0000a0a0: 7479 206e 616d 653d 2276 6973 6962 6c65  ty name="visible
-0000a0b0: 223e 5472 7565 3c2f 7072 6f70 6572 7479  ">True</property
-0000a0c0: 3e0a 2020 2020 3c70 726f 7065 7274 7920  >.    <property 
-0000a0d0: 6e61 6d65 3d22 7374 6f63 6b22 3e67 746b  name="stock">gtk
-0000a0e0: 2d6e 6577 3c2f 7072 6f70 6572 7479 3e0a  -new</property>.
-0000a0f0: 2020 3c2f 6f62 6a65 6374 3e0a 2020 3c6f    </object>.  <o
-0000a100: 626a 6563 7420 636c 6173 733d 2247 746b  bject class="Gtk
-0000a110: 496d 6167 6522 2069 643d 2269 6d61 6765  Image" id="image
-0000a120: 3137 223e 0a20 2020 203c 7072 6f70 6572  17">.    <proper
-0000a130: 7479 206e 616d 653d 2276 6973 6962 6c65  ty name="visible
-0000a140: 223e 5472 7565 3c2f 7072 6f70 6572 7479  ">True</property
-0000a150: 3e0a 2020 2020 3c70 726f 7065 7274 7920  >.    <property 
-0000a160: 6e61 6d65 3d22 7374 6f63 6b22 3e67 746b  name="stock">gtk
-0000a170: 2d63 6f70 793c 2f70 726f 7065 7274 793e  -copy</property>
-0000a180: 0a20 203c 2f6f 626a 6563 743e 0a20 203c  .  </object>.  <
-0000a190: 6f62 6a65 6374 2063 6c61 7373 3d22 4774  object class="Gt
-0000a1a0: 6b49 6d61 6765 2220 6964 3d22 696d 6167  kImage" id="imag
-0000a1b0: 6531 3922 3e0a 2020 2020 3c70 726f 7065  e19">.    <prope
-0000a1c0: 7274 7920 6e61 6d65 3d22 7669 7369 626c  rty name="visibl
-0000a1d0: 6522 3e54 7275 653c 2f70 726f 7065 7274  e">True</propert
-0000a1e0: 793e 0a20 2020 203c 7072 6f70 6572 7479  y>.    <property
-0000a1f0: 206e 616d 653d 2273 746f 636b 223e 6774   name="stock">gt
-0000a200: 6b2d 7072 6566 6572 656e 6365 733c 2f70  k-preferences</p
-0000a210: 726f 7065 7274 793e 0a20 203c 2f6f 626a  roperty>.  </obj
-0000a220: 6563 743e 0a20 203c 6f62 6a65 6374 2063  ect>.  <object c
-0000a230: 6c61 7373 3d22 4774 6b4c 6973 7453 746f  lass="GtkListSto
-0000a240: 7265 2220 6964 3d22 7261 6365 5f61 6374  re" id="race_act
-0000a250: 696f 6e5f 6d6f 6465 6c22 3e0a 2020 2020  ion_model">.    
-0000a260: 3c63 6f6c 756d 6e73 3e0a 2020 2020 2020  <columns>.      
-0000a270: 3c21 2d2d 2063 6f6c 756d 6e2d 6e61 6d65  <!-- column-name
-0000a280: 2063 6f64 6520 2d2d 3e0a 2020 2020 2020   code -->.      
-0000a290: 3c63 6f6c 756d 6e20 7479 7065 3d22 6763  <column type="gc
-0000a2a0: 6861 7261 7272 6179 222f 3e0a 2020 2020  hararray"/>.    
-0000a2b0: 2020 3c21 2d2d 2063 6f6c 756d 6e2d 6e61    <!-- column-na
-0000a2c0: 6d65 2073 7472 202d 2d3e 0a20 2020 2020  me str -->.     
-0000a2d0: 203c 636f 6c75 6d6e 2074 7970 653d 2267   <column type="g
-0000a2e0: 6368 6172 6172 7261 7922 2f3e 0a20 2020  chararray"/>.   
-0000a2f0: 203c 2f63 6f6c 756d 6e73 3e0a 2020 2020   </columns>.    
-0000a300: 3c64 6174 613e 0a20 2020 2020 203c 726f  <data>.      <ro
-0000a310: 773e 0a20 2020 2020 2020 203c 636f 6c20  w>.        <col 
-0000a320: 6964 3d22 3022 2074 7261 6e73 6c61 7461  id="0" translata
-0000a330: 626c 653d 2279 6573 223e 636f 6d3c 2f63  ble="yes">com</c
-0000a340: 6f6c 3e0a 2020 2020 2020 2020 3c63 6f6c  ol>.        <col
-0000a350: 2069 643d 2231 2220 7472 616e 736c 6174   id="1" translat
-0000a360: 6162 6c65 3d22 7965 7322 3e41 6464 2063  able="yes">Add c
-0000a370: 6f6d 6d65 6e74 3c2f 636f 6c3e 0a20 2020  omment</col>.   
-0000a380: 2020 203c 2f72 6f77 3e0a 2020 2020 3c2f     </row>.    </
-0000a390: 6461 7461 3e0a 2020 3c2f 6f62 6a65 6374  data>.  </object
-0000a3a0: 3e0a 2020 3c6f 626a 6563 7420 636c 6173  >.  <object clas
-0000a3b0: 733d 2247 746b 496d 6167 6522 2069 643d  s="GtkImage" id=
-0000a3c0: 2269 6d61 6765 3234 223e 0a20 2020 203c  "image24">.    <
-0000a3d0: 7072 6f70 6572 7479 206e 616d 653d 2276  property name="v
-0000a3e0: 6973 6962 6c65 223e 5472 7565 3c2f 7072  isible">True</pr
-0000a3f0: 6f70 6572 7479 3e0a 2020 2020 3c70 726f  operty>.    <pro
-0000a400: 7065 7274 7920 6e61 6d65 3d22 7374 6f63  perty name="stoc
-0000a410: 6b22 3e67 746b 2d72 6566 7265 7368 3c2f  k">gtk-refresh</
-0000a420: 7072 6f70 6572 7479 3e0a 2020 3c2f 6f62  property>.  </ob
-0000a430: 6a65 6374 3e0a 2020 3c6f 626a 6563 7420  ject>.  <object 
-0000a440: 636c 6173 733d 2247 746b 496d 6167 6522  class="GtkImage"
-0000a450: 2069 643d 2269 6d61 6765 3232 223e 0a20   id="image22">. 
-0000a460: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-0000a470: 653d 2276 6973 6962 6c65 223e 5472 7565  e="visible">True
-0000a480: 3c2f 7072 6f70 6572 7479 3e0a 2020 2020  </property>.    
-0000a490: 3c70 726f 7065 7274 7920 6e61 6d65 3d22  <property name="
-0000a4a0: 7374 6f63 6b22 3e67 746b 2d65 6469 743c  stock">gtk-edit<
-0000a4b0: 2f70 726f 7065 7274 793e 0a20 203c 2f6f  /property>.  </o
-0000a4c0: 626a 6563 743e 0a3c 2f69 6e74 6572 6661  bject>.</interfa
-0000a4d0: 6365 3e0a                                ce>.
+00008b00: 2020 2020 3c70 726f 7065 7274 7920 6e61      <property na
+00008b10: 6d65 3d22 7669 7369 626c 6522 3e54 7275  me="visible">Tru
+00008b20: 653c 2f70 726f 7065 7274 793e 0a20 2020  e</property>.   
+00008b30: 2020 2020 203c 7369 676e 616c 206e 616d       <signal nam
+00008b40: 653d 2261 6374 6976 6174 6522 2068 616e  e="activate" han
+00008b50: 646c 6572 3d22 6d65 6e75 5f69 6d70 6f72  dler="menu_impor
+00008b60: 745f 6368 6970 6669 6c65 5f61 6374 6976  t_chipfile_activ
+00008b70: 6174 655f 6362 222f 3e0a 2020 2020 2020  ate_cb"/>.      
+00008b80: 3c2f 6f62 6a65 6374 3e0a 2020 2020 3c2f  </object>.    </
+00008b90: 6368 696c 643e 0a20 203c 2f6f 626a 6563  child>.  </objec
+00008ba0: 743e 0a3c 2f69 6e74 6572 6661 6365 3e0a  t>.</interface>.
```

### Comparing `metarace-roadmeet-1.13.2/src/roadmeet/ui/swap_rider.ui` & `metarace-roadmeet-1.13.3/src/roadmeet/ui/swap_rider.ui`

 * *Files identical despite different names*

### Comparing `metarace-roadmeet-1.13.2/src/roadmeet/uiutil.py` & `metarace-roadmeet-1.13.3/src/roadmeet/uiutil.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 # Font-overrides
 DIGITFONT = Pango.FontDescription('Noto Mono Medium 22')
 MONOFONT = Pango.FontDescription('Noto Mono')
 LOGVIEWFONT = Pango.FontDescription('Noto Mono 11')
 
 # Cell renderer styles
-STYLE_OBLIQUE = Pango.Style.OBLIQUE
+STYLE_ITALIC = Pango.Style.ITALIC
 STYLE_NORMAL = Pango.Style.NORMAL
 
 # Timer text
 FIELDWIDTH = '00h00:00.0000'
 ARMTEXT = '       0.0   '
 
 # Button indications
@@ -395,15 +395,15 @@
         self.set_split()
         self.set_time()
         self.b.update('idle', 'Idle')
         self.b.set_sensitive(False)
 
     def __init__(self, label='Timer', doser=False):
         """Constructor."""
-        _log.debug('building the timerpane')
+        _log.debug('Building timerpane: %r', label)
         s = Gtk.Frame.new(label)
         s.set_border_width(5)
         s.set_shadow_type(Gtk.ShadowType.IN)
         s.show()
         self.doser = doser
 
         #v = Gtk.VBox(False, 5)
@@ -1126,15 +1126,16 @@
         return True
 
     def add_control(self, grid, row):
         """Create a new control and add it to the provided grid"""
         lbl = Gtk.Label(label=self._prompt)
         lbl.set_single_line_mode(True)
         lbl.set_halign(Gtk.Align.START)
-        lbl.set_attributes(Pango.AttrList.from_string('0 -1 style oblique'))
+        if hasattr(Pango.AttrList, 'from_string'):
+            lbl.set_attributes(Pango.AttrList.from_string('0 -1 style italic'))
         if row != 0:
             lbl.set_margin_top(15)
         lbl.show()
         grid.attach(lbl, 0, row, 5, 1)
         return 1
 
 
@@ -1328,23 +1329,23 @@
         ctr.add(self._view)
         ctr.show()
         self._dlg.get_content_area().pack_start(ctr, True, True, 4)
         bb = Gtk.ButtonBox()
         bb.set_layout(Gtk.ButtonBoxStyle.START)
         bb.show()
 
-        but = Gtk.Button.new_from_icon_name('list-add',
+        but = Gtk.Button.new_from_icon_name('list-add-symbolic',
                                             Gtk.IconSize.LARGE_TOOLBAR)
         but.set_always_show_image(True)
         but.show()
         but.connect('clicked', self.add_empty)
         bb.pack_start(but, False, False, 0)
         bb.set_child_non_homogeneous(but, True)
 
-        but = Gtk.Button.new_from_icon_name('list-remove',
+        but = Gtk.Button.new_from_icon_name('list-remove-symbolic',
                                             Gtk.IconSize.LARGE_TOOLBAR)
         but.set_always_show_image(True)
         but.show()
         but.connect('clicked', self.del_selected)
         bb.pack_start(but, False, False, 0)
         bb.set_child_non_homogeneous(but, True)
```

