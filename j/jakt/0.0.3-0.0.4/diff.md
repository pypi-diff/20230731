# Comparing `tmp/jakt-0.0.3.tar.gz` & `tmp/jakt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jakt-0.0.3.tar", last modified: Tue Jul 18 19:58:57 2023, max compression
+gzip compressed data, was "jakt-0.0.4.tar", last modified: Mon Jul 31 12:54:34 2023, max compression
```

## Comparing `jakt-0.0.3.tar` & `jakt-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:58:57.659689 jakt-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-18 19:58:46.000000 jakt-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-18 19:58:57.659689 jakt-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-18 19:58:46.000000 jakt-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:58:57.659689 jakt-0.0.3/jakt/
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-07-18 19:58:46.000000 jakt-0.0.3/jakt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 19:58:46.000000 jakt-0.0.3/jakt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-18 19:58:46.000000 jakt-0.0.3/jakt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-18 19:58:46.000000 jakt-0.0.3/jakt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-18 19:58:46.000000 jakt-0.0.3/jakt/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-18 19:58:46.000000 jakt-0.0.3/jakt/timeslot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:58:57.659689 jakt-0.0.3/jakt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-18 19:58:57.000000 jakt-0.0.3/jakt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-18 19:58:57.000000 jakt-0.0.3/jakt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:58:57.000000 jakt-0.0.3/jakt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:58:57.000000 jakt-0.0.3/jakt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 19:58:57.000000 jakt-0.0.3/jakt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 19:58:57.000000 jakt-0.0.3/jakt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-18 19:58:46.000000 jakt-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 19:58:46.000000 jakt-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:58:57.659689 jakt-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:54:34.343167 jakt-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-31 12:54:24.000000 jakt-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-31 12:54:34.343167 jakt-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-31 12:54:24.000000 jakt-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:54:34.343167 jakt-0.0.4/jakt/
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-07-31 12:54:24.000000 jakt-0.0.4/jakt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 12:54:24.000000 jakt-0.0.4/jakt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-07-31 12:54:24.000000 jakt-0.0.4/jakt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-31 12:54:24.000000 jakt-0.0.4/jakt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-31 12:54:24.000000 jakt-0.0.4/jakt/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-31 12:54:24.000000 jakt-0.0.4/jakt/timeslot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:54:34.343167 jakt-0.0.4/jakt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-31 12:54:34.000000 jakt-0.0.4/jakt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-31 12:54:34.000000 jakt-0.0.4/jakt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 12:54:34.000000 jakt-0.0.4/jakt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 12:54:34.000000 jakt-0.0.4/jakt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 12:54:34.000000 jakt-0.0.4/jakt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 12:54:34.000000 jakt-0.0.4/jakt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-31 12:54:24.000000 jakt-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 12:54:24.000000 jakt-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 12:54:34.343167 jakt-0.0.4/setup.cfg
```

### Comparing `jakt-0.0.3/LICENSE` & `jakt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jakt-0.0.3/jakt/cli.py` & `jakt-0.0.4/jakt/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,91 +1,102 @@
 import click
 from datetime import datetime
 
 from .__init__ import jakt
 from .timeslot import timeslot
 from .exceptions import *
 
+
 @click.group()
-@click.version_option(version="0.0.3", prog_name="jakt")
+@click.version_option(version="0.0.4", prog_name="jakt")
 @click.pass_context
 def cli(ctx):
     """Jakt is just another (k)ommandline timetracker.
 
     Jakt helps you keep track of how you spend your time.
     Whether you want to keep better track of how much time
     you spend on each project or want to keep yourself
     accountable while working, jakt is the perfect tool."""
 
     ctx.ensure_object(dict)
-    ctx.obj['jakt'] = jakt()
-    
+    ctx.obj["jakt"] = jakt()
 
 
 @cli.command()
 @click.argument("project")
-@click.argument("tags", nargs = -1)
+@click.argument("tags", nargs=-1)
 @click.pass_context
 def start(ctx, project, tags):
     """Start a new timeslot"""
-    jkt = ctx.obj['jakt']
+    jkt = ctx.obj["jakt"]
 
     try:
         response = jkt.start(project=project, tags=tags)
 
-        project = click.style(project, fg='blue', bold=True)
-        hrStart = click.style(datetime.fromtimestamp(response["start"]).strftime('%H:%M'), fg='red', bold=True )
-        tags = click.style(' '.join(str(t) for t in response['tags']), fg='green')
+        project = click.style(response.project, fg="blue", bold=True)
+        hrStart = click.style(
+            datetime.fromtimestamp(response.start).strftime("%H:%M"),
+            fg="red",
+            bold=True,
+        )
+        tags = click.style(" ".join(str(t) for t in response.tags), fg="green")
 
         click.echo(f"{project} started at {hrStart}")
         click.echo(f"Tags: {tags}")
 
-
     except JaktActiveError:
-
         click.echo("Other timer already running")
         ctx.invoke(status)
 
