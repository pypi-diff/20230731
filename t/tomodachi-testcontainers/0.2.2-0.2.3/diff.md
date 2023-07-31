# Comparing `tmp/tomodachi_testcontainers-0.2.2.tar.gz` & `tmp/tomodachi_testcontainers-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomodachi_testcontainers-0.2.2.tar", max compression
+gzip compressed data, was "tomodachi_testcontainers-0.2.3.tar", max compression
```

## Comparing `tomodachi_testcontainers-0.2.2.tar` & `tomodachi_testcontainers-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1071 2023-07-23 09:35:29.084747 tomodachi_testcontainers-0.2.2/LICENSE
--rw-r--r--   0        0        0    26649 2023-07-29 08:49:13.268083 tomodachi_testcontainers-0.2.2/README.md
--rw-r--r--   0        0        0     3734 2023-07-29 08:49:20.113888 tomodachi_testcontainers-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086660 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086809 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/clients/__init__.py
--rw-r--r--   0        0        0     2465 2023-07-29 06:48:22.554642 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/clients/snssqs_client.py
--rw-r--r--   0        0        0      618 2023-07-23 10:30:40.087330 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/__init__.py
--rw-r--r--   0        0        0     3855 2023-07-29 08:49:13.268726 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/common.py
--rw-r--r--   0        0        0     1818 2023-07-27 14:17:21.582876 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/localstack.py
--rw-r--r--   0        0        0     2085 2023-07-27 14:17:21.583252 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/moto.py
--rw-r--r--   0        0        0     3129 2023-07-27 14:17:21.583523 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/sftp.py
--rw-r--r--   0        0        0      930 2023-07-27 14:17:21.583737 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/tomodachi.py
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.088391 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/py.typed
--rw-r--r--   0        0        0     1346 2023-07-29 07:46:42.840748 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/pytest/__init__.py
--rw-r--r--   0        0        0      503 2023-07-23 10:30:40.088800 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/pytest/assertions.py
--rw-r--r--   0        0        0     2290 2023-07-27 13:30:06.032389 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/pytest/localstack_fixtures.py
--rw-r--r--   0        0        0     2109 2023-07-27 13:30:09.023818 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/pytest/moto_fixtures.py
--rw-r--r--   0        0        0     1594 2023-07-27 13:30:16.939169 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/pytest/sftp_fixtures.py
--rw-r--r--   0        0        0      609 2023-07-29 08:49:13.269030 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py
--rw-r--r--   0        0        0      323 2023-07-23 10:30:40.089565 tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/utils.py
--rw-r--r--   0        0        0    27838 1970-01-01 00:00:00.000000 tomodachi_testcontainers-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-23 09:35:29.084747 tomodachi_testcontainers-0.2.3/LICENSE
+-rw-r--r--   0        0        0    26880 2023-07-31 18:13:07.890597 tomodachi_testcontainers-0.2.3/README.md
+-rw-r--r--   0        0        0     3996 2023-07-31 18:51:23.321971 tomodachi_testcontainers-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086660 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086809 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/clients/__init__.py
+-rw-r--r--   0        0        0     3487 2023-07-31 18:13:07.895096 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/clients/snssqs_client.py
+-rw-r--r--   0        0        0      618 2023-07-23 10:30:40.087330 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/__init__.py
+-rw-r--r--   0        0        0     3944 2023-07-31 18:13:07.895679 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/common.py
+-rw-r--r--   0        0        0     1739 2023-07-31 18:13:07.895948 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/localstack.py
+-rw-r--r--   0        0        0     2335 2023-07-31 18:50:45.229403 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/moto.py
+-rw-r--r--   0        0        0     3129 2023-07-27 14:17:21.583523 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/sftp.py
+-rw-r--r--   0        0        0      930 2023-07-27 14:17:21.583737 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/tomodachi.py
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.088391 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/py.typed
+-rw-r--r--   0        0        0     1394 2023-07-31 18:13:07.896643 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/pytest/__init__.py
+-rw-r--r--   0        0        0      503 2023-07-23 10:30:40.088800 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/pytest/assertions.py
+-rw-r--r--   0        0        0     2312 2023-07-31 18:13:07.897004 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/pytest/localstack_fixtures.py
+-rw-r--r--   0        0        0     2126 2023-07-31 18:13:07.897240 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/pytest/moto_fixtures.py
+-rw-r--r--   0        0        0     1594 2023-07-31 12:23:17.273453 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/pytest/sftp_fixtures.py
+-rw-r--r--   0        0        0      609 2023-07-29 08:49:13.269030 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py
+-rw-r--r--   0        0        0      323 2023-07-23 10:30:40.089565 tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/utils.py
+-rw-r--r--   0        0        0    28069 1970-01-01 00:00:00.000000 tomodachi_testcontainers-0.2.3/PKG-INFO
```

### Comparing `tomodachi_testcontainers-0.2.2/LICENSE` & `tomodachi_testcontainers-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.2/README.md` & `tomodachi_testcontainers-0.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -77,17 +77,17 @@
 import tomodachi
 from aiohttp import web
 
 
 class TomodachiServiceHealthcheck(tomodachi.Service):
     name = "service-healthcheck"
 
