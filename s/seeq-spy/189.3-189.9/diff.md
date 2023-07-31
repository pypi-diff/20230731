# Comparing `tmp/seeq-spy-189.3.tar.gz` & `tmp/seeq-spy-189.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seeq-spy-189.3.tar", last modified: Thu Jul 13 17:41:44 2023, max compression
+gzip compressed data, was "seeq-spy-189.9.tar", last modified: Mon Jul 31 16:48:31 2023, max compression
```

## Comparing `seeq-spy-189.3.tar` & `seeq-spy-189.9.tar`

### file list

```diff
@@ -1,151 +1,152 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.116257 seeq-spy-189.3/
--rw-rw-rw-   0        0        0    33551 2023-03-28 23:18:24.000000 seeq-spy-189.3/LICENSE
--rw-rw-rw-   0        0        0      207 2023-03-28 23:18:24.000000 seeq-spy-189.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4606 2023-07-13 17:41:44.115257 seeq-spy-189.3/PKG-INFO
--rw-rw-rw-   0        0        0     4091 2023-06-21 15:08:28.000000 seeq-spy-189.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 17:41:43.961258 seeq-spy-189.3/seeq/
-drwxrwxrwx   0        0        0        0 2023-07-13 17:41:43.977256 seeq-spy-189.3/seeq/base/
--rw-rw-rw-   0        0        0       36 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/base/__init__.py
--rw-rw-rw-   0        0        0      875 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/base/proputil.py
--rw-rw-rw-   0        0        0    33155 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/base/seeq_names.py
--rw-rw-rw-   0        0        0      157 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/base/system.py
--rw-rw-rw-   0        0        0     4788 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/base/util.py
-drwxrwxrwx   0        0        0        0 2023-07-13 17:41:43.997258 seeq-spy-189.3/seeq/spy/
--rw-rw-rw-   0        0        0     1953 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/__init__.py
--rw-rw-rw-   0        0        0    32021 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_common.py
--rw-rw-rw-   0        0        0     4687 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_config.py
--rw-rw-rw-   0        0        0     4424 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_datalab.py
--rw-rw-rw-   0        0        0     9914 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_errors.py
--rw-rw-rw-   0        0        0    49041 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_login.py
--rw-rw-rw-   0        0        0    95701 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_metadata.py
--rw-rw-rw-   0        0        0     5822 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_metadata_push_results.py
--rw-rw-rw-   0        0        0     2954 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_plot.py
--rw-rw-rw-   0        0        0    55646 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_pull.py
--rw-rw-rw-   0        0        0    68835 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_push.py
--rw-rw-rw-   0        0        0     5155 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_redaction.py
--rw-rw-rw-   0        0        0    57799 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_search.py
--rw-rw-rw-   0        0        0    20456 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_session.py
--rw-rw-rw-   0        0        0    16874 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_status.py
--rw-rw-rw-   0        0        0    20657 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_swap.py
--rw-rw-rw-   0        0        0     3471 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_upgrade.py
--rw-rw-rw-   0        0        0    10707 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/_url.py
-drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.000257 seeq-spy-189.3/seeq/spy/acl/
--rw-rw-rw-   0        0        0      104 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/acl/__init__.py
--rw-rw-rw-   0        0        0    12172 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/acl/_pull.py
--rw-rw-rw-   0        0        0    11351 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/acl/_push.py
-drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.005256 seeq-spy-189.3/seeq/spy/addons/
--rw-rw-rw-   0        0        0      188 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/addons/__init__.py
--rw-rw-rw-   0        0        0    26376 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/addons/_install.py
--rw-rw-rw-   0        0        0     2408 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/addons/_permissions.py
--rw-rw-rw-   0        0        0    12137 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/addons/_search.py
--rw-rw-rw-   0        0        0     5334 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/addons/_uninstall.py
-drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.011256 seeq-spy-189.3/seeq/spy/assets/
--rw-rw-rw-   0        0        0      336 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/__init__.py
--rw-rw-rw-   0        0        0     3638 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_brochure.py
--rw-rw-rw-   0        0        0    12419 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_build.py
--rw-rw-rw-   0        0        0     3133 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_context.py
--rw-rw-rw-   0        0        0    48189 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_model.py
-drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.023257 seeq-spy-189.3/seeq/spy/assets/_trees/
--rw-rw-rw-   0        0        0       69 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_trees/__init__.py
--rw-rw-rw-   0        0        0     1375 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_trees/_constants.py
--rw-rw-rw-   0        0        0     7350 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_trees/_csv.py
--rw-rw-rw-   0        0        0    22068 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_trees/_match.py
--rw-rw-rw-   0        0        0     2629 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_trees/_pandas.py
--rw-rw-rw-   0        0        0     6458 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_trees/_path.py
--rw-rw-rw-   0        0        0    23208 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_trees/_properties.py
--rw-rw-rw-   0        0        0    13479 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_trees/_pull.py
--rw-rw-rw-   0        0        0    58791 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_trees/_tree.py
--rw-rw-rw-   0        0        0     5897 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_trees/_utils.py
--rw-rw-rw-   0        0        0    25525 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/_trees/_validate.py
--rw-rw-rw-   0        0        0     2538 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/assets/brochure.html
-drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.025257 seeq-spy-189.3/seeq/spy/docs/
-drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.048256 seeq-spy-189.3/seeq/spy/docs/Documentation/
-drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.049259 seeq-spy-189.3/seeq/spy/docs/Documentation/Administration/
--rw-rw-rw-   0        0        0     8501 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Administration/User Migration.ipynb
-drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.056256 seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/
--rw-rw-rw-   0        0        0    17428 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb
--rw-rw-rw-   0        0        0    33412 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb
--rw-rw-rw-   0        0        0    16700 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb
--rw-rw-rw-   0        0        0     8406 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb
--rw-rw-rw-   0        0        0    38889 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb
--rw-rw-rw-   0        0        0      870 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg
--rw-rw-rw-   0        0        0   186560 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb
--rw-rw-rw-   0        0        0   239024 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb
--rw-rw-rw-   0        0        0   229026 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb
--rw-rw-rw-   0        0        0    24627 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb
-drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.065256 seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/
--rw-rw-rw-   0        0        0   135771 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg
--rw-rw-rw-   0        0        0   152116 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg
--rw-rw-rw-   0        0        0   207271 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg
--rw-rw-rw-   0        0        0      325 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/Readme.txt
--rw-rw-rw-   0        0        0   141516 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png
--rw-rw-rw-   0        0        0   439966 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png
--rw-rw-rw-   0        0        0   189377 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png
--rw-rw-rw-   0        0        0    23874 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Command Reference.ipynb
--rw-rw-rw-   0        0        0   190416 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Data Lab Visualizations.ipynb
-drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.072255 seeq-spy-189.3/seeq/spy/docs/Documentation/Support Files/
--rw-rw-rw-   0        0        0   100268 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Support Files/Example Export.zip
--rw-rw-rw-   0        0        0   113732 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip
--rw-rw-rw-   0        0        0   645282 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip
--rw-rw-rw-   0        0        0  1083835 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv
--rw-rw-rw-   0        0        0      429 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Support Files/spy_tree_example.csv
--rw-rw-rw-   0        0        0   674658 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Tutorial.ipynb
--rw-rw-rw-   0        0        0    11595 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Version Considerations.ipynb
--rw-rw-rw-   0        0        0  1559074 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/Workbook Templates.ipynb
--rw-rw-rw-   0        0        0    54071 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/spy.acl.ipynb
--rw-rw-rw-   0        0        0    11195 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/spy.jobs.ipynb
--rw-rw-rw-   0        0        0    13015 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/spy.login.ipynb
--rw-rw-rw-   0        0        0   128103 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/spy.pull.ipynb
--rw-rw-rw-   0        0        0    99541 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/spy.push.ipynb
--rw-rw-rw-   0        0        0    57647 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/spy.search.ipynb
--rw-rw-rw-   0        0        0    95777 2023-07-13 17:41:40.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/spy.swap.ipynb
--rw-rw-rw-   0        0        0    10829 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/spy.widgets.ipynb
--rw-rw-rw-   0        0        0    69828 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/Documentation/spy.workbooks.ipynb
--rw-rw-rw-   0        0        0       60 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/__init__.py
--rw-rw-rw-   0        0        0     1704 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/docs/_copy.py
-drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.077256 seeq-spy-189.3/seeq/spy/jobs/
--rw-rw-rw-   0        0        0      491 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/jobs/__init__.py
--rw-rw-rw-   0        0        0     9869 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/jobs/_execute.py
--rw-rw-rw-   0        0        0     6111 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/jobs/_pull.py
--rw-rw-rw-   0        0        0     9398 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/jobs/_push.py
--rw-rw-rw-   0        0        0    25737 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/jobs/_schedule.py
-drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.080258 seeq-spy-189.3/seeq/spy/notifications/
--rw-rw-rw-   0        0        0      153 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/notifications/__init__.py
--rw-rw-rw-   0        0        0    11927 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/notifications/_emails.py
-drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.081256 seeq-spy-189.3/seeq/spy/utils/
--rw-rw-rw-   0        0        0     1569 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.084257 seeq-spy-189.3/seeq/spy/widgets/
--rw-rw-rw-   0        0        0      200 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/widgets/__init__.py
--rw-rw-rw-   0        0        0     4158 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/widgets/_ipy_utils.py
--rw-rw-rw-   0        0        0    30480 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/widgets/_widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.106257 seeq-spy-189.3/seeq/spy/workbooks/
--rw-rw-rw-   0        0        0     3012 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/__init__.py
--rw-rw-rw-   0        0        0    43797 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_annotation.py
--rw-rw-rw-   0        0        0    34087 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_content.py
--rw-rw-rw-   0        0        0    40974 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_data.py
--rw-rw-rw-   0        0        0     6639 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_folder.py
--rw-rw-rw-   0        0        0    14611 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_item.py
--rw-rw-rw-   0        0        0     5586 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_item_map.py
--rw-rw-rw-   0        0        0     3033 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_load.py
--rw-rw-rw-   0        0        0     3790 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_mustache.py
--rw-rw-rw-   0        0        0    14175 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_pull.py
--rw-rw-rw-   0        0        0    23108 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_push.py
--rw-rw-rw-   0        0        0     6316 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_render.py
--rw-rw-rw-   0        0        0    27127 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_report_content_utilities.py
--rw-rw-rw-   0        0        0     4729 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_save.py
--rw-rw-rw-   0        0        0    15545 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_search.py
--rw-rw-rw-   0        0        0    38578 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_template.py
--rw-rw-rw-   0        0        0    11995 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_user.py
--rw-rw-rw-   0        0        0    52454 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_workbook.py
--rw-rw-rw-   0        0        0    48919 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_worksheet.py
--rw-rw-rw-   0        0        0    51518 2023-07-13 17:41:42.000000 seeq-spy-189.3/seeq/spy/workbooks/_workstep.py
--rw-rw-rw-   0        0        0   427362 2023-07-13 17:41:41.000000 seeq-spy-189.3/seeq/spy/workbooks/app.css
-drwxrwxrwx   0        0        0        0 2023-07-13 17:41:44.114256 seeq-spy-189.3/seeq_spy.egg-info/
--rw-rw-rw-   0        0        0     4606 2023-07-13 17:41:43.000000 seeq-spy-189.3/seeq_spy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4759 2023-07-13 17:41:43.000000 seeq-spy-189.3/seeq_spy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 17:41:43.000000 seeq-spy-189.3/seeq_spy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-10 16:46:50.000000 seeq-spy-189.3/seeq_spy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      311 2023-07-13 17:41:43.000000 seeq-spy-189.3/seeq_spy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-13 17:41:43.000000 seeq-spy-189.3/seeq_spy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 17:41:44.116257 seeq-spy-189.3/setup.cfg
--rw-rw-rw-   0        0        0     1677 2023-07-13 17:38:47.000000 seeq-spy-189.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:48:31.351792 seeq-spy-189.9/
+-rw-rw-rw-   0        0        0    33551 2023-03-28 23:18:24.000000 seeq-spy-189.9/LICENSE
+-rw-rw-rw-   0        0        0      207 2023-03-28 23:18:24.000000 seeq-spy-189.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4606 2023-07-31 16:48:31.350743 seeq-spy-189.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4091 2023-06-21 15:08:28.000000 seeq-spy-189.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 16:48:31.092652 seeq-spy-189.9/seeq/
+drwxrwxrwx   0        0        0        0 2023-07-31 16:48:31.115206 seeq-spy-189.9/seeq/base/
+-rw-rw-rw-   0        0        0       36 2023-07-31 16:48:24.000000 seeq-spy-189.9/seeq/base/__init__.py
+-rw-rw-rw-   0        0        0      875 2023-07-31 16:48:24.000000 seeq-spy-189.9/seeq/base/proputil.py
+-rw-rw-rw-   0        0        0    33299 2023-07-31 16:48:24.000000 seeq-spy-189.9/seeq/base/seeq_names.py
+-rw-rw-rw-   0        0        0      157 2023-07-31 16:48:24.000000 seeq-spy-189.9/seeq/base/system.py
+-rw-rw-rw-   0        0        0     4788 2023-07-31 16:48:24.000000 seeq-spy-189.9/seeq/base/util.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:48:31.147204 seeq-spy-189.9/seeq/spy/
+-rw-rw-rw-   0        0        0     1953 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/__init__.py
+-rw-rw-rw-   0        0        0    32021 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/_common.py
+-rw-rw-rw-   0        0        0     4687 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/_config.py
+-rw-rw-rw-   0        0        0     4424 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/_datalab.py
+-rw-rw-rw-   0        0        0     9914 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/_errors.py
+-rw-rw-rw-   0        0        0    48952 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/_login.py
+-rw-rw-rw-   0        0        0    95701 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/_metadata.py
+-rw-rw-rw-   0        0        0     5822 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/_metadata_push_results.py
+-rw-rw-rw-   0        0        0     2954 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/_plot.py
+-rw-rw-rw-   0        0        0    56368 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/_pull.py
+-rw-rw-rw-   0        0        0    68835 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/_push.py
+-rw-rw-rw-   0        0        0     5155 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/_redaction.py
+-rw-rw-rw-   0        0        0    57993 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/_search.py
+-rw-rw-rw-   0        0        0    23581 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/_session.py
+-rw-rw-rw-   0        0        0    17060 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/_status.py
+-rw-rw-rw-   0        0        0    20657 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/_swap.py
+-rw-rw-rw-   0        0        0     3471 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/_upgrade.py
+-rw-rw-rw-   0        0        0    10707 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/_url.py
+-rw-rw-rw-   0        0        0     8090 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/_usage.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:48:31.152204 seeq-spy-189.9/seeq/spy/acl/
+-rw-rw-rw-   0        0        0      104 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/acl/__init__.py
+-rw-rw-rw-   0        0        0    12172 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/acl/_pull.py
+-rw-rw-rw-   0        0        0    11351 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/acl/_push.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:48:31.160204 seeq-spy-189.9/seeq/spy/addons/
+-rw-rw-rw-   0        0        0      188 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/addons/__init__.py
+-rw-rw-rw-   0        0        0    26376 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/addons/_install.py
+-rw-rw-rw-   0        0        0     2408 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/addons/_permissions.py
+-rw-rw-rw-   0        0        0    12137 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/addons/_search.py
+-rw-rw-rw-   0        0        0     5334 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/addons/_uninstall.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:48:31.168813 seeq-spy-189.9/seeq/spy/assets/
+-rw-rw-rw-   0        0        0      336 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/assets/__init__.py
+-rw-rw-rw-   0        0        0     3638 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/assets/_brochure.py
+-rw-rw-rw-   0        0        0    12419 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/assets/_build.py
+-rw-rw-rw-   0        0        0     3133 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/assets/_context.py
+-rw-rw-rw-   0        0        0    48189 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/assets/_model.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:48:31.186815 seeq-spy-189.9/seeq/spy/assets/_trees/
+-rw-rw-rw-   0        0        0       69 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/assets/_trees/__init__.py
+-rw-rw-rw-   0        0        0     1375 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/assets/_trees/_constants.py
+-rw-rw-rw-   0        0        0     7350 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/assets/_trees/_csv.py
+-rw-rw-rw-   0        0        0    22068 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/assets/_trees/_match.py
+-rw-rw-rw-   0        0        0     2629 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/assets/_trees/_pandas.py
+-rw-rw-rw-   0        0        0     6458 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/assets/_trees/_path.py
+-rw-rw-rw-   0        0        0    23208 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/assets/_trees/_properties.py
+-rw-rw-rw-   0        0        0    13479 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/assets/_trees/_pull.py
+-rw-rw-rw-   0        0        0    58791 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/assets/_trees/_tree.py
+-rw-rw-rw-   0        0        0     5897 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/assets/_trees/_utils.py
+-rw-rw-rw-   0        0        0    25525 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/assets/_trees/_validate.py
+-rw-rw-rw-   0        0        0     2538 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/assets/brochure.html
+drwxrwxrwx   0        0        0        0 2023-07-31 16:48:31.189814 seeq-spy-189.9/seeq/spy/docs/
+drwxrwxrwx   0        0        0        0 2023-07-31 16:48:31.228456 seeq-spy-189.9/seeq/spy/docs/Documentation/
+drwxrwxrwx   0        0        0        0 2023-07-31 16:48:31.230458 seeq-spy-189.9/seeq/spy/docs/Documentation/Administration/
+-rw-rw-rw-   0        0        0     8501 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Administration/User Migration.ipynb
+drwxrwxrwx   0        0        0        0 2023-07-31 16:48:31.242457 seeq-spy-189.9/seeq/spy/docs/Documentation/Advanced Scheduling/
+-rw-rw-rw-   0        0        0    17428 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb
+-rw-rw-rw-   0        0        0    33412 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb
+-rw-rw-rw-   0        0        0    16736 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb
+-rw-rw-rw-   0        0        0     8406 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb
+-rw-rw-rw-   0        0        0    38889 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb
+-rw-rw-rw-   0        0        0      870 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg
+-rw-rw-rw-   0        0        0   186560 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb
+-rw-rw-rw-   0        0        0   239024 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb
+-rw-rw-rw-   0        0        0   229026 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb
+-rw-rw-rw-   0        0        0    24627 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb
+drwxrwxrwx   0        0        0        0 2023-07-31 16:48:31.257462 seeq-spy-189.9/seeq/spy/docs/Documentation/Attached Images/
+-rw-rw-rw-   0        0        0   135771 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg
+-rw-rw-rw-   0        0        0   152116 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg
+-rw-rw-rw-   0        0        0   207271 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg
+-rw-rw-rw-   0        0        0      325 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Attached Images/Readme.txt
+-rw-rw-rw-   0        0        0   141516 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png
+-rw-rw-rw-   0        0        0   439966 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png
+-rw-rw-rw-   0        0        0   189377 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png
+-rw-rw-rw-   0        0        0    23874 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Command Reference.ipynb
+-rw-rw-rw-   0        0        0   190416 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Data Lab Visualizations.ipynb
+drwxrwxrwx   0        0        0        0 2023-07-31 16:48:31.271986 seeq-spy-189.9/seeq/spy/docs/Documentation/Support Files/
+-rw-rw-rw-   0        0        0   100268 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Support Files/Example Export.zip
+-rw-rw-rw-   0        0        0   113732 2023-07-31 16:48:26.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip
+-rw-rw-rw-   0        0        0   645282 2023-07-31 16:48:26.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip
+-rw-rw-rw-   0        0        0  1083835 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv
+-rw-rw-rw-   0        0        0      429 2023-07-31 16:48:26.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Support Files/spy_tree_example.csv
+-rw-rw-rw-   0        0        0   674658 2023-07-31 16:48:26.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Tutorial.ipynb
+-rw-rw-rw-   0        0        0    12580 2023-07-31 16:48:26.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Version Considerations.ipynb
+-rw-rw-rw-   0        0        0  1559074 2023-07-31 16:48:26.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/Workbook Templates.ipynb
+-rw-rw-rw-   0        0        0    54071 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/spy.acl.ipynb
+-rw-rw-rw-   0        0        0    11195 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/spy.jobs.ipynb
+-rw-rw-rw-   0        0        0    13015 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/spy.login.ipynb
+-rw-rw-rw-   0        0        0   138622 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/spy.pull.ipynb
+-rw-rw-rw-   0        0        0    99541 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/spy.push.ipynb
+-rw-rw-rw-   0        0        0    57647 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/spy.search.ipynb
+-rw-rw-rw-   0        0        0    95777 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/spy.swap.ipynb
+-rw-rw-rw-   0        0        0    10829 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/spy.widgets.ipynb
+-rw-rw-rw-   0        0        0    69828 2023-07-31 16:48:25.000000 seeq-spy-189.9/seeq/spy/docs/Documentation/spy.workbooks.ipynb
+-rw-rw-rw-   0        0        0       60 2023-07-31 16:48:26.000000 seeq-spy-189.9/seeq/spy/docs/__init__.py
+-rw-rw-rw-   0        0        0     1704 2023-07-31 16:48:26.000000 seeq-spy-189.9/seeq/spy/docs/_copy.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:48:31.280976 seeq-spy-189.9/seeq/spy/jobs/
+-rw-rw-rw-   0        0        0      491 2023-07-31 16:48:26.000000 seeq-spy-189.9/seeq/spy/jobs/__init__.py
+-rw-rw-rw-   0        0        0    14158 2023-07-31 16:48:26.000000 seeq-spy-189.9/seeq/spy/jobs/_execute.py
+-rw-rw-rw-   0        0        0     6155 2023-07-31 16:48:26.000000 seeq-spy-189.9/seeq/spy/jobs/_pull.py
+-rw-rw-rw-   0        0        0    10454 2023-07-31 16:48:26.000000 seeq-spy-189.9/seeq/spy/jobs/_push.py
+-rw-rw-rw-   0        0        0    28125 2023-07-31 16:48:26.000000 seeq-spy-189.9/seeq/spy/jobs/_schedule.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:48:31.283978 seeq-spy-189.9/seeq/spy/notifications/
+-rw-rw-rw-   0        0        0      153 2023-07-31 16:48:26.000000 seeq-spy-189.9/seeq/spy/notifications/__init__.py
+-rw-rw-rw-   0        0        0    11927 2023-07-31 16:48:26.000000 seeq-spy-189.9/seeq/spy/notifications/_emails.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:48:31.285976 seeq-spy-189.9/seeq/spy/utils/
+-rw-rw-rw-   0        0        0     1569 2023-07-31 16:48:26.000000 seeq-spy-189.9/seeq/spy/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:48:31.290976 seeq-spy-189.9/seeq/spy/widgets/
+-rw-rw-rw-   0        0        0      200 2023-07-31 16:48:26.000000 seeq-spy-189.9/seeq/spy/widgets/__init__.py
+-rw-rw-rw-   0        0        0     4158 2023-07-31 16:48:26.000000 seeq-spy-189.9/seeq/spy/widgets/_ipy_utils.py
+-rw-rw-rw-   0        0        0    30480 2023-07-31 16:48:26.000000 seeq-spy-189.9/seeq/spy/widgets/_widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:48:31.330978 seeq-spy-189.9/seeq/spy/workbooks/
+-rw-rw-rw-   0        0        0     3012 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/workbooks/__init__.py
+-rw-rw-rw-   0        0        0    43797 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/workbooks/_annotation.py
+-rw-rw-rw-   0        0        0    34087 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/workbooks/_content.py
+-rw-rw-rw-   0        0        0    40974 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/workbooks/_data.py
+-rw-rw-rw-   0        0        0     6639 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/workbooks/_folder.py
+-rw-rw-rw-   0        0        0    14611 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/workbooks/_item.py
+-rw-rw-rw-   0        0        0     5586 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/workbooks/_item_map.py
+-rw-rw-rw-   0        0        0     3033 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/workbooks/_load.py
+-rw-rw-rw-   0        0        0     4502 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/workbooks/_mustache.py
+-rw-rw-rw-   0        0        0    14175 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/workbooks/_pull.py
+-rw-rw-rw-   0        0        0    23108 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/workbooks/_push.py
+-rw-rw-rw-   0        0        0     6316 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/workbooks/_render.py
+-rw-rw-rw-   0        0        0    27127 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/workbooks/_report_content_utilities.py
+-rw-rw-rw-   0        0        0     4729 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/workbooks/_save.py
+-rw-rw-rw-   0        0        0    15545 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/workbooks/_search.py
+-rw-rw-rw-   0        0        0    38578 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/workbooks/_template.py
+-rw-rw-rw-   0        0        0    11995 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/workbooks/_user.py
+-rw-rw-rw-   0        0        0    52454 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/workbooks/_workbook.py
+-rw-rw-rw-   0        0        0    48919 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/workbooks/_worksheet.py
+-rw-rw-rw-   0        0        0    51518 2023-07-31 16:48:28.000000 seeq-spy-189.9/seeq/spy/workbooks/_workstep.py
+-rw-rw-rw-   0        0        0   427362 2023-07-31 16:48:26.000000 seeq-spy-189.9/seeq/spy/workbooks/app.css
+drwxrwxrwx   0        0        0        0 2023-07-31 16:48:31.347704 seeq-spy-189.9/seeq_spy.egg-info/
+-rw-rw-rw-   0        0        0     4606 2023-07-31 16:48:30.000000 seeq-spy-189.9/seeq_spy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4778 2023-07-31 16:48:30.000000 seeq-spy-189.9/seeq_spy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 16:48:30.000000 seeq-spy-189.9/seeq_spy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-10 16:46:50.000000 seeq-spy-189.9/seeq_spy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      311 2023-07-31 16:48:30.000000 seeq-spy-189.9/seeq_spy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-31 16:48:30.000000 seeq-spy-189.9/seeq_spy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 16:48:31.352321 seeq-spy-189.9/setup.cfg
+-rw-rw-rw-   0        0        0     1677 2023-07-31 16:44:10.000000 seeq-spy-189.9/setup.py
```

### Comparing `seeq-spy-189.3/LICENSE` & `seeq-spy-189.9/LICENSE`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/PKG-INFO` & `seeq-spy-189.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq-spy
-Version: 189.3
+Version: 189.9
 Summary: Easy-to-use Python interface for Seeq
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seeq-spy-189.3/README.md` & `seeq-spy-189.9/README.md`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/base/proputil.py` & `seeq-spy-189.9/seeq/base/proputil.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/base/seeq_names.py` & `seeq-spy-189.9/seeq/base/seeq_names.py`

 * *Files 1% similar despite different names*

```diff
@@ -777,14 +777,16 @@
         cron_schedule = 'Cron Schedule'
         background = 'Background'
         condition_formula_now = 'Condition Formula Now'
         notebook_path = 'Notebook Path'
         previous_run_time = 'Previous Run Time'
         cron_schedules_to_indices = 'Cron Schedules To Indices'
         label = 'Label'