+
 @cli.command()
 @click.pass_context
 def stop(ctx):
     """Stops current project"""
-    jkt = ctx.obj['jakt']
+    jkt = ctx.obj["jakt"]
 
     try:
         ts = jkt.stop()
 
-        project = click.style(ts.project, fg='blue', bold=True)
-        tags = click.style(' '.join(str(t) for t in ts.tags), fg='green')
+        project = click.style(ts.project, fg="blue", bold=True)
+        tags = click.style(" ".join(str(t) for t in ts.tags), fg="green")
 
-        hrStop = click.style(ts.end_dt.strftime('%H:%M'), fg='red', bold=True )
+        hrStop = click.style(ts.end_dt.strftime("%H:%M"), fg="red", bold=True)
         dur = ts.getDurationHR()
-        runtime = click.style(f"{dur['hh']:02}:{dur['M']:02}", fg="green", bold = True)
+        runtime = click.style(f"{dur['hh']:02}:{dur['M']:02}", fg="green", bold=True)
 
         click.echo(f"{project} stopped at {hrStop}")
         click.echo(f"Tags: {tags}")
         click.echo(f"Timer ran for {runtime}")
 
     except JaktNotActiveError:
         click.echo("No timer started.")
 
 
 @cli.command()
 @click.pass_context
 def status(ctx):
     """Displays current status"""
-    jkt = ctx.obj['jakt']
+    jkt = ctx.obj["jakt"]
 
     try:
         response = jkt.status()
 
-        project = click.style(response["project"], fg='blue', bold=True)
-        hrStart = click.style(datetime.fromtimestamp(response["start"]).strftime('%H:%M'), fg='red', bold=True )
-        tags = click.style(' '.join(str(t) for t in response["tags"]), fg='green')
-        runtime = click.style(f"{response['elapsedHour']:02}:{response['elapsedMin']:02}", fg="green", bold = True)
+        project = click.style(response["project"], fg="blue", bold=True)
+        hrStart = click.style(
+            datetime.fromtimestamp(response["start"]).strftime("%H:%M"),
+            fg="red",
+            bold=True,
+        )
+        tags = click.style(" ".join(str(t) for t in response["tags"]), fg="green")
+        runtime = click.style(
+            f"{response['elapsedHour']:02}:{response['elapsedMin']:02}",
+            fg="green",
+            bold=True,
+        )
 
         click.echo(f"{project} started at {hrStart}.")
         click.echo(f"Tags: {tags}")
         click.echo(f"Runtime is {runtime}")
 
     except JaktNotActiveError:
         click.echo("No timer started.")
@@ -109,16 +120,15 @@
 )
 @click.option("-p", "--projects", is_flag=True, default=False, help="Display projects")
 @click.option("-t", "--tags", is_flag=True, default=False, help="Display tags")
 # TODO: Display all timeslots using -a
 @click.pass_context
 def ls(ctx, to, from_, categories, projects, tags):
     """Lists timeslots and other data"""
-    jkt = ctx.obj['jakt']
-
+    jkt = ctx.obj["jakt"]
 
     if categories:
         categories = jkt.getCategories()
 
         for cat in categories:
             click.echo(f"{click.style(cat, fg='red', bold=True)}")
 
@@ -136,23 +146,22 @@
         tags = jkt.getTags()
 
         for tag in tags:
             click.echo(f"{click.style(tag, fg='green')}")
 
         return
 
-
     if from_ or to:
         # A few cases of input sanitation
         if from_ and (not to):
             to = datetime.now()
 
         elif to and (not from_):
             click.echo("--from must be set if --to is set")
-            return 
+            return
 
         if from_ > to:
             # Switch the parameters if they are given in the wrong order
             a = from_
             from_ = to
             to = a
             click.echo("--to/--from in wrong order. Flipping them.")
@@ -168,37 +177,39 @@
         if i == 10:
             click.echo(f"{len(timeslots)-i} timeslots not shown.")
             break
 
         ts = timeslots[i]
 
         # Define all styles and shown data
-        ts_id = click.style(ts.id, fg='yellow')
-        ts_project = click.style(ts.project, fg='blue', bold=True)
-        
+        ts_id = click.style(ts.id, fg="yellow")
+        ts_project = click.style(ts.project, fg="blue", bold=True)
+
         # Make sure time is readable and makes sense
         ts_start = ts.start_dt
         ts_end = ts.end_dt
 
         if ts_start.date() == ts_end.date():
             ts_start_hr = ts_start.strftime("%H:%M")
         else:
             ts_start_hr = ts_start.strftime("%H:%M %d-%m-%y")
 
         ts_end_hr = ts_end.strftime("%H:%M %d-%m-%y")
 
         s = str(ts.duration).split(":")
-        ts_duration = click.style(f"{int(s[0]):02}:{int(s[1]):02}:{int(s[2]):02}", fg='green')
+        ts_duration = click.style(
+            f"{int(s[0]):02}:{int(s[1]):02}:{int(s[2]):02}", fg="green"
+        )
 