- @tomodachi.http("GET", r"/health")
- async def healthcheck(self, request: web.Request) -> web.Response:
- return web.json_response(data={"status": "ok"})
+    @tomodachi.http("GET", r"/health")
+        async def healthcheck(self, request: web.Request) -> web.Response:
+        return web.json_response(data={"status": "ok"})
 ```
 
 The following `tomodachi_container` fixture builds and runs the service as a Docker container.
 
 ```python
 from typing import Generator, cast
 
@@ -257,46 +257,49 @@
 from tomodachi_testcontainers.utils import get_available_port
 
 
 @pytest.fixture()
 def tomodachi_container(
     tomodachi_image: DockerImage,
     localstack_container: LocalStackContainer,
-    _restart_localstack_container: None,
 ) -> Generator[TomodachiContainer, None, None]:
     with (
         TomodachiContainer(image=str(tomodachi_image.id), edge_port=get_available_port())
-        .with_env("AWS_REGION", "eu-west-1")
+        .with_env("AWS_REGION", "us-east-1")
         .with_env("AWS_ACCESS_KEY_ID", "testing")
         .with_env("AWS_SECRET_ACCESS_KEY", "testing")
         .with_env("AWS_S3_ENDPOINT_URL", localstack_container.get_internal_url())
         .with_command("tomodachi run app.py --production")
     ) as container:
         yield cast(TomodachiContainer, container)
+    localstack_container.restart_container()
 ```
 
 This time, `tomodachi_container` fixture is more involved. It uses
 `localstack_container` fixture, provided by `tomodachi_testcontainers` library.
 The fixture starts a `LocalStackContainer`.
 
 After the `LocalStackContainer` is started, we can use its `get_internal_url` method
 to get the URL of the container that is accessible _inside_ the Docker network.
 This time, we need the internal URL of the container, because the `TomodachiContainer`
 needs to communicate with `LocalStackContainer`, and they both run in the same Docker network.
 
 The LocalStack's `internal_url` is passed to `TomodachiContainer` as an environment variable `AWS_S3_ENDPOINT_URL`,
 following [12-factor app principle of providing app configuration in environment variables](https://12factor.net/config).
 
-The `tomodachi_container` fixture also uses the `_restart_localstack_container` fixture,
-that restarts the `LocalStackContainer` after every test.
-It resets the state of LocalStack after every test so that each new test starts
-from a clean and predictable state. That way, we avoid flaky tests that depend on the
-state of the previous test or their execution order.
-As a downside, it takes a bit more time to restart the container after every test,
-so it might not be necessary for every test.
+On `tomodachi_container` fixture teardown, `LocalStack` container is restarted
+to reset its state - delete all S3 buckets and files. This way we can be sure
+that each test starts with a clean state.
+As alternative for calling `restart_container` method explicitly,
+you can use `_restart_localstack_container_on_teardown` fixture.
+We avoid flaky tests that depend on the state of the previous test or their execution order,
+and avoid leaking test data from one test to another.
+As a drawback, it takes a more time to restart a container after every test.
+To improve test execution speed, you can explicitly cleanup AWS resources, for example,
+deleting all S3 buckets and DynamoDB tables after every test.
 
 That's the setup, now on to the application test. 🧪
 
 ```python
 import httpx
 import pytest
 from types_aiobotocore_s3 import S3Client
