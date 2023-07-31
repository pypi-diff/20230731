# Comparing `tmp/sqs-workers-0.5.8.tar.gz` & `tmp/sqs_workers-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqs-workers-0.5.8.tar", max compression
+gzip compressed data, was "sqs_workers-0.5.9.tar", max compression
```

## Comparing `sqs-workers-0.5.8.tar` & `sqs_workers-0.5.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1062 2022-08-31 14:05:52.505571 sqs-workers-0.5.8/LICENSE
--rw-r--r--   0        0        0    16748 2022-08-31 14:05:52.505571 sqs-workers-0.5.8/README.md
--rw-r--r--   0        0        0      914 2022-08-31 14:05:52.509571 sqs-workers-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      689 2022-08-31 14:05:52.509571 sqs-workers-0.5.8/sqs_workers/__init__.py
--rw-r--r--   0        0        0     3162 2022-08-31 14:05:52.509571 sqs-workers-0.5.8/sqs_workers/async_task.py
--rw-r--r--   0        0        0     1443 2022-08-31 14:05:52.509571 sqs-workers-0.5.8/sqs_workers/backoff_policies.py
--rw-r--r--   0        0        0     1265 2022-08-31 14:05:52.509571 sqs-workers-0.5.8/sqs_workers/batching.py
--rw-r--r--   0        0        0     1023 2022-08-31 14:05:52.509571 sqs-workers-0.5.8/sqs_workers/codecs.py
--rw-r--r--   0        0        0     1556 2022-08-31 14:05:52.509571 sqs-workers-0.5.8/sqs_workers/config.py
--rw-r--r--   0        0        0     2802 2022-08-31 14:05:52.509571 sqs-workers-0.5.8/sqs_workers/context.py
--rw-r--r--   0        0        0     1984 2022-08-31 14:05:52.509571 sqs-workers-0.5.8/sqs_workers/core.py
--rw-r--r--   0        0        0     2055 2022-08-31 14:05:52.509571 sqs-workers-0.5.8/sqs_workers/deadletter_queue.py
--rw-r--r--   0        0        0       36 2022-08-31 14:05:52.509571 sqs-workers-0.5.8/sqs_workers/exceptions.py
--rw-r--r--   0        0        0     7947 2022-08-31 14:05:52.509571 sqs-workers-0.5.8/sqs_workers/memory_sqs.py
--rw-r--r--   0        0        0     4616 2022-08-31 14:05:52.509571 sqs-workers-0.5.8/sqs_workers/processors.py
--rw-r--r--   0        0        0    19698 2022-08-31 14:05:52.509571 sqs-workers-0.5.8/sqs_workers/queue.py
--rw-r--r--   0        0        0     2919 2022-08-31 14:05:52.509571 sqs-workers-0.5.8/sqs_workers/shutdown_policies.py
--rw-r--r--   0        0        0     5469 2022-08-31 14:05:52.509571 sqs-workers-0.5.8/sqs_workers/sqs_env.py
--rw-r--r--   0        0        0     2076 2022-08-31 14:05:52.509571 sqs-workers-0.5.8/sqs_workers/sqs_manage.py
--rw-r--r--   0        0        0     4478 2022-08-31 14:05:52.509571 sqs-workers-0.5.8/sqs_workers/utils.py
--rw-r--r--   0        0        0    18085 1970-01-01 00:00:00.000000 sqs-workers-0.5.8/setup.py
--rw-r--r--   0        0        0    17670 1970-01-01 00:00:00.000000 sqs-workers-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-01-11 15:16:04.435091 sqs_workers-0.5.9/LICENSE
+-rw-r--r--   0        0        0    17511 2023-01-11 15:16:04.435091 sqs_workers-0.5.9/README.md
+-rw-r--r--   0        0        0      914 2023-01-11 15:16:04.435091 sqs_workers-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      689 2023-01-11 15:16:04.435091 sqs_workers-0.5.9/sqs_workers/__init__.py
+-rw-r--r--   0        0        0     3110 2023-01-11 15:16:04.435091 sqs_workers-0.5.9/sqs_workers/async_task.py
+-rw-r--r--   0        0        0     1443 2023-01-11 15:16:04.435091 sqs_workers-0.5.9/sqs_workers/backoff_policies.py
+-rw-r--r--   0        0        0     1265 2023-01-11 15:16:04.435091 sqs_workers-0.5.9/sqs_workers/batching.py
+-rw-r--r--   0        0        0     1530 2023-01-11 15:16:04.435091 sqs_workers-0.5.9/sqs_workers/codecs.py
+-rw-r--r--   0        0        0     1556 2023-01-11 15:16:04.435091 sqs_workers-0.5.9/sqs_workers/config.py
+-rw-r--r--   0        0        0     2802 2023-01-11 15:16:04.435091 sqs_workers-0.5.9/sqs_workers/context.py
+-rw-r--r--   0        0        0     1984 2023-01-11 15:16:04.435091 sqs_workers-0.5.9/sqs_workers/core.py
+-rw-r--r--   0        0        0     2055 2023-01-11 15:16:04.435091 sqs_workers-0.5.9/sqs_workers/deadletter_queue.py
+-rw-r--r--   0        0        0       36 2023-01-11 15:16:04.435091 sqs_workers-0.5.9/sqs_workers/exceptions.py
+-rw-r--r--   0        0        0     7947 2023-01-11 15:16:04.435091 sqs_workers-0.5.9/sqs_workers/memory_sqs.py
+-rw-r--r--   0        0        0     4616 2023-01-11 15:16:04.435091 sqs_workers-0.5.9/sqs_workers/processors.py
+-rw-r--r--   0        0        0    19986 2023-01-11 15:16:04.435091 sqs_workers-0.5.9/sqs_workers/queue.py
+-rw-r--r--   0        0        0     2919 2023-01-11 15:16:04.435091 sqs_workers-0.5.9/sqs_workers/shutdown_policies.py
+-rw-r--r--   0        0        0     5577 2023-01-11 15:16:04.435091 sqs_workers-0.5.9/sqs_workers/sqs_env.py
+-rw-r--r--   0        0        0     2076 2023-01-11 15:16:04.435091 sqs_workers-0.5.9/sqs_workers/sqs_manage.py
+-rw-r--r--   0        0        0     4478 2023-01-11 15:16:04.435091 sqs_workers-0.5.9/sqs_workers/utils.py
+-rw-r--r--   0        0        0    18862 1970-01-01 00:00:00.000000 sqs_workers-0.5.9/setup.py
+-rw-r--r--   0        0        0    18484 1970-01-01 00:00:00.000000 sqs_workers-0.5.9/PKG-INFO
```

### Comparing `sqs-workers-0.5.8/LICENSE` & `sqs_workers-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sqs-workers-0.5.8/README.md` & `sqs_workers-0.5.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -420,14 +420,27 @@
     >>> foo.copy_processors(foo_dead)
     >>>
     >>> from sqs_workers.shutdown_policies IdleShutdown
     >>> foo_dead.process_queue(shutdown_policy=IdleShutdown(10))
 
 This code takes all the messages in the foo_dead queue and executes them with processors from the "foo" queue. Then it waits 10 seconds to ensure no new messages appear, and quit.
 