-
-        ts_tags = click.style(' '.join(str(t) for t in ts.tags), fg='green')
+        ts_tags = click.style(" ".join(str(t) for t in ts.tags), fg="green")
 
         # Display data on single line
         click.echo(
-            f"{ts_id} {ts_duration} ({ts_start_hr} - {ts_end_hr}) {ts_project} {ts_tags}")
+            f"{ts_id} {ts_duration} ({ts_start_hr} - {ts_end_hr}) {ts_project} {ts_tags}"
+        )
 
 
 @cli.command()
 @click.option(
     "--to",
     "to",
     type=click.DateTime(formats=["%d-%m-%y %H:%M", "%d-%m-%y %H:%M:%S"]),
@@ -209,92 +220,114 @@
     "--from",
     "from_",
     type=click.DateTime(formats=["%d-%m-%y %H:%M", "%d-%m-%y %H:%M:%S"]),
     help="Endtime",
     required=True,
 )
 @click.argument("project")
-@click.argument("tags", nargs = -1)
+@click.argument("tags", nargs=-1)
 @click.pass_context
 def add(ctx, to, from_, project, tags):
     """Add a timeslot that was not logged live"""
-    jkt = ctx.obj['jakt']
+    jkt = ctx.obj["jakt"]
 
     ts = timeslot(
         ID=jkt.generateUniqueID(),
-        start= int(from_.strftime('%s')),
-        end= int(to.strftime('%s')),
+        start=int(from_.strftime("%s")),
+        end=int(to.strftime("%s")),
         project=project,
-        tags=tags
+        tags=tags,
     )
 
     jkt.add(ts)
-    
 
 
+"""
 @cli.command()
 @click.argument("index")
 def edit(index):
-    """Edits categories, projects, tags and timeslots"""
+    # Edits categories, projects, tags and timeslots
     pass
+"""
 
 
 @cli.command()
 @click.option("-p", "--project", default="", help="Show only specified project")
 @click.option("-t", "--tag", default="", help="Show only specified tag")
 @click.pass_context
 def report(ctx, project, tag):
     """Generates reports from timetracker data"""
-    jkt = ctx.obj['jakt']
+    jkt = ctx.obj["jakt"]
 
     jkt_report = jkt.report()
 
     if project:
         projects = jkt_report.getProjectReport(project=project)
     else:
         projects = jkt_report.getProjectReport()
 
     for project in projects:
-
-        hrProject = click.style(project['project'], fg='blue', bold=True)
-        hrTime = click.style(project['time'], fg='red', bold=True)
+        hrProject = click.style(project["project"], fg="blue", bold=True)
+        hrTime = click.style(project["time"], fg="red", bold=True)
         click.echo(f"{hrProject}  {hrTime}")
 
-        tags = jkt_report.getTagReport(project['project'])
+        tags = jkt_report.getTagReport(project["project"])
         for tag in tags:
-
-            hrTag = click.style(tag['tag'], fg='green', bold=True)
-            hrTagTime = click.style(tag['time'], fg='yellow')
+            hrTag = click.style(tag["tag"], fg="green", bold=True)
+            hrTagTime = click.style(tag["time"], fg="yellow")
 
             click.echo(f" - {hrTag}  {hrTagTime}")
 
 
+
 @cli.command()
-def pause():
-    """Takes a break in current timeslot"""
-    pass
+@click.pass_context
+def resume(ctx):
+    """
+    Start new timeslot with same settings
+    """
+    jkt = ctx.obj["jakt"]
+
+    try:
+        response = jkt.resume()
 
+        project = click.style(response.project, fg="blue", bold=True)
+        hrStart = click.style(
+            datetime.fromtimestamp(response.start).strftime("%H:%M"),
+            fg="red",
+            bold=True,
+        )
+        tags = click.style(" ".join(str(t) for t in response.tags), fg="green")
 
+        click.echo(f"{project} started at {hrStart}")
+        click.echo(f"Tags: {tags}")
+
+    except JaktActiveError:
+        click.echo("Other timer already running")
+        ctx.invoke(status)
+
+
+"""
 @cli.command()
-def resume():
-    """Resumes paused timeslot"""
+def pause():
+    # Takes a break in current timeslot
     pass
 
-
 @cli.command()
 def config():
-    """Sets new values in configuration file"""
+    # Sets new values in configuration file
     pass
 
 
 @cli.command()
 def sync():
-    """Syncronizes data with server"""
+    # Syncronizes data with server
     pass
 
 @cli.command()
 def license():
-    """Outputs license"""
+    # Outputs license
     pass
+"""
 
 if __name__ == "__main__":
     cli(obj={})
```

### Comparing `jakt-0.0.3/pyproject.toml` & `jakt-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "jakt"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="kwillno", email="kristian@kwill.no" },
 ]
-description = "Just another timetracker"
+description = "Just another (k)ommandline timetracker"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX",
 ]
```