```

### Comparing `tomodachi_testcontainers-0.2.2/pyproject.toml` & `tomodachi_testcontainers-0.2.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tomodachi-testcontainers"
-version = "0.2.2"
+version = "0.2.3"
 description = "Collection of Testcontainers, pytest fixtures and test clients for end-to-end/integration testing for Python Tomodachi framework. A great starting point to learn more about Testcontainers and necessity of integration testing."
 authors = ["Filips Nastins <nastinsfilips@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 homepage = "https://github.com/filipsnastins/tomodachi-testcontainers"
 repository = "https://github.com/filipsnastins/tomodachi-testcontainers"
@@ -162,11 +162,17 @@
 [tool.pytest.ini_options]
 minversion = "7.0"
 junit_family = "xunit2"
 testpaths = ["tests"]
 norecursedirs = [".venv", "__pycache__", ".git"]
 log_cli_level = "INFO"
 env = [
+    # Set dummy AWS credentials so that we don't accidentally mutate real infrastructure
+    "AWS_ACCESS_KEY_ID=testing",
+    "AWS_DEFAULT_REGION=us-east-1",
+    "AWS_SECRET_ACCESS_KEY=testing",
+    "AWS_SECURITY_TOKEN=testing",
+    "AWS_SESSION_TOKEN=testing",
+    "DOCKER_BUILDKIT=1",
     "TESTCONTAINER_DOCKER_NETWORK=tomodachi-testcontainers",
     "TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH=examples/Dockerfile",
-    "DOCKER_BUILDKIT=1",
 ]
```

### Comparing `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/clients/snssqs_client.py` & `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/clients/snssqs_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
-from typing import Any, List, Protocol, Type, TypeVar, Union
+from typing import Any, Dict, List, Protocol, Type, TypeVar, Union
 
 from types_aiobotocore_sns import SNSClient
 from types_aiobotocore_sqs import SQSClient
+from types_aiobotocore_sqs.literals import QueueAttributeFilterType, QueueAttributeNameType
 
 MessageType = TypeVar("MessageType")
 
 
 class TomodachiSNSSQSEnvelope(Protocol):
     @classmethod
     async def build_message(cls: "TomodachiSNSSQSEnvelope", service: Any, topic: str, data: Any, **kwargs: Any) -> str:
@@ -14,14 +15,15 @@
 
     @classmethod
     async def parse_message(cls: "TomodachiSNSSQSEnvelope", payload: str, **kwargs: Any) -> Union[dict, tuple]:
         ...
 
 
 async def subscribe_to(sns_client: SNSClient, sqs_client: SQSClient, topic: str, queue: str) -> None:
+    """Subscribe a SQS queue to a SNS topic; create the topic and queue if they don't exist."""
     create_topic_response = await sns_client.create_topic(Name=topic)
     topic_arn = create_topic_response["TopicArn"]
 
     create_queue_response = await sqs_client.create_queue(QueueName=queue)
     queue_url = create_queue_response["QueueUrl"]
 
     get_queue_attributes_response = await sqs_client.get_queue_attributes(
@@ -35,30 +37,45 @@
 async def receive(
     sqs_client: SQSClient,
     queue_name: str,
     envelope: TomodachiSNSSQSEnvelope,
     message_type: Type[MessageType],
     max_messages: int = 10,
 ) -> List[MessageType]:
+    """Receive messages from a SQS queue."""
     get_queue_url_response = await sqs_client.get_queue_url(QueueName=queue_name)
     queue_url = get_queue_url_response["QueueUrl"]
 
     received_messages_response = await sqs_client.receive_message(QueueUrl=queue_url, MaxNumberOfMessages=max_messages)
     received_messages = received_messages_response.get("Messages")
     if not received_messages:
         return []
 
     parsed_messages: List[MessageType] = []
     for received_message in received_messages:
         payload = json.loads(received_message["Body"])["Message"]
         parsed_message = await envelope.parse_message(payload=payload, proto_class=message_type)
         parsed_messages.append(parsed_message[0]["data"])
+        await sqs_client.delete_message(QueueUrl=queue_url, ReceiptHandle=received_message["ReceiptHandle"])
     return parsed_messages
 
 
 async def publish(sns_client: SNSClient, topic: str, data: Any, envelope: TomodachiSNSSQSEnvelope) -> None:
+    """Publish a message to a SNS topic."""
     message = await envelope.build_message(service={}, topic=topic, data=data)
 
-    create_topic_response = await sns_client.create_topic(Name=topic)
-    topic_arn = create_topic_response["TopicArn"]
+    list_topics_response = await sns_client.list_topics()
+    topic_arn = next((v["TopicArn"] for v in list_topics_response["Topics"] if v["TopicArn"].endswith(topic)), None)
+    if not topic_arn:
+        raise ValueError(f"Topic does not exist: {topic}")
 
     await sns_client.publish(TopicArn=topic_arn, Message=message)
+
+
+async def get_queue_attributes(
+    sqs_client: SQSClient, queue: str, attributes: List[QueueAttributeFilterType]
+) -> Dict[QueueAttributeNameType, str]:
+    """Get attributes for a SQS queue."""
+    get_queue_response = await sqs_client.get_queue_url(QueueName=queue)
+    queue_url = get_queue_response["QueueUrl"]
+    get_queue_attributes_response = await sqs_client.get_queue_attributes(QueueUrl=queue_url, AttributeNames=attributes)
+    return get_queue_attributes_response["Attributes"]
```

### Comparing `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/__init__.py` & `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/common.py` & `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,17 @@
         container = self.get_docker_client().get_container(self.get_wrapped_container().id)
         return container["NetworkSettings"]["Networks"][self.network]["IPAddress"]
 
     def get_container_gateway_ip(self) -> str:
         container = self.get_docker_client().get_container(self.get_wrapped_container().id)
         return container["NetworkSettings"]["Networks"][self.network]["Gateway"]
 
+    def restart_container(self) -> None:
+        self.get_wrapped_container().restart()
+
 
 class EphemeralDockerImage:
     def __init__(self, dockerfile: Path, docker_client_kw: Optional[Dict] = None) -> None:
         self.client = DockerClient(**(docker_client_kw or {}))
         self.image = self.build_image(dockerfile)
 
     def __enter__(self) -> DockerImage:
```

### Comparing `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/localstack.py` & `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/localstack.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         region_name: Optional[str] = None,
         **kwargs: Any,
     ) -> None:
         super().__init__(image, **kwargs)
         self.internal_port = internal_port
         self.edge_port = edge_port
 
-        self.region_name = region_name or os.environ.get("AWS_DEFAULT_REGION") or "eu-west-1"
+        self.region_name = region_name or os.environ.get("AWS_DEFAULT_REGION") or "us-east-1"
         self.aws_access_key_id = os.environ.get("AWS_ACCESS_KEY_ID") or "testing"  # nosec: B105
         self.aws_secret_access_key = os.environ.get("AWS_SECRET_ACCESS_KEY") or "testing"  # nosec: B105
 
         self.with_bind_ports(self.internal_port, self.edge_port)
 
     def get_internal_url(self) -> str:
         ip = self.get_container_internal_ip()
@@ -42,10 +42,7 @@
             endpoint_url=self.get_external_url(),
         )
 
     def start(self, timeout: int = 10) -> "LocalStackContainer":
         super().start()
         wait_for_logs(self, r"Ready\.\n", timeout=timeout)
         return self
