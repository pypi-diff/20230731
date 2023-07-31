# Comparing `tmp/cloudwatcher-0.1.2.tar.gz` & `tmp/cloudwatcher-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudwatcher-0.1.2.tar", max compression
+gzip compressed data, was "cloudwatcher-0.2.0.tar", max compression
```

## Comparing `cloudwatcher-0.1.2.tar` & `cloudwatcher-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35149 2022-04-29 13:49:17.399996 cloudwatcher-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2022-11-08 17:17:56.329911 cloudwatcher-0.1.2/cloudwatcher/__init__.py
--rw-r--r--   0        0        0      268 2022-11-08 17:17:56.332910 cloudwatcher-0.1.2/cloudwatcher/__main__.py
--rw-r--r--   0        0        0     7820 2022-11-08 17:17:56.335160 cloudwatcher-0.1.2/cloudwatcher/argparser.py
--rw-r--r--   0        0        0     4184 2022-11-23 15:54:35.903406 cloudwatcher-0.1.2/cloudwatcher/cli.py
--rw-r--r--   0        0        0     1303 2022-11-08 17:17:56.338573 cloudwatcher-0.1.2/cloudwatcher/cloudwatcher.py
--rw-r--r--   0        0        0      525 2022-11-08 17:17:56.340165 cloudwatcher-0.1.2/cloudwatcher/const.py
--rw-r--r--   0        0        0     7910 2022-11-08 17:17:56.341795 cloudwatcher-0.1.2/cloudwatcher/logwatcher.py
--rw-r--r--   0        0        0     9071 2022-11-23 20:10:05.059310 cloudwatcher-0.1.2/cloudwatcher/metric_handlers.py
--rw-r--r--   0        0        0    15096 2022-11-23 22:03:05.960148 cloudwatcher-0.1.2/cloudwatcher/metricwatcher.py
--rw-r--r--   0        0        0     7356 2022-11-23 20:10:05.063630 cloudwatcher-0.1.2/cloudwatcher/preset.py
--rw-r--r--   0        0        0      396 2022-11-23 20:10:05.065400 cloudwatcher-0.1.2/cloudwatcher/presets/nephele_cpu_usage_user.json
--rw-r--r--   0        0        0      576 2022-11-23 20:10:05.067279 cloudwatcher-0.1.2/cloudwatcher/presets/nephele_disk_used_percent.json
--rw-r--r--   0        0        0      595 2022-11-23 20:10:05.068714 cloudwatcher-0.1.2/cloudwatcher/presets/nephele_disk_used_percent_nephele_data.json
--rw-r--r--   0        0        0      290 2022-11-23 20:10:05.069888 cloudwatcher-0.1.2/cloudwatcher/presets/nephele_mem.json
--rw-r--r--   0        0        0      298 2022-11-23 20:10:05.071304 cloudwatcher-0.1.2/cloudwatcher/presets/nephele_mem_cached.json
--rw-r--r--   0        0        0      245 2022-11-08 17:17:56.356080 cloudwatcher-0.1.2/cloudwatcher/presets/nephele_processes_dead.json
--rw-r--r--   0        0        0      240 2022-11-08 17:17:56.357149 cloudwatcher-0.1.2/cloudwatcher/presets/nephele_swap_used.json
--rw-r--r--   0        0        0      250 2022-11-08 17:17:56.358427 cloudwatcher-0.1.2/cloudwatcher/presets/nephele_swap_used_percent.json
--rw-r--r--   0        0        0      814 2022-11-23 22:03:05.962760 cloudwatcher-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      936 2022-11-23 22:03:18.773189 cloudwatcher-0.1.2/setup.py
--rw-r--r--   0        0        0      700 2022-11-23 22:03:18.773452 cloudwatcher-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-04-29 13:49:17.399996 cloudwatcher-0.2.0/LICENSE
+-rw-r--r--   0        0        0        0 2022-11-08 17:17:56.329911 cloudwatcher-0.2.0/cloudwatcher/__init__.py
+-rw-r--r--   0        0        0      268 2022-11-08 17:17:56.332910 cloudwatcher-0.2.0/cloudwatcher/__main__.py
+-rw-r--r--   0        0        0     7820 2023-07-31 14:46:03.902402 cloudwatcher-0.2.0/cloudwatcher/argparser.py
+-rw-r--r--   0        0        0     4407 2023-07-31 14:46:03.903605 cloudwatcher-0.2.0/cloudwatcher/cli.py
+-rw-r--r--   0        0        0     1228 2023-07-31 14:46:03.904930 cloudwatcher-0.2.0/cloudwatcher/cloudwatcher.py
+-rw-r--r--   0        0        0      409 2023-07-31 14:46:03.905982 cloudwatcher-0.2.0/cloudwatcher/const.py
+-rw-r--r--   0        0        0    10907 2023-07-31 14:46:03.906823 cloudwatcher-0.2.0/cloudwatcher/logwatcher.py
+-rw-r--r--   0        0        0     8501 2023-07-31 14:46:03.907747 cloudwatcher-0.2.0/cloudwatcher/metric_handlers.py
+-rw-r--r--   0        0        0    15789 2023-07-31 14:46:03.908751 cloudwatcher-0.2.0/cloudwatcher/metricwatcher.py
+-rw-r--r--   0        0        0     7814 2023-07-31 14:46:03.909700 cloudwatcher-0.2.0/cloudwatcher/preset.py
+-rw-r--r--   0        0        0      397 2023-07-31 14:46:03.910436 cloudwatcher-0.2.0/cloudwatcher/presets/nephele_cpu_usage_user.json
+-rw-r--r--   0        0        0      577 2023-07-31 14:46:03.911333 cloudwatcher-0.2.0/cloudwatcher/presets/nephele_disk_used_percent.json
+-rw-r--r--   0        0        0      591 2023-07-31 14:46:03.912143 cloudwatcher-0.2.0/cloudwatcher/presets/nephele_disk_used_percent_nephele_data.json
+-rw-r--r--   0        0        0      291 2023-07-31 14:46:03.912841 cloudwatcher-0.2.0/cloudwatcher/presets/nephele_mem.json
+-rw-r--r--   0        0        0      299 2023-07-31 14:46:03.913495 cloudwatcher-0.2.0/cloudwatcher/presets/nephele_mem_cached.json
+-rw-r--r--   0        0        0      246 2023-07-31 14:46:03.914157 cloudwatcher-0.2.0/cloudwatcher/presets/nephele_processes_dead.json
+-rw-r--r--   0        0        0      241 2023-07-31 14:46:03.914932 cloudwatcher-0.2.0/cloudwatcher/presets/nephele_swap_used.json
+-rw-r--r--   0        0        0      251 2023-07-31 14:46:03.915740 cloudwatcher-0.2.0/cloudwatcher/presets/nephele_swap_used_percent.json
+-rw-r--r--   0        0        0      812 2023-07-31 14:46:03.923974 cloudwatcher-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      912 2023-07-31 15:02:11.721799 cloudwatcher-0.2.0/setup.py
+-rw-r--r--   0        0        0      662 2023-07-31 15:02:11.722137 cloudwatcher-0.2.0/PKG-INFO
```

### Comparing `cloudwatcher-0.1.2/LICENSE` & `cloudwatcher-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudwatcher-0.1.2/cloudwatcher/argparser.py` & `cloudwatcher-0.2.0/cloudwatcher/argparser.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ Computing configuration representation """
 
 import argparse
+from importlib.metadata import version
 
 from cloudwatcher.const import CLI_DEFAULTS, LOG_CMD, METRIC_CMD, SUBPARSER_MESSAGES
-from importlib.metadata import version
 
 cloudwatcher_version = version("cloudwatcher")
 
 
 class _VersionInHelpParser(argparse.ArgumentParser):
     def format_help(self):
         """Add version information to help text."""
```

### Comparing `cloudwatcher-0.1.2/cloudwatcher/cli.py` & `cloudwatcher-0.2.0/cloudwatcher/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import logging
 import os
 import sys
 
-from rich.logging import RichHandler
 from rich.console import Console
-from pathlib import Path
+from rich.logging import RichHandler
 
 from cloudwatcher.const import LOG_CMD, METRIC_CMD
 from cloudwatcher.logwatcher import LogWatcher
 
 from .argparser import build_argparser
 from .metricwatcher import MetricWatcher
-from .preset import get_metric_watcher_setup, PresetFilesInventory
+from .preset import Dimension, PresetFilesInventory, get_metric_watcher_setup
 
 
 def main():
     """
     Main entry point for the CLI.
     """
     parser = build_argparser()
@@ -80,29 +79,34 @@
         if args.plot:
             metric_watcher.save_metric_plot(
                 file_path=os.path.join(args.dir, f"{name_prefix}.png"),
                 response=response,
             )
 
         if args.uptime:
-            if not args.dimension_name == "InstanceId":
+            dimensions_list = [Dimension.from_cli(dimension_str) for dimension_str in args.dimensions]
+            for dimension in dimensions_list:
+                if dimension.Name == "InstanceId":
+                    ec2_instance_id = dimension.Value
+                    break
+            else:
                 _LOGGER.error(
                     "Uptime is only available for EC2 instances. "
                     "Please provide 'InstanceId' as dimension name and EC2 instance id"
                     " as the dimension value."
                 )
                 sys.exit(1)
             try:
                 seconds_run = metric_watcher.get_ec2_uptime(
                     days=max(
                         15, args.days
                     ),  # metrics with a period of 60 seconds are available for 15 days
                     hours=args.hours,
                     minutes=args.minutes,
-                    ec2_instance_id=args.dimension_value,
+                    ec2_instance_id=ec2_instance_id,
                 )
                 if seconds_run is not None:
                     _LOGGER.info(f"Instance uptime is {int(seconds_run)} seconds")
             except Exception as e:
                 _LOGGER.warning(f"Failed to get instance uptime ({e})")
 
     if args.command == LOG_CMD:
```

### Comparing `cloudwatcher-0.1.2/cloudwatcher/cloudwatcher.py` & `cloudwatcher-0.2.0/cloudwatcher/cloudwatcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,18 +17,18 @@
         aws_session_token: Optional[str] = None,
     ) -> None:
         """
         Initialize CloudWatcher
 
         Args:
             service_name (str): The name of the service to use