+        notify_on_skipped_execution = 'Notify On Skipped Execution'
+        notify_on_automatic_unschedule = 'Notify On Automatic Unschedule'
         total_run_time = 'Total Run Time'
         average_run_time = 'Average Run Time'
         is_fixed_with = 'Is Fixed Width'
         is_ck_enabled = 'Is CK Enabled'
         froala_backup = 'Froala Backup'
         original_has_workstep_guid = 'Original HasWorkstep GUID'
         in_development = 'In Development'
```

### Comparing `seeq-spy-189.3/seeq/base/util.py` & `seeq-spy-189.9/seeq/base/util.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/__init__.py` & `seeq-spy-189.9/seeq/spy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,8 +54,8 @@
 """
 
 __all__ = ['acl', 'addons', 'assets', 'docs', 'workbooks', 'widgets', 'login', 'logout', 'plot', 'pull', 'push',
            'search', 'swap', 'PATH_ROOT', 'DEFAULT_WORKBOOK_PATH', 'GLOBALS_ONLY', 'GLOBALS_AND_ALL_WORKBOOKS',
            'INHERIT_FROM_WORKBOOK', 'Session', 'Status', 'options', 'session', 'client', 'user',
            'server_version', 'jobs', 'notifications', 'upgrade', 'utils', 'errors']
 
-__version__ = '%d.%d' % (int('189'), int('3'))
+__version__ = '%d.%d' % (int('189'), int('9'))
```

### Comparing `seeq-spy-189.3/seeq/spy/_common.py` & `seeq-spy-189.9/seeq/spy/_common.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/_config.py` & `seeq-spy-189.9/seeq/spy/_config.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/_datalab.py` & `seeq-spy-189.9/seeq/spy/_datalab.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/_errors.py` & `seeq-spy-189.9/seeq/spy/_errors.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/_login.py` & `seeq-spy-189.9/seeq/spy/_login.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import datetime
 import json
 import logging
 import os
 import re
 import warnings
+from dataclasses import dataclass
 from typing import Optional, Tuple, Union
 from urllib.parse import urlparse, quote
 
 import pandas as pd
 import pkg_resources
 import pytz
 import requests
@@ -19,15 +20,14 @@
 from urllib3.connectionpool import MaxRetryError, SSLError
 
 from seeq import spy, sdk
 from seeq.base import util
 from seeq.sdk import *
 from seeq.spy import _common, _datalab
 from seeq.spy._config import Setting
-from seeq.spy._datalab import is_datalab_functions_project
 from seeq.spy._errors import *
 from seeq.spy._session import Session
 from seeq.spy._status import Status
 
 AUTOMATIC_PROXY_DETECTION = '__auto__'
 
 
@@ -90,15 +90,15 @@
 
     credentials_file : str, optional
         Reads username and password from the specified file. If specified, the
         file should be plane text and contain two lines, the first line being
         the username, the second being the user's password.
 
     force : str, default True
-        If True, re-logs in even if already already logged in. If False, skips
+        If True, re-logs in even if already logged in. If False, skips
         login if already logged in. You should include a spy.login(force=False)
         cell if you are creating example notebooks that may be used in Jupyter
         environments like Anaconda, AWS SageMaker or Azure Notebooks.)
 
     quiet : bool, default False
         If True, suppresses progress output. Note that when status is
         provided, the quiet setting of the Status object that is passed
@@ -121,20 +121,22 @@
         Private argument for Data Lab use only.
 
     csrf_token : str
         Private argument for Data Lab use only.
 
     request_origin_label : str
         Used for tracking Data Consumption. If supplied, this label will be added as a header to all requests from
-        the logged in user. Not necessary in Data Lab because the header will already be filled in.
+        the logged in user. Not necessary in Data Lab because the header will already be filled in. You can also specify
+        this value after login by setting the spy.session.request_origin_label property.
 
     request_origin_url : str
         Used for tracking Data Consumption. If supplied, this label will be added as a header to all requests from
         the logged in user. Not necessary in Data Lab because the header will already be filled in. If NOT in Data
-        Lab, supply a full URL that leads to the tool/plugin that is consuming data, if applicable.
+        Lab, supply a full URL that leads to the tool/plugin that is consuming data, if applicable. You can also specify
+        this value after login by setting the spy.session.request_origin_url property.
 
     Examples
     --------
     Log in to two different servers at the same time:
 
     >>> session1 = Session()
     >>> session2 = Session()
@@ -143,27 +145,29 @@
 
     """
     _common.validate_argument_types([
         (username, 'username', str),
         (password, 'password', str),
         (access_key, 'access_key', str),
         (url, 'url', str),
-        (private_url, 'private_url', str),
         (directory, 'directory', str),
         (ignore_ssl_errors, 'ignore_ssl_errors', bool),
         (proxy, 'proxy', str),
         (credentials_file, 'credentials_file', str),
+        (force, 'force', bool),
+        (quiet, 'quiet', bool),
+        (status, 'status', Status),
+        (session, 'session', Session),
+        (private_url, 'private_url', str),
         # Note: Although auth_token is no longer a supported authentication method for non-Seeq Data Lab scenarios,
         # it is still used by Seeq Data Lab code to log the user in.
         (auth_token, 'auth_token', str),
         (csrf_token, 'csrf_token', str),
-        (force, 'force', bool),
-        (quiet, 'quiet', bool),
-        (status, 'status', Status),
-        (session, 'session', Session)
+        (request_origin_label, 'request_origin_label', str),
+        (request_origin_url, 'request_origin_url', str),
     ])
 
     status = Status.validate(status, quiet)
     session = Session.validate(session)
 
     if private_url is not None and url is None:
         raise SPyValueError('private_url argument cannot be specified without also specifying url argument')
@@ -172,32 +176,15 @@
         _login(username, password, access_key, url, directory, ignore_ssl_errors, proxy,
                credentials_file, auth_token, private_url, force, status, csrf_token, session, request_origin_url,
                request_origin_label)
     except SPyException as e:
         status.update(str(e), Status.FAILURE)
         raise
 
-    user_string = session.user.username
-    user_profile = ''
-    if session.user.first_name:
-        user_profile = session.user.first_name
-    if session.user.last_name:
-        user_profile += ' ' + session.user.last_name
-    if session.user.is_admin:
-        user_profile += ' [Admin]'
-    if len(user_profile) > 0:
-        user_string += ' (%s)' % user_profile.strip()
-
-    message = f'Logged in to <strong>{session.public_url}</strong> successfully as <strong>{user_string}</strong>.\n'
-
-    message += (f'Seeq Server Version: <strong>{spy.server_version}</strong>\n'
-                f'Seeq SDK Module Version: <strong>{sdk.__version__}</strong> @ {os.path.dirname(sdk.__file__)}\n'
-                f'Seeq SPy Module Version: <strong>{spy.__version__}</strong> @ {os.path.dirname(spy.__file__)}')
-
-    status.update(message, Status.SUCCESS)
+    status.update(session.get_info(html=True), Status.SUCCESS)
 
 
 def _login(username, password, access_key, url, directory, ignore_ssl_errors, proxy, credentials_file, auth_token,
            private_url, force, status, csrf_token, session: Session, request_origin_url=None,
            request_origin_label=None):
     if access_key and username:
         raise SPyValueError('"username" argument must be omitted when supplying "access_key" argument')
@@ -241,14 +228,26 @@
         validate_data_lab_license(session)
 
         users_api = UsersApi(session.client)
         session.user = users_api.get_me()
 
         folders_api = FoldersApi(session.client)
 
+        default_request_origin = _retrieve_default_request_origin(session)
+        if default_request_origin is not None:
+            if request_origin_label is None:
+                request_origin_label = default_request_origin.label
+            if request_origin_url is None:
+                request_origin_url = default_request_origin.url
+
+        if request_origin_label is not None:
+            session.request_origin_label = request_origin_label
+        if request_origin_url is not None:
+            session.request_origin_url = request_origin_url
+
         # noinspection PyBroadException
         try:
             session.corporate_folder = folders_api.get_folder(folder_id='corporate')
         except BaseException:
             # This can happen in cases where the user does not have access rights to the Corporate folder
             session.corporate_folder = None
 
@@ -281,16 +280,20 @@
             session.client_configuration.proxy = os.environ['HTTP_PROXY']
     elif proxy is not None:
         session.client_configuration.proxy = proxy
 
     _client = ApiClient(api_client_url, configuration=session.client_configuration)
     if _datalab.is_datalab_api():
         _client.set_default_header('x-sq-origin', 'Add-on')
+    elif _datalab.is_executor():
+        _client.set_default_header('x-sq-origin', 'Data Lab (Job)')
+    elif _datalab.is_datalab():
+        _client.set_default_header('x-sq-origin', 'Data Lab (Interactive)')
     else:
-        _client.set_default_header('x-sq-origin', 'Data Lab')
+        _client.set_default_header('x-sq-origin', 'SPy (Standalone)')
 
     auth_api = AuthApi(_client)
     directories = dict()
     try:
         auth_providers_output = auth_api.get_auth_providers()  # type: AuthProvidersOutputV1
     except MaxRetryError as e:
         if isinstance(e.reason, SSLError):
@@ -393,45 +396,14 @@
 
     # Now that we have succeeded, set all the session variables
     session.client = _client
     session.https_verify_ssl = not ignore_ssl_errors
     session.https_key_file = key_file
     session.https_cert_file = cert_file
 