-
-    def restart(self) -> None:
-        self.get_wrapped_container().restart()
```

### Comparing `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/moto.py` & `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/moto.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,23 +16,29 @@
         region_name: Optional[str] = None,
         **kwargs: Any,
     ) -> None:
         super().__init__(image, **kwargs)
         self.internal_port = internal_port
         self.edge_port = edge_port
 
-        self.region_name = region_name or os.environ.get("AWS_DEFAULT_REGION") or "eu-west-1"
+        self.region_name = region_name or os.environ.get("AWS_DEFAULT_REGION") or "us-east-1"
         self.aws_access_key_id = os.environ.get("AWS_ACCESS_KEY_ID") or "testing"  # nosec: B105
         self.aws_secret_access_key = os.environ.get("AWS_SECRET_ACCESS_KEY") or "testing"  # nosec: B105
 
         self.with_bind_ports(self.internal_port, self.edge_port)
         self.with_env("AWS_DEFAULT_REGION", self.region_name)
         self.with_env("AWS_ACCESS_KEY_ID", self.aws_access_key_id)
         self.with_env("AWS_SECRET_ACCESS_KEY", self.aws_secret_access_key)
 
+        self.with_env("MOTO_PORT", str(self.internal_port))
+
+        # Docker is needed for Lambda
+        self.with_env("MOTO_DOCKER_NETWORK_NAME", self.network)
+        self.with_volume_mapping("/var/run/docker.sock", "/var/run/docker.sock")
+
     def get_internal_url(self) -> str:
         ip = self.get_container_internal_ip()
         return f"http://{ip}:{self.internal_port}"
 
     def get_external_url(self) -> str:
         host = self.get_container_host_ip()
         return f"http://{host}:{self.edge_port}"