-            aws_region_name (Optional[str]): The AWS region name. Defaults to 'us-east-1'
-            aws_access_key_id (Optional[str]): The AWS access key ID. Defaults to None
-            aws_secret_access_key (Optional[str]): The AWS secret access key. Defaults to None
-            aws_session_token (Optional[str]): The AWS session token. Defaults to None
+            aws_region_name (Optional[str]): The AWS region name.
+            aws_access_key_id (Optional[str]): The AWS access key ID.
+            aws_secret_access_key (Optional[str]): The AWS secret access key.
+            aws_session_token (Optional[str]): The AWS session token.
         """
         self.aws_region_name = aws_region_name or "us-east-1"
         self.service_name = service_name
         self.client: boto3.Session.client = boto3.client(
             service_name=self.service_name,
             region_name=self.aws_region_name,
             aws_access_key_id=aws_access_key_id,
```

### Comparing `cloudwatcher-0.1.2/cloudwatcher/logwatcher.py` & `cloudwatcher-0.2.0/cloudwatcher/logwatcher.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,151 @@
-# TODO: query the AWS multiple times if query json provided
-
 import logging
 import re
 from datetime import datetime
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, Generator, List, Optional, Tuple
 
-from cloudwatcher.cloudwatcher import CloudWatcher
+from pydantic import BaseModel
 
-Event = Dict[str, str]
+from cloudwatcher.cloudwatcher import CloudWatcher
 
 _LOGGER = logging.getLogger(__name__)
 
 
+class LogEvent(BaseModel):
+    """
+    A class for AWS CloudWatch log events
+
+    Attributes:
+        message (str): The log message
+        timestamp (datetime): The log timestamp
+    """
+
+    message: str
+    timestamp: datetime
+
+    @classmethod
+    def from_response(cls, response: Dict[str, Any]) -> "LogEvent":
+        """
+        Create a LogEvent object from a response
+
+        Args:
+            response (Dict[str, Any]): The response from AWS
+
+        Returns:
+            LogEvent: The LogEvent object
+        """
+        return cls(
+            message=response["message"],
+            timestamp=datetime.fromtimestamp(response["timestamp"] / 1000),
+        )
+
+    def format_message(
+        self,
+        regex: Optional[str] = None,
+        fmt_str_log: Optional[str] = None,
+        fmt_str_datetime: Optional[str] = None,
+    ) -> "LogEvent":
+        """
+        Format the message by removing the embedded timestamp and adding a UTC timestamp
+
+        Args:
+            regex (str): regex to match the timestamp in the message
+            fmt_str_log (str): format string for the log message
+            fmt_str_datetime (str): format string for the datetime
+
+        Returns:
+            str: formatted message
+        """
+        regex = regex or r"^\[\d+-\d+-\d+\s\d+:\d+:\d+(.|,)\d+(\]|\s-\s\w+\])"
+        fmt_str_log = fmt_str_log or "[{time} UTC] {message}"
+        fmt_str_datetime = fmt_str_datetime or "%d-%m-%Y %H:%M:%S"
+        m = re.search(regex, self.message)
+        msg = self.message[m.end() :] if m else self.message
+        formatted_message = fmt_str_log.format(
+            time=self.timestamp.strftime(fmt_str_datetime), message=msg.strip()
+        )
+        return LogEvent(message=formatted_message, timestamp=self.timestamp)
+
+    def __bool__(self) -> bool:
+        """
+        Return True if the message is not empty
+
+        Returns:
+            bool: True if the message is not empty
+        """
+        return bool(self.message)
+
+
+class LogEventsList(BaseModel):
+    """
+    A class for AWS CloudWatch log events list
+
+    Attributes:
+        events (List[LogEvent]): The list of log events
+        next_forward_token (Optional[str]): The next forward token
+        next_backward_token (Optional[str]): The next backward token
+    """
+
+    events: List[LogEvent]
+    next_forward_token: Optional[str]
+    next_backward_token: Optional[str]
+
+    @classmethod
+    def from_response(cls, response: Dict[str, Any]) -> "LogEventsList":
+        """
+        Create a LogEventsList object from a response
+
+        Args:
+            response (Dict[str, Any]): The response from AWS
+
+        Returns:
+            LogEventsList: The LogEventsList object
+        """
+        return cls(
+            events=[LogEvent.from_response(event) for event in response["events"]],
+            next_forward_token=response.get("nextForwardToken"),
+            next_backward_token=response.get("nextBackwardToken"),
+        )
+
+    def format_messages(
+        self,
+        regex: Optional[str] = None,
+        fmt_str_datetime: Optional[str] = None,
+        fmt_str_log: Optional[str] = None,
+    ) -> "LogEventsList":
+        """
+        Format the messages by removing the embedded timestamp
+        and adding a UTC timestamp
+
+        Args:
+            regex (str): regex to match the timestamp in the message
+            fmt_str_log (str): format string for the log message
+            fmt_str_datetime (str): format string for the datetime
+
+        Returns:
+            LogEventsList: The LogEventsList object, with formatted messages
+        """
+        self.events = [
+            event.format_message(
+                regex=regex, fmt_str_datetime=fmt_str_datetime, fmt_str_log=fmt_str_log
+            )
+            for event in self.events
+        ]
+        return self
+
+    def __bool__(self) -> bool:
+        """
+        Return True if the events list is not empty
+
+        Returns:
+            bool: True if the events list is not empty
+        """
+        return bool(self.events)
+
+
 class LogWatcher(CloudWatcher):
     """
     A class for AWS CloudWatch log events retrieval and parsing
     """
 
     def __init__(
         self,
@@ -29,19 +159,19 @@
     ) -> None:
         """
         Initialize LogWatcher
 
         Args:
             log_group_name (str): The name of the log group
             log_stream_name (str): The name of the log stream