-    # Now that we are logged in, retrieve path and url for data consumption
-    if ((_datalab.is_datalab() or _datalab.is_executor())
-            and not _datalab.is_datalab_api()
-            and request_origin_url is None
-            and request_origin_label is None):
-        # noinspection PyBroadException
-        try:
-            if _datalab.is_executor():
-                project_name = os.environ.get('SEEQ_PROJECT_NAME', '')
-                file_path = os.environ.get('SEEQ_SDL_FILE_PATH', '')
-                project_url = _datalab.get_data_lab_project_url(use_private_url=False)
-                notebook_url = f"{project_url}/notebooks/{file_path}"
-                request_origin_label = f"[Scheduled] {project_name} - {file_path}"
-                request_origin_url = quote(urlparse(notebook_url).path)
-            else:
-                notebook_url = _datalab.get_notebook_url(session)
-                request_origin_url = quote(urlparse(notebook_url).path)
-
-                project_name = _datalab.get_data_lab_project_name(session)
-                file_path = notebook_url.split('notebooks/', 1)[1]
-                request_origin_label = project_name + " - " + file_path
-        except BaseException:
-            pass
-
-    if request_origin_label is not None:
-        if is_datalab_functions_project() and not request_origin_label.startswith("[Data Lab Functions]"):
-            request_origin_label = f"[Data Lab Functions] {request_origin_label}"
-        _client.set_default_header('x-sq-origin-label', request_origin_label)
-    if request_origin_url is not None:
-        _client.set_default_header('x-sq-origin-url', request_origin_url)
-
 
 @Status.handle_keyboard_interrupt()
 def logout(quiet=None, status=None, session: Session = None):
     """
     Logs you out of your current session.
 
     Parameters
@@ -1093,7 +1065,39 @@
         # Before ~ March 2020, users commonly accessed spy._login.client when they wanted to leverage the SPy login
         # in their use of SDK functions.
         util.deprecation_warning("Use of spy._login.client deprecated, use spy.client instead")
         return spy.client
     else:
         # fallback to default module attribute access
         raise AttributeError
+
+
+@dataclass
+class RequestOrigin:
+    label: Optional[str]
+    url: Optional[str]
+
+
+def _retrieve_default_request_origin(session: Session) -> Optional[RequestOrigin]:
+    if not ((_datalab.is_datalab() or _datalab.is_executor()) and not _datalab.is_datalab_api()):
+        return None
+
+    # noinspection PyBroadException
+    try:
+        if _datalab.is_executor():
+            project_name = os.environ.get('SEEQ_PROJECT_NAME', '')
+            file_path = os.environ.get('SEEQ_SDL_FILE_PATH', '')
+            project_url = _datalab.get_data_lab_project_url(use_private_url=False)
+            notebook_url = f"{project_url}/notebooks/{file_path}"
+            request_origin_label = f"[Scheduled] {project_name} - {file_path}"
+            request_origin_url = quote(urlparse(notebook_url).path)
+        else:
+            notebook_url = _datalab.get_notebook_url(session)
+            request_origin_url = quote(urlparse(notebook_url).path)
+
+            project_name = _datalab.get_data_lab_project_name(session)
+            file_path = notebook_url.split('notebooks/', 1)[1]
+            request_origin_label = project_name + " - " + file_path
+
+        return RequestOrigin(label=request_origin_label, url=request_origin_url)
+    except BaseException:
+        return None
```

### Comparing `seeq-spy-189.3/seeq/spy/_metadata.py` & `seeq-spy-189.9/seeq/spy/_metadata.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/_metadata_push_results.py` & `seeq-spy-189.9/seeq/spy/_metadata_push_results.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/_plot.py` & `seeq-spy-189.9/seeq/spy/_plot.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/_pull.py` & `seeq-spy-189.9/seeq/spy/_pull.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from seeq import spy
 from seeq.sdk import *
 from seeq.spy import _common
 from seeq.spy import _login
 from seeq.spy._errors import *
 from seeq.spy._redaction import request_safely, safely
 from seeq.spy._session import Session
-from seeq.spy._status import Status
+from seeq.spy._status import Status, Usage
 
 ENUM_REGEX = r'ENUM{{(\d+)\|(.+?)}}'
 ENUM_PATTERN = re.compile(ENUM_REGEX)
 
 
 @Status.handle_keyboard_interrupt()
 def pull(items, *, start=None, end=None, grid='15min', header='__auto__', group_by=None, shape='auto',
@@ -353,14 +353,15 @@
 
     status_columns = [c for c in ['ID', 'Path', 'Asset', 'Name'] if c in items]
 
     status.df = items[status_columns].copy()
     status.df['Time'] = 0
     status.df['Count'] = 0
     status.df['Pages'] = 0
+    status.df['Data Processed'] = Usage()
     status.df['Result'] = 'Pulling'
 
     query_df = items  # type: pd.DataFrame
     output = types.SimpleNamespace(df=pd.DataFrame())
     at_least_one_signal = len(query_df[query_df['Type'].str.endswith('Signal', na=False)]) > 0
     at_least_one_asset = len(query_df[query_df['Type'].str.endswith('Asset', na=False)]) > 0
     calculation_is_signal = False
@@ -539,29 +540,29 @@
 
     row = query_df.loc[row_index]
 
     if phase == 'signals' and not _common.present(row, 'ID'):
         status.df.at[row_index, 'Result'] = 'No "ID" column - skipping'
         return None
 
-    item_id, item_name, item_type = _get_item_details(session, header, row)
+    item_id, item_name, item_type = _get_item_details(session, header, row, query_df)
 
     calculation_to_use = calculation
     if item_type == 'Asset':
         # If we're pulling assets, then we're actually pulling a calculated item (signal, condition or scalar) that
         # has been swapped to that asset. So use the swap API to find the appropriate item and then use that item's
         # ID instead of the asset's ID. Everything else just works the same as if the user had specified the swap
         # item directly.
         @request_safely(action_description=f'find swapped calculations below asset "{item_name}" {item_id}',
                         status=status,
                         default_value=(item_id, item_type, calculation_to_use))
         def _request_swap_items(_item_id, _item_type, _calculation_to_use):
             swap_input = SwapInputV1()
             swap_input.swap_in = _item_id
-            calc_item_id, _, _item_type = _get_item_details(session, header, calculation)
+            calc_item_id, _, _item_type = _get_item_details(session, header, calculation, query_df)
 
             item_dependency_output = items_api.get_formula_dependencies(id=calc_item_id)  # type: ItemDependencyOutputV1
 
             unique_assets = set(dep.ancestors[-1].id
                                 for dep in item_dependency_output.dependencies
                                 if len(dep.ancestors) > 0)
 
@@ -639,57 +640,62 @@
     timer = _common.timer_start()
     capsule_count = 0
     current_start = pd_start.value
     offset = 0
     page_count = 0
     indices_to_update = {row_index}
 
-    def _update_status_rows(_message, _capsule_count, _page_count):
+    def _update_status_rows(_message, _capsule_count, _page_count, _usage):
         for _row_index_to_update in indices_to_update:
             status.send_update(_row_index_to_update, {
                 'Result': _message,
                 'Count': _capsule_count,
                 'Pages': _page_count,
-                'Time': _common.timer_elapsed(timer)
+                'Time': _common.timer_elapsed(timer),
+                'Data Processed': _usage
             })
 
+    usage = Usage()
     while True:
         # When we want capsule summary statistics, fetch as a capsule table
         if shape == 'capsules' and at_least_one_signal:
             if calculation_to_use is not None:
                 raise SPyRuntimeError("If shape='capsules' and at least one signal is present, calculation "
                                       "argument cannot be supplied")
 
-            this_capsule_count, next_start, result_df = \
+            this_capsule_count, next_start, result_df, http_headers = \
                 _pull_condition_as_a_table(session, capsule_properties, current_start, query_df, item_id, item_name,
                                            header, offset, pd_end, tz, result_df, column_names, indices_to_update)
         else:
-            this_capsule_count, next_start, result_df = _pull_condition_via_formula_api(
+            this_capsule_count, next_start, result_df, http_headers = _pull_condition_via_formula_api(
                 session, calculation_to_use, shape, capsule_properties, current_start,
                 index_to_use, item_id, item_name, offset, pd_end, tz, result_df, column_names)
 
         # Note that capsule_count here can diverge from the exact count in the output due to pagination
         capsule_count += this_capsule_count
 
+        usage.add(http_headers)
+
         page_count += 1
 
         if this_capsule_count < session.options.pull_page_size:
             break
 
         if next_start == current_start:
             # This can happen if the page is full of capsules that all have the same start time
             offset += session.options.pull_page_size
         else:
             offset = 0
 
         current_start = next_start
 
-        _update_status_rows(f'Pulling {_common.convert_to_timestamp(current_start, tz)}', capsule_count, page_count)
+        _update_status_rows(f'Pulling {_common.convert_to_timestamp(current_start, tz)}', capsule_count, page_count,
+                            usage)
 
-    _update_status_rows(f'Success', capsule_count, page_count)
+    _update_status_rows(f'Success', capsule_count, page_count, usage)
 
     return RowResult(row_index, column_names, result_df)
 
 
 def _is_capsule_dupe(result_df, item_name, pd_capsule_start, pd_capsule_end):
     return 'Condition' in result_df and \
         'Capsule Start' in result_df and \
@@ -798,28 +804,28 @@
 
             if not pd.isna(capsule_start) and capsule_start > next_start:
                 next_start = capsule_start
 
         result_df = (pd.concat([result_df, pd.DataFrame(capsule_dict_list)])
                      if len(result_df) != 0 else pd.DataFrame(capsule_dict_list))
 
-    return len(capsules_output['capsules']), next_start, result_df
+    return len(capsules_output['capsules']), next_start, result_df, http_headers
 
 
 def _build_limit_fragment(offset, limit):
     start_row = offset + 1  # Table object is 1-based, not 0
     end_row = start_row + limit
     return f'.limit({start_row}, {end_row})'
 
 
 def _build_stat_formula_fragment_and_update_parameters(session: Session, signals_df, header, parameters,
-                                                       indices_to_update):
+                                                       indices_to_update, query_df):
     signal_id_to_stats = defaultdict(list)
     for signal_index, signal_row in signals_df.iterrows():
-        signal_item_id, signal_item_name, signal_item_type = _get_item_details(session, header, signal_row)
+        signal_item_id, signal_item_name, signal_item_type = _get_item_details(session, header, signal_row, query_df)
         statistic = signal_row['Statistic'] if 'Statistic' in signal_row else 'average'
 
         stat_formula = _common.statistic_to_aggregation_function(statistic, allow_condition_stats=False).split('(')[0]
         stat_formula = stat_formula + '()'  # Some stats come back without the parenthesis, this forces it on each
         stat_header = f'{signal_item_name} ({statistic})'
 
         signal_id_to_stats[signal_item_id].append((stat_formula, stat_header))
@@ -860,15 +866,15 @@
     parameters = ['condition=%s' % item_id]
     capsule = f"capsule('{start_string}', '{end_string}')"
     group_segment = _build_group_segment(all_property_columns)
     limit_fragment = _build_limit_fragment(offset, session.options.pull_page_size)
     property_column_fragment = f'capsuleTable({capsule}, CapsuleBoundary.Overlap, {group_segment}, $condition)'
     sort_fragment = ".sort('Capsule ID', 'inv, asc', 'Condition Id', 'asc', 'Capsule SortKey', 'asc')"
     stat_fragment, parameters, stat_headers = _build_stat_formula_fragment_and_update_parameters(
-        session, signals_df, header, parameters, indices_to_update)
+        session, signals_df, header, parameters, indices_to_update, query_df)
     formula = property_column_fragment + stat_fragment + sort_fragment + limit_fragment
     limit = session.options.pull_page_size
 
     formula_run_output: dict
     formula_run_output, _, http_headers = formulas_api.run_formula_with_http_info(
         formula=formula,
         parameters=parameters,
@@ -919,28 +925,29 @@
 
         if not pd.isna(capsule_start) and capsule_start > next_start:
             next_start = capsule_end
 
     formula_result_df = (pd.concat([result_df, pd.DataFrame(capsule_df_rows)])
                          if len(result_df) != 0 else pd.DataFrame(capsule_df_rows))
 
-    return len(formula_table), next_start, formula_result_df
+    return len(formula_table), next_start, formula_result_df, http_headers
 
 
 def _pull_signal(session: Session, formula, parameters, item_id, item_name, pd_start, pd_end, tz,
                  status: Status = None, row_index=None, bounding_values=False, invalid_values_as=np.nan,
                  enums_as='string'):
     formulas_api = FormulasApi(session.client)
 
     # noinspection PyBroadException
     series = None
     timer = _common.timer_start()
     current_start = pd_start
     last_key = 0
     page_count = 0
+    usage = Usage()
 
     while True:
         start_string = '%d ns' % current_start.value
         end_string = '%d ns' % pd_end.value
         formula_run_output: dict
         formula_run_output, status_code, http_headers = formulas_api.run_formula_with_http_info(
             formula=formula,
@@ -950,14 +957,16 @@
             offset=0,
             limit=session.options.pull_page_size,
 
             # It's about 300% faster to process the signal data as json - see CRAB-33451
             _response_type='json'
         )
 
+        usage.add(http_headers)
+
         if not _common.present(formula_run_output, 'samples'):
             # noinspection PyStringFormat
             raise SPyRuntimeError('formula_run_output.samples is None.\n'
                                   'status_code: %d\nformula: %s\nparameters: %s\n'
                                   'start: %s\nend:%s\n'
                                   'formula_run_output:\n%s' %
                                   (status_code, formula, parameters,
@@ -1010,25 +1019,27 @@
             current_start = time_index[-1]
 
         if status is not None:
             status.send_update(row_index, {
                 'Result': f'Pulling: {current_start}',
                 'Count': len(series),
                 'Pages': page_count,
-                'Time': _common.timer_elapsed(timer)
+                'Time': _common.timer_elapsed(timer),
+                'Data Processed': usage
             })
 
     series = series.fillna(invalid_values_as)
 
     if status is not None:
         status.send_update(row_index, {
             'Result': 'Success',
             'Count': len(series),
             'Pages': page_count,
-            'Time': _common.timer_elapsed(timer)
+            'Time': _common.timer_elapsed(timer),
+            'Data Processed': usage
         })
 
     return RowResult(row_index, {item_id: [item_name]}, pd.DataFrame({item_name: series}))
 
 
 def _sanitize_pi_enums(value, enums_as):
     if enums_as is None:
@@ -1045,20 +1056,23 @@
     return int(match.group(1)), match.group(2)
 
 
 def _pull_scalar(session: Session, formula, parameters, row_index, item_id, item_name, index_to_use, invalid_values_as,
                  status: Status):
     formulas_api = FormulasApi(session.client)
     timer = _common.timer_start()
+    usage = Usage()
 
     formula_run_output, _, http_headers = formulas_api.run_formula_with_http_info(
-        formula=formula,
-        parameters=parameters)  # type: FormulaRunOutputV1
+        formula=formula, parameters=parameters)
+
+    usage.add(http_headers)
 
-    status.send_update(row_index, {'Result': 'Success', 'Count': 1, 'Time': _common.timer_elapsed(timer)})
+    status.send_update(row_index, {'Result': 'Success', 'Count': 1, 'Time': _common.timer_elapsed(timer),
+                                   'Data Processed': usage})
 
     if len(index_to_use) == 0:
         index_to_use = pd.Series([0])
 
     result_df = pd.DataFrame(index=index_to_use)
     value = invalid_values_as if formula_run_output.scalar.value is None else formula_run_output.scalar.value
     result_df[item_name] = value
@@ -1068,15 +1082,15 @@
 class RowResult:
     def __init__(self, row_index, column_names, result):
         self.row_index = row_index
         self.column_names = column_names
         self.result = result
 
 
-def _get_item_details(session: Session, header, row):
+def _get_item_details(session: Session, header, row, query_df):
     # This is a somewhat complex function that tries its best to pick a column header (item_name) for the output
     # DataFrame by either honoring the user's "header" argument or auto-picking something that makes sense.
 
     items_api = ItemsApi(session.client)
 
     item_id = _common.get(row, 'ID')
 
@@ -1095,16 +1109,18 @@
         item_name = _common.get(row, header)
     else:
         if not item:
             item = items_api.get_item_and_all_properties(id=item_id)  # type: ItemOutputV1
 
         item_name = ''
         if header == '__auto__' and _common.present(row, 'Path'):
+            old_asset_format = (hasattr(query_df, 'spy') and hasattr(query_df.spy, 'old_asset_format') and
+                                query_df.spy.old_asset_format)
             item_name = _common.get(row, 'Path') + ' >> '
-            if item_type != 'Asset' and _common.present(row, 'Asset'):
+            if (item_type != 'Asset' or old_asset_format) and _common.present(row, 'Asset'):
                 item_name += _common.get(row, 'Asset') + ' >> '
 
         if header in ['__auto__', 'Name']:
             item_name += item.name
         elif header == 'Description':
             item_name += item.description
         else:
```

### Comparing `seeq-spy-189.3/seeq/spy/_push.py` & `seeq-spy-189.9/seeq/spy/_push.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/_redaction.py` & `seeq-spy-189.9/seeq/spy/_redaction.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/_search.py` & `seeq-spy-189.9/seeq/spy/_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -453,14 +453,19 @@
                                                               quiet=context.status.quiet)
         queries = worksheet.display_items.to_dict(orient='records')
         context.comparison = '=='
     else:
         queries = [query]
         context.comparison = '~='
 
+    # Handle the case where the user provides a lower-case ID (CRAB-38168)
+    for query in queries:
+        if _common.present(query, 'ID'):
+            query['ID'] = query['ID'].upper()
+
     context.status.df = pd.DataFrame(queries)
     context.status.df['Time'] = 0
     context.status.df['Count'] = 0
     context.status.df['Pages'] = 0
     context.status.df['Result'] = 'Queued'
     context.status.update('Initializing', Status.RUNNING)
```

### Comparing `seeq-spy-189.3/seeq/spy/_session.py` & `seeq-spy-189.9/seeq/spy/_session.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from __future__ import annotations
 
 import os
+import re
 import textwrap
 from dataclasses import dataclass
 from typing import Optional, List
 
 import pytz
 import requests
 from dateutil.tz import tz
 
-from seeq import spy
+from seeq import spy, sdk
 from seeq.sdk import *
 from seeq.sdk.configuration import ClientConfiguration
 from seeq.spy import _url, _common, _datalab, _errors
+from seeq.spy._datalab import is_datalab_functions_project
 from seeq.spy._errors import *
 
 SEEQ_SDK_RETRY_TIMEOUT_IN_SECONDS_ENV_VAR_NAME = 'SEEQ_SDK_RETRY_TIMEOUT_IN_SECONDS'
 DEFAULT_REQUESTS_TIMEOUT = 90
 
 
 @dataclass(repr=False)
@@ -54,28 +56,59 @@
         self.options = options if options is not None else Options(self.client_configuration)
 
         # We have this mechanism so that test_run_notebooks() is able to increase the timeout for the child kernels
         if Session.get_global_sdk_retry_timeout_in_seconds() is not None:
             self.options.retry_timeout_in_seconds = Session.get_global_sdk_retry_timeout_in_seconds()
 
     def __repr__(self):
-        if not self.client:
-            return 'Not logged in'
-        url_part = self.public_url
-        if self.private_url != self.public_url:
-            url_part += f' ({self.private_url})'
-        return f'{url_part} as {self.user.name} ({self.user.username})'
+        return self.get_info()
 
     def __getstate__(self):
         # We can only pickle certain members. This has to mirror __setstate__().
         return self.options
 
     def __setstate__(self, state):
         self.options = state
 
+    def get_info(self, *, html: bool = False) -> str:
+        if self.client:
+            url_part = self.public_url
+            if self.private_url != self.public_url:
+                url_part += f' ({self.private_url})'
+            info = f'Logged in to <strong>{url_part}</strong> as <strong>{self.user_string}</strong>.\n'
+            info += f'Seeq Server Version: <strong>{spy.server_version}</strong>\n'
+        else:
+            info = 'Not logged in.\n'
+
+        info += (f'Seeq SDK Module Version: <strong>{sdk.__version__}</strong> @ {os.path.dirname(sdk.__file__)}\n'
+                 f'Seeq SPy Module Version: <strong>{spy.__version__}</strong> @ {os.path.dirname(spy.__file__)}')
+
+        if not html:
+            info = re.sub(r'<[^>]*?>', '', info)
+
+        return info
+
+    @property
+    def user_string(self) -> str:
+        if self.user is None:
+            return 'Not logged in.'
+
+        user_string = self.user.username
+        user_profile = ''
+        if self.user.first_name:
+            user_profile = self.user.first_name
+        if self.user.last_name:
+            user_profile += ' ' + self.user.last_name
+        if self.user.is_admin:
+            user_profile += ' [Admin]'
+        if len(user_profile) > 0:
+            user_string += ' (%s)' % user_profile.strip()
+
+        return user_string
+
     @staticmethod
     def validate(session):
         return spy.session if session is None else session
 
     @staticmethod
     def set_global_sdk_retry_timeout_in_seconds(timeout: Optional[int]):
         """
@@ -274,14 +307,57 @@
     def options(self, value):
         self._options = value
 
     @property
     def requests(self):
         return SqAuthRequests(self)
 
+    @property
+    def request_origin_label(self) -> str:
+        """
+        Used for tracking Data Consumption. If supplied, this label will be added as a header to all requests from
+        the logged in user. Data Lab will automatically provide a default that you can choose to override.
+        """
+        return self.client.default_headers.get('x-sq-origin-label')
+
+    @request_origin_label.setter
+    def request_origin_label(self, value: str):
+        if self.client is None:
+            raise RuntimeError("Cannot set request_origin_label before logging in")
+
+        if value is None:
+            if 'x-sq-origin-label' in self.client.default_headers:
+                del self.client.default_headers['x-sq-origin-label']
+            return
+
+        if is_datalab_functions_project() and not value.startswith("[Data Lab Functions]"):
+            value = f"[Data Lab Functions] {value}"
+        self.client.set_default_header('x-sq-origin-label', value)
+
+    @property
+    def request_origin_url(self) -> str:
+        """
+        Used for tracking Data Consumption. If supplied, this label will be added as a header to all requests from
+        the logged in user. Data Lab will automatically provide a default that you can choose to override. If NOT in
+        Data Lab, supply a full URL that leads to the tool/plugin that is consuming data, if applicable.
+        """
+        return self.client.default_headers.get('x-sq-origin-url')
+
+    @request_origin_url.setter
+    def request_origin_url(self, value: str):
+        if self.client is None:
+            raise RuntimeError("Cannot set request_origin_url before logging in")
+
+        if value is None:
+            if 'x-sq-origin-url' in self.client.default_headers:
+                del self.client.default_headers['x-sq-origin-url']
+            return
+
+        self.client.set_default_header('x-sq-origin-url', value)
+
 
 class Options:
     _DEFAULT_SEARCH_PAGE_SIZE = 1000
     _DEFAULT_PULL_PAGE_SIZE = 1000000
     _DEFAULT_PUSH_PAGE_SIZE = 100000
     _DEFAULT_METADATA_PUSH_BATCH_SIZE = 1000
     _DEFAULT_MAX_CONCURRENT_REQUESTS = 8
```

### Comparing `seeq-spy-189.3/seeq/spy/_status.py` & `seeq-spy-189.9/seeq/spy/_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import pandas as pd
 from IPython.display import display, HTML
 
 from seeq.spy import _common, _datalab
 from seeq.spy._errors import *
 from seeq.spy._session import Session