+## Codecs
+
+Before being added to SQS, task parameters are encoded using a `Codec`. At the moment, 3 codecs are available:
+- `pickle`: serialize with Pickle, using the default protocol version;
+- `pickle_compat`: serialize with Pickle, using protocol version 2, which is compatible with Python 2;
+- `json`: serialize with JSON.
+
+By default, `pickle_compat` is used, for backward compatibility with previous versions of sqs-workers.
+
+JSON is recommended if using untrusted data (see the notes about security in the [pickle docs](https://docs.python.org/3/library/pickle.html), or for compatibility with other systems. In all other cases, you should use `pickle` instead of `pickle_compat`, as it's more compact and efficient:
+
+    >>> env = SQSEnv(codec="pickle")
+
 ## Using in unit tests with MemorySession
 
 There is a special MemorySession, which can be used as a quick and dirty replacement for real queues in unit tests. If you have a function `create_task` which adds some tasks to the queue and you want to test how it works, you can technically write your tests like this:
 
 ```python
 from sqs_workers import SQSEnv
 env = SQSEnv()
```

### Comparing `sqs-workers-0.5.8/pyproject.toml` & `sqs_workers-0.5.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqs-workers"
-version = "0.5.8"
+version = "0.5.9"
 description = "An opinionated queue processor for Amazon SQS"
 authors = ["Doist Developers <dev@doist.com>"]
 license = "MIT"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `sqs-workers-0.5.8/sqs_workers/__init__.py` & `sqs_workers-0.5.9/sqs_workers/__init__.py`

 * *Files identical despite different names*

### Comparing `sqs-workers-0.5.8/sqs_workers/async_task.py` & `sqs_workers-0.5.9/sqs_workers/async_task.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from contextlib import contextmanager
 from typing import TYPE_CHECKING, Callable
 
-from sqs_workers.codecs import DEFAULT_CONTENT_TYPE
 from sqs_workers.utils import bind_arguments
 
 if TYPE_CHECKING:
     from sqs_workers.queue import JobQueue
 
 
 class AsyncTask(object):
@@ -46,15 +45,15 @@
         with self.queue.add_batch():
             yield
 
     def delay(self, *args, **kwargs):
         """
         Run the task asynchronously.
         """
-        _content_type = kwargs.pop("_content_type", DEFAULT_CONTENT_TYPE)
+        _content_type = kwargs.pop("_content_type", self.queue.env.codec)
         _delay_seconds = kwargs.pop("_delay_seconds", None)
         _deduplication_id = kwargs.pop("_deduplication_id", None)
         _group_id = kwargs.pop("_group_id", None)
 
         if self.queue.batching_policy.batching_enabled:
             if len(args) > 0:
                 raise TypeError("Must use keyword arguments only for batch read queues")
```

### Comparing `sqs-workers-0.5.8/sqs_workers/backoff_policies.py` & `sqs_workers-0.5.9/sqs_workers/backoff_policies.py`

 * *Files identical despite different names*

### Comparing `sqs-workers-0.5.8/sqs_workers/batching.py` & `sqs_workers-0.5.9/sqs_workers/batching.py`

 * *Files identical despite different names*

### Comparing `sqs-workers-0.5.8/sqs_workers/config.py` & `sqs_workers-0.5.9/sqs_workers/config.py`

 * *Files identical despite different names*

### Comparing `sqs-workers-0.5.8/sqs_workers/context.py` & `sqs_workers-0.5.9/sqs_workers/context.py`

 * *Files identical despite different names*

### Comparing `sqs-workers-0.5.8/sqs_workers/core.py` & `sqs_workers-0.5.9/sqs_workers/core.py`

 * *Files identical despite different names*

### Comparing `sqs-workers-0.5.8/sqs_workers/deadletter_queue.py` & `sqs_workers-0.5.9/sqs_workers/deadletter_queue.py`

 * *Files identical despite different names*

### Comparing `sqs-workers-0.5.8/sqs_workers/memory_sqs.py` & `sqs_workers-0.5.9/sqs_workers/memory_sqs.py`

 * *Files identical despite different names*

### Comparing `sqs-workers-0.5.8/sqs_workers/processors.py` & `sqs_workers-0.5.9/sqs_workers/processors.py`

 * *Files identical despite different names*

### Comparing `sqs-workers-0.5.8/sqs_workers/queue.py` & `sqs_workers-0.5.9/sqs_workers/queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -473,24 +473,26 @@
                 for error in errors:
                     error["_message"] = msg_by_id[error["Id"]]
                 raise SQSBatchError(errors)
 
     def add_job(
         self,
         job_name,
-        _content_type=codecs.DEFAULT_CONTENT_TYPE,
+        _content_type=None,
         _delay_seconds=None,
         _deduplication_id=None,
         _group_id=None,
         **job_kwargs
     ):
         """
         Add job to the queue. The body of the job will be converted to the text
-        with one of the codes (by default it's "pickle")
+        with one of the codecs (by default it's "pickle_compat")
         """
+        if not _content_type:
+            _content_type = self.env.codec
         codec = codecs.get_codec(_content_type)
         message_body = codec.serialize(job_kwargs)
         job_context = codec.serialize(self.env.context.to_dict())
         return self.add_raw_job(
             job_name,
             message_body,
             job_context,
@@ -577,15 +579,22 @@
             else:
                 result = self.process_message_fallback(job_name)
                 results.append(result)
 
         return all(results)
 
     def process_message_fallback(self, job_name):
-        logger.warning("Error while processing %s.%s", self.name, job_name)
+        # Note: we don't set exc_info=True, since source of the error is almost
+        # certainly in another code base.
+        logger.error(
+            "Could not find an SQS processor for %s.%s. "
+            "Has it been registered correctly?",
+            self.name,
+            job_name,
+        )
         return False
 
     def copy_processors(self, dst_queue: "JobQueue"):
         """
         Copy processors from self to dst_queue. Can be helpful to process d
         ead-letter queue with processors from the main queue.
```

### Comparing `sqs-workers-0.5.8/sqs_workers/shutdown_policies.py` & `sqs_workers-0.5.9/sqs_workers/shutdown_policies.py`

 * *Files identical despite different names*

### Comparing `sqs-workers-0.5.8/sqs_workers/sqs_env.py` & `sqs_workers-0.5.9/sqs_workers/sqs_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 AnyQueue = Union[GenericQueue, JobQueue, RawQueue]
 
 
 @attr.s
 class SQSEnv(object):
     session = attr.ib(default=boto3)
     queue_prefix = attr.ib(default="")
+    codec: str = attr.ib(default=codecs.DEFAULT_CONTENT_TYPE)
 
     # queue-specific settings
     backoff_policy = attr.ib(default=DEFAULT_BACKOFF)
 
     # jobqueue-specific settings
     processor_maker = attr.ib(default=processors.Processor)
     context_maker = attr.ib(default=context.SQSContext)
@@ -88,27 +89,29 @@
         q: RawQueue = self.queue(queue_name, queue_maker=RawQueue)  # type: ignore
         return q.raw_processor()
 
     def add_job(
         self,
         queue_name,
         job_name,
-        _content_type=codecs.DEFAULT_CONTENT_TYPE,
+        _content_type=None,
         _delay_seconds=None,
         _deduplication_id=None,
         _group_id=None,
         **job_kwargs,
     ):
         """
         Add job to the queue.
         """
         warnings.warn(
             "sqs.add_job() is deprecated. Use sqs.queue(...).add_job() instead",
             DeprecationWarning,
         )
+        if not _content_type:
+            _content_type = self.codec
         q = self.queue(queue_name, queue_maker=JobQueue)  # type: JobQueue
         return q.add_job(
             job_name,
             _content_type=_content_type,
             _delay_seconds=_delay_seconds,
             _deduplication_id=_deduplication_id,
             _group_id=_group_id,
```

### Comparing `sqs-workers-0.5.8/sqs_workers/sqs_manage.py` & `sqs_workers-0.5.9/sqs_workers/sqs_manage.py`

 * *Files identical despite different names*

### Comparing `sqs-workers-0.5.8/sqs_workers/utils.py` & `sqs_workers-0.5.9/sqs_workers/utils.py`

 * *Files identical despite different names*

### Comparing `sqs-workers-0.5.8/setup.py` & `sqs_workers-0.5.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['attrs>=22.1.0,<23.0.0', 'boto3>=1.24.62,<2.0.0']
 
 setup_kwargs = {
     'name': 'sqs-workers',
-    'version': '0.5.8',
+    'version': '0.5.9',
     'description': 'An opinionated queue processor for Amazon SQS',
-    'long_description': '# SQS Workers\n\nAn opinionated queue processor for Amazon SQS.\n\n## Usage\n\nInstall the package with\n\n```bash\npip install sqs-workers\n```\n\nConfigure your boto3 library to provide access requisites for your installation with [something like this](https://boto3.readthedocs.io/en/latest/guide/quickstart.html#configuration):\n\n```bash\naws configure\n```\n\nDon\'t forget to set your preferred AWS region.\n\nThen you will start managing two systems (most likely, from the same codebase): one of them adds messages to the queue, and another one executes them.\n\n```python\nfrom sqs_workers import SQSEnv, create_standard_queue\n\n# This environment will use AWS requisites from ~/.aws/ directory\nsqs = SQSEnv()\n\n# Create a new queue.\n# Note that you can use the AWS web interface for the same action as well, the\n# web interface provides more options. You only need to do it once.\ncreate_standard_queue(sqs, "emails")\n\n# Get the queue object\nqueue = sqs.queue("emails")\n\n# Register a queue processor\n@queue.processor("send_email")\ndef send_email(to, subject, body):\n    print(f"Sending email {subject} to {to}")\n```\n\nThen there are two ways of adding tasks to the queue. Classic (aka "explicit"):\n\n```python\nqueue.add_job("send_email", to="user@example.com", subject="Hello world", body="hello world")\n```\n\nAnd the "Celery way" (we mimic the Celery API to some extent)\n\n```python\nsend_email.delay(to="user@example.com", subject="Hello world", body="hello world")\n```\n\nTo process the queue, you have to run workers manually. Create a new file which will contain the definition of the sqs object and register all processors (most likely, by importing necessary modules from your project), and then run SQS\n\n```python\nfrom sqs_workers import SQSEnv\nsqs = SQSEnv()\n...\nsqs.queue(\'emails\').process_queue()\n```\n\nIn production, we usually don\'t handle multiple queues in the same process, but for the development environment it\'s easier to tackle with all the queues at once with\n\n```python\nsqs.process_queues()\n```\n\n## Serialization\n\nThere are two serializers: JSON and pickle.\n\n## Baked tasks\n\nYou can create so-called "baked async tasks," entities which, besides the task itself, contain arguments which have to be used to call the task.\n\nThink of baked tasks as of light version of [Celery signatures](http://docs.celeryproject.org/en/latest/userguide/canvas.html#signatures)\n\n```python\ntask = send_email.bake(to=\'user@example.com\', subject=\'Hello world\', body=\'hello world\')\ntask.delay()\n```\n\nIs the same as\n\n```python\nsend_email.delay(to=\'user@example.com\', subject=\'Hello world\', body=\'hello world\')\n```\n\n## Batch Writes\n\nIf you have many tasks to enqueue, it may be more efficient to use batching when adding them:\n\n```python\n# Classic ("explicit") API\nwith queue.add_batch():\n    queue.add_job("send_email", to="user1@example.com", subject="Hello world", body="hello world")\n    queue.add_job("send_email", to="user2@example.com", subject="Hello world", body="hello world")\n\n# "Celery way"\nwith send_email.batch():\n    send_email.delay(to="user1@example.com", subject="Hello world", body="hello world")\n    send_email.delay(to="user2@example.com", subject="Hello world", body="hello world")\n```\n\nWhen batching is enabled:\n\n- tasks are added to SQS by batches of 10, reducing the number of AWS operations\n- it is not possible to get the task `MessageId`, as it is not known until the batch is sent\n- care has to be taken about message size, as SQS limits both the individual message size and the maximum total payload size to 256 kB.\n\n## Batch Reads\n\nIf you wish to consume and process batches of messages from a queue at once (say to speed up ingestion)\nyou can set the `batching_policy` at queue level.\n\nThe underlying function is expected to have a single parameter which will receive the list of messages.\n\n```python\nfrom sqs_workers.batching import BatchMessages\nfrom sqs_workers import SQSEnv, create_standard_queue\n\nsqs = SQSEnv()\n\ncreate_standard_queue(sqs, "emails")\n\nqueue = sqs.queue("emails", batching_policy=BatchMessages(batch_size=10))\n\n@queue.processor("send_email")\ndef send_email(messages: list):\n    for email in messages:\n        print(f"Sending email {email[\'subject\']} to {email[\'to\']}")\n```\n\nThis function will receive up to 10 messages at once based on:\n\n* How many are available on the queue being consumed\n* How many of those messages on the `emails` queue are for the `send_email` job\n\n## Synchronous task execution\n\nIn Celery, you can run any task synchronously if you just call it as a function with arguments. Our AsyncTask raises a RuntimeError for this case.\n\n```python\nsend_email(to=\'user@example.com\', subject=\'Hello world\', body=\'hello world\')\n...\nRuntimeError: Async task email.send_email called synchronously (probably,\nby mistake). Use either AsyncTask.run(...) to run the task synchronously\nor AsyncTask.delay(...) to add it to the queue.\n```\n\nIf you want to run a task synchronously, use `run()` method of the task.\n\n```\nsend_email.run(to=\'user@example.com\', subject=\'Hello world\', body=\'hello world\')\n```\n\n## FIFO queues\n\nFifo queues can be created with `create_fifo_queue` and have to have the name, which ends with ".fifo".\n\n```python\nfrom sqs_workers import SQSEnv, create_fifo_queue\nsqs = SQSEnv()\n\ncreate_fifo_queue(sqs, \'emails_dead.fifo\')\ncreate_fifo_queue(sqs, \'emails.fifo\',\n    redrive_policy=sqs.redrive_policy(\'emails_dead.fifo\', 3)\n)\n```\n\nUnless the flag `content_based_deduplication` is set, every message has to be sent with an attribute `_deduplication_id`. By default, all messages have the same message group `default`, but you can change it with `_group_id`.\n\n```python\nsqs.queue("emails.fifo").add_job(\n    \'send_email\', _deduplication_id=subject, _group_id=email, **kwargs)\n```\n\n[More about FIFO queues on AWS](https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/FIFO-queues.html)\n\n## Exception processing\n\nIf task processing ended up with an exception, the error is logged, and the task is returned back to the queue after a while. The exact behavior is defined by queue settings.\n\n## Custom processors\n\nYou can define your own processor if you need to perform some specific actions before of after executing a particular task.\n\nExample for the custom processor\n\n```python\nfrom sqs_workers import SQSEnv\nfrom sqs_workers.processors import Processor\n\nclass CustomProcessor(Processor):\n    def process(self, job_kwargs):\n        print(f\'Processing {self.queue_name}.{self.job_name} with {job_kwargs}\')\n        super(CustomProcessor, self).process(job_kwargs)\n\nsqs = SQSEnv(processor_maker=CustomProcessor)\n```\n\n## Working with contexts\n\nContext is implicitly passed to the worker via the job message and can be used for logging or profiling purposes.\n\nUsage example.\n\n```python\nqueue = sqs.queue("q1")\n\n@queue.processor(\'q1\', \'hello_world\', pass_context=True)\ndef hello_world(username=None, context=None):\n    print(f\'Hello {username} from {context["remote_addr"]}\')\n\nwith sqs.context(remote_addr=\'127.0.0.1\'):\n    hello_world.delay(username=\'Foo\')\n\nqueue.process_batch()\n```\n\nAlternatively, you can set a context like this.\n\n```python\nsqs.context[\'remote_addr\'] = \'127.0.0.1\'\nhello_world.delay(username=\'Foo\')\n```\n\nAnd then, when the context needs to be cleared:\n\n```python\nsqs.context.clear()\n```\n\nIn a web application, you usually call it at the end of the processing of the web request.\n\n## Automatic applying of the context for all tasks\n\nInstead of dealing with the context inside every processing function, you can perform this in processors by subclassing them.\n\n```python\nimport os\nfrom sqs_workers import SQSEnv\nfrom sqs_workers.processors import Processor\n\nclass CustomProcessor(Processor):\n    def process(self, job_kwargs, job_context):\n        os.environ[\'REMOTE_ADDR\'] = job_context[\'remote_addr\']\n        super(CustomProcessor, self).process(job_kwargs, job_context)\n        os.unsetenv(\'REMOTE_ADDR\')\n\nsqs = SQSEnv(\n    processor_maker=CustomProcessor,\n)\n```\n\n## Raw queues\n\nRaw queues can have only one processor, which should be a function, accepting the message as its only argument.\n\nRaw queues are helpful to process messages, added to SQS from external sources, such as CloudWatch events.\n\nYou start the processor the same way, creating a new standard queue if needed.\n\n```python\nfrom sqs_workers import SQSEnv, create_standard_queue\nsqs = SQSEnv()\ncreate_standard_queue(sqs, \'cron\')\n```\n\nThen you get a queue, but provide a queue_maker parameter to it, to create a queue of the necessary type, and define a processor for it.\n\n```python\nfrom sqs_workers import RawQueue\n\ncron = sqs.queue(\'cron\', RawQueue)\n\n@cron.raw_processor()\ndef processor(message):\n    print(message.body)\n```\n\nThen start processing your queue as usual:\n\n```python\ncron.process_queue()\n```\n\nYou can also send raw messages to the queue, but this is probably less useful:\n\n```python\ncron.add_raw_job("Hello world")\n```\n\n## Processing Messages from CloudWatch\n\nBy default message body by CloudWatch scheduler has following JSON structure.\n\n```json\n{\n  "version": "0",\n  "id": "a9a10406-9a1f-0ddc-51ae-08db551fac42",\n  "detail-type": "Scheduled Event",\n  "source": "aws.events",\n  "account": "NNNNNNNNNN",\n  "time": "2019-09-20T09:19:56Z",\n  "region": "eu-west-1",\n  "resources": ["arn:aws:events:eu-west-1:NNNNNNNNNN:rule/Playground"],\n  "detail": {}\n}\n```\n\nHeaders of the message:\n\n```python\n{\n    \'SenderId\': \'AIDAJ2E....\',\n    \'ApproximateFirstReceiveTimestamp\': \'1568971264367\',\n    \'ApproximateReceiveCount\': \'1\',\n    \'SentTimestamp\': \'1568971244845\',\n}\n```\n\nYou can pass any valid JSON as a message, though, and it will be passed as-is to the message body. Something like this:\n\n```json\n{ "message": "Hello world" }\n```\n\n## Dead-letter queues and redrive\n\nOn creating the queue, you can set the fallback dead-letter queue and redrive policy, which can look like this.\n\n```python\nfrom sqs_workers import SQSEnv, create_standard_queue\nsqs = SQSEnv()\n\ncreate_standard_queue(sqs, \'emails_dead\')\ncreate_standard_queue(sqs, \'emails\',\n    redrive_policy=sqs.redrive_policy(\'emails_dead\', 3)\n)\n```\n\nIt means "move the message to the email_deadletters queue after four (3 + 1) failed attempts to send it to the recipient."\n\n## Backoff policies\n\nYou can define the backoff policy for the entire environment or specific queue.\n\n```python\nqueue = sqs.queue("emails", backoff_policy=DEFAULT_BACKOFF)\n\n@queue.processor(\'send_email\')\ndef send_email(to, subject, body):\n    print(f"Sending email {subject} to {to}")\n```\n\nThe default policy is the exponential backoff. We recommend setting both the backoff policy and the dead-letter queue to limit the maximum number of execution attempts.\n\nAlternatively, you can set the backoff to IMMEDIATE_RETURN to re-execute the failed task immediately.\n\n```python\nqueue = sqs.queue("emails", backoff_policy=IMMEDIATE_RETURN)\n\n@queue.processor(\'send_email\')\ndef send_email(to, subject, body):\n    print(f"Sending email {subject} to {to}")\n```\n\n## Shutdown policies\n\nWhen launching the queue processor with process_queue(), it\'s possible to optionally set when it has to be stopped.\n\nFollowing shutdown policies are supported:\n\n- IdleShutdown(idle_seconds): return from function when no new tasks are sent for a specific period.\n\n- MaxTasksShutdown(max_tasks): return from function after processing at least max_task jobs. It can be helpful to prevent memory leaks.\n\nThe default policy is NeverShutdown. It\'s also possible to combine two previous policies with OrShutdown or AndShutdown policies or create custom classes for specific behavior.\n\nExample of stopping processing the queue after 5 minutes of inactivity:\n\n```python\nfrom sqs_workers import SQSEnv\nfrom sqs_workers.shutdown_policies import IdleShutdown\n\nsqs = SQSEnv()\nsqs.queue("foo").process_queue(shutdown_policy=IdleShutdown(idle_seconds=300))\n```\n\n## Processing a dead-letter queue by pushing back failed messages\n\nThe most common way to process a dead-letter queue is to fix the main bug causing messages to appear there in the first place and then to re-process these messages again.\n\nWith sqs-workers, in can be done by putting back all the messages from a dead-letter queue back to the main one. While processing the queue, the processor takes every message and pushes it back to the upstream queue with a hard-coded delay of 1 second.\n\nUsage example:\n\n    >>> from sqs_workers import JobQueue\n    >>> from sqs_workers.shutdown_policies IdleShutdown\n    >>> from sqs_workers.deadletter_queue import DeadLetterQueue\n    >>> env = SQSEnv()\n    >>> foo = env.queue("foo")\n    >>> foo_dead = env.queue("foo_dead", DeadLetterQueue.maker(foo))\n    >>> foo_dead.process_queue(shutdown_policy=IdleShutdown(10))\n\nThis code takes all the messages in the foo_dead queue and pushes them back to the foo queue. Then it waits 10 seconds to ensure no new messages appear, and quit.\n\n## Processing a dead-letter queue by executing tasks in-place\n\nInstead of pushing the tasks back to the main queue, you can execute them in place. For this, you need to copy the queue processors from the main queue to the deadletter.\n\nUsage example:\n\n    >>> env = SQSEnv()\n    >>> foo = env.queue("foo")\n    >>> foo_dead = env.queue("foo_dead")\n    >>> foo.copy_processors(foo_dead)\n    >>>\n    >>> from sqs_workers.shutdown_policies IdleShutdown\n    >>> foo_dead.process_queue(shutdown_policy=IdleShutdown(10))\n\nThis code takes all the messages in the foo_dead queue and executes them with processors from the "foo" queue. Then it waits 10 seconds to ensure no new messages appear, and quit.\n\n## Using in unit tests with MemorySession\n\nThere is a special MemorySession, which can be used as a quick and dirty replacement for real queues in unit tests. If you have a function `create_task` which adds some tasks to the queue and you want to test how it works, you can technically write your tests like this:\n\n```python\nfrom sqs_workers import SQSEnv\nenv = SQSEnv()\n\ndef test_task_creation_side_effects():\n    create_task()\n    env.process_batch(\'foo\')\n    ...\n```\n\nThe problem is that your test starts depending on AWS (or localstack) infrastructure, which you don\'t always need. What you can do instead is you can pass MemorySession to your SQSEnv instance.\n\n```python\nfrom sqs_workers import SQSEnv, MemorySession\nenv = SQSEnv(MemorySession())\n```\n\nPlease note that MemorySession has some serious limitations, and may not fit well your use-case. Namely, when you work with MemorySession:\n\n- Redrive policy doesn\'t work\n- There is no differences between standard and FIFO queues\n- FIFO queues don\'t support content-based deduplication\n- Delayed tasks are executed ineffectively: the task is gotten from the queue, and if the time hasn\'t come, the task is put back.\n- API can return slightly different results\n\n## Contributing\n\nPlease see our guide [here](./CONTRIBUTING.md)\n\n## Local Development\n\nWe use Poetry for dependency management & packaging.  Please see [here for setup instructions](https://python-poetry.org/docs/#installation).\n\nOnce you have Poetry installed, you can run the following to install the dependencies in a virtual environment:\n\n```bash\npoetry install\n```\n\n## Testing\n\nWe use pytest to run unittests, and tox to run them for all supported Python versions.\n\nIf you just run `pytest` or `tox`, all tests will be run against AWS, localstack, and MemorySession. You can disable those you don\'t want to use using the pytest `-k` flag, for instance using `-k localstack` or `-k \'not aws\'`.\n\n### Testing with AWS\n\nMake sure you have your boto3 client configured ([ref](https://boto3.readthedocs.io/en/latest/guide/quickstart.html#configuration)) and then run\n\n```bash\npoetry run pytest -k aws\n```\n\nAlternatively, to test all supported versions, run\n\n```bash\npoetry run tox -- -k aws\n```\n\n### Testing with localstack\n\nLocalstack tests should perform faster than testing against AWS, and besides, they work well in offline.\n\nRun [ElasticMQ](https://github.com/softwaremill/elasticmq) and make sure that the SQS endpoint is available by the address localhost:4566:\n\n```bash\ndocker run -p 4566:9324 --rm -it softwaremill/elasticmq-native\n```\n\nThen run\n\n```bash\npoetry run pytest -k localstack\n```\n\nor\n\n```bash\npoetry run tox -- -k localstack\n```\n\n### Testing with MemorySession\n\nMemorySession should be even faster, but has all the limitations documented above. But it can still be useful to test some logic changes.\n\nSimply run\n\n```bash\npoetry run pytest -k memory\n```\n\nor\n\n```bash\npoetry run tox -- -k memory\n```\n\n## Releasing new versions\n\n- Bump version in `pyproject.toml`\n- Update the CHANGELOG\n- Commit the changes with a commit message "Version X.X.X"\n- Tag the current commit with `vX.X.X`\n- Create a new release on GitHub named `vX.X.X`\n- GitHub Actions will publish the new version to PIP for you\n',
+    'long_description': '# SQS Workers\n\nAn opinionated queue processor for Amazon SQS.\n\n## Usage\n\nInstall the package with\n\n```bash\npip install sqs-workers\n```\n\nConfigure your boto3 library to provide access requisites for your installation with [something like this](https://boto3.readthedocs.io/en/latest/guide/quickstart.html#configuration):\n\n```bash\naws configure\n```\n\nDon\'t forget to set your preferred AWS region.\n\nThen you will start managing two systems (most likely, from the same codebase): one of them adds messages to the queue, and another one executes them.\n\n```python\nfrom sqs_workers import SQSEnv, create_standard_queue\n\n# This environment will use AWS requisites from ~/.aws/ directory\nsqs = SQSEnv()\n\n# Create a new queue.\n# Note that you can use the AWS web interface for the same action as well, the\n# web interface provides more options. You only need to do it once.\ncreate_standard_queue(sqs, "emails")\n\n# Get the queue object\nqueue = sqs.queue("emails")\n\n# Register a queue processor\n@queue.processor("send_email")\ndef send_email(to, subject, body):\n    print(f"Sending email {subject} to {to}")\n```\n\nThen there are two ways of adding tasks to the queue. Classic (aka "explicit"):\n\n```python\nqueue.add_job("send_email", to="user@example.com", subject="Hello world", body="hello world")\n```\n\nAnd the "Celery way" (we mimic the Celery API to some extent)\n\n```python\nsend_email.delay(to="user@example.com", subject="Hello world", body="hello world")\n```\n\nTo process the queue, you have to run workers manually. Create a new file which will contain the definition of the sqs object and register all processors (most likely, by importing necessary modules from your project), and then run SQS\n\n```python\nfrom sqs_workers import SQSEnv\nsqs = SQSEnv()\n...\nsqs.queue(\'emails\').process_queue()\n```\n\nIn production, we usually don\'t handle multiple queues in the same process, but for the development environment it\'s easier to tackle with all the queues at once with\n\n```python\nsqs.process_queues()\n```\n\n## Serialization\n\nThere are two serializers: JSON and pickle.\n\n## Baked tasks\n\nYou can create so-called "baked async tasks," entities which, besides the task itself, contain arguments which have to be used to call the task.\n\nThink of baked tasks as of light version of [Celery signatures](http://docs.celeryproject.org/en/latest/userguide/canvas.html#signatures)\n\n```python\ntask = send_email.bake(to=\'user@example.com\', subject=\'Hello world\', body=\'hello world\')\ntask.delay()\n```\n\nIs the same as\n\n```python\nsend_email.delay(to=\'user@example.com\', subject=\'Hello world\', body=\'hello world\')\n```\n\n## Batch Writes\n\nIf you have many tasks to enqueue, it may be more efficient to use batching when adding them:\n\n```python\n# Classic ("explicit") API\nwith queue.add_batch():\n    queue.add_job("send_email", to="user1@example.com", subject="Hello world", body="hello world")\n    queue.add_job("send_email", to="user2@example.com", subject="Hello world", body="hello world")\n\n# "Celery way"\nwith send_email.batch():\n    send_email.delay(to="user1@example.com", subject="Hello world", body="hello world")\n    send_email.delay(to="user2@example.com", subject="Hello world", body="hello world")\n```\n\nWhen batching is enabled:\n\n- tasks are added to SQS by batches of 10, reducing the number of AWS operations\n- it is not possible to get the task `MessageId`, as it is not known until the batch is sent\n- care has to be taken about message size, as SQS limits both the individual message size and the maximum total payload size to 256 kB.\n\n## Batch Reads\n\nIf you wish to consume and process batches of messages from a queue at once (say to speed up ingestion)\nyou can set the `batching_policy` at queue level.\n\nThe underlying function is expected to have a single parameter which will receive the list of messages.\n\n```python\nfrom sqs_workers.batching import BatchMessages\nfrom sqs_workers import SQSEnv, create_standard_queue\n\nsqs = SQSEnv()\n\ncreate_standard_queue(sqs, "emails")\n\nqueue = sqs.queue("emails", batching_policy=BatchMessages(batch_size=10))\n\n@queue.processor("send_email")\ndef send_email(messages: list):\n    for email in messages:\n        print(f"Sending email {email[\'subject\']} to {email[\'to\']}")\n```\n\nThis function will receive up to 10 messages at once based on:\n\n* How many are available on the queue being consumed\n* How many of those messages on the `emails` queue are for the `send_email` job\n\n## Synchronous task execution\n\nIn Celery, you can run any task synchronously if you just call it as a function with arguments. Our AsyncTask raises a RuntimeError for this case.\n\n```python\nsend_email(to=\'user@example.com\', subject=\'Hello world\', body=\'hello world\')\n...\nRuntimeError: Async task email.send_email called synchronously (probably,\nby mistake). Use either AsyncTask.run(...) to run the task synchronously\nor AsyncTask.delay(...) to add it to the queue.\n```\n\nIf you want to run a task synchronously, use `run()` method of the task.\n\n```\nsend_email.run(to=\'user@example.com\', subject=\'Hello world\', body=\'hello world\')\n```\n\n## FIFO queues\n\nFifo queues can be created with `create_fifo_queue` and have to have the name, which ends with ".fifo".\n\n```python\nfrom sqs_workers import SQSEnv, create_fifo_queue\nsqs = SQSEnv()\n\ncreate_fifo_queue(sqs, \'emails_dead.fifo\')\ncreate_fifo_queue(sqs, \'emails.fifo\',\n    redrive_policy=sqs.redrive_policy(\'emails_dead.fifo\', 3)\n)\n```\n\nUnless the flag `content_based_deduplication` is set, every message has to be sent with an attribute `_deduplication_id`. By default, all messages have the same message group `default`, but you can change it with `_group_id`.\n\n```python\nsqs.queue("emails.fifo").add_job(\n    \'send_email\', _deduplication_id=subject, _group_id=email, **kwargs)\n```\n\n[More about FIFO queues on AWS](https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/FIFO-queues.html)\n\n## Exception processing\n\nIf task processing ended up with an exception, the error is logged, and the task is returned back to the queue after a while. The exact behavior is defined by queue settings.\n\n## Custom processors\n\nYou can define your own processor if you need to perform some specific actions before of after executing a particular task.\n\nExample for the custom processor\n\n```python\nfrom sqs_workers import SQSEnv\nfrom sqs_workers.processors import Processor\n\nclass CustomProcessor(Processor):\n    def process(self, job_kwargs):\n        print(f\'Processing {self.queue_name}.{self.job_name} with {job_kwargs}\')\n        super(CustomProcessor, self).process(job_kwargs)\n\nsqs = SQSEnv(processor_maker=CustomProcessor)\n```\n\n## Working with contexts\n\nContext is implicitly passed to the worker via the job message and can be used for logging or profiling purposes.\n\nUsage example.\n\n```python\nqueue = sqs.queue("q1")\n\n@queue.processor(\'q1\', \'hello_world\', pass_context=True)\ndef hello_world(username=None, context=None):\n    print(f\'Hello {username} from {context["remote_addr"]}\')\n\nwith sqs.context(remote_addr=\'127.0.0.1\'):\n    hello_world.delay(username=\'Foo\')\n\nqueue.process_batch()\n```\n\nAlternatively, you can set a context like this.\n\n```python\nsqs.context[\'remote_addr\'] = \'127.0.0.1\'\nhello_world.delay(username=\'Foo\')\n```\n\nAnd then, when the context needs to be cleared:\n\n```python\nsqs.context.clear()\n```\n\nIn a web application, you usually call it at the end of the processing of the web request.\n\n## Automatic applying of the context for all tasks\n\nInstead of dealing with the context inside every processing function, you can perform this in processors by subclassing them.\n\n```python\nimport os\nfrom sqs_workers import SQSEnv\nfrom sqs_workers.processors import Processor\n\nclass CustomProcessor(Processor):\n    def process(self, job_kwargs, job_context):\n        os.environ[\'REMOTE_ADDR\'] = job_context[\'remote_addr\']\n        super(CustomProcessor, self).process(job_kwargs, job_context)\n        os.unsetenv(\'REMOTE_ADDR\')\n\nsqs = SQSEnv(\n    processor_maker=CustomProcessor,\n)\n```\n\n## Raw queues\n\nRaw queues can have only one processor, which should be a function, accepting the message as its only argument.\n\nRaw queues are helpful to process messages, added to SQS from external sources, such as CloudWatch events.\n\nYou start the processor the same way, creating a new standard queue if needed.\n\n```python\nfrom sqs_workers import SQSEnv, create_standard_queue\nsqs = SQSEnv()\ncreate_standard_queue(sqs, \'cron\')\n```\n\nThen you get a queue, but provide a queue_maker parameter to it, to create a queue of the necessary type, and define a processor for it.\n\n```python\nfrom sqs_workers import RawQueue\n\ncron = sqs.queue(\'cron\', RawQueue)\n\n@cron.raw_processor()\ndef processor(message):\n    print(message.body)\n```\n\nThen start processing your queue as usual:\n\n```python\ncron.process_queue()\n```\n\nYou can also send raw messages to the queue, but this is probably less useful:\n\n```python\ncron.add_raw_job("Hello world")\n```\n\n## Processing Messages from CloudWatch\n\nBy default message body by CloudWatch scheduler has following JSON structure.\n\n```json\n{\n  "version": "0",\n  "id": "a9a10406-9a1f-0ddc-51ae-08db551fac42",\n  "detail-type": "Scheduled Event",\n  "source": "aws.events",\n  "account": "NNNNNNNNNN",\n  "time": "2019-09-20T09:19:56Z",\n  "region": "eu-west-1",\n  "resources": ["arn:aws:events:eu-west-1:NNNNNNNNNN:rule/Playground"],\n  "detail": {}\n}\n```\n\nHeaders of the message:\n\n```python\n{\n    \'SenderId\': \'AIDAJ2E....\',\n    \'ApproximateFirstReceiveTimestamp\': \'1568971264367\',\n    \'ApproximateReceiveCount\': \'1\',\n    \'SentTimestamp\': \'1568971244845\',\n}\n```\n\nYou can pass any valid JSON as a message, though, and it will be passed as-is to the message body. Something like this:\n\n```json\n{ "message": "Hello world" }\n```\n\n## Dead-letter queues and redrive\n\nOn creating the queue, you can set the fallback dead-letter queue and redrive policy, which can look like this.\n\n```python\nfrom sqs_workers import SQSEnv, create_standard_queue\nsqs = SQSEnv()\n\ncreate_standard_queue(sqs, \'emails_dead\')\ncreate_standard_queue(sqs, \'emails\',\n    redrive_policy=sqs.redrive_policy(\'emails_dead\', 3)\n)\n```\n\nIt means "move the message to the email_deadletters queue after four (3 + 1) failed attempts to send it to the recipient."\n\n## Backoff policies\n\nYou can define the backoff policy for the entire environment or specific queue.\n\n```python\nqueue = sqs.queue("emails", backoff_policy=DEFAULT_BACKOFF)\n\n@queue.processor(\'send_email\')\ndef send_email(to, subject, body):\n    print(f"Sending email {subject} to {to}")\n```\n\nThe default policy is the exponential backoff. We recommend setting both the backoff policy and the dead-letter queue to limit the maximum number of execution attempts.\n\nAlternatively, you can set the backoff to IMMEDIATE_RETURN to re-execute the failed task immediately.\n\n```python\nqueue = sqs.queue("emails", backoff_policy=IMMEDIATE_RETURN)\n\n@queue.processor(\'send_email\')\ndef send_email(to, subject, body):\n    print(f"Sending email {subject} to {to}")\n```\n\n## Shutdown policies\n\nWhen launching the queue processor with process_queue(), it\'s possible to optionally set when it has to be stopped.\n\nFollowing shutdown policies are supported:\n\n- IdleShutdown(idle_seconds): return from function when no new tasks are sent for a specific period.\n\n- MaxTasksShutdown(max_tasks): return from function after processing at least max_task jobs. It can be helpful to prevent memory leaks.\n\nThe default policy is NeverShutdown. It\'s also possible to combine two previous policies with OrShutdown or AndShutdown policies or create custom classes for specific behavior.\n\nExample of stopping processing the queue after 5 minutes of inactivity:\n\n```python\nfrom sqs_workers import SQSEnv\nfrom sqs_workers.shutdown_policies import IdleShutdown\n\nsqs = SQSEnv()\nsqs.queue("foo").process_queue(shutdown_policy=IdleShutdown(idle_seconds=300))\n```\n\n## Processing a dead-letter queue by pushing back failed messages\n\nThe most common way to process a dead-letter queue is to fix the main bug causing messages to appear there in the first place and then to re-process these messages again.\n\nWith sqs-workers, in can be done by putting back all the messages from a dead-letter queue back to the main one. While processing the queue, the processor takes every message and pushes it back to the upstream queue with a hard-coded delay of 1 second.\n\nUsage example:\n\n    >>> from sqs_workers import JobQueue\n    >>> from sqs_workers.shutdown_policies IdleShutdown\n    >>> from sqs_workers.deadletter_queue import DeadLetterQueue\n    >>> env = SQSEnv()\n    >>> foo = env.queue("foo")\n    >>> foo_dead = env.queue("foo_dead", DeadLetterQueue.maker(foo))\n    >>> foo_dead.process_queue(shutdown_policy=IdleShutdown(10))\n\nThis code takes all the messages in the foo_dead queue and pushes them back to the foo queue. Then it waits 10 seconds to ensure no new messages appear, and quit.\n\n## Processing a dead-letter queue by executing tasks in-place\n\nInstead of pushing the tasks back to the main queue, you can execute them in place. For this, you need to copy the queue processors from the main queue to the deadletter.\n\nUsage example:\n\n    >>> env = SQSEnv()\n    >>> foo = env.queue("foo")\n    >>> foo_dead = env.queue("foo_dead")\n    >>> foo.copy_processors(foo_dead)\n    >>>\n    >>> from sqs_workers.shutdown_policies IdleShutdown\n    >>> foo_dead.process_queue(shutdown_policy=IdleShutdown(10))\n\nThis code takes all the messages in the foo_dead queue and executes them with processors from the "foo" queue. Then it waits 10 seconds to ensure no new messages appear, and quit.\n\n## Codecs\n\nBefore being added to SQS, task parameters are encoded using a `Codec`. At the moment, 3 codecs are available:\n- `pickle`: serialize with Pickle, using the default protocol version;\n- `pickle_compat`: serialize with Pickle, using protocol version 2, which is compatible with Python 2;\n- `json`: serialize with JSON.\n\nBy default, `pickle_compat` is used, for backward compatibility with previous versions of sqs-workers.\n\nJSON is recommended if using untrusted data (see the notes about security in the [pickle docs](https://docs.python.org/3/library/pickle.html), or for compatibility with other systems. In all other cases, you should use `pickle` instead of `pickle_compat`, as it\'s more compact and efficient:\n\n    >>> env = SQSEnv(codec="pickle")\n\n## Using in unit tests with MemorySession\n\nThere is a special MemorySession, which can be used as a quick and dirty replacement for real queues in unit tests. If you have a function `create_task` which adds some tasks to the queue and you want to test how it works, you can technically write your tests like this:\n\n```python\nfrom sqs_workers import SQSEnv\nenv = SQSEnv()\n\ndef test_task_creation_side_effects():\n    create_task()\n    env.process_batch(\'foo\')\n    ...\n```\n\nThe problem is that your test starts depending on AWS (or localstack) infrastructure, which you don\'t always need. What you can do instead is you can pass MemorySession to your SQSEnv instance.\n\n```python\nfrom sqs_workers import SQSEnv, MemorySession\nenv = SQSEnv(MemorySession())\n```\n\nPlease note that MemorySession has some serious limitations, and may not fit well your use-case. Namely, when you work with MemorySession:\n\n- Redrive policy doesn\'t work\n- There is no differences between standard and FIFO queues\n- FIFO queues don\'t support content-based deduplication\n- Delayed tasks are executed ineffectively: the task is gotten from the queue, and if the time hasn\'t come, the task is put back.\n- API can return slightly different results\n\n## Contributing\n\nPlease see our guide [here](./CONTRIBUTING.md)\n\n## Local Development\n\nWe use Poetry for dependency management & packaging.  Please see [here for setup instructions](https://python-poetry.org/docs/#installation).\n\nOnce you have Poetry installed, you can run the following to install the dependencies in a virtual environment:\n\n```bash\npoetry install\n```\n\n## Testing\n\nWe use pytest to run unittests, and tox to run them for all supported Python versions.\n\nIf you just run `pytest` or `tox`, all tests will be run against AWS, localstack, and MemorySession. You can disable those you don\'t want to use using the pytest `-k` flag, for instance using `-k localstack` or `-k \'not aws\'`.\n\n### Testing with AWS\n\nMake sure you have your boto3 client configured ([ref](https://boto3.readthedocs.io/en/latest/guide/quickstart.html#configuration)) and then run\n\n```bash\npoetry run pytest -k aws\n```\n\nAlternatively, to test all supported versions, run\n\n```bash\npoetry run tox -- -k aws\n```\n\n### Testing with localstack\n\nLocalstack tests should perform faster than testing against AWS, and besides, they work well in offline.\n\nRun [ElasticMQ](https://github.com/softwaremill/elasticmq) and make sure that the SQS endpoint is available by the address localhost:4566:\n\n```bash\ndocker run -p 4566:9324 --rm -it softwaremill/elasticmq-native\n```\n\nThen run\n\n```bash\npoetry run pytest -k localstack\n```\n\nor\n\n```bash\npoetry run tox -- -k localstack\n```\n\n### Testing with MemorySession\n\nMemorySession should be even faster, but has all the limitations documented above. But it can still be useful to test some logic changes.\n\nSimply run\n\n```bash\npoetry run pytest -k memory\n```\n\nor\n\n```bash\npoetry run tox -- -k memory\n```\n\n## Releasing new versions\n\n- Bump version in `pyproject.toml`\n- Update the CHANGELOG\n- Commit the changes with a commit message "Version X.X.X"\n- Tag the current commit with `vX.X.X`\n- Create a new release on GitHub named `vX.X.X`\n- GitHub Actions will publish the new version to PIP for you\n',
     'author': 'Doist Developers',
     'author_email': 'dev@doist.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Doist/sqs-workers',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `sqs-workers-0.5.8/PKG-INFO` & `sqs_workers-0.5.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: sqs-workers
-Version: 0.5.8
+Version: 0.5.9
 Summary: An opinionated queue processor for Amazon SQS
 Home-page: https://github.com/Doist/sqs-workers
 License: MIT
 Author: Doist Developers
 Author-email: dev@doist.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: attrs (>=22.1.0,<23.0.0)
 Requires-Dist: boto3 (>=1.24.62,<2.0.0)
 Description-Content-Type: text/markdown
@@ -444,14 +445,27 @@
     >>> foo.copy_processors(foo_dead)
     >>>
     >>> from sqs_workers.shutdown_policies IdleShutdown
     >>> foo_dead.process_queue(shutdown_policy=IdleShutdown(10))
 
 This code takes all the messages in the foo_dead queue and executes them with processors from the "foo" queue. Then it waits 10 seconds to ensure no new messages appear, and quit.
 
+## Codecs
+
+Before being added to SQS, task parameters are encoded using a `Codec`. At the moment, 3 codecs are available:
+- `pickle`: serialize with Pickle, using the default protocol version;
+- `pickle_compat`: serialize with Pickle, using protocol version 2, which is compatible with Python 2;
+- `json`: serialize with JSON.
+
+By default, `pickle_compat` is used, for backward compatibility with previous versions of sqs-workers.
+
+JSON is recommended if using untrusted data (see the notes about security in the [pickle docs](https://docs.python.org/3/library/pickle.html), or for compatibility with other systems. In all other cases, you should use `pickle` instead of `pickle_compat`, as it's more compact and efficient:
+
+    >>> env = SQSEnv(codec="pickle")
+
 ## Using in unit tests with MemorySession
 
 There is a special MemorySession, which can be used as a quick and dirty replacement for real queues in unit tests. If you have a function `create_task` which adds some tasks to the queue and you want to test how it works, you can technically write your tests like this:
 
 ```python
 from sqs_workers import SQSEnv
 env = SQSEnv()
```