-            start_token (Optional[str]): The token to use for the next query. Defaults to None
-            aws_access_key_id (Optional[str]): The AWS access key ID. Defaults to None
-            aws_secret_access_key (Optional[str]): The AWS secret access key. Defaults to None
-            aws_session_token (Optional[str]): The AWS session token. Defaults to None
-            aws_region_name (Optional[str]): The AWS region name. Defaults to 'us-east-1'
+            start_token (Optional[str]): The token to use for the next query
+            aws_access_key_id (Optional[str]): The AWS access key ID
+            aws_secret_access_key (Optional[str]): The AWS secret access key
+            aws_session_token (Optional[str]): The AWS session token
+            aws_region_name (Optional[str]): The AWS region name
         """
         super().__init__(
             service_name="logs",
             aws_access_key_id=aws_access_key_id,
             aws_secret_access_key=aws_secret_access_key,
             aws_session_token=aws_session_token,
             aws_region_name=aws_region_name,
@@ -72,31 +202,32 @@
                 logStreamNamePrefix=self.log_stream_name,
             )
             return True if response["logStreams"] else False
         except Exception as e:
             _LOGGER.error(f"Error checking if log stream exists: {e}")
             return False
 
-    def _get_events(self, query_kwargs: Dict[str, Any]) -> List[Event]:
+    def _get_events(self, query_kwargs: Dict[str, Any]) -> LogEventsList:
         """
         Get events from CloudWatch and update the arguments
         for the next query with 'nextForwardToken'
 
         Args:
             query_kwargs (Dict[str, Any]): The query arguments
         Returns:
             List[Event]: The list of log events
         """
         response = self.client.get_log_events(**query_kwargs)
-        query_kwargs.update({"nextToken": response["nextForwardToken"]})
-        return response["events"], response["nextForwardToken"]
+        log_events_list = LogEventsList.from_response(response)
+        query_kwargs.update({"nextToken": log_events_list.next_forward_token})
+        return log_events_list
 
     def stream_cloudwatch_logs(
         self, events_limit: int = 1000, max_retry_attempts: int = 5
-    ) -> List[Event]:
+    ) -> Generator[LogEventsList, None, None]:
         """
         A generator that retrieves desired number of log events per iteration
 
         Args:
             events_limit (int): The number of events to retrieve per iteration.
             max_retry_attempts (int): The number of retry attempts.
         Returns:
@@ -109,110 +240,80 @@
             startFromHead=True,
         )
         if self.start_token:
             query_kwargs.update({"nextToken": self.start_token})
         _LOGGER.debug(
             f"Retrieving log events from: {self.log_group_name}/{self.log_stream_name}"
         )
-        events, token = self._get_events(query_kwargs)
-        yield events, token
-        while events:
-            events, token = self._get_events(query_kwargs)
+        log_events_list = self._get_events(query_kwargs)
+        yield log_events_list
+        while log_events_list:
+            log_events_list = self._get_events(query_kwargs)
             retry_attempts = 0
-            while not events and max_retry_attempts > retry_attempts:
-                events, token = self._get_events(query_kwargs)
+            while not log_events_list and max_retry_attempts > retry_attempts:
+                log_events_list = self._get_events(query_kwargs)
                 retry_attempts += 1
                 _LOGGER.debug(
                     f"Received empty log events list. Retry attempt: {retry_attempts}"
                 )