+from seeq.spy._usage import Usage
 
 
 class Status:
     """
     Tracks the progress status of various SPy functions.
 
     Parameters
@@ -320,14 +321,16 @@
                 html += '<td style="vertical-align: top;">%s</td>' % index
                 for cell in row:
                     if isinstance(cell, datetime.timedelta):
                         hours, remainder = divmod(cell.seconds, 3600)
                         minutes, seconds = divmod(remainder, 60)
                         html += '<td style="vertical-align: top;">{:02}:{:02}:{:02}.{:02}</td>'.format(
                             int(hours), int(minutes), int(seconds), int((cell.microseconds + 5000) / 10000))
+                    elif isinstance(cell, Usage):
+                        html += f'<td style="text-align: right; vertical-align: top;">{cell}</td>'
                     else:
                         align = 'left' if isinstance(cell, str) else 'right'
                         html += '<td style="text-align: %s; vertical-align: top;">%s</td>' % \
                                 (align, Status._massage_cell(cell, links=True))
                 html += '</tr>'
 
             html += '</table>'
```

### Comparing `seeq-spy-189.3/seeq/spy/_swap.py` & `seeq-spy-189.9/seeq/spy/_swap.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/_upgrade.py` & `seeq-spy-189.9/seeq/spy/_upgrade.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/_url.py` & `seeq-spy-189.9/seeq/spy/_url.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/acl/_pull.py` & `seeq-spy-189.9/seeq/spy/acl/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/acl/_push.py` & `seeq-spy-189.9/seeq/spy/acl/_push.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/addons/_install.py` & `seeq-spy-189.9/seeq/spy/addons/_install.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/addons/_permissions.py` & `seeq-spy-189.9/seeq/spy/addons/_permissions.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/addons/_search.py` & `seeq-spy-189.9/seeq/spy/addons/_search.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/addons/_uninstall.py` & `seeq-spy-189.9/seeq/spy/addons/_uninstall.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/assets/_brochure.py` & `seeq-spy-189.9/seeq/spy/assets/_brochure.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/assets/_build.py` & `seeq-spy-189.9/seeq/spy/assets/_build.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/assets/_context.py` & `seeq-spy-189.9/seeq/spy/assets/_context.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/assets/_model.py` & `seeq-spy-189.9/seeq/spy/assets/_model.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/assets/_trees/_constants.py` & `seeq-spy-189.9/seeq/spy/assets/_trees/_constants.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/assets/_trees/_csv.py` & `seeq-spy-189.9/seeq/spy/assets/_trees/_csv.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/assets/_trees/_match.py` & `seeq-spy-189.9/seeq/spy/assets/_trees/_match.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/assets/_trees/_pandas.py` & `seeq-spy-189.9/seeq/spy/assets/_trees/_pandas.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/assets/_trees/_path.py` & `seeq-spy-189.9/seeq/spy/assets/_trees/_path.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/assets/_trees/_properties.py` & `seeq-spy-189.9/seeq/spy/assets/_trees/_properties.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/assets/_trees/_pull.py` & `seeq-spy-189.9/seeq/spy/assets/_trees/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/assets/_trees/_tree.py` & `seeq-spy-189.9/seeq/spy/assets/_trees/_tree.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/assets/_trees/_utils.py` & `seeq-spy-189.9/seeq/spy/assets/_trees/_utils.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/assets/_trees/_validate.py` & `seeq-spy-189.9/seeq/spy/assets/_trees/_validate.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/assets/brochure.html` & `seeq-spy-189.9/seeq/spy/assets/brochure.html`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Administration/User Migration.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Administration/User Migration.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999886156648452%*

 * *Differences: {"'cells'": "{8: {'source': {insert: [(42, '        pdf_response = requests.get(pdf_url, "*

 * *            "cookies=cookies, headers=headers)\\n')], delete: [42]}}}"}*

```diff
@@ -199,15 +199,15 @@
                 "    headers = {\n",
                 "        'Content-Type': 'application/json',\n",
                 "        'x-sq-csrf': spy.client.csrf_token\n",
                 "    }\n",
                 "    try:\n",
                 "        response = requests.post(screenshots_url, data=json.dumps(pdf_specs), cookies=cookies, headers=headers)\n",
                 "        pdf_url = f'{base_url}{response.headers[\"Location\"]}'\n",
-                "        pdf_response = requests.get(pdf_url)\n",
+                "        pdf_response = requests.get(pdf_url, cookies=cookies, headers=headers)\n",
                 "        filename = pathlib.PurePosixPath(pdf_url).name\n",
                 "        attachment = MIMEApplication(\n",
                 "            pdf_response.content,\n",
                 "            Name=filename\n",
                 "        )\n",
                 "        attachment['Content-Disposition'] = f'attachment; filename=\"{filename}\"'\n",
                 "        return attachment\n",
```

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Command Reference.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Command Reference.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Data Lab Visualizations.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Data Lab Visualizations.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Support Files/Example Export.zip` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Support Files/Example Export.zip`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Tutorial.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Version Considerations.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Version Considerations.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975484360410831%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(4, 'For Seeq R59 and earlier, both the Seeq SDK and Seeq "*

 * *            'SPy Module were distributed in a single PyPI package called '*

 * *            '**[seeq](https://pypi.org/project/seeq/)**. It had a versioning scheme that was an '*

 * *            'amalgamation of both the Seeq SDK version (which is tied directly to the Seeq Server '*

 * *            'version it supports) and the SPy version (which is independent of the Seeq Server '*

 * *            "version). It took the following […]*

```diff
@@ -13,23 +13,23 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Packaging\n",
                 "\n",
                 "### Seeq R59 and Earlier\n",
                 "\n",
-                "For Seeq R59 and earlier, both the Seeq SDK and Seeq SPy Module were distributed in a single PyPI package called **seeq**. It had a versioning scheme that was an amalgamation of both the Seeq SDK version (which is tied directly to the Seeq Server version it supports) and the SPy version (which is independent of the Seeq Server version). It took the following form:\n",
+                "For Seeq R59 and earlier, both the Seeq SDK and Seeq SPy Module were distributed in a single PyPI package called **[seeq](https://pypi.org/project/seeq/)**. It had a versioning scheme that was an amalgamation of both the Seeq SDK version (which is tied directly to the Seeq Server version it supports) and the SPy version (which is independent of the Seeq Server version). It took the following form:\n",
                 "\n",
                 "**a.b.c.F.G**\n",
                 "\n",
                 "For example, `seeq` package version [59.1.2.185.2](https://pypi.org/project/seeq/59.1.2.185.2/) supports Seeq Server version R59 and includes SPy version 185.2.\n",
                 "\n",
                 "### Seeq R60 and Later\n",
                 "\n",
-                "For Seeq R60 and later, the Seeq SDK is distributed in the  PyPI package **seeq** and the Seeq SPy Module is distributed in a separate PyPI package called **seeq-spy**. The **seeq** package versioning scheme is tied directly to the Seeq Server version it supports and the **seeq-spy** package version is independent of the Seeq Server version.\n",
+                "For Seeq R60 and later, the Seeq SDK is distributed in the  PyPI package **[seeq](https://pypi.org/project/seeq/)** and the Seeq SPy Module is distributed in a separate PyPI package called **[seeq-spy](https://pypi.org/project/seeq-spy/)**. The **seeq** package versioning scheme is tied directly to the Seeq Server version it supports and the **seeq-spy** package version is independent of the Seeq Server version.\n",
                 "\n",
                 "The two packages can be upgraded independently. However, when using Data Lab, then the user should _only_ upgrade the SPy package and allow the SDK package to be managed directly by Data Lab."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -43,25 +43,62 @@
                 "```"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "## Displaying Version Information\n",
+                "\n",
+                "If you'd like to check what version you're running with, just print out the current session information, like so:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "metadata": {
+                "keep_output_in_docs": true
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "Not logged in.\n",
+                            "Seeq SDK Module Version: 63.0.0 @ C:\\GitHub\\crab\\sdk\\pypi\\seeq\\sdk\n",
+                            "Seeq SPy Module Version: 189.1 @ C:\\GitHub\\crab\\sdk\\pypi\\seeq\\spy"
+                        ]
+                    },
+                    "execution_count": 4,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "from seeq import spy\n",
+                "\n",
+                "spy.session"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "## Checking for a Sufficient Version\n",
                 "\n",
                 "If you are writing a reusable notebook or script, or you are writing an add-on, you may wish to include a _version check_ in your code. Version checks are notoriously difficult to code correctly, so the `spy.utils` module includes some convenience functions to do the hard work for you.\n",
                 "\n",
                 "Here are some examples:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
-            "metadata": {},
+            "metadata": {
+                "keep_output_in_docs": true
+            },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Logged in to <strong>http://localhost:34216</strong> successfully as <strong>agent_api_key (Mark Derbecker)</strong>.<br>Seeq Server Version: <strong>R61.0.0-SNAPSHOT</strong><br>Seeq SDK Module Version: <strong>61.0.0</strong> @ C:\\GitHub\\crab\\sdk\\pypi\\seeq\\sdk<br>Seeq SPy Module Version: <strong>185.3</strong> @ C:\\GitHub\\crab\\sdk\\pypi\\seeq\\spy</div>"
                         ],
                         "text/plain": [
@@ -283,13 +320,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.8"
+            "version": "3.8.10"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/Workbook Templates.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/Workbook Templates.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/spy.acl.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/spy.acl.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/spy.jobs.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/spy.jobs.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/spy.login.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/spy.login.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/spy.pull.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/spy.pull.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9896164962309899%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/html\': [\'<div style="background-color: '*

 * *            '#EEFFEE;color:black; text-align: left;">Logged in to '*

 * *            '<strong>http://localhost:34216</strong> as <strong>agent_api_key</strong>.<br>Seeq '*

 * *            'Server Version: <strong>R63.0.0-SNAPSHOT</strong><br>Seeq SDK Module Version: '*

 * *            '<strong>63.0.0</strong> @ C:\\\\GitHub\\\\crab\\\\sdk\\\\pypi\\\\seeq\\\\sdk<br>Seeq '*

 * *            'SPy Module Version: <strong>189.3</strong>  […]*

```diff
@@ -17,15 +17,15 @@
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Logged in to <strong>http://localhost:34216</strong> successfully as <strong>agent_api_key</strong>.<br>Seeq Server Version: <strong>R57.0.0-SNAPSHOT</strong><br>Seeq Python Module Version: <strong>57.0.0.182.42</strong></div>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Logged in to <strong>http://localhost:34216</strong> as <strong>agent_api_key</strong>.<br>Seeq Server Version: <strong>R63.0.0-SNAPSHOT</strong><br>Seeq SDK Module Version: <strong>63.0.0</strong> @ C:\\GitHub\\crab\\sdk\\pypi\\seeq\\sdk<br>Seeq SPy Module Version: <strong>189.3</strong> @ C:\\GitHub\\crab\\sdk\\pypi\\seeq\\spy</div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -66,15 +66,15 @@
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Query successful</div><table style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Path</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">Example >> Cooling Tower 1 >> Area A</td><td style=\"text-align: left; vertical-align: top;\">Compressor</td><td style=\"vertical-align: top;\">00:00:00.06</td><td style=\"text-align: right; vertical-align: top;\">2</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Query successful</div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">Path</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">Example >> Cooling Tower 1 >> Area A</td><td style=\"text-align: left; vertical-align: top;\">Compressor</td><td style=\"vertical-align: top;\">00:00:00.04</td><td style=\"text-align: right; vertical-align: top;\">2</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -110,27 +110,27 @@
                             "      <th>Datasource Name</th>\n",
                             "      <th>Archived</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>FC68ACEF-1CCD-47DF-987D-184F3C24AC76</td>\n",
+                            "      <td>0EE22861-3FA5-F900-8703-4A2E6D5B0F14</td>\n",
                             "      <td>Example &gt;&gt; Cooling Tower 1</td>\n",
                             "      <td>Area A</td>\n",
                             "      <td>Compressor Power</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>kW</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>47942D39-96F8-4298-B8F5-6DCA2D870425</td>\n",
+                            "      <td>0EE22861-3FE7-77B0-953A-6D12E9970A6F</td>\n",
                             "      <td>Example &gt;&gt; Cooling Tower 1</td>\n",
                             "      <td>Area A</td>\n",
                             "      <td>Compressor Stage</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>string</td>\n",
                             "      <td>Example Data</td>\n",
@@ -138,16 +138,16 @@
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                                     ID                        Path   Asset  \\\n",
-                            "0  FC68ACEF-1CCD-47DF-987D-184F3C24AC76  Example >> Cooling Tower 1  Area A   \n",
-                            "1  47942D39-96F8-4298-B8F5-6DCA2D870425  Example >> Cooling Tower 1  Area A   \n",
+                            "0  0EE22861-3FA5-F900-8703-4A2E6D5B0F14  Example >> Cooling Tower 1  Area A   \n",
+                            "1  0EE22861-3FE7-77B0-953A-6D12E9970A6F  Example >> Cooling Tower 1  Area A   \n",
                             "\n",
                             "               Name  Description          Type Value Unit Of Measure  \\\n",
                             "0  Compressor Power          NaN  StoredSignal                    kW   \n",
                             "1  Compressor Stage          NaN  StoredSignal                string   \n",
                             "\n",
                             "  Datasource Name  Archived  \n",
                             "0    Example Data     False  \n",
@@ -179,15 +179,15 @@
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Pull successful from <strong>2019-01-01 00:00:00+00:00</strong> to <strong>2019-01-07 00:00:00+00:00</strong></div><table style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Path</td><td style=\"background-color: #EEFFEE; text-align: left;\">Asset</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">FC68ACEF-1CCD-47DF-987D-184F3C24AC76</td><td style=\"text-align: left; vertical-align: top;\">Example >> Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area A</td><td style=\"text-align: left; vertical-align: top;\">Compressor Power</td><td style=\"text-align: right; vertical-align: top;\">577</td><td style=\"vertical-align: top;\">00:00:00.07</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">47942D39-96F8-4298-B8F5-6DCA2D870425</td><td style=\"text-align: left; vertical-align: top;\">Example >> Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area A</td><td style=\"text-align: left; vertical-align: top;\">Compressor Stage</td><td style=\"text-align: right; vertical-align: top;\">577</td><td style=\"vertical-align: top;\">00:00:00.09</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pull successful from <strong>2019-01-01 00:00:00+00:00</strong> to <strong>2019-01-07 00:00:00+00:00</strong></div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Path</td><td style=\"background-color: #EEFFEE; text-align: left;\">Asset</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Data Processed</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">0EE22861-3FA5-F900-8703-4A2E6D5B0F14</td><td style=\"text-align: left; vertical-align: top;\">Example >> Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area A</td><td style=\"text-align: left; vertical-align: top;\">Compressor Power</td><td style=\"vertical-align: top;\">00:00:00.05</td><td style=\"text-align: right; vertical-align: top;\">577</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">69 KB</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">0EE22861-3FE7-77B0-953A-6D12E9970A6F</td><td style=\"text-align: left; vertical-align: top;\">Example >> Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area A</td><td style=\"text-align: left; vertical-align: top;\">Compressor Stage</td><td style=\"vertical-align: top;\">00:00:00.07</td><td style=\"text-align: right; vertical-align: top;\">577</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">69 KB</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -330,15 +330,15 @@
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Pull successful from <strong>2019-01-01 00:00:00-08:00</strong> to <strong>2019-01-07 00:00:00-08:00</strong></div><table style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Path</td><td style=\"background-color: #EEFFEE; text-align: left;\">Asset</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">FC68ACEF-1CCD-47DF-987D-184F3C24AC76</td><td style=\"text-align: left; vertical-align: top;\">Example >> Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area A</td><td style=\"text-align: left; vertical-align: top;\">Compressor Power</td><td style=\"text-align: right; vertical-align: top;\">577</td><td style=\"vertical-align: top;\">00:00:00.07</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">47942D39-96F8-4298-B8F5-6DCA2D870425</td><td style=\"text-align: left; vertical-align: top;\">Example >> Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area A</td><td style=\"text-align: left; vertical-align: top;\">Compressor Stage</td><td style=\"text-align: right; vertical-align: top;\">577</td><td style=\"vertical-align: top;\">00:00:00.06</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pull successful from <strong>2019-01-01 00:00:00-08:00</strong> to <strong>2019-01-07 00:00:00-08:00</strong></div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Path</td><td style=\"background-color: #EEFFEE; text-align: left;\">Asset</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Data Processed</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">0EE22861-3FA5-F900-8703-4A2E6D5B0F14</td><td style=\"text-align: left; vertical-align: top;\">Example >> Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area A</td><td style=\"text-align: left; vertical-align: top;\">Compressor Power</td><td style=\"vertical-align: top;\">00:00:00.04</td><td style=\"text-align: right; vertical-align: top;\">577</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">12 KB</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">0EE22861-3FE7-77B0-953A-6D12E9970A6F</td><td style=\"text-align: left; vertical-align: top;\">Example >> Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area A</td><td style=\"text-align: left; vertical-align: top;\">Compressor Stage</td><td style=\"vertical-align: top;\">00:00:00.04</td><td style=\"text-align: right; vertical-align: top;\">577</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">12 KB</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -532,15 +532,15 @@
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Pull successful from <strong>2019-01-01 12:00:00+00:00</strong> to <strong>2019-01-01 13:00:00+00:00</strong></div><table style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Path</td><td style=\"background-color: #EEFFEE; text-align: left;\">Asset</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">FC68ACEF-1CCD-47DF-987D-184F3C24AC76</td><td style=\"text-align: left; vertical-align: top;\">Example >> Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area A</td><td style=\"text-align: left; vertical-align: top;\">Compressor Power</td><td style=\"text-align: right; vertical-align: top;\">5</td><td style=\"vertical-align: top;\">00:00:00.01</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">47942D39-96F8-4298-B8F5-6DCA2D870425</td><td style=\"text-align: left; vertical-align: top;\">Example >> Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area A</td><td style=\"text-align: left; vertical-align: top;\">Compressor Stage</td><td style=\"text-align: right; vertical-align: top;\">5</td><td style=\"vertical-align: top;\">00:00:00.02</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pull successful from <strong>2019-01-01 12:00:00+00:00</strong> to <strong>2019-01-01 13:00:00+00:00</strong></div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Path</td><td style=\"background-color: #EEFFEE; text-align: left;\">Asset</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Data Processed</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">0EE22861-3FA5-F900-8703-4A2E6D5B0F14</td><td style=\"text-align: left; vertical-align: top;\">Example >> Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area A</td><td style=\"text-align: left; vertical-align: top;\">Compressor Power</td><td style=\"vertical-align: top;\">00:00:00.01</td><td style=\"text-align: right; vertical-align: top;\">5</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">80 B</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">0EE22861-3FE7-77B0-953A-6D12E9970A6F</td><td style=\"text-align: left; vertical-align: top;\">Example >> Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area A</td><td style=\"text-align: left; vertical-align: top;\">Compressor Stage</td><td style=\"vertical-align: top;\">00:00:00.01</td><td style=\"text-align: right; vertical-align: top;\">5</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">80 B</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -633,15 +633,15 @@
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Pull successful from <strong>2019-01-01 00:00:00+00:00</strong> to <strong>2019-01-01 03:00:00+00:00</strong></div><table style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">B817FE37-136B-4AD9-8064-7A40DE0ED3CE</td><td style=\"text-align: left; vertical-align: top;\">Area A_Temperature</td><td style=\"text-align: right; vertical-align: top;\">4</td><td style=\"vertical-align: top;\">00:00:00.02</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pull successful from <strong>2019-01-01 00:00:00+00:00</strong> to <strong>2019-01-01 03:00:00+00:00</strong></div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Data Processed</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">0EE22861-3EA7-EA80-8C51-AC8632AC9EA3</td><td style=\"text-align: left; vertical-align: top;\">Area A_Temperature</td><td style=\"vertical-align: top;\">00:00:00.03</td><td style=\"text-align: right; vertical-align: top;\">4</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">4 KB</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -729,15 +729,15 @@
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>C3CB3C68-35A4-453F-96A8-D2D570E22509</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/2D207275-CACB-413E-BD9D-A134589AD72C/workbook/C3CB3C68-35A4-453F-96A8-D2D570E22509/worksheet/77ACF254-40DF-4530-812A-CAD2495D0E2A\" target=\"_new\">http://localhost:34216/2D207275-CACB-413E-BD9D-A134589AD72C/workbook/C3CB3C68-35A4-453F-96A8-D2D570E22509/worksheet/77ACF254-40DF-4530-812A-CAD2495D0E2A</a></div>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>0EE22861-ABF7-60E0-98C7-650CB85547E5</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/0EE22861-AB73-7380-86F4-76CA140D72A0/workbook/0EE22861-ABF7-60E0-98C7-650CB85547E5/worksheet/0EE22861-AC69-ECD0-927E-CDB442643F0F\" target=\"_blank\">http://localhost:34216/0EE22861-AB73-7380-86F4-76CA140D72A0/workbook/0EE22861-ABF7-60E0-98C7-650CB85547E5/worksheet/0EE22861-AC69-ECD0-927E-CDB442643F0F</a></div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -763,50 +763,55 @@
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>Type</th>\n",
                             "      <th>Name</th>\n",
                             "      <th>Formula</th>\n",
                             "      <th>Formula Parameters</th>\n",
+                            "      <th>Scoped To</th>\n",
                             "      <th>Datasource Class</th>\n",
                             "      <th>Datasource ID</th>\n",
                             "      <th>Data ID</th>\n",
                             "      <th>ID</th>\n",
                             "      <th>Push Result</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>CalculatedSignal</td>\n",
                             "      <td>Dew Point</td>\n",
                             "      <td>$T - ((100 - $RH.setUnits(''))/5)</td>\n",
-                            "      <td>[RH=C767CC93-BF81-4041-B409-BAD058EF8281, T=94...</td>\n",
+                            "      <td>[RH=0EE22861-3E76-FD40-A8A7-FBA3AC8F34D9, T=0E...</td>\n",
+                            "      <td>0EE22861-ABF7-60E0-98C7-650CB85547E5</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[C3CB3C68-35A4-453F-96A8-D2D570E22509] {Signal...</td>\n",
-                            "      <td>4F8FD79B-3CE0-4586-8E28-25F61579595E</td>\n",
+                            "      <td>[0EE22861-ABF7-60E0-98C7-650CB85547E5] {Signal...</td>\n",
+                            "      <td>0EE22861-B26E-7540-AAD6-B42B4D29577A</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "               Type       Name                            Formula  \\\n",
                             "0  CalculatedSignal  Dew Point  $T - ((100 - $RH.setUnits(''))/5)   \n",
                             "\n",
-                            "                                  Formula Parameters Datasource Class  \\\n",
-                            "0  [RH=C767CC93-BF81-4041-B409-BAD058EF8281, T=94...    Seeq Data Lab   \n",
+                            "                                  Formula Parameters  \\\n",
+                            "0  [RH=0EE22861-3E76-FD40-A8A7-FBA3AC8F34D9, T=0E...   \n",
                             "\n",
-                            "   Datasource ID                                            Data ID  \\\n",
-                            "0  Seeq Data Lab  [C3CB3C68-35A4-453F-96A8-D2D570E22509] {Signal...   \n",
+                            "                              Scoped To Datasource Class  Datasource ID  \\\n",
+                            "0  0EE22861-ABF7-60E0-98C7-650CB85547E5    Seeq Data Lab  Seeq Data Lab   \n",
+                            "\n",
+                            "                                             Data ID  \\\n",
+                            "0  [0EE22861-ABF7-60E0-98C7-650CB85547E5] {Signal...   \n",
                             "\n",
                             "                                     ID Push Result  \n",
-                            "0  4F8FD79B-3CE0-4586-8E28-25F61579595E     Success  "
+                            "0  0EE22861-B26E-7540-AAD6-B42B4D29577A     Success  "
                         ]
                     },
                     "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -840,15 +845,15 @@
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Pull successful from <strong>2021-12-28 22:27:03.132122+00:00</strong> to <strong>2021-12-28 23:27:03.132122+00:00</strong></div><table style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Path</td><td style=\"background-color: #EEFFEE; text-align: left;\">Asset</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">2BA1346B-0776-4664-B4F4-B1BD0BECAD0E</td><td style=\"text-align: left; vertical-align: top;\">Example</td><td style=\"text-align: left; vertical-align: top;\">Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area A</td><td style=\"text-align: right; vertical-align: top;\">4</td><td style=\"vertical-align: top;\">00:00:00.24</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">6E419480-3466-461D-B220-982F52B36229</td><td style=\"text-align: left; vertical-align: top;\">Example</td><td style=\"text-align: left; vertical-align: top;\">Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area B</td><td style=\"text-align: right; vertical-align: top;\">4</td><td style=\"vertical-align: top;\">00:00:00.28</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">2</td><td style=\"text-align: left; vertical-align: top;\">C2DBA4CB-7E64-4AA5-924D-621E979B2E19</td><td style=\"text-align: left; vertical-align: top;\">Example</td><td style=\"text-align: left; vertical-align: top;\">Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area C</td><td style=\"text-align: right; vertical-align: top;\">4</td><td style=\"vertical-align: top;\">00:00:00.27</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">3</td><td style=\"text-align: left; vertical-align: top;\">5A896ADD-EB51-4999-BB31-76DC2E04461C</td><td style=\"text-align: left; vertical-align: top;\">Example</td><td style=\"text-align: left; vertical-align: top;\">Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area G</td><td style=\"text-align: right; vertical-align: top;\">4</td><td style=\"vertical-align: top;\">00:00:00.30</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">4</td><td style=\"text-align: left; vertical-align: top;\">46E64890-EE6C-4D73-9524-D546DE4D4013</td><td style=\"text-align: left; vertical-align: top;\">Example</td><td style=\"text-align: left; vertical-align: top;\">Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area H</td><td style=\"text-align: right; vertical-align: top;\">4</td><td style=\"vertical-align: top;\">00:00:00.29</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">5</td><td style=\"text-align: left; vertical-align: top;\">AEA9FB07-B7A3-4541-BBE0-D7F09809E6D3</td><td style=\"text-align: left; vertical-align: top;\">Example</td><td style=\"text-align: left; vertical-align: top;\">Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area I</td><td style=\"text-align: right; vertical-align: top;\">4</td><td style=\"vertical-align: top;\">00:00:00.28</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">6</td><td style=\"text-align: left; vertical-align: top;\">B3EE0043-B672-4BE0-92AB-CCB221920406</td><td style=\"text-align: left; vertical-align: top;\">Example</td><td style=\"text-align: left; vertical-align: top;\">Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area J</td><td style=\"text-align: right; vertical-align: top;\">4</td><td style=\"vertical-align: top;\">00:00:00.28</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">7</td><td style=\"text-align: left; vertical-align: top;\">5AB0DC87-2EAF-4E5C-A524-83068C54489A</td><td style=\"text-align: left; vertical-align: top;\">Example</td><td style=\"text-align: left; vertical-align: top;\">Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area K</td><td style=\"text-align: right; vertical-align: top;\">4</td><td style=\"vertical-align: top;\">00:00:00.28</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pull successful from <strong>2023-07-14 20:03:08.674244+00:00</strong> to <strong>2023-07-14 21:03:08.674244+00:00</strong></div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Path</td><td style=\"background-color: #EEFFEE; text-align: left;\">Asset</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Data Processed</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">0EE22861-4227-EA70-AE50-277D5424ECAF</td><td style=\"text-align: left; vertical-align: top;\">Example</td><td style=\"text-align: left; vertical-align: top;\">Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area A</td><td style=\"vertical-align: top;\">00:00:00.43</td><td style=\"text-align: right; vertical-align: top;\">4</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">1 KB</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">0EE22861-4222-EC50-B76E-43DA4010CBAF</td><td style=\"text-align: left; vertical-align: top;\">Example</td><td style=\"text-align: left; vertical-align: top;\">Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area B</td><td style=\"vertical-align: top;\">00:00:00.42</td><td style=\"text-align: right; vertical-align: top;\">4</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">1 KB</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">2</td><td style=\"text-align: left; vertical-align: top;\">0EE22861-4222-EC50-BD3E-B2C277D6B342</td><td style=\"text-align: left; vertical-align: top;\">Example</td><td style=\"text-align: left; vertical-align: top;\">Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area C</td><td style=\"vertical-align: top;\">00:00:00.44</td><td style=\"text-align: right; vertical-align: top;\">4</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">1 KB</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">3</td><td style=\"text-align: left; vertical-align: top;\">0EE22861-4225-7360-A238-3CADA4E414C0</td><td style=\"text-align: left; vertical-align: top;\">Example</td><td style=\"text-align: left; vertical-align: top;\">Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area G</td><td style=\"vertical-align: top;\">00:00:00.43</td><td style=\"text-align: right; vertical-align: top;\">4</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">1 KB</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">4</td><td style=\"text-align: left; vertical-align: top;\">0EE22861-4225-7360-9EF4-E53829169596</td><td style=\"text-align: left; vertical-align: top;\">Example</td><td style=\"text-align: left; vertical-align: top;\">Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area H</td><td style=\"vertical-align: top;\">00:00:00.41</td><td style=\"text-align: right; vertical-align: top;\">4</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">1 KB</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">5</td><td style=\"text-align: left; vertical-align: top;\">0EE22861-4222-EC50-8B1F-658033DF4A4E</td><td style=\"text-align: left; vertical-align: top;\">Example</td><td style=\"text-align: left; vertical-align: top;\">Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area I</td><td style=\"vertical-align: top;\">00:00:00.44</td><td style=\"text-align: right; vertical-align: top;\">4</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">1 KB</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">6</td><td style=\"text-align: left; vertical-align: top;\">0EE22861-4222-EC50-A8BA-D790277F0CD3</td><td style=\"text-align: left; vertical-align: top;\">Example</td><td style=\"text-align: left; vertical-align: top;\">Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area J</td><td style=\"vertical-align: top;\">00:00:00.43</td><td style=\"text-align: right; vertical-align: top;\">4</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">1 KB</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">7</td><td style=\"text-align: left; vertical-align: top;\">0EE22861-4222-EC50-B68C-A13D78401431</td><td style=\"text-align: left; vertical-align: top;\">Example</td><td style=\"text-align: left; vertical-align: top;\">Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area K</td><td style=\"vertical-align: top;\">00:00:00.44</td><td style=\"text-align: right; vertical-align: top;\">4</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">1 KB</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -882,109 +887,109 @@
                             "      <th>Example &gt;&gt; Cooling Tower 1 &gt;&gt; Area I</th>\n",
                             "      <th>Example &gt;&gt; Cooling Tower 1 &gt;&gt; Area J</th>\n",
                             "      <th>Example &gt;&gt; Cooling Tower 1 &gt;&gt; Area K</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th>2021-12-28 22:30:00+00:00</th>\n",
-                            "      <td>69.436828</td>\n",
-                            "      <td>64.729514</td>\n",
-                            "      <td>69.818953</td>\n",
-                            "      <td>79.693327</td>\n",
-                            "      <td>69.598924</td>\n",
-                            "      <td>73.375498</td>\n",
-                            "      <td>82.039074</td>\n",
-                            "      <td>84.005874</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2021-12-28 22:45:00+00:00</th>\n",
-                            "      <td>68.748897</td>\n",
-                            "      <td>65.070595</td>\n",
-                            "      <td>69.778688</td>\n",
-                            "      <td>80.303275</td>\n",
-                            "      <td>71.628658</td>\n",
-                            "      <td>74.726609</td>\n",
-                            "      <td>82.706610</td>\n",
-                            "      <td>84.032210</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2021-12-28 23:00:00+00:00</th>\n",
-                            "      <td>67.878454</td>\n",
-                            "      <td>63.419983</td>\n",
-                            "      <td>68.978997</td>\n",
-                            "      <td>80.625185</td>\n",
-                            "      <td>72.309137</td>\n",
-                            "      <td>76.091041</td>\n",
-                            "      <td>84.231956</td>\n",
-                            "      <td>85.594545</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2021-12-28 23:15:00+00:00</th>\n",
-                            "      <td>67.634819</td>\n",
-                            "      <td>65.679323</td>\n",
-                            "      <td>67.657408</td>\n",
-                            "      <td>81.592753</td>\n",
-                            "      <td>73.233225</td>\n",
-                            "      <td>77.356376</td>\n",
-                            "      <td>84.576420</td>\n",
-                            "      <td>86.070030</td>\n",
+                            "      <th>2023-07-14 20:15:00+00:00</th>\n",
+                            "      <td>78.610786</td>\n",
+                            "      <td>76.187588</td>\n",
+                            "      <td>76.594915</td>\n",
+                            "      <td>78.628710</td>\n",
+                            "      <td>72.219807</td>\n",
+                            "      <td>36.937707</td>\n",
+                            "      <td>70.810772</td>\n",
+                            "      <td>75.548995</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2023-07-14 20:30:00+00:00</th>\n",
+                            "      <td>79.167795</td>\n",
+                            "      <td>71.631429</td>\n",
+                            "      <td>78.045345</td>\n",
+                            "      <td>79.138048</td>\n",
+                            "      <td>72.470195</td>\n",
+                            "      <td>64.158818</td>\n",
+                            "      <td>72.561467</td>\n",
+                            "      <td>76.361568</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2023-07-14 20:45:00+00:00</th>\n",
+                            "      <td>79.723214</td>\n",
+                            "      <td>74.413405</td>\n",
+                            "      <td>77.451970</td>\n",
+                            "      <td>79.629025</td>\n",
+                            "      <td>76.635550</td>\n",
+                            "      <td>76.524077</td>\n",
+                            "      <td>72.934563</td>\n",
+                            "      <td>77.285547</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2023-07-14 21:00:00+00:00</th>\n",
+                            "      <td>80.602099</td>\n",
+                            "      <td>77.433867</td>\n",
+                            "      <td>80.045725</td>\n",
+                            "      <td>80.307846</td>\n",
+                            "      <td>75.792275</td>\n",
+                            "      <td>78.272043</td>\n",
+                            "      <td>75.021305</td>\n",
+                            "      <td>77.483076</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                           Example >> Cooling Tower 1 >> Area A  \\\n",
-                            "2021-12-28 22:30:00+00:00                             69.436828   \n",
-                            "2021-12-28 22:45:00+00:00                             68.748897   \n",
-                            "2021-12-28 23:00:00+00:00                             67.878454   \n",
-                            "2021-12-28 23:15:00+00:00                             67.634819   \n",
+                            "2023-07-14 20:15:00+00:00                             78.610786   \n",
+                            "2023-07-14 20:30:00+00:00                             79.167795   \n",
+                            "2023-07-14 20:45:00+00:00                             79.723214   \n",
+                            "2023-07-14 21:00:00+00:00                             80.602099   \n",
                             "\n",
                             "                           Example >> Cooling Tower 1 >> Area B  \\\n",
-                            "2021-12-28 22:30:00+00:00                             64.729514   \n",
-                            "2021-12-28 22:45:00+00:00                             65.070595   \n",
-                            "2021-12-28 23:00:00+00:00                             63.419983   \n",
-                            "2021-12-28 23:15:00+00:00                             65.679323   \n",
+                            "2023-07-14 20:15:00+00:00                             76.187588   \n",
+                            "2023-07-14 20:30:00+00:00                             71.631429   \n",
+                            "2023-07-14 20:45:00+00:00                             74.413405   \n",
+                            "2023-07-14 21:00:00+00:00                             77.433867   \n",
                             "\n",
                             "                           Example >> Cooling Tower 1 >> Area C  \\\n",
-                            "2021-12-28 22:30:00+00:00                             69.818953   \n",
-                            "2021-12-28 22:45:00+00:00                             69.778688   \n",
-                            "2021-12-28 23:00:00+00:00                             68.978997   \n",
-                            "2021-12-28 23:15:00+00:00                             67.657408   \n",
+                            "2023-07-14 20:15:00+00:00                             76.594915   \n",
+                            "2023-07-14 20:30:00+00:00                             78.045345   \n",
+                            "2023-07-14 20:45:00+00:00                             77.451970   \n",
+                            "2023-07-14 21:00:00+00:00                             80.045725   \n",
                             "\n",
                             "                           Example >> Cooling Tower 1 >> Area G  \\\n",
-                            "2021-12-28 22:30:00+00:00                             79.693327   \n",
-                            "2021-12-28 22:45:00+00:00                             80.303275   \n",
-                            "2021-12-28 23:00:00+00:00                             80.625185   \n",
-                            "2021-12-28 23:15:00+00:00                             81.592753   \n",
+                            "2023-07-14 20:15:00+00:00                             78.628710   \n",
+                            "2023-07-14 20:30:00+00:00                             79.138048   \n",
+                            "2023-07-14 20:45:00+00:00                             79.629025   \n",
+                            "2023-07-14 21:00:00+00:00                             80.307846   \n",
                             "\n",
                             "                           Example >> Cooling Tower 1 >> Area H  \\\n",
-                            "2021-12-28 22:30:00+00:00                             69.598924   \n",
-                            "2021-12-28 22:45:00+00:00                             71.628658   \n",
-                            "2021-12-28 23:00:00+00:00                             72.309137   \n",
-                            "2021-12-28 23:15:00+00:00                             73.233225   \n",
+                            "2023-07-14 20:15:00+00:00                             72.219807   \n",
+                            "2023-07-14 20:30:00+00:00                             72.470195   \n",
+                            "2023-07-14 20:45:00+00:00                             76.635550   \n",
+                            "2023-07-14 21:00:00+00:00                             75.792275   \n",
                             "\n",
                             "                           Example >> Cooling Tower 1 >> Area I  \\\n",
-                            "2021-12-28 22:30:00+00:00                             73.375498   \n",
-                            "2021-12-28 22:45:00+00:00                             74.726609   \n",
-                            "2021-12-28 23:00:00+00:00                             76.091041   \n",
-                            "2021-12-28 23:15:00+00:00                             77.356376   \n",
+                            "2023-07-14 20:15:00+00:00                             36.937707   \n",
+                            "2023-07-14 20:30:00+00:00                             64.158818   \n",
+                            "2023-07-14 20:45:00+00:00                             76.524077   \n",
+                            "2023-07-14 21:00:00+00:00                             78.272043   \n",
                             "\n",
                             "                           Example >> Cooling Tower 1 >> Area J  \\\n",
-                            "2021-12-28 22:30:00+00:00                             82.039074   \n",
-                            "2021-12-28 22:45:00+00:00                             82.706610   \n",
-                            "2021-12-28 23:00:00+00:00                             84.231956   \n",
-                            "2021-12-28 23:15:00+00:00                             84.576420   \n",
+                            "2023-07-14 20:15:00+00:00                             70.810772   \n",
+                            "2023-07-14 20:30:00+00:00                             72.561467   \n",
+                            "2023-07-14 20:45:00+00:00                             72.934563   \n",
+                            "2023-07-14 21:00:00+00:00                             75.021305   \n",
                             "\n",
                             "                           Example >> Cooling Tower 1 >> Area K  \n",
-                            "2021-12-28 22:30:00+00:00                             84.005874  \n",
-                            "2021-12-28 22:45:00+00:00                             84.032210  \n",
-                            "2021-12-28 23:00:00+00:00                             85.594545  \n",
-                            "2021-12-28 23:15:00+00:00                             86.070030  "
+                            "2023-07-14 20:15:00+00:00                             75.548995  \n",
+                            "2023-07-14 20:30:00+00:00                             76.361568  \n",
+                            "2023-07-14 20:45:00+00:00                             77.285547  \n",
+                            "2023-07-14 21:00:00+00:00                             77.483076  "
                         ]
                     },
                     "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1016,15 +1021,15 @@
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>C3CB3C68-35A4-453F-96A8-D2D570E22509</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/2D207275-CACB-413E-BD9D-A134589AD72C/workbook/C3CB3C68-35A4-453F-96A8-D2D570E22509/worksheet/77ACF254-40DF-4530-812A-CAD2495D0E2A\" target=\"_new\">http://localhost:34216/2D207275-CACB-413E-BD9D-A134589AD72C/workbook/C3CB3C68-35A4-453F-96A8-D2D570E22509/worksheet/77ACF254-40DF-4530-812A-CAD2495D0E2A</a></div>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>0EE22861-ABF7-60E0-98C7-650CB85547E5</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/0EE22861-AB73-7380-86F4-76CA140D72A0/workbook/0EE22861-ABF7-60E0-98C7-650CB85547E5/worksheet/0EE22861-AC69-ECD0-927E-CDB442643F0F\" target=\"_blank\">http://localhost:34216/0EE22861-AB73-7380-86F4-76CA140D72A0/workbook/0EE22861-ABF7-60E0-98C7-650CB85547E5/worksheet/0EE22861-AC69-ECD0-927E-CDB442643F0F</a></div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -1050,53 +1055,58 @@
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>Name</th>\n",
                             "      <th>Type</th>\n",
                             "      <th>Formula Parameters</th>\n",
                             "      <th>Formula</th>\n",
+                            "      <th>Scoped To</th>\n",
                             "      <th>Datasource Class</th>\n",
                             "      <th>Datasource ID</th>\n",
                             "      <th>Data ID</th>\n",
                             "      <th>ID</th>\n",
                             "      <th>Push Result</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>Compressor on High</td>\n",
                             "      <td>CalculatedCondition</td>\n",
-                            "      <td>[cp=FC68ACEF-1CCD-47DF-987D-184F3C24AC76]</td>\n",
+                            "      <td>[cp=0EE22861-3FA5-F900-8703-4A2E6D5B0F14]</td>\n",
                             "      <td>$cp.valueSearch(isGreaterThan(25kW))</td>\n",
+                            "      <td>0EE22861-ABF7-60E0-98C7-650CB85547E5</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[C3CB3C68-35A4-453F-96A8-D2D570E22509] {Condit...</td>\n",
-                            "      <td>393B46BD-C3F2-4D82-BCC2-1819B0EADE87</td>\n",
+                            "      <td>[0EE22861-ABF7-60E0-98C7-650CB85547E5] {Condit...</td>\n",
+                            "      <td>0EE2289D-6ABA-60A0-9B42-AD47B40F751B</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                 Name                 Type  \\\n",
                             "0  Compressor on High  CalculatedCondition   \n",
                             "\n",
                             "                          Formula Parameters  \\\n",
-                            "0  [cp=FC68ACEF-1CCD-47DF-987D-184F3C24AC76]   \n",
+                            "0  [cp=0EE22861-3FA5-F900-8703-4A2E6D5B0F14]   \n",
+                            "\n",
+                            "                                Formula                             Scoped To  \\\n",
+                            "0  $cp.valueSearch(isGreaterThan(25kW))  0EE22861-ABF7-60E0-98C7-650CB85547E5   \n",
                             "\n",
-                            "                                Formula Datasource Class  Datasource ID  \\\n",
-                            "0  $cp.valueSearch(isGreaterThan(25kW))    Seeq Data Lab  Seeq Data Lab   \n",
+                            "  Datasource Class  Datasource ID  \\\n",
+                            "0    Seeq Data Lab  Seeq Data Lab   \n",
                             "\n",
                             "                                             Data ID  \\\n",
-                            "0  [C3CB3C68-35A4-453F-96A8-D2D570E22509] {Condit...   \n",
+                            "0  [0EE22861-ABF7-60E0-98C7-650CB85547E5] {Condit...   \n",
                             "\n",
                             "                                     ID Push Result  \n",
-                            "0  393B46BD-C3F2-4D82-BCC2-1819B0EADE87     Success  "
+                            "0  0EE2289D-6ABA-60A0-9B42-AD47B40F751B     Success  "
                         ]
                     },
                     "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1129,15 +1139,15 @@
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Pull successful from <strong>2019-01-01 04:00:00+00:00</strong> to <strong>2019-01-09 02:00:00+00:00</strong></div><table style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">393B46BD-C3F2-4D82-BCC2-1819B0EADE87</td><td style=\"text-align: left; vertical-align: top;\">Compressor on High</td><td style=\"text-align: right; vertical-align: top;\">9</td><td style=\"vertical-align: top;\">00:00:00.11</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pull successful from <strong>2019-01-01 04:00:00+00:00</strong> to <strong>2019-01-09 02:00:00+00:00</strong></div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Data Processed</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">0EE2289D-6ABA-60A0-9B42-AD47B40F751B</td><td style=\"text-align: left; vertical-align: top;\">Compressor on High</td><td style=\"vertical-align: top;\">00:00:00.12</td><td style=\"text-align: right; vertical-align: top;\">9</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">91 KB</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -1289,15 +1299,15 @@
             "cell_type": "code",
             "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Pull successful from <strong>2019-01-01 04:00:00+00:00</strong> to <strong>2019-01-09 02:00:00+00:00</strong></div><table style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">393B46BD-C3F2-4D82-BCC2-1819B0EADE87</td><td style=\"text-align: left; vertical-align: top;\">Compressor on High</td><td style=\"text-align: right; vertical-align: top;\">9</td><td style=\"vertical-align: top;\">00:00:00.08</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pull successful from <strong>2019-01-01 04:00:00+00:00</strong> to <strong>2019-01-09 02:00:00+00:00</strong></div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Data Processed</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">0EE2289D-6ABA-60A0-9B42-AD47B40F751B</td><td style=\"text-align: left; vertical-align: top;\">Compressor on High</td><td style=\"vertical-align: top;\">00:00:00.08</td><td style=\"text-align: right; vertical-align: top;\">9</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">46 KB</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -1455,15 +1465,15 @@
             "cell_type": "code",
             "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Pull successful from <strong>2019-01-01 00:00:00+00:00</strong> to <strong>2019-01-01 12:00:00+00:00</strong></div><table style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">393B46BD-C3F2-4D82-BCC2-1819B0EADE87</td><td style=\"text-align: left; vertical-align: top;\">Compressor on High</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"vertical-align: top;\">00:00:00.02</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pull successful from <strong>2019-01-01 00:00:00+00:00</strong> to <strong>2019-01-01 12:00:00+00:00</strong></div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Data Processed</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">0EE2289D-6ABA-60A0-9B42-AD47B40F751B</td><td style=\"text-align: left; vertical-align: top;\">Compressor on High</td><td style=\"vertical-align: top;\">00:00:00.01</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">128 B</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -1491,83 +1501,83 @@
                             "      <th></th>\n",
                             "      <th>Compressor on High</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 00:00:00+00:00</th>\n",
-                            "      <td>1</td>\n",
+                            "      <td>1.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 01:00:00+00:00</th>\n",
-                            "      <td>1</td>\n",
+                            "      <td>1.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 02:00:00+00:00</th>\n",
-                            "      <td>1</td>\n",
+                            "      <td>1.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 03:00:00+00:00</th>\n",
-                            "      <td>1</td>\n",
+                            "      <td>1.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 04:00:00+00:00</th>\n",
-                            "      <td>1</td>\n",
+                            "      <td>1.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 05:00:00+00:00</th>\n",
-                            "      <td>1</td>\n",
+                            "      <td>1.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 06:00:00+00:00</th>\n",
-                            "      <td>0</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 07:00:00+00:00</th>\n",
-                            "      <td>0</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 08:00:00+00:00</th>\n",
-                            "      <td>0</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 09:00:00+00:00</th>\n",
-                            "      <td>0</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 10:00:00+00:00</th>\n",
-                            "      <td>0</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 11:00:00+00:00</th>\n",
-                            "      <td>0</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 12:00:00+00:00</th>\n",
-                            "      <td>0</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                           Compressor on High\n",
-                            "2019-01-01 00:00:00+00:00                   1\n",
-                            "2019-01-01 01:00:00+00:00                   1\n",
-                            "2019-01-01 02:00:00+00:00                   1\n",
-                            "2019-01-01 03:00:00+00:00                   1\n",
-                            "2019-01-01 04:00:00+00:00                   1\n",
-                            "2019-01-01 05:00:00+00:00                   1\n",
-                            "2019-01-01 06:00:00+00:00                   0\n",
-                            "2019-01-01 07:00:00+00:00                   0\n",
-                            "2019-01-01 08:00:00+00:00                   0\n",
-                            "2019-01-01 09:00:00+00:00                   0\n",
-                            "2019-01-01 10:00:00+00:00                   0\n",
-                            "2019-01-01 11:00:00+00:00                   0\n",
-                            "2019-01-01 12:00:00+00:00                   0"
+                            "2019-01-01 00:00:00+00:00                 1.0\n",
+                            "2019-01-01 01:00:00+00:00                 1.0\n",
+                            "2019-01-01 02:00:00+00:00                 1.0\n",
+                            "2019-01-01 03:00:00+00:00                 1.0\n",
+                            "2019-01-01 04:00:00+00:00                 1.0\n",
+                            "2019-01-01 05:00:00+00:00                 1.0\n",
+                            "2019-01-01 06:00:00+00:00                 0.0\n",
+                            "2019-01-01 07:00:00+00:00                 0.0\n",
+                            "2019-01-01 08:00:00+00:00                 0.0\n",
+                            "2019-01-01 09:00:00+00:00                 0.0\n",
+                            "2019-01-01 10:00:00+00:00                 0.0\n",
+                            "2019-01-01 11:00:00+00:00                 0.0\n",
+                            "2019-01-01 12:00:00+00:00                 0.0"
                         ]
                     },
                     "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1588,15 +1598,15 @@
             "cell_type": "code",
             "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Pull successful from <strong>2019-01-01 00:00:00+00:00</strong> to <strong>2019-01-01 12:00:00+00:00</strong></div><table style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Path</td><td style=\"background-color: #EEFFEE; text-align: left;\">Asset</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">FC68ACEF-1CCD-47DF-987D-184F3C24AC76</td><td style=\"text-align: left; vertical-align: top;\">Example >> Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area A</td><td style=\"text-align: left; vertical-align: top;\">Compressor Power</td><td style=\"text-align: right; vertical-align: top;\">13</td><td style=\"vertical-align: top;\">00:00:00.01</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">393B46BD-C3F2-4D82-BCC2-1819B0EADE87</td><td style=\"text-align: right; vertical-align: top;\">nan</td><td style=\"text-align: right; vertical-align: top;\">nan</td><td style=\"text-align: left; vertical-align: top;\">Compressor on High</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"vertical-align: top;\">00:00:00.02</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pull successful from <strong>2019-01-01 00:00:00+00:00</strong> to <strong>2019-01-01 12:00:00+00:00</strong></div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Path</td><td style=\"background-color: #EEFFEE; text-align: left;\">Asset</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Data Processed</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">0EE22861-3FA5-F900-8703-4A2E6D5B0F14</td><td style=\"text-align: left; vertical-align: top;\">Example >> Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area A</td><td style=\"text-align: left; vertical-align: top;\">Compressor Power</td><td style=\"vertical-align: top;\">00:00:00.01</td><td style=\"text-align: right; vertical-align: top;\">13</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">5 KB</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">0EE2289D-6ABA-60A0-9B42-AD47B40F751B</td><td style=\"text-align: right; vertical-align: top;\">nan</td><td style=\"text-align: right; vertical-align: top;\">nan</td><td style=\"text-align: left; vertical-align: top;\">Compressor on High</td><td style=\"vertical-align: top;\">00:00:00.01</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">128 B</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -1626,95 +1636,95 @@
                             "      <th>Compressor on High</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 00:00:00+00:00</th>\n",
                             "      <td>39.189300</td>\n",
-                            "      <td>1</td>\n",
+                            "      <td>1.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 01:00:00+00:00</th>\n",
                             "      <td>39.326496</td>\n",
-                            "      <td>1</td>\n",
+                            "      <td>1.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 02:00:00+00:00</th>\n",
                             "      <td>40.223175</td>\n",
-                            "      <td>1</td>\n",
+                            "      <td>1.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 03:00:00+00:00</th>\n",
                             "      <td>39.431483</td>\n",
-                            "      <td>1</td>\n",
+                            "      <td>1.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 04:00:00+00:00</th>\n",
                             "      <td>39.139759</td>\n",
-                            "      <td>1</td>\n",
+                            "      <td>1.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 05:00:00+00:00</th>\n",
                             "      <td>39.154395</td>\n",
-                            "      <td>1</td>\n",
+                            "      <td>1.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 06:00:00+00:00</th>\n",
                             "      <td>0.002923</td>\n",
-                            "      <td>0</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 07:00:00+00:00</th>\n",
                             "      <td>0.002923</td>\n",
-                            "      <td>0</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 08:00:00+00:00</th>\n",
                             "      <td>0.002923</td>\n",
-                            "      <td>0</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 09:00:00+00:00</th>\n",
                             "      <td>0.002923</td>\n",
-                            "      <td>0</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 10:00:00+00:00</th>\n",
                             "      <td>0.002923</td>\n",
-                            "      <td>0</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 11:00:00+00:00</th>\n",
                             "      <td>0.002923</td>\n",
-                            "      <td>0</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2019-01-01 12:00:00+00:00</th>\n",
                             "      <td>0.002923</td>\n",
-                            "      <td>0</td>\n",
+                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                           Compressor Power  Compressor on High\n",
-                            "2019-01-01 00:00:00+00:00         39.189300                   1\n",
-                            "2019-01-01 01:00:00+00:00         39.326496                   1\n",
-                            "2019-01-01 02:00:00+00:00         40.223175                   1\n",
-                            "2019-01-01 03:00:00+00:00         39.431483                   1\n",
-                            "2019-01-01 04:00:00+00:00         39.139759                   1\n",
-                            "2019-01-01 05:00:00+00:00         39.154395                   1\n",
-                            "2019-01-01 06:00:00+00:00          0.002923                   0\n",
-                            "2019-01-01 07:00:00+00:00          0.002923                   0\n",
-                            "2019-01-01 08:00:00+00:00          0.002923                   0\n",
-                            "2019-01-01 09:00:00+00:00          0.002923                   0\n",
-                            "2019-01-01 10:00:00+00:00          0.002923                   0\n",
-                            "2019-01-01 11:00:00+00:00          0.002923                   0\n",
-                            "2019-01-01 12:00:00+00:00          0.002923                   0"
+                            "2019-01-01 00:00:00+00:00         39.189300                 1.0\n",
+                            "2019-01-01 01:00:00+00:00         39.326496                 1.0\n",
+                            "2019-01-01 02:00:00+00:00         40.223175                 1.0\n",
+                            "2019-01-01 03:00:00+00:00         39.431483                 1.0\n",
+                            "2019-01-01 04:00:00+00:00         39.139759                 1.0\n",
+                            "2019-01-01 05:00:00+00:00         39.154395                 1.0\n",
+                            "2019-01-01 06:00:00+00:00          0.002923                 0.0\n",
+                            "2019-01-01 07:00:00+00:00          0.002923                 0.0\n",
+                            "2019-01-01 08:00:00+00:00          0.002923                 0.0\n",
+                            "2019-01-01 09:00:00+00:00          0.002923                 0.0\n",
+                            "2019-01-01 10:00:00+00:00          0.002923                 0.0\n",
+                            "2019-01-01 11:00:00+00:00          0.002923                 0.0\n",
+                            "2019-01-01 12:00:00+00:00          0.002923                 0.0"
                         ]
                     },
                     "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1778,41 +1788,41 @@
                             "      <th>Asset</th>\n",
                             "      <th>Statistic</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>393B46BD-C3F2-4D82-BCC2-1819B0EADE87</td>\n",
+                            "      <td>0EE2289D-6ABA-60A0-9B42-AD47B40F751B</td>\n",
                             "      <td>Compressor on High</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>CalculatedCondition</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>False</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>FC68ACEF-1CCD-47DF-987D-184F3C24AC76</td>\n",
+                            "      <td>0EE22861-3FA5-F900-8703-4A2E6D5B0F14</td>\n",
                             "      <td>Compressor Power</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>kW</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>Example &gt;&gt; Cooling Tower 1</td>\n",
                             "      <td>Area A</td>\n",
                             "      <td>maximum</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>FC68ACEF-1CCD-47DF-987D-184F3C24AC76</td>\n",
+                            "      <td>0EE22861-3FA5-F900-8703-4A2E6D5B0F14</td>\n",
                             "      <td>Compressor Power</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>StoredSignal</td>\n",
                             "      <td>kW</td>\n",
                             "      <td>Example Data</td>\n",
                             "      <td>False</td>\n",
                             "      <td>Example &gt;&gt; Cooling Tower 1</td>\n",
@@ -1821,17 +1831,17 @@
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                                     ID                Name  Description  \\\n",
-                            "0  393B46BD-C3F2-4D82-BCC2-1819B0EADE87  Compressor on High          NaN   \n",
-                            "1  FC68ACEF-1CCD-47DF-987D-184F3C24AC76    Compressor Power          NaN   \n",
-                            "2  FC68ACEF-1CCD-47DF-987D-184F3C24AC76    Compressor Power          NaN   \n",
+                            "0  0EE2289D-6ABA-60A0-9B42-AD47B40F751B  Compressor on High          NaN   \n",
+                            "1  0EE22861-3FA5-F900-8703-4A2E6D5B0F14    Compressor Power          NaN   \n",
+                            "2  0EE22861-3FA5-F900-8703-4A2E6D5B0F14    Compressor Power          NaN   \n",
                             "\n",
                             "                  Type Value Unit Of Measure Datasource Name  Archived  \\\n",
                             "0  CalculatedCondition                   NaN   Seeq Data Lab     False   \n",
                             "1         StoredSignal                    kW    Example Data     False   \n",
                             "2         StoredSignal                    kW    Example Data     False   \n",
                             "\n",
                             "                         Path   Asset  Statistic  \n",
@@ -1882,15 +1892,15 @@
             "cell_type": "code",
             "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Pull successful from <strong>2019-01-01 00:00:00+00:00</strong> to <strong>2019-01-07 00:00:00+00:00</strong></div><table style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Path</td><td style=\"background-color: #EEFFEE; text-align: left;\">Asset</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">393B46BD-C3F2-4D82-BCC2-1819B0EADE87</td><td style=\"text-align: right; vertical-align: top;\">nan</td><td style=\"text-align: right; vertical-align: top;\">nan</td><td style=\"text-align: left; vertical-align: top;\">Compressor on High</td><td style=\"text-align: right; vertical-align: top;\">7</td><td style=\"vertical-align: top;\">00:00:00.04</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">FC68ACEF-1CCD-47DF-987D-184F3C24AC76</td><td style=\"text-align: left; vertical-align: top;\">Example >> Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area A</td><td style=\"text-align: left; vertical-align: top;\">Compressor Power</td><td style=\"text-align: right; vertical-align: top;\">7</td><td style=\"vertical-align: top;\">00:00:00.04</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">2</td><td style=\"text-align: left; vertical-align: top;\">FC68ACEF-1CCD-47DF-987D-184F3C24AC76</td><td style=\"text-align: left; vertical-align: top;\">Example >> Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area A</td><td style=\"text-align: left; vertical-align: top;\">Compressor Power</td><td style=\"text-align: right; vertical-align: top;\">7</td><td style=\"vertical-align: top;\">00:00:00.04</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pull successful from <strong>2019-01-01 00:00:00+00:00</strong> to <strong>2019-01-07 00:00:00+00:00</strong></div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Path</td><td style=\"background-color: #EEFFEE; text-align: left;\">Asset</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Data Processed</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">0EE2289D-6ABA-60A0-9B42-AD47B40F751B</td><td style=\"text-align: right; vertical-align: top;\">nan</td><td style=\"text-align: right; vertical-align: top;\">nan</td><td style=\"text-align: left; vertical-align: top;\">Compressor on High</td><td style=\"vertical-align: top;\">00:00:00.16</td><td style=\"text-align: right; vertical-align: top;\">7</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">43 KB</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">1</td><td style=\"text-align: left; vertical-align: top;\">0EE22861-3FA5-F900-8703-4A2E6D5B0F14</td><td style=\"text-align: left; vertical-align: top;\">Example >> Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area A</td><td style=\"text-align: left; vertical-align: top;\">Compressor Power</td><td style=\"vertical-align: top;\">00:00:00.16</td><td style=\"text-align: right; vertical-align: top;\">7</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">43 KB</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">2</td><td style=\"text-align: left; vertical-align: top;\">0EE22861-3FA5-F900-8703-4A2E6D5B0F14</td><td style=\"text-align: left; vertical-align: top;\">Example >> Cooling Tower 1</td><td style=\"text-align: left; vertical-align: top;\">Area A</td><td style=\"text-align: left; vertical-align: top;\">Compressor Power</td><td style=\"vertical-align: top;\">00:00:00.16</td><td style=\"text-align: right; vertical-align: top;\">7</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">43 KB</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -2040,15 +2050,15 @@
             "cell_type": "code",
             "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>C3CB3C68-35A4-453F-96A8-D2D570E22509</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/2D207275-CACB-413E-BD9D-A134589AD72C/workbook/C3CB3C68-35A4-453F-96A8-D2D570E22509/worksheet/77ACF254-40DF-4530-812A-CAD2495D0E2A\" target=\"_new\">http://localhost:34216/2D207275-CACB-413E-BD9D-A134589AD72C/workbook/C3CB3C68-35A4-453F-96A8-D2D570E22509/worksheet/77ACF254-40DF-4530-812A-CAD2495D0E2A</a></div>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pushed successfully to datasource <strong>Seeq Data Lab [Datasource ID: Seeq Data Lab]</strong> and scoped to workbook ID <strong>0EE22861-ABF7-60E0-98C7-650CB85547E5</strong><br>Click the following link to see what you pushed in Seeq:<br><a href=\"http://localhost:34216/0EE22861-AB73-7380-86F4-76CA140D72A0/workbook/0EE22861-ABF7-60E0-98C7-650CB85547E5/worksheet/0EE22861-AC69-ECD0-927E-CDB442643F0F\" target=\"_blank\">http://localhost:34216/0EE22861-AB73-7380-86F4-76CA140D72A0/workbook/0EE22861-ABF7-60E0-98C7-650CB85547E5/worksheet/0EE22861-AC69-ECD0-927E-CDB442643F0F</a></div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -2073,46 +2083,53 @@
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>Name</th>\n",
                             "      <th>Type</th>\n",
                             "      <th>Formula</th>\n",
+                            "      <th>Scoped To</th>\n",
                             "      <th>Datasource Class</th>\n",
                             "      <th>Datasource ID</th>\n",
+                            "      <th>Formula Parameters</th>\n",
                             "      <th>Data ID</th>\n",
                             "      <th>ID</th>\n",
                             "      <th>Push Result</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>Compressor Power Limit</td>\n",
-                            "      <td>CalculatedScalar</td>\n",
+                            "      <td>LiteralScalar</td>\n",
                             "      <td>50kW</td>\n",
+                            "      <td>0EE22861-ABF7-60E0-98C7-650CB85547E5</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
                             "      <td>Seeq Data Lab</td>\n",
-                            "      <td>[C3CB3C68-35A4-453F-96A8-D2D570E22509] {Scalar...</td>\n",
-                            "      <td>7B70FE24-7BCF-45E7-8143-85D6643DF4BB</td>\n",
+                            "      <td>[]</td>\n",
+                            "      <td>[0EE22861-ABF7-60E0-98C7-650CB85547E5] {Scalar...</td>\n",
+                            "      <td>0EE2289D-7AF5-7500-A966-AB5EEC6BD1CD</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "                     Name              Type Formula Datasource Class  \\\n",
-                            "0  Compressor Power Limit  CalculatedScalar    50kW    Seeq Data Lab   \n",
+                            "                     Name           Type Formula  \\\n",
+                            "0  Compressor Power Limit  LiteralScalar    50kW   \n",
+                            "\n",
+                            "                              Scoped To Datasource Class  Datasource ID  \\\n",
+                            "0  0EE22861-ABF7-60E0-98C7-650CB85547E5    Seeq Data Lab  Seeq Data Lab   \n",
                             "\n",
-                            "   Datasource ID                                            Data ID  \\\n",
-                            "0  Seeq Data Lab  [C3CB3C68-35A4-453F-96A8-D2D570E22509] {Scalar...   \n",
+                            "  Formula Parameters                                            Data ID  \\\n",
+                            "0                 []  [0EE22861-ABF7-60E0-98C7-650CB85547E5] {Scalar...   \n",
                             "\n",
                             "                                     ID Push Result  \n",
-                            "0  7B70FE24-7BCF-45E7-8143-85D6643DF4BB     Success  "
+                            "0  0EE2289D-7AF5-7500-A966-AB5EEC6BD1CD     Success  "
                         ]
                     },
                     "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -2130,15 +2147,15 @@
             "cell_type": "code",
             "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style=\"background-color: #EEFFEE;color:black;text-align: left;\">Pull successful from <strong>2021-12-28 22:27:07.269113+00:00</strong> to <strong>2021-12-28 23:27:07.269113+00:00</strong></div><table style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">7B70FE24-7BCF-45E7-8143-85D6643DF4BB</td><td style=\"text-align: left; vertical-align: top;\">Compressor Power Limit</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"vertical-align: top;\">00:00:00.01</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pull successful from <strong>2023-07-14 20:03:12.331663+00:00</strong> to <strong>2023-07-14 21:03:12.331663+00:00</strong></div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Data Processed</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">0EE2289D-7AF5-7500-A966-AB5EEC6BD1CD</td><td style=\"text-align: left; vertical-align: top;\">Compressor Power Limit</td><td style=\"vertical-align: top;\">00:00:00.02</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">0</td><td style=\"text-align: right; vertical-align: top;\">0 B</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -2258,64 +2275,72 @@
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>ID</th>\n",
                             "      <th>Path</th>\n",
                             "      <th>Asset</th>\n",
                             "      <th>Name</th>\n",
-                            "      <th>Count</th>\n",
                             "      <th>Time</th>\n",
+                            "      <th>Count</th>\n",
+                            "      <th>Pages</th>\n",
+                            "      <th>Data Processed</th>\n",
                             "      <th>Result</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>393B46BD-C3F2-4D82-BCC2-1819B0EADE87</td>\n",
+                            "      <td>0EE2289D-6ABA-60A0-9B42-AD47B40F751B</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>NaN</td>\n",
                             "      <td>Compressor on High</td>\n",
+                            "      <td>0:00:00.156000</td>\n",
                             "      <td>7</td>\n",
-                            "      <td>0:00:00.038004</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>43 KB</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>FC68ACEF-1CCD-47DF-987D-184F3C24AC76</td>\n",
+                            "      <td>0EE22861-3FA5-F900-8703-4A2E6D5B0F14</td>\n",
                             "      <td>Example &gt;&gt; Cooling Tower 1</td>\n",
                             "      <td>Area A</td>\n",
                             "      <td>Compressor Power</td>\n",
+                            "      <td>0:00:00.156000</td>\n",
                             "      <td>7</td>\n",
-                            "      <td>0:00:00.038004</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>43 KB</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>FC68ACEF-1CCD-47DF-987D-184F3C24AC76</td>\n",
+                            "      <td>0EE22861-3FA5-F900-8703-4A2E6D5B0F14</td>\n",
                             "      <td>Example &gt;&gt; Cooling Tower 1</td>\n",
                             "      <td>Area A</td>\n",
                             "      <td>Compressor Power</td>\n",
+                            "      <td>0:00:00.156000</td>\n",
                             "      <td>7</td>\n",
-                            "      <td>0:00:00.038004</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>43 KB</td>\n",
                             "      <td>Success</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                                     ID                        Path   Asset  \\\n",
-                            "0  393B46BD-C3F2-4D82-BCC2-1819B0EADE87                         NaN     NaN   \n",
-                            "1  FC68ACEF-1CCD-47DF-987D-184F3C24AC76  Example >> Cooling Tower 1  Area A   \n",
-                            "2  FC68ACEF-1CCD-47DF-987D-184F3C24AC76  Example >> Cooling Tower 1  Area A   \n",
-                            "\n",
-                            "                 Name  Count            Time   Result  \n",
-                            "0  Compressor on High      7  0:00:00.038004  Success  \n",
-                            "1    Compressor Power      7  0:00:00.038004  Success  \n",
-                            "2    Compressor Power      7  0:00:00.038004  Success  "
+                            "0  0EE2289D-6ABA-60A0-9B42-AD47B40F751B                         NaN     NaN   \n",
+                            "1  0EE22861-3FA5-F900-8703-4A2E6D5B0F14  Example >> Cooling Tower 1  Area A   \n",
+                            "2  0EE22861-3FA5-F900-8703-4A2E6D5B0F14  Example >> Cooling Tower 1  Area A   \n",
+                            "\n",
+                            "                 Name            Time  Count  Pages Data Processed   Result  \n",
+                            "0  Compressor on High  0:00:00.156000      7      1          43 KB  Success  \n",
+                            "1    Compressor Power  0:00:00.156000      7      1          43 KB  Success  \n",
+                            "2    Compressor Power  0:00:00.156000      7      1          43 KB  Success  "
                         ]
                     },
                     "execution_count": 21,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -2323,61 +2348,139 @@
                 "unpickled_pull.spy.status.df"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "## Performance Metrics\n",
+                "\n",
+                "If your pull operation takes a long time to complete, you can take a look at the timing information for data processing by inspecting the \"Data Processed\" cell in the status DataFrame like so:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 22,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div style=\"background-color: #EEFFEE;color:black; text-align: left;\">Pull successful from <strong>2019-01-01 00:00:00+00:00</strong> to <strong>2019-03-01 00:00:00+00:00</strong></div><table class=\"tex2jax_ignore\" style=\"color:black;\"><tr><td style=\"background-color: #EEFFEE;\"></td><td style=\"background-color: #EEFFEE; text-align: left;\">ID</td><td style=\"background-color: #EEFFEE; text-align: left;\">Name</td><td style=\"background-color: #EEFFEE; text-align: left;\">Time</td><td style=\"background-color: #EEFFEE; text-align: right;\">Count</td><td style=\"background-color: #EEFFEE; text-align: right;\">Pages</td><td style=\"background-color: #EEFFEE; text-align: left;\">Data Processed</td><td style=\"background-color: #EEFFEE; text-align: left;\">Result</td></tr><tr style=\"background-color: #EEFFEE;\"><td style=\"vertical-align: top;\">0</td><td style=\"text-align: left; vertical-align: top;\">0EE22861-3F8F-F970-A063-3575416842E6</td><td style=\"text-align: left; vertical-align: top;\">Area B_Compressor Power</td><td style=\"vertical-align: top;\">00:00:00.27</td><td style=\"text-align: right; vertical-align: top;\">42481</td><td style=\"text-align: right; vertical-align: top;\">1</td><td style=\"text-align: right; vertical-align: top;\">679 KB</td><td style=\"text-align: left; vertical-align: top;\">Success</td></tr></table>"
+                        ],
+                        "text/plain": [
+                            "<IPython.core.display.HTML object>"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "# Pull two months of data\n",
+                "pull_results = spy.pull(spy.search({'Name': 'Area B_Compressor Power'}), start='2019-01-01', end='2019-03-01', grid=None)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 23,
+            "metadata": {
+                "keep_output_in_docs": true
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "Time spent in Request Queue:           0:00:00.000110\n",
+                            "Time spent reading Metadata:           0:00:00.001640\n",
+                            "Time spent waiting for Datasource(s):  0:00:00\n",
+                            "Time spent reading from Seeq Cache:    0:00:00\n",
+                            "Time spent in Calc Engine Queue:       0:00:00\n",
+                            "Time spent in Calc Engine:             0:00:00.189600\n",
+                            "Time spent reclaiming Memory:          0:00:00\n",
+                            "\n",
+                            "Metadata items read:                                2\n",
+                            "Metadata relationships read:                        0\n",
+                            "Samples read from Datasource(s):                42481\n",
+                            "Samples read from Persistent Cache:                 0\n",
+                            "Samples read from In-Memory Cache:                  0\n",
+                            "Capsules read from Datasource(s):                   0\n",
+                            "Capsules read from Persistent Cache:                0\n",
+                            "Capsules read from In-Memory Cache:                 0\n",
+                            "Total bytes processed:                         679696"
+                        ]
+                    },
+                    "execution_count": 23,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "# Inspect the 'Data Processed' column in the first row of the status DataFrame\n",
+                "pull_results.spy.status.df.iloc[0]['Data Processed']"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Note that the \"Time spent\" values here are inclusive of the time spent within the Seeq service. They are _exclusive_ of time spent transmitting the data from the Seeq service to SPy, and the time spent by SPy organizing the data into a Pandas DataFrame."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "## Detailed Help\n",
                 "\n",
                 "All SPy functions have detailed documentation to help you use them. Just execute `help(spy.<func>)` like\n",
                 "you see below.\n",
                 "\n",
                 "**Make sure you re-execute the cell below to see the latest documentation. It otherwise might be from an\n",
                 "earlier version of SPy.**"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 24,
             "metadata": {
                 "pycharm": {
                     "name": "#%% \n"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Help on function pull in module seeq.spy._pull:\n",
                         "\n",
-                        "pull(items, *, start=None, end=None, grid='15min', header='__auto__', group_by=None, shape='auto', capsule_properties=None, tz_convert=None, calculation=None, bounding_values=False, invalid_values_as=nan, enums_as='string', errors='raise', quiet=False, status: seeq.spy._common.Status = None, session: Union[seeq.spy._session.Session, NoneType] = None, capsules_as=None)\n",
+                        "pull(items, *, start=None, end=None, grid='15min', header='__auto__', group_by=None, shape='auto', capsule_properties=None, tz_convert=None, calculation=None, bounding_values=False, invalid_values_as=nan, enums_as='string', errors=None, quiet=None, status: 'Status' = None, session: 'Optional[Session]' = None, capsules_as=None)\n",
                         "    Retrieves signal, condition or scalar data from Seeq Server and returns it\n",
                         "    in a DataFrame.\n",
                         "    \n",
                         "    Parameters\n",
                         "    ----------\n",
                         "    items : {str, pd.DataFrame, pd.Series}\n",
                         "        A DataFrame or Series containing ID and Type columns that can be used\n",
                         "        to identify the items to pull. This is usually created via a call to\n",
                         "        spy.search(). Alternatively, you can supply URL of a Seeq Workbench\n",
                         "        worksheet as a str.\n",
                         "    \n",
-                        "    start : {str, pd.Timestamp}\n",
+                        "    start : {str, pd.Timestamp}, optional\n",
                         "        The starting time for which to pull data. This argument must be a\n",
                         "        string that pandas.to_datetime() can parse, or a pandas.Timestamp.\n",
                         "        If not provided, 'start' will default to 'end' minus 1 hour. Note\n",
                         "        that Seeq will potentially return one additional row that is earlier\n",
                         "        than this time (if it exists), as a \"bounding value\" for interpolation\n",
                         "        purposes. If both 'start' and 'end' are not provided and items\n",
                         "        is a str, 'start' will default to the start of the display range\n",
                         "        in Seeq Trend View.\n",
                         "    \n",
-                        "    end : {str, pd.Timestamp}\n",
+                        "    end : {str, pd.Timestamp}, optional\n",
                         "        The end time for which to pull data. This argument must be a string\n",
                         "        that pandas.to_datetime() can parse, or a pandas.Timestamp.\n",
                         "        If not provided, 'end' will default to now. Note that Seeq will\n",
                         "        potentially return one additional row that is later than this time\n",
                         "        (if it exists), as a \"bounding value\" for interpolation purposes.\n",
                         "        If both 'start' and 'end' are not provided and items is a str,\n",
                         "        'end' will default to the end of the display range in Seeq Trend View.\n",
@@ -2395,43 +2498,43 @@
                         "        If grid='auto' and the 'Estimated Sample Period' column does not exist\n",
                         "        in 'items', additional queries will be made to estimate the sample period\n",
                         "        which could potentially impact performance for large pulls. Interpolation\n",
                         "        is either linear or step and is set per signal at the time of the signal's\n",
                         "        creation. To change the interpolation type for a given signal, change the\n",
                         "        signal's interpolation or use the appropriate 'calculation' argument.\n",
                         "    \n",
-                        "    header : str default '__auto__'\n",
+                        "    header : str, default '__auto__'\n",
                         "        The metadata property to use as the header of each column. Common\n",
                         "        values would be 'ID' or 'Name'. '__auto__' concatenates Path and Name\n",
                         "        if they are present.\n",
                         "    \n",
-                        "    group_by : {str, list(str)}\n",
+                        "    group_by : {str, list(str)}, optional\n",
                         "        The name of a column or list of columns for which to group by. Often\n",
                         "        necessary when pulling data across assets: When you want header='Name',\n",
                         "        you typically need group_by=['Path', 'Asset']\n",
                         "    \n",
                         "    shape : {'auto', 'samples', 'capsules'}, default 'auto'\n",
                         "        If 'auto', returns capsules as a time series of 0 or 1 when signals are\n",
                         "        also present in the items argument, or returns capsules as individual\n",
                         "        rows if no signals are present. 'samples' or 'capsules' forces the\n",
                         "        output to the former or the latter, if possible.\n",
                         "    \n",
-                        "    capsule_properties : list(str)\n",
+                        "    capsule_properties : list(str), optional\n",
                         "        A list of capsule properties to retrieve when shape='capsules'.\n",
                         "        By default, if no signals are present in the items DataFrame, then all\n",
                         "        properties found on a capsule are automatically returned (because\n",
                         "        the nature of the query allows them to be returned \"for free\").\n",
                         "        Otherwise, you must provide a list of names of properties to retrieve.\n",
                         "    \n",
-                        "    tz_convert : {str, datetime.tzinfo}\n",
+                        "    tz_convert : {str, datetime.tzinfo}, optional\n",
                         "        The time zone in which to return all timestamps. If the time zone\n",
                         "        string is not recognized, the list of supported time zone strings will\n",
                         "        be returned in the exception text.\n",
                         "    \n",
-                        "    calculation : {str, pandas.Series, pandas.DataFrame}\n",
+                        "    calculation : {str, pandas.Series, pandas.DataFrame}, optional\n",
                         "        When applying a calculation across assets, the 'calculation' argument\n",
                         "        must be a one-row DataFrame (or a Series) and the 'items' argument must\n",
                         "        be full of assets. When applying a calculation to a signal/condition/\n",
                         "        scalar, calculation must be a string with a single variable in it:\n",
                         "        $signal, $condition or $scalar.\n",
                         "    \n",
                         "    bounding_values : bool, default False\n",
@@ -2460,18 +2563,18 @@
                         "        (e.g., (1, 'ON') or (0, 'OFF')).\n",
                         "    \n",
                         "    errors : {'raise', 'catalog'}, default 'raise'\n",
                         "        If 'raise', any errors encountered will cause an exception. If\n",
                         "        'catalog', errors will be added to a 'Result' column in the status.df\n",
                         "        DataFrame.\n",
                         "    \n",
-                        "    quiet : bool\n",
+                        "    quiet : bool, default False\n",
                         "        If True, suppresses progress output. Note that when status is\n",
                         "        provided, the quiet setting of the Status object that is passed\n",
-                        "        in takes precedent.\n",
+                        "        in takes precedence.\n",
                         "    \n",
                         "    status : spy.Status, optional\n",
                         "        If specified, the supplied Status object will be updated as the command\n",
                         "        progresses. It gets filled in with the same information you would see\n",
                         "        in Jupyter in the blue/green/red table below your code while the\n",
                         "        command is executed. The table itself is accessible as a DataFrame via\n",
                         "        the status.df property.\n",
@@ -2484,15 +2587,15 @@
                         "    capsules_as : str\n",
                         "        Deprecated, use shape argument instead.\n",
                         "    \n",
                         "    Returns\n",
                         "    -------\n",
                         "    pandas.DataFrame\n",
                         "        A DataFrame with the requested data. Additionally, the following\n",
-                        "        properties are stored in the output DataFrame:\n",
+                        "        properties are stored on the \"spy\" attribute of the output DataFrame:\n",
                         "    \n",
                         "        =================== ===================================================\n",
                         "        Property            Description\n",
                         "        =================== ===================================================\n",
                         "        func                A str value of 'spy.pull'\n",
                         "        kwargs              A dict with the values of the input parameters\n",
                         "                            passed to spy.pull to get the output DataFrame\n",
@@ -2515,20 +2618,20 @@
                         "    Pull a list of signals and convert the timezone to another timezone\n",
                         "    \n",
                         "    >>> items = pd.DataFrame([{'ID': '8543F427-2963-4B4E-9825-220D9FDCAD4E', 'Type': 'CalculatedSignal'}])\n",
                         "    >>> my_signals = spy.pull(items=items, grid='15min', calculation='$signal.toStep()',\n",
                         "    >>>          start='2019-10-5T02:53:45.567Z', end='2019-10-6', tz_convert='US/Eastern')\n",
                         "    \n",
                         "    To access the stored properties\n",
-                        "    >>> my_signals.kwargs\n",
-                        "    >>> my_signals.query_df\n",
-                        "    >>> my_signals.start\n",
-                        "    >>> my_signals.end\n",
-                        "    >>> my_signals.grid\n",
-                        "    >>> my_signals.status.df\n",
+                        "    >>> my_signals.spy.kwargs\n",
+                        "    >>> my_signals.spy.query_df\n",
+                        "    >>> my_signals.spy.start\n",
+                        "    >>> my_signals.spy.end\n",
+                        "    >>> my_signals.spy.grid\n",
+                        "    >>> my_signals.spy.status.df\n",
                         "    \n",
                         "    Pull a list of signals with an auto-calculated grid\n",
                         "    >>> signals = spy.search({'Name': 'Area ?_*', 'Datasource Name': 'Example Data'},\n",
                         "    >>>                        estimate_sample_period=dict(Start='2018-01-01T00:00:00Z',\n",
                         "    >>>                        End='2018-01-01T12:00:00Z'))\n",
                         "    >>> spy.pull(signals,\n",
                         "    >>>          start='2018-01-01T00:00:00Z',\n",
```

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/spy.push.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/spy.push.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/spy.search.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/spy.search.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/spy.swap.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/spy.swap.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/spy.widgets.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/spy.widgets.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/Documentation/spy.workbooks.ipynb` & `seeq-spy-189.9/seeq/spy/docs/Documentation/spy.workbooks.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/docs/_copy.py` & `seeq-spy-189.9/seeq/spy/docs/_copy.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/jobs/_pull.py` & `seeq-spy-189.9/seeq/spy/jobs/_pull.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 from seeq.spy._session import Session
 from seeq.spy._status import Status
 from seeq.spy.jobs import _push
 from seeq.spy.jobs import _schedule
 
 
 # noinspection PyShadowingBuiltins
-def pull(datalab_notebook_url=None, label=None, interactive_index: Union[Optional[int], Optional[str]] = None,
+def pull(datalab_notebook_url: Optional[str] = None, label: Optional[str] = None,
+         interactive_index: Union[Optional[int], Optional[str]] = None,
          all: bool = False, session: Optional[Session] = None) -> Optional[pd.Series]:
     """
     Retrieves a jobs DataFrame previously created by a call to spy.jobs.push or
     spy.jobs.schedule.  The DataFrame will have been stored as a pickle (.pkl)
     file in the _Job DataFrames folder within the parent folder of the Notebook
     specified by the datalab_notebook_url, or of the current Notebook if no
     datalab_notebook_url is specified.