@@ -46,9 +52,9 @@
         )
 
     def start(self, timeout: float = 10) -> "MotoContainer":
         super().start()
         wait_for_logs(self, "Running on all addresses", timeout=timeout)
         return self
 
-    def reset(self) -> None:
+    def reset_moto(self) -> None:
         self.exec(["sh", "-c", "curl", "-X", "POST", f"http://localhost:{self.internal_port}/moto-api/reset"])
```

### Comparing `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/sftp.py` & `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/sftp.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/containers/tomodachi.py` & `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/containers/tomodachi.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/pytest/__init__.py` & `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/pytest/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import contextlib
 
 import pytest
 
 from tomodachi_testcontainers.pytest.localstack_fixtures import (
-    _restart_localstack_container,
+    _restart_localstack_container_on_teardown,
     localstack_container,
     localstack_dynamodb_client,
     localstack_s3_client,
     localstack_sns_client,
     localstack_sqs_client,
     localstack_ssm_client,
 )
 from tomodachi_testcontainers.pytest.moto_fixtures import (
-    _reset_moto_container,
+    _reset_moto_container_on_teardown,
     moto_container,
     moto_dynamodb_client,
     moto_s3_client,
     moto_sns_client,
     moto_sqs_client,
     moto_ssm_client,
 )