-            yield events, token
+            yield log_events_list
 
     def stream_formatted_logs(
         self,
         events_limit: int = 1000,
         max_retry_attempts: int = 5,
         sep: str = "<br>",
-    ) -> Tuple[List[str], str]:
+    ) -> Generator[Tuple[str, Optional[str]], None, None]:
         """
         A generator that yields formatted log events
 
         Args:
             events_limit (int): The number of events to retrieve per iteration.
             max_retry_attempts (int): The number of retry attempts.
             sep (str): The separator to use between log events.
         Returns:
             Tuple[List[str], str]: The list of formatted log events and the next token
         """
-        for events, token in self.stream_cloudwatch_logs(
+        for log_events_list in self.stream_cloudwatch_logs(
             events_limit=events_limit,
             max_retry_attempts=max_retry_attempts,
         ):
-            yield sep.join(self.format_logs_events(log_events=events)), token
+            formatted_log_events = log_events_list.format_messages().events
+            yield sep.join(
+                [event.message for event in formatted_log_events]
+            ), log_events_list.next_forward_token
 
     def return_formatted_logs(
         self, events_limit: int = 1000, max_retry_attempts: int = 5
-    ) -> Tuple[str, str]:
+    ) -> Tuple[str, Optional[str]]:
         """
         A generator that yields formatted log events
 
         Args:
             events_limit (int): The number of events to retrieve per iteration.
             max_retry_attempts (int): The number of retry attempts.
         Returns:
             Tuple[str, str]: The list of formatted log events and the next token
         """
         formatted_events = ""