```

### Comparing `seeq-spy-189.3/seeq/spy/jobs/_push.py` & `seeq-spy-189.9/seeq/spy/jobs/_push.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from seeq.spy.jobs import _schedule
 
 
 @Status.handle_keyboard_interrupt(errors='raise')
 def push(jobs_df: pd.DataFrame, spread: Optional[str] = None, datalab_notebook_url: Optional[str] = None,
          label: Optional[str] = None, user: Optional[str] = None,
          interactive_index: Union[Optional[int], Optional[str]] = None, suspend: bool = False,
+         notify_on_skipped_execution: bool = True, notify_on_automatic_unschedule: bool = True,
          quiet: Optional[bool] = None, status: Optional[Status] = None, session: Optional[Session] = None):
     """
     Schedules the automatic execution of a notebook and returns the row
     corresponding for the currently running schedule.
 
     When used inside a Data Lab notebook, the current notebook is scheduled
     for execution. A notebook can be scheduled also by specifying its URL, and
@@ -90,14 +91,25 @@
 
     suspend : bool default False
         If True, un-schedules all jobs for the specified notebook. This is used
         in scenarios where you wish to work with a notebook interactively and
         temporarily prevent job execution. Remove the argument (or change it
         to False) when you are ready to resume job execution.
 
+    notify_on_skipped_execution: bool, default True
+        If True, on skipped execution, the user on whose behalf the notebook
+        is executed is notified, making it possible to investigate the problem
+        and even try the execution if needed
+
+    notify_on_automatic_unschedule: bool, default True
+        If True, in case the notebook is automatically unscheduled because of a
+        system error, the user on whose behalf the notebook is executed is
+        notified, making it possible to investigate the problem and reschedule
+        the notebook if needed
+
     quiet : bool, default False
         If True, suppresses progress output. Note that when status is
         provided, the quiet setting of the Status object that is passed
         in takes precedence.
 
     status : spy.Status, optional
         If specified, the supplied Status object will be updated as the command
@@ -123,25 +135,30 @@
         (jobs_df, 'jobs_df', pd.DataFrame),
         (spread, 'spread', str),
         (datalab_notebook_url, 'datalab_notebook_url', str),
         (label, 'label', str),
         (user, 'user', str),
         (interactive_index, 'interactive_index', (int, str)),
         (suspend, 'suspend', bool),
+        (notify_on_skipped_execution, 'notify_on_skipped_execution', bool),
+        (notify_on_automatic_unschedule, 'notify_on_automatic_unschedule', bool),
         (quiet, 'quiet', bool),
         (status, 'status', Status),
         (session, 'session', Session)
     ])
 
     status = Status.validate(status, quiet)
     session = Session.validate(session)
 
     try:
         _schedule.schedule_df(session, jobs_df=jobs_df, spread=spread, datalab_notebook_url=datalab_notebook_url,
-                              label=label, user=user, suspend=suspend, status=status)
+                              label=label, user=user, suspend=suspend,
+                              notify_on_skipped_execution=notify_on_skipped_execution,
+                              notify_on_automatic_unschedule=notify_on_automatic_unschedule,
+                              status=status)
     except SchedulePostingError:
         # When the notebook is executed as a job, push will first re-schedule the notebook. If any errors will happen
         # during that reschedule, an exception forces an exit from the method, and the currently executing notebook will
         # not get the needed parameters and will have a failed execution (assuming it needs the parameters). Most of
         # the time, such transient errors are unnecessary to the running of a job. One example where a failed schedule
         # call is actually expected is when you schedule a notebook to run exactly once, with a fixed date. When the
         # notebook is executing on schedule, the date is already in the past, and that means the schedule will fail
```

### Comparing `seeq-spy-189.3/seeq/spy/jobs/_schedule.py` & `seeq-spy-189.9/seeq/spy/jobs/_schedule.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,33 +4,35 @@
 import json
 import os
 import pathlib
 import pickle
 import re
 import types
 from datetime import datetime, timedelta
-from typing import Optional
+from typing import Optional, List, Tuple, Any, Dict
 from urllib.parse import unquote
 
-import cron_descriptor
 import pandas as pd
 import pytz as tz
+from cron_descriptor import ExpressionDescriptor
 from recurrent import RecurringEvent
 
 from seeq.sdk import *
 from seeq.spy import _common, _login, _datalab
 from seeq.spy._errors import *
 from seeq.spy._session import Session
 from seeq.spy._status import Status
 
 
 @Status.handle_keyboard_interrupt(errors='raise')
 def schedule(schedule_spec: str, datalab_notebook_url: Optional[str] = None, label: Optional[str] = None,
-             user: Optional[str] = None, suspend: bool = False, quiet: Optional[bool] = None,
-             status: Optional[Status] = None, session: Optional[Session] = None):
+             user: Optional[str] = None, suspend: bool = False,
+             notify_on_skipped_execution: Optional[bool] = True, notify_on_automatic_unschedule: Optional[bool] = True,
+             quiet: Optional[bool] = None, status: Optional[Status] = None, session: Optional[Session] = None) -> \
+        pd.DataFrame:
     """
     Schedules the automatic execution of a Seeq Data Lab notebook.
 
     The current notebook is scheduled for execution unless datalab_notebook_url
     is supplied. Scheduling can be done on behalf of another user by a user with
     admin privileges.
 