@@ -26,16 +26,16 @@
     from tomodachi_testcontainers.pytest.sftp_fixtures import sftp_container, userpass_sftp_client, userssh_sftp_client
 
 
 pytest.register_assert_rewrite("tomodachi_testcontainers.pytest.assertions")
 
 
 __all__ = [
-    "_reset_moto_container",
-    "_restart_localstack_container",
+    "_reset_moto_container_on_teardown",
+    "_restart_localstack_container_on_teardown",
     "localstack_container",
     "localstack_dynamodb_client",
     "localstack_s3_client",
     "localstack_sns_client",
     "localstack_sqs_client",
     "localstack_ssm_client",
     "moto_container",
```

### Comparing `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/pytest/localstack_fixtures.py` & `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/pytest/localstack_fixtures.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 def localstack_container() -> Generator[LocalStackContainer, None, None]:
     image = os.environ.get("LOCALSTACK_TESTCONTAINER_IMAGE_ID", "localstack/localstack:2.1")
     with LocalStackContainer(image=image, edge_port=get_available_port()) as container:
         yield container
 
 
 @pytest.fixture()
-def _restart_localstack_container(localstack_container: LocalStackContainer) -> Generator[None, None, None]:
+def _restart_localstack_container_on_teardown(localstack_container: LocalStackContainer) -> Generator[None, None, None]:
     yield
-    localstack_container.restart()
+    localstack_container.restart_container()
 
 
 @pytest_asyncio.fixture()
 async def localstack_sns_client(localstack_container: LocalStackContainer) -> AsyncGenerator[SNSClient, None]:
     async with get_session().create_client("sns", **localstack_container.get_aws_client_config()) as c:
         yield c
```

### Comparing `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/pytest/moto_fixtures.py` & `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/pytest/moto_fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 def moto_container() -> Generator[MotoContainer, None, None]:
     image = os.environ.get("MOTO_TESTCONTAINER_IMAGE_ID", "motoserver/moto:latest")
     with MotoContainer(image=image, edge_port=get_available_port()) as container:
         yield container
 
 
 @pytest.fixture()
-def _reset_moto_container(moto_container: MotoContainer) -> Generator[None, None, None]:
+def _reset_moto_container_on_teardown(moto_container: MotoContainer) -> Generator[None, None, None]:
     yield
-    moto_container.reset()
+    moto_container.reset_moto()
 
 
 @pytest_asyncio.fixture()
 async def moto_sns_client(moto_container: MotoContainer) -> AsyncGenerator[SNSClient, None]:
     async with get_session().create_client("sns", **moto_container.get_aws_client_config()) as c:
         yield c
```

### Comparing `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/pytest/sftp_fixtures.py` & `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/pytest/sftp_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.2/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py` & `tomodachi_testcontainers-0.2.3/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.2/PKG-INFO` & `tomodachi_testcontainers-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomodachi-testcontainers
-Version: 0.2.2
+Version: 0.2.3
 Summary: Collection of Testcontainers, pytest fixtures and test clients for end-to-end/integration testing for Python Tomodachi framework. A great starting point to learn more about Testcontainers and necessity of integration testing.
 Home-page: https://github.com/filipsnastins/tomodachi-testcontainers
 License: MIT
 Author: Filips Nastins
 Author-email: nastinsfilips@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -101,17 +101,17 @@
 import tomodachi
 from aiohttp import web
 
 
 class TomodachiServiceHealthcheck(tomodachi.Service):
     name = "service-healthcheck"
 
- @tomodachi.http("GET", r"/health")
- async def healthcheck(self, request: web.Request) -> web.Response:
- return web.json_response(data={"status": "ok"})
+    @tomodachi.http("GET", r"/health")
+        async def healthcheck(self, request: web.Request) -> web.Response:
+        return web.json_response(data={"status": "ok"})
 ```
 
 The following `tomodachi_container` fixture builds and runs the service as a Docker container.
 
 ```python
 from typing import Generator, cast
 
@@ -281,46 +281,49 @@
 from tomodachi_testcontainers.utils import get_available_port
 
 
 @pytest.fixture()
 def tomodachi_container(
     tomodachi_image: DockerImage,
     localstack_container: LocalStackContainer,
-    _restart_localstack_container: None,
 ) -> Generator[TomodachiContainer, None, None]:
     with (
         TomodachiContainer(image=str(tomodachi_image.id), edge_port=get_available_port())
-        .with_env("AWS_REGION", "eu-west-1")
+        .with_env("AWS_REGION", "us-east-1")
         .with_env("AWS_ACCESS_KEY_ID", "testing")
         .with_env("AWS_SECRET_ACCESS_KEY", "testing")
         .with_env("AWS_S3_ENDPOINT_URL", localstack_container.get_internal_url())
         .with_command("tomodachi run app.py --production")
     ) as container:
         yield cast(TomodachiContainer, container)
+    localstack_container.restart_container()
 ```
 
 This time, `tomodachi_container` fixture is more involved. It uses
 `localstack_container` fixture, provided by `tomodachi_testcontainers` library.
 The fixture starts a `LocalStackContainer`.
 
 After the `LocalStackContainer` is started, we can use its `get_internal_url` method
 to get the URL of the container that is accessible _inside_ the Docker network.
 This time, we need the internal URL of the container, because the `TomodachiContainer`
 needs to communicate with `LocalStackContainer`, and they both run in the same Docker network.
 
 The LocalStack's `internal_url` is passed to `TomodachiContainer` as an environment variable `AWS_S3_ENDPOINT_URL`,
 following [12-factor app principle of providing app configuration in environment variables](https://12factor.net/config).
 
-The `tomodachi_container` fixture also uses the `_restart_localstack_container` fixture,
-that restarts the `LocalStackContainer` after every test.
-It resets the state of LocalStack after every test so that each new test starts
-from a clean and predictable state. That way, we avoid flaky tests that depend on the
-state of the previous test or their execution order.
-As a downside, it takes a bit more time to restart the container after every test,
-so it might not be necessary for every test.
+On `tomodachi_container` fixture teardown, `LocalStack` container is restarted
+to reset its state - delete all S3 buckets and files. This way we can be sure
+that each test starts with a clean state.
+As alternative for calling `restart_container` method explicitly,
+you can use `_restart_localstack_container_on_teardown` fixture.
+We avoid flaky tests that depend on the state of the previous test or their execution order,
+and avoid leaking test data from one test to another.
+As a drawback, it takes a more time to restart a container after every test.
+To improve test execution speed, you can explicitly cleanup AWS resources, for example,
+deleting all S3 buckets and DynamoDB tables after every test.
 
 That's the setup, now on to the application test. 🧪
 
 ```python
 import httpx
 import pytest
 from types_aiobotocore_s3 import S3Client
```