-        for events, token in self.stream_cloudwatch_logs(
+        for log_events_list in self.stream_cloudwatch_logs(
             events_limit=events_limit, max_retry_attempts=max_retry_attempts
         ):
-            formatted_events += "\n".join(self.format_logs_events(log_events=events))
-        return formatted_events, token
-
-    def format_logs_events(
-        self,
-        log_events: List[Event],
-        regex: str = r"^\[\d+-\d+-\d+\s\d+:\d+:\d+(.|,)\d+(\]|\s-\s\w+\])",
-        fmt_str: str = "[{time} UTC] {message}",
-    ) -> List[str]:
-        """
-        Format log events
-
-        Args:
-            log_events (List[Event]): The list of log events.
-            regex (str): The regex to use to extract the time and message.
-            fmt_str (str): The format string to use to format the time and message.
-        """
-
-        def _datestr(timestamp: int, fmt_str: str = "%d-%m-%Y %H:%M:%S") -> str:
-            """
-            Convert milliseconds after Jan 1, 1970 UTC to a string date repr
-
-            Args:
-                timestamp (int): milliseconds after Jan 1, 1970 UTC
-                fmt_str (str): format string for the date
-            Returns:
-                str: date string
-            """
-            return datetime.fromtimestamp(timestamp / 1000.0).strftime(fmt_str)
-
-        formatted_log_list = []
-        for e in log_events:
-            m = re.search(regex, e["message"])
-            msg = e["message"][m.end() :] if m else e["message"]
-            formatted_log_list.append(
-                fmt_str.format(time=_datestr(e["timestamp"]), message=msg.strip())
+            formatted_log_events_list = log_events_list.format_messages()
+            formatted_events += "\n".join(
+                [event.message for event in formatted_log_events_list.events]
             )
-        return formatted_log_list
+        return formatted_events, formatted_log_events_list.next_forward_token
 
     def save_log_file(self, file_path: str) -> None:
         """
         Save the log file to the specified path
 
         Args:
             file_path (str): The path to save the log file to.
         """
         logs, _ = self.return_formatted_logs()
         with open(file_path, "w") as f:
             f.write(logs)
         _LOGGER.info(
             f"Logs '{self.log_group_name}/{self.log_stream_name}' saved to: {file_path}"
-        )
+        )
```

### Comparing `cloudwatcher-0.1.2/cloudwatcher/metric_handlers.py` & `cloudwatcher-0.2.0/cloudwatcher/metric_handlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import csv
 import json
 import logging
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from datetime import datetime
-from typing import List, Tuple
+from typing import Callable, List, Optional, Tuple
 
 import matplotlib.pyplot as plt
 import pytz
 from rich.console import Console
 from rich.table import Table
 
 _LOGGER = logging.getLogger(__name__)
 
 
-def convert_mem(value: int, force_suffix: str = None) -> Tuple[float, str]:
+def convert_mem(value: float, force_suffix: Optional[str] = None) -> Tuple[float, str]:
     """
     Convert memory in bytes to the highest possible, or desired memory unit
 
     Args:
         value (int): The memory in bytes
         force_suffix (str): The desired memory unit
 
@@ -32,15 +32,15 @@
         except ValueError:
             raise ValueError(f"Forced memory unit must me one of: {suffixes}")
         else:
             return value / float(pow(1024, idx)), force_suffix
     suffixIndex = 0
     while value > 1024 and suffixIndex < len(suffixes) - 1:
         suffixIndex += 1
-        value = value / 1024.0
+        value /= 1024.0
     return value, suffixes[suffixIndex]
 
 
 @dataclass
 class TimedMetric:
     """
     Timed metric object
@@ -49,65 +49,38 @@
         timestamps (List[datetime]): The timestamps of the metric
         values (List[float]): The values of the metric
         label (str): The label of the metric
     """
 
     label: str
     timestamps: List[datetime]
-    values: List[str]
+    values: List[float]
 
     def __len__(self):
         if len(self.timestamps) == len(self.values):
             return len(self.values)
         raise ValueError("The internal timed metric lengths are not equal")
 
 
-class Handler(ABC):
-    """
-    Abstract class to establish the interface for data handling
-    """
-
-    @abstractmethod
-    def __init__(self, response: dict, logger: logging.Logger) -> None:
-        """
-        Initialize the handler
-
-        Args:
-            response (dict): The response from the AWS API
-            logger (logging.Logger): The logger to use
-        """
-        pass
-
-    @abstractmethod
-    def __call__(self, target: str) -> None:
-        """
-        Execute the handler
-
-        Args:
-            target (str): The target to use for the handler
-        """
-        pass
-
-
-class ResponseHandler(Handler):
+class ResponseHandler:
     """
     Abstract class to establish the interface for a response handling
     """
 
     def __init__(self, response: dict) -> None:
         """
         Initialize the handler
 
         Args:
             response (dict): The response from the AWS API
         """
         self.response = response
 
 
-class TimedMetricHandler(Handler):
+class TimedMetricHandler:
     """
     Class to establish the interface for a timed metric handling
     """
 
     def __init__(self, timed_metric: TimedMetric) -> None:
         """
         Initialize the handler
@@ -145,14 +118,15 @@
             raise NotImplementedError(
                 "Logging responses to a file is not yet implemented."
             )
         _LOGGER.debug(json.dumps(self.response, indent=4, default=str))
 
 
 class TimedMetricPlotter(TimedMetricHandler):
+
     def __call__(self, target: str, metric_unit: str) -> None:
         """
         Plot the timed metric
 
         Args:
             target (str): The target file to save the plot to
             metric_unit (str): The unit of the metric
@@ -186,23 +160,24 @@
 
 
 class TimedMetricSummarizer(TimedMetricHandler):
     def __call__(
         self,
         target: str,
         metric_unit: str,
-        summarizer: Tuple[str, callable],
+        summarizer: Tuple[str, Callable],
     ) -> None:
         """
         Summarize the metric
 
         Args:
             target (str): The target file to save the summary to
             metric_unit (str): The unit of the metric
-            summarizer (Tuple[str, callable]): The summarizer to use and the function to use
+            summarizer (Tuple[str, callable]): The summarizer to use
+                and the function to use
         """
         if target is not None:
             raise NotImplementedError("Logging to a file is not yet implemented.")
         timespan = self.timed_metric.timestamps[0] - self.timed_metric.timestamps[-1]
         _LOGGER.info(
             f"Retrieved '{self.timed_metric.label}' {len(self.timed_metric.values)} "
             f"measurements over {timespan} timespan"
@@ -239,15 +214,15 @@
             table.add_row(
                 self.timed_metric.timestamps[i].strftime("%H:%M:%S"), values[i]
             )
         console = Console()
         console.print(table)
 
     @staticmethod
-    def mem_to_str(size: int, precision: int = 3) -> str:
+    def mem_to_str(size: float, precision: int = 3) -> str:
         """
         Convert bytes to human readable string
 
         Args:
             size (int): The size in bytes
             precision (int): The precision to use, number of decimal places
```

### Comparing `cloudwatcher-0.1.2/cloudwatcher/metricwatcher.py` & `cloudwatcher-0.2.0/cloudwatcher/metricwatcher.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,54 @@
 import datetime
 import logging
-from typing import Any, Dict, List, Optional
+from typing import Dict, List, Optional, Type
 
 import boto3
 import pytz
 
 from cloudwatcher.cloudwatcher import CloudWatcher
-from cloudwatcher.const import DEFAULT_QUERY_KWARGS
 from cloudwatcher.metric_handlers import (
-    ResponseHandler,
     ResponseLogger,
     ResponseSaver,
     TimedMetric,
     TimedMetricCsvSaver,
-    TimedMetricHandler,
     TimedMetricJsonSaver,
     TimedMetricLogger,
     TimedMetricPlotter,
     TimedMetricSummarizer,
 )
+from cloudwatcher.preset import Dimension
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class MetricWatcher(CloudWatcher):
     """
     A class for AWS CloudWatch metric retrieval and parsing
     """
 
     def __init__(
         self,
         namespace: str,
-        dimensions_list: List[Dict[str, str]],
+        dimensions_list: List[Dimension],
         metric_name: str,
         metric_id: str,
         metric_unit: Optional[str] = None,
         metric_description: Optional[str] = None,
         aws_access_key_id: Optional[str] = None,
         aws_secret_access_key: Optional[str] = None,
         aws_session_token: Optional[str] = None,
         aws_region_name: Optional[str] = None,
     ) -> None:
         """
         Initialize MetricWatcher
 
         Args:
             namespace (str): the namespace of the metric
-            dimensions_list (List[Dict[str, str]]): the dimensions of the metric
+            dimensions_list (List[Dimension]): the dimensions of the metric
             metric_name (str): the name of the metric
             metric_id (str): the ID of the metric
             metric_unit (Optional[str]): the unit of the metric
             aws_access_key_id (Optional[str]): the AWS access key ID
             aws_secret_access_key (Optional[str]): the AWS secret access key
             aws_session_token (Optional[str]): the AWS session token
             aws_region_name (Optional[str]): the AWS region name
@@ -70,23 +68,24 @@
         self.ec2_resource = boto3.resource(
             service_name="ec2",
             region_name=self.aws_region_name,
             aws_access_key_id=aws_access_key_id,
             aws_secret_access_key=aws_secret_access_key,
             aws_session_token=aws_session_token,
         )
+        self.metric_description = metric_description
 
     def query_ec2_metrics(
         self,
         days: int,
         hours: int,
         minutes: int,
         stat: str,
         period: int,
-    ) -> Dict:
+    ) -> Optional[Dict]:
         """
         Query EC2 metrics
 
         Args:
             days (int): how many days to subtract from the current date to determine
                 the metric collection start time
             hours (int): how many hours to subtract from the current time to determine
@@ -96,19 +95,28 @@
             stat (str): the statistic to query
             period (int): the period of the metric
 
         Returns:
             Dict: the response from the query, check the structure of the
             response [here](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.get_metric_data) # noqa: E501
         """
+        if self.namespace is None:
+            raise ValueError(f"Invalid metric namespace to watch: {self.namespace}")
         # Create CloudWatch client
         now = datetime.datetime.now(pytz.utc)
         start_time = now - datetime.timedelta(days=days, hours=hours, minutes=minutes)
 
-        _time = lambda x: x.strftime("%Y-%m-%d %H:%M:%S")
+        def _time(x: datetime.datetime):
+            """
+            Format a datetime object for logging
+
+            Args:
+                x (datetime.datetime): the datetime object to format
+            """
+            return x.strftime("%Y-%m-%d %H:%M:%S")
 
         _LOGGER.info(
             f"Querying '{self.metric_name}' for dimensions {self.dimensions_list} "
             f"from {_time(start_time)} to {_time(now)}"
         )
 
         response = self.client.get_metric_data(
@@ -131,39 +139,40 @@
             ],
             StartTime=start_time,
             EndTime=now,
         )
         resp_status = response["ResponseMetadata"]["HTTPStatusCode"]
         if resp_status != 200:
             _LOGGER.error(f"Invalid response status code: {resp_status}")
-            return
+            return None
         _LOGGER.debug(f"Response status code: {resp_status}")
         return response
 
     def get_ec2_uptime(
         self,
         ec2_instance_id: str,
         days: int,
         hours: int,
         minutes: int,
-    ) -> int:
+        period: int = 60,
+    ) -> Optional[float]:
         """
         Get the runtime of an EC2 instance
 
         Args:
             ec2_instance_id (str): the ID of the EC2 instance
             days (int): how many days to subtract from the current date to determine
                 the metric collection start time
             hours (int): how many hours to subtract from the current time to determine
                  the metric collection start time
             minutes (int): how many minutes to subtract from the current time to
                 determine the metric collection start time
 
         Returns:
-            int: the runtime of the EC2 instance in minutes
+            float: the runtime of the EC2 instance in minutes
         """
         if not self.is_ec2_running(ec2_instance_id):
             _LOGGER.info(
                 f"Instance '{ec2_instance_id}' is not running anymore. "
                 f"Uptime will be estimated based on reported metrics in "
                 f"the last {days} days"
             )
@@ -172,55 +181,57 @@
             )
             # get the latest reported metric
             metrics_response = self.query_ec2_metrics(
                 days=days,
                 hours=hours,
                 minutes=minutes,
                 stat="Maximum",  # any stat works
-                period=60,  # most precise period that AWS stores for instances where
-                # start time is between 3 hours and 15 days ago
+                period=period,  # most precise period that AWS stores for instances
+                # where start time is between 3 hours and 15 days ago is 60 seconds
             )
+            if metrics_response is None:
+                return None
             # extract the latest metric report time
             timed_metrics = self.timed_metric_factory(metrics_response)
             try:
                 earliest_metric_report_time = timed_metrics[-1].timestamps[0]
                 latest_metric_report_time = timed_metrics[-1].timestamps[-1]
                 return (
                     earliest_metric_report_time - latest_metric_report_time
                 ).total_seconds()
             except IndexError:
                 _LOGGER.warning(f"No metric data found for EC2: {ec2_instance_id}")
-                return
+                return None
         instances = self.ec2_resource.instances.filter(
             Filters=[{"Name": "instance-id", "Values": [ec2_instance_id]}]
         )
-        for instance in instances:
-            _LOGGER.info(
-                f"Instance '{ec2_instance_id}' is still running. "
-                f"Launch time: {instance.launch_time}"
-            )
-            return (
-                datetime.datetime.now(pytz.utc) - instance.launch_time
-            ).total_seconds()
+        if len(list(instances)) != 1:
+            raise Exception(f"Multiple EC2 instances matched by ID: {ec2_instance_id}")
+        instance = list(instances)[0]
+        _LOGGER.info(
+            f"Instance '{ec2_instance_id}' is still running. "
+            f"Launch time: {instance.launch_time}"
+        )
+        return (datetime.datetime.now(pytz.utc) - instance.launch_time).total_seconds()
 
     def is_ec2_running(self, ec2_instance_id: str) -> bool:
         """
         Check if EC2 instance is running
 
         Args:
             ec2_instance_id (str): the ID of the EC2 instance
 
         Returns:
-            bool: True if EC2 instance is running, False otherwise
+            bool: True if EC2 instance is running, False otherwise.
         """
         instances = self.ec2_resource.instances.filter(
             Filters=[{"Name": "instance-id", "Values": [ec2_instance_id]}]
         )
         if len(list(instances)) == 0:
-            return None
+            return False
         if len(list(instances)) > 1:
             raise Exception(f"Multiple EC2 instances matched by ID: {ec2_instance_id}")
         for instance in instances:
             # check the status codes and their meanings:
             # https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_InstanceState.html # noqa: E501
             if instance.state["Code"] <= 16:
                 return True
@@ -244,72 +255,85 @@
                 values=metric_data_result["Values"],
             )
             for metric_data_result in response["MetricDataResults"]
         ]
 
     def _exec_timed_metric_handler(
         self,
-        handler_class: TimedMetricHandler,
+        handler_class: Type,
         response: Optional[Dict] = None,
         query_kwargs: Optional[Dict] = None,
         **kwargs,
     ) -> None:
         """
         Internal method to execute a TimedMetricHandler
 
         Args:
             handler_class (TimedMetricHandler): the TimedMetricHandler to execute
             response (Optional[Dict]): the response from the query
             query_kwargs (Optional[Dict]): the query kwargs to use for the query
             **kwargs: additional kwargs to pass to the handler
         """
         _LOGGER.debug(f"Executing '{handler_class.__name__}'")
-        response = response or self.query_ec2_metrics(**query_kwargs)
+        if response is None:
+            if query_kwargs is not None:
+                response = self.query_ec2_metrics(**query_kwargs)
+            else:
+                raise ValueError("Either response or query_kwargs must be provided")
+        if response is None:
+            return None
         timed_metrics = self.timed_metric_factory(response)
         for timed_metric in timed_metrics:
             if len(timed_metric.values) < 1:
                 continue
             handler = handler_class(timed_metric=timed_metric)
             handler(**kwargs)
 
     def _exec_response_handler(
         self,
-        handler_class: ResponseHandler,
+        handler_class: Type,
         response: Optional[Dict] = None,
         query_kwargs: Optional[Dict] = None,
         **kwargs,
     ) -> None:
         """
         Internal method to execute a ResponseHandler
 
         Args:
             handler_class (ResponseHandler): the ResponseHandler to execute
             response (Optional[Dict]): the response from the query
             query_kwargs (Optional[Dict]): the query kwargs to use for the query
             **kwargs: additional kwargs to pass to the handler
 
         """
-        _LOGGER.debug(f"Executing '{handler_class.__name__}'")
-        response = response or self.query_ec2_metrics(**query_kwargs)
+        _LOGGER.debug(f"Executing '{handler_class.__class__.__name__}'")
+        if response is None:
+            if query_kwargs is not None:
+                response = self.query_ec2_metrics(**query_kwargs)
+            else:
+                raise ValueError("Either response or query_kwargs must be provided")
         handler = handler_class(response=response)
-        handler(**kwargs)
+        if kwargs is None:
+            handler()
+        else:
+            handler(**kwargs)
 
     def save_metric_json(
         self,
         file_path: str,
         response: Optional[Dict] = None,
         query_kwargs: Optional[Dict] = None,
     ):
         """
         Query and save the metric data to a JSON file
 
         Args:
             file_path (str): the file path to save the metric data to
             response (Optional[Dict]): the response from the query
-            query_preset (Optional[str]): the query preset to use for the query
+            query_kwargs (Optional[str]): the query preset to use for the query
         """
         self._exec_timed_metric_handler(
             TimedMetricJsonSaver,
             target=file_path,
             response=response,
             query_kwargs=query_kwargs,
         )
@@ -322,32 +346,29 @@
     ):
         """
         Query and save the metric data to a CSV file
 
         Args:
             file_path (str): the file path to save the metric data to
             response (Optional[Dict]): the response from the query
-            query_preset (Optional[str]): the query preset to use for the query
+            query_kwargs (Optional[str]): the query preset to use for the query
         """
         self._exec_timed_metric_handler(
             TimedMetricCsvSaver,
             target=file_path,
             response=response,
             query_kwargs=query_kwargs,
         )
 
-    def log_metric(
-        self, response: Optional[Dict] = None, query_preset: Optional[str] = None
-    ):
+    def log_metric(self, response: Optional[Dict] = None):
         """
         Query and log the metric data
 
         Args:
             response (Optional[Dict]): the response from the query
-            query_preset (Optional[str]): the query preset to use for the query
         """
         self._exec_timed_metric_handler(
             TimedMetricLogger,
             target=None,  # TODO: add support for saving to file
             response=response,
         )
 
@@ -359,15 +380,15 @@
     ):
         """
         Query and plot the metric data
 
         Args:
             file_path (str): the file path to save the metric data to
             response (Optional[Dict]): the response from the query
-            query_preset (Optional[str]): the query preset to use for the query
+            query_kwargs (Optional[str]): the query preset to use for the query
         """
         self._exec_timed_metric_handler(
             TimedMetricPlotter,
             target=file_path,
             metric_unit=self.metric_unit,
             response=response,
             query_kwargs=query_kwargs,
@@ -375,15 +396,14 @@
 
     def log_metric_summary(self, response: Optional[Dict] = None):
         """
         Query and summarize the metric data to a JSON file
 
         Args:
             response (Optional[Dict]): the response from the query
-            query_preset (Optional[str]): the query preset to use for the query
         """
         self._exec_timed_metric_handler(
             TimedMetricSummarizer,
             target=None,  # TODO: add support for saving to file
             metric_unit=self.metric_unit,
             summarizer=("Max", max),
             response=response,
@@ -397,29 +417,28 @@
     ):
         """
         Query and save the response data to a JSON file
 
         Args:
             file_path (str): the file path to save the response data to
             response (Optional[Dict]): the response from the query
-            query_preset (Optional[str]): the query preset to use for the query
+            query_kwargs (Optional[str]): the query preset to use for the query
         """
         self._exec_response_handler(
             ResponseSaver,
             target=file_path,
             response=response,
             query_kwargs=query_kwargs,
         )
 
     def log_response(self, response: Optional[Dict] = None):
         """
         Query and log the response
 
         Args:
             response (Optional[Dict]): the response from the query
-            query_preset (Optional[str]): the query preset to use for the query
         """
         self._exec_response_handler(
             ResponseLogger,
             target=None,
             response=response,
         )
```

### Comparing `cloudwatcher-0.1.2/cloudwatcher/preset.py` & `cloudwatcher-0.2.0/cloudwatcher/preset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-import os
 import argparse
+import json
 import logging
-from typing import List, Dict, Union
+import os
 from dataclasses import dataclass
-from pydantic import BaseModel
 from pathlib import Path
-from rich.table import Table
+from typing import Dict, List, Optional, Union
 
-from typing import List
-import json
+from pydantic import BaseModel
+from rich.table import Table
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class PresetFilesInventory:
-    def __init__(self, presets_dir: Union[Path, str] = None) -> None:
+    def __init__(self, presets_dir: Optional[Union[Path, str]] = None) -> None:
         """
         Initialize the preset inventory
 
         Args:
             presets_dir (Path): The path to the presets directory
 
         Raises:
@@ -31,15 +30,15 @@
         )
         if not preset_dir.exists():
             raise ValueError(f"Presets directory {preset_dir} does not exist")
         self._presets_dir = preset_dir
         _LOGGER.debug(f"Presets directory: {self.presets_dir}")
         self._presets = self._get_available_presets(self.presets_dir)
 