@@ -88,14 +90,25 @@
 
     suspend : bool, default False
         If True, unschedules all jobs for the specified notebook. This is used
         in scenarios where you wish to work with a notebook interactively and
         temporarily "pause" job execution. Remove the argument (or change it
         to False) when you are ready to resume job execution.
 
+    notify_on_skipped_execution: bool, default True
+        If True, on skipped execution, the user on whose behalf the notebook
+        is executed is notified, making it possible to investigate the problem
+        and even try the execution if needed
+
+    notify_on_automatic_unschedule: bool, default True
+        If True, in case the notebook is automatically unscheduled because of a
+        system error, the user on whose behalf the notebook is executed is
+        notified, making it possible to investigate the problem and reschedule
+        the notebook if needed
+
     quiet : bool, default False
         If True, suppresses progress output. Note that when status is
         provided, the quiet setting of the Status object that is passed
         in takes precedence.
 
     status : spy.Status, optional
         If specified, the supplied Status object will be updated as the command
@@ -117,26 +130,29 @@
     """
     _common.validate_argument_types([
         (schedule_spec, 'schedule_string', str),
         (datalab_notebook_url, 'datalab_notebook_url', str),
         (label, 'label', str),
         (user, 'user', str),
         (suspend, 'suspend', bool),
+        (notify_on_skipped_execution, 'notify_on_skipped_execution', bool),
+        (notify_on_automatic_unschedule, 'notify_on_automatic_unschedule', bool),
         (quiet, 'quiet', bool),
         (status, 'status', Status),
         (session, 'session', Session)
     ])
 
     status = Status.validate(status, quiet)
     session = Session.validate(session)
 
     try:
         return schedule_df(session, pd.DataFrame([{'Schedule': schedule_spec}]) if schedule_spec else None,
                            datalab_notebook_url=datalab_notebook_url, label=label, user=user, suspend=suspend,
-                           status=status)
+                           notify_on_skipped_execution=notify_on_skipped_execution,
+                           notify_on_automatic_unschedule=notify_on_automatic_unschedule, status=status)
     except SchedulePostingError:
         # See _push.push() for why we swallow this error in the executor
         if not _datalab.is_executor():
             raise
 
 
 def unschedule(datalab_notebook_url: Optional[str] = None, label: Optional[str] = None, quiet: Optional[bool] = None,
@@ -191,22 +207,26 @@
     ])
 
     status = Status.validate(status, quiet, errors='raise')
     session = Session.validate(session)
     schedule_df(session, jobs_df=None, datalab_notebook_url=datalab_notebook_url, label=label, status=status)
 
 
-def schedule_df(session: Session, jobs_df=None, spread=None, datalab_notebook_url=None, label=None, user=None,
-                suspend=False, status=None):
+def schedule_df(session: Session, jobs_df: pd.DataFrame = None, spread: Optional[str] = None,
+                datalab_notebook_url: Optional[str] = None, label: Optional[str] = None,
+                user: Optional[str] = None, suspend: bool = False, notify_on_skipped_execution: Optional[bool] = True,
+                notify_on_automatic_unschedule: Optional[bool] = True, status: Optional[Status] = None) -> pd.DataFrame:
     input_args = _common.validate_argument_types([
         (jobs_df, 'jobs_df', pd.DataFrame),
         (datalab_notebook_url, 'datalab_notebook_url', str),
         (label, 'label', str),
         (user, 'user', str),
         (suspend, 'suspend', bool),
+        (notify_on_skipped_execution, 'notify_on_skipped_execution', bool),
+        (notify_on_automatic_unschedule, 'notify_on_automatic_unschedule', bool),
         (status, 'status', Status)
     ])
 
     if jobs_df is None:
         jobs_df = pd.DataFrame()
 
     _login.validate_login(session, status)
@@ -226,15 +246,16 @@
         _verify_existing_and_accessible(session, datalab_notebook_url)
 
     try:
         user_identity = _login.find_user(session, user) if user is not None else None
         if len(indexed_cron_expressions) == 0:
             _call_unschedule_notebook_api(session, project_id, file_path, label)
         else:
-            _call_schedule_notebook_api(session, indexed_cron_expressions, project_id, file_path, label, user_identity)
+            _call_schedule_notebook_api(session, indexed_cron_expressions, project_id, file_path, label, user_identity,
+                                        notify_on_skipped_execution, notify_on_automatic_unschedule)
     except BaseException as e:
         status.exception(e)
         raise SchedulePostingError(e)
 
     with_label_text = f' with label <strong>{label}</strong> ' if label else ' '
     if indexed_cron_expressions:
         status.update(f'Scheduled the notebook <strong>{file_path}</strong>{with_label_text}successfully.\n'
@@ -259,21 +280,29 @@
                       f'</strong>{with_label_text}successfully.', Status.SUCCESS)
         if pickle_path:
             status.update(f'{status.message}  The Job DataFrame at {pickle_path} has been cleared.')
 
     if indexed_cron_expressions:
         cron_expressions = [cron for idx, cron in indexed_cron_expressions]
         schedule_result_df = pd.concat(
-            [jobs_df,
-             pd.Series(cron_expressions, index=jobs_df.index).rename('Scheduled').map(cron_descriptor.get_description)],
+            [
+                jobs_df,
+                pd.Series(cron_expressions, index=jobs_df.index)
+                .rename('Scheduled')
+                .map(lambda expr: ExpressionDescriptor(expr, day_of_week_start_index_zero=False).get_description())
+            ],
             axis=1
         )
         schedule_result_df = pd.concat(
-            [schedule_result_df,
-             pd.Series(cron_expressions, index=jobs_df.index).rename('Next Run').map(lambda ce: next_trigger_map[ce])],
+            [
+                schedule_result_df,
+                pd.Series(cron_expressions, index=jobs_df.index)
+                .rename('Next Run')
+                .map(lambda ce: next_trigger_map[ce])
+            ],
             axis=1
         )
     else:
         schedule_result_df = pd.DataFrame()
 
     schedule_df_properties = types.SimpleNamespace(
         func='spy.schedule',
@@ -375,15 +404,15 @@
 
 
 def dump_pickle(df, path):
     with open(pathlib.PurePosixPath(_common.DATALAB_HOME, path), mode='wb') as pickle_file:
         pickle.dump(df, pickle_file)
 
 
-def validate_and_get_next_trigger(session: Session, cron_expression_list):
+def validate_and_get_next_trigger(session: Session, cron_expression_list) -> Dict[str, str]:
     jobs_api = JobsApi(session.client)
     validate_cron_input = ValidateCronListInputV1()
     validate_cron_input.timezone = _login.get_fallback_timezone(session)
     validate_cron_input.next_valid_time_after = datetime.now(tz.timezone(_login.get_fallback_timezone(session))) \
         .replace(microsecond=0)
     validate_cron_input.schedules = cron_expression_list
     validation_output = jobs_api.validate_cron(body=validate_cron_input)
@@ -394,28 +423,32 @@
             invalid_cron_expressions.append({'string': cron_validation.quartz_cron_expression,
                                              'error': cron_validation.error})
     if invalid_cron_expressions:
         raise SPyRuntimeError('The following schedules are invalid: ' + str(invalid_cron_expressions))
     return dict((s.quartz_cron_expression, s.next_run_time) for s in validation_output.schedules)
 
 
-def _call_schedule_notebook_api(session: Session, cron_expressions, project_id, file_path, label, user_identity):
+def _call_schedule_notebook_api(session: Session, cron_expressions: List[Tuple[Any, str]], project_id: str, file_path,
+                                label: Optional[str], user_identity: Optional[UserOutputV1],
+                                notify_on_skipped_execution: bool, notify_on_automatic_unschedule: bool) -> None:
     projects_api = ProjectsApi(session.client)
     schedule_input = ScheduledNotebookInputV1()
     schedule_input.file_path = file_path
     schedule_input.schedules = [ScheduleInputV1(key=idx, cron_schedule=cron) for idx, cron in cron_expressions]
     schedule_input.timezone = _login.get_fallback_timezone(session)
     schedule_input.label = label
+    schedule_input.notify_on_skipped_execution = notify_on_skipped_execution
+    schedule_input.notify_on_automatic_unschedule = notify_on_automatic_unschedule
     if user_identity is not None:
         schedule_input.user_id = user_identity.id
 
     projects_api.schedule_notebook(id=project_id, body=schedule_input)
 
 
-def _call_unschedule_notebook_api(session: Session, project_id, file_path, label):
+def _call_unschedule_notebook_api(session: Session, project_id: str, file_path: str, label: Optional[str]) -> None:
     if label is None:
         ProjectsApi(session.client).unschedule_notebook(id=project_id, file_path=file_path)
     else:
         ProjectsApi(session.client).unschedule_notebook(id=project_id, file_path=file_path, label=label)
 
 
 def retrieve_notebook_path(session: Session, datalab_notebook_url=None, use_private_url=True):
@@ -440,15 +473,15 @@
                 data_lab_url = _datalab.get_data_lab_orchestrator_url(use_private_url)
             else:
                 raise SPyRuntimeError('Path for Seeq Data Lab Notebook URL must include protocol and host if not '
                                       'running in Data Lab')
         return data_lab_url, project_id, file_path
 
 
-def is_referencing_this_project(datalab_notebook_url):
+def is_referencing_this_project(datalab_notebook_url: Optional[str]) -> bool:
     if datalab_notebook_url is None:
         return True
     else:
         project_url_public = _datalab.get_data_lab_project_url(use_private_url=False).lower()
         project_url_private = _datalab.get_data_lab_project_url(use_private_url=True).lower()
         return datalab_notebook_url.lower().startswith(tuple([project_url_public, project_url_private]))
 
@@ -487,39 +520,39 @@
             parts[2] = re.sub(r'(.+?)(/.+)?', rf'{int(current_slot.total_seconds() / (60 * 60))}\2', parts[2])
         new_expressions.append((idx, ' '.join(parts)))
         current_slot += spacing
 
     return new_expressions
 
 
-def _get_cron_expression_list(jobs_df):
+def _get_cron_expression_list(jobs_df: pd.DataFrame) -> List[Tuple[Any, str]]:
     if jobs_df is None or jobs_df.empty:
         return []
 
     if 'Schedule' not in jobs_df:
         schedule_column = jobs_df.columns[0]
     else:
         schedule_column = 'Schedule'
 
     return [(idx, parse_schedule_string(row[schedule_column])) for idx, row in jobs_df.iterrows()]
 
 
-def parse_schedule_string(schedule_string):
+def parse_schedule_string(schedule_string: str) -> str:
     # noinspection PyBroadException
     try:
         # If cron_descriptor can parse it, then it's a valid cron schedule already
-        cron_descriptor.get_description(schedule_string)
+        ExpressionDescriptor(schedule_string, day_of_week_start_index_zero=False).get_description()
         return schedule_string
     except BaseException:
         pass
 
     return friendly_schedule_to_quartz_cron(schedule_string)
 
 
-def friendly_schedule_to_quartz_cron(schedule_string):
+def friendly_schedule_to_quartz_cron(schedule_string: str) -> str:
     r = RecurringEvent()
     r.parse(schedule_string)
 
     rules = r.get_params()
     if len(rules) == 0 or 'freq' not in rules or 'interval' not in rules:
         raise SPyValueError(f'Could not interpret "{schedule_string}" as a schedule')
     days = {'SU': 1, 'MO': 2, 'TU': 3, 'WE': 4, 'TH': 5, 'FR': 6, 'SA': 7}
@@ -551,15 +584,15 @@
         second, minute, hour, day_of_month = convert_seconds(interval)
 
     cron = f'{second} {minute} {hour} {day_of_month} {month} {day_of_week}'
 
     return cron
 
 
-def convert_seconds(seconds_val: str) -> list:
+def convert_seconds(seconds_val: str) -> List[str]:
     """
     Convert seconds value to appropriate time value.
     If it is detected that the time value is partial it will raise an exception.
     """
 
     t = timedelta(seconds=int(seconds_val))
     time_values = {
```

### Comparing `seeq-spy-189.3/seeq/spy/notifications/_emails.py` & `seeq-spy-189.9/seeq/spy/notifications/_emails.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/utils/__init__.py` & `seeq-spy-189.9/seeq/spy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/widgets/_ipy_utils.py` & `seeq-spy-189.9/seeq/spy/widgets/_ipy_utils.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/widgets/_widgets.py` & `seeq-spy-189.9/seeq/spy/widgets/_widgets.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/workbooks/__init__.py` & `seeq-spy-189.9/seeq/spy/workbooks/__init__.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/workbooks/_annotation.py` & `seeq-spy-189.9/seeq/spy/workbooks/_annotation.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/workbooks/_content.py` & `seeq-spy-189.9/seeq/spy/workbooks/_content.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/workbooks/_data.py` & `seeq-spy-189.9/seeq/spy/workbooks/_data.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/workbooks/_folder.py` & `seeq-spy-189.9/seeq/spy/workbooks/_folder.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/workbooks/_item.py` & `seeq-spy-189.9/seeq/spy/workbooks/_item.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/workbooks/_item_map.py` & `seeq-spy-189.9/seeq/spy/workbooks/_item_map.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/workbooks/_load.py` & `seeq-spy-189.9/seeq/spy/workbooks/_load.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/workbooks/_pull.py` & `seeq-spy-189.9/seeq/spy/workbooks/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/workbooks/_push.py` & `seeq-spy-189.9/seeq/spy/workbooks/_push.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/workbooks/_render.py` & `seeq-spy-189.9/seeq/spy/workbooks/_render.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/workbooks/_report_content_utilities.py` & `seeq-spy-189.9/seeq/spy/workbooks/_report_content_utilities.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/workbooks/_save.py` & `seeq-spy-189.9/seeq/spy/workbooks/_save.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/workbooks/_search.py` & `seeq-spy-189.9/seeq/spy/workbooks/_search.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/workbooks/_template.py` & `seeq-spy-189.9/seeq/spy/workbooks/_template.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/workbooks/_user.py` & `seeq-spy-189.9/seeq/spy/workbooks/_user.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/workbooks/_workbook.py` & `seeq-spy-189.9/seeq/spy/workbooks/_workbook.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/workbooks/_worksheet.py` & `seeq-spy-189.9/seeq/spy/workbooks/_worksheet.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/workbooks/_workstep.py` & `seeq-spy-189.9/seeq/spy/workbooks/_workstep.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq/spy/workbooks/app.css` & `seeq-spy-189.9/seeq/spy/workbooks/app.css`

 * *Files identical despite different names*

### Comparing `seeq-spy-189.3/seeq_spy.egg-info/PKG-INFO` & `seeq-spy-189.9/seeq_spy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq-spy
-Version: 189.3
+Version: 189.9
 Summary: Easy-to-use Python interface for Seeq
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seeq-spy-189.3/seeq_spy.egg-info/SOURCES.txt` & `seeq-spy-189.9/seeq_spy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 seeq/spy/_redaction.py
 seeq/spy/_search.py
 seeq/spy/_session.py
 seeq/spy/_status.py
 seeq/spy/_swap.py
 seeq/spy/_upgrade.py
 seeq/spy/_url.py
+seeq/spy/_usage.py
 seeq/spy/acl/__init__.py
 seeq/spy/acl/_pull.py
 seeq/spy/acl/_push.py
 seeq/spy/addons/__init__.py
 seeq/spy/addons/_install.py
 seeq/spy/addons/_permissions.py
 seeq/spy/addons/_search.py
```

### Comparing `seeq-spy-189.3/setup.py` & `seeq-spy-189.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seeq-spy",
-    version="189.3",
+    version="189.9",
     author="Seeq Corporation",
     author_email="support@seeq.com",
     description="Easy-to-use Python interface for Seeq",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.seeq.com",
     project_urls={
```