-    def _get_available_presets(self, presets_dir: Path) -> List[str]:
+    def _get_available_presets(self, presets_dir: Path) -> Dict[str, Path]:
         return {
             preset_file.stem: preset_file
             for preset_file in presets_dir.iterdir()
             if preset_file.is_file() and preset_file.suffix == ".json"
         }
 
     @property
@@ -119,32 +118,45 @@
     Value: str
 
     def __str__(self):
         return f"{self.Name}:{self.Value}"
 
     def __repr__(self):
         return self.__str__()
+    
+    @classmethod
+    def from_cli(cls, cli_arg: str):
+        """
+        Create a Dimension object from a CLI argument
+
+        Args:
+            cli_arg (str): The CLI argument
+        """
+        name, value = cli_arg.split(":")
+        if name is None or value is None:
+            raise ValueError(f"Invalid dimension: {cli_arg}. Unable to parse.")
+        return cls(Name=name, Value=value)
 
 
 @dataclass
 class MetricWatcherSetup:
     """
     A class for the setup of the MetricWatcher
     """
 
     namespace: str
     dimensions_list: List[Dimension]
     metric_name: str
     metric_id: str
     metric_unit: str
-    aws_access_key_id: str = None
-    aws_secret_access_key: str = None
-    aws_session_token: str = None
-    aws_region_name: str = None
-    metric_description: str = None
+    aws_access_key_id: Optional[str] = None
+    aws_secret_access_key: Optional[str] = None
+    aws_session_token: Optional[str] = None
+    aws_region_name: Optional[str] = None
+    metric_description: Optional[str] = None
 
     def __post_init__(self):
         self.aws_access_key_id = self.aws_access_key_id or os.environ.get(
             "AWS_ACCESS_KEY_ID"
         )
         self.aws_secret_access_key = self.aws_secret_access_key or os.environ.get(
             "AWS_SECRET_ACCESS_KEY"
@@ -166,15 +178,15 @@
 
         Args:
             data (dict): The dictionary to use
         """
         return cls(**data)
 
     @classmethod
-    def from_json(cls, file_path: str) -> "MetricWatcherSetup":
+    def from_json(cls, file_path: Path) -> "MetricWatcherSetup":
         """
         Create a MetricWatcherSetup object from a JSON file
 
         Args:
             file_path (str): The path to the JSON file
         """
         with open(file_path) as f:
@@ -186,20 +198,20 @@
         Convert the MetricWatcherSetup object to a dictionary
 
         Returns:
             dict: The dictionary representation of the object
         """
         return self.__dict__
 
-    def upsert_dimensions(self, dimensions_specs: List[str] = None):
+    def upsert_dimensions(self, dimensions_specs: Optional[List[str]] = None):
         """
         Upsert the dimensions list with the dimensions specified in the environment
 
         Args:
-            dimensions_spec (List[str]): A list of strings in the format of "Name:Value"
+            dimensions_specs (List[str]): A list of strings. Format: "Name:Value"
         """
         if dimensions_specs is None:
             return
         for dimension_spec in dimensions_specs:
             name, value = dimension_spec.split(":")
             for dimension in self.dimensions_list:
                 if dimension.Name == name:
```

### Comparing `cloudwatcher-0.1.2/cloudwatcher/presets/nephele_disk_used_percent.json` & `cloudwatcher-0.2.0/cloudwatcher/presets/nephele_disk_used_percent.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9947916666666666%*

 * *Differences: {"'dimensions_list'": "{3: {'Value': 'nvme0n1p1'}}"}*

```diff
@@ -10,15 +10,15 @@
         },
         {
             "Name": "fstype",
             "Value": "ext4"
         },
         {
             "Name": "device",
-            "Value": "nvme2n1p1"
+            "Value": "nvme0n1p1"
         }
     ],
     "metric_description": "Percentage of disk used over time. Path: <code>/</code> (root)",
     "metric_id": "root",
     "metric_name": "disk_used_percent",
     "metric_unit": "Percent",
     "namespace": "NepheleNamespaceEC2"
```

### Comparing `cloudwatcher-0.1.2/cloudwatcher/presets/nephele_disk_used_percent_nephele_data.json` & `cloudwatcher-0.2.0/cloudwatcher/presets/nephele_disk_used_percent_nephele_data.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'metric_id'": "'nephele'"}*

```diff
@@ -14,12 +14,12 @@
         },
         {
             "Name": "device",
             "Value": "md0"
         }
     ],
     "metric_description": "Percentage of disk used over time. Path: <code>/nephele_data</code>",
-    "metric_id": "nephele_data",
+    "metric_id": "nephele",
     "metric_name": "disk_used_percent",
     "metric_unit": "Percent",
     "namespace": "NepheleNamespaceEC2"
 }
```

### Comparing `cloudwatcher-0.1.2/pyproject.toml` & `cloudwatcher-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "cloudwatcher"
-version = "0.1.2"
+version = "0.2.0"
 description = "A tool for monitoring AWS CloudWatch metrics"
 authors = ["Michal Stolarczyk <stolarczyk.michal93@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-rich = "^12.2.0"
-black = "^22.3.0"
-matplotlib = "^3.5.1"
-pytz = "^2022.1"
-boto3 = "^1.21.46"
-pydantic = "^1.10.2"
+rich = "~12.2.0"
+matplotlib = "~3.5.1"
+pytz = "~2022.1"
+boto3 = "~1.26.62"
+pydantic = "~1.10.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.1"
 pre-commit = "^2.18.1"
 ipython = "7.32.0"
 ipykernel = "^6.13.0"
 nbconvert = "^6.5.0"
 black = {extras = ["jupyter"], version = "^22.3.0"}
-mkdocstrings = {extras = ["python"], version = "^0.19.0"}
-mkdocs-material = "^8.3.4"
+mkdocstrings = {extras = ["python"], version = "^0.20.0"}
+mkdocs-material = "^9.0.0"
 notebook = "^6.5.2"
 python-dotenv = "^0.21.0"
+mypy = "^1.4.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 cloudwatcher = 'cloudwatcher.__main__:main'
```

### Comparing `cloudwatcher-0.1.2/setup.py` & `cloudwatcher-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,27 +4,26 @@
 packages = \
 ['cloudwatcher']
 
 package_data = \
 {'': ['*'], 'cloudwatcher': ['presets/*']}
 
 install_requires = \
-['black>=22.3.0,<23.0.0',
- 'boto3>=1.21.46,<2.0.0',
- 'matplotlib>=3.5.1,<4.0.0',
- 'pydantic>=1.10.2,<2.0.0',
- 'pytz>=2022.1,<2023.0',
- 'rich>=12.2.0,<13.0.0']
+['boto3>=1.26.62,<1.27.0',
+ 'matplotlib>=3.5.1,<3.6.0',
+ 'pydantic>=1.10.2,<1.11.0',
+ 'pytz>=2022.1,<2022.2',
+ 'rich>=12.2.0,<12.3.0']
 
 entry_points = \
 {'console_scripts': ['cloudwatcher = cloudwatcher.__main__:main']}
 
 setup_kwargs = {
     'name': 'cloudwatcher',
-    'version': '0.1.2',
+    'version': '0.2.0',
     'description': 'A tool for monitoring AWS CloudWatch metrics',
     'long_description': None,
     'author': 'Michal Stolarczyk',
     'author_email': 'stolarczyk.michal93@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `cloudwatcher-0.1.2/PKG-INFO` & `cloudwatcher-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: cloudwatcher
-Version: 0.1.2
+Version: 0.2.0
 Summary: A tool for monitoring AWS CloudWatch metrics
 Author: Michal Stolarczyk
 Author-email: stolarczyk.michal93@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: black (>=22.3.0,<23.0.0)
-Requires-Dist: boto3 (>=1.21.46,<2.0.0)
-Requires-Dist: matplotlib (>=3.5.1,<4.0.0)
-Requires-Dist: pydantic (>=1.10.2,<2.0.0)
-Requires-Dist: pytz (>=2022.1,<2023.0)
-Requires-Dist: rich (>=12.2.0,<13.0.0)
+Requires-Dist: boto3 (>=1.26.62,<1.27.0)
+Requires-Dist: matplotlib (>=3.5.1,<3.6.0)
+Requires-Dist: pydantic (>=1.10.2,<1.11.0)
+Requires-Dist: pytz (>=2022.1,<2022.2)
+Requires-Dist: rich (>=12.2.0,<12.3.0)
```

