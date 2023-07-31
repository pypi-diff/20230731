# Comparing `tmp/stigg_api_client_v2-0.514.0.tar.gz` & `tmp/stigg_api_client_v2-0.515.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.514.0.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.515.3.tar", max compression
```

## Comparing `stigg_api_client_v2-0.514.0.tar` & `stigg_api_client_v2-0.515.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1644 2023-07-31 04:59:48.403418 stigg_api_client_v2-0.514.0/README.md
--rw-r--r--   0        0        0      452 2023-07-31 05:00:39.428008 stigg_api_client_v2-0.514.0/pyproject.toml
--rw-r--r--   0        0        0       62 2023-07-31 04:59:48.403418 stigg_api_client_v2-0.514.0/stigg/__init__.py
--rw-r--r--   0        0        0     4711 2023-07-31 04:59:48.403418 stigg_api_client_v2-0.514.0/stigg/client.py
--rw-r--r--   0        0        0      932 2023-07-31 04:59:48.403418 stigg_api_client_v2-0.514.0/stigg/edge_utils.py
--rw-r--r--   0        0        0    40986 2023-07-31 05:00:37.499984 stigg_api_client_v2-0.514.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0      460 2023-07-31 05:00:35.907964 stigg_api_client_v2-0.514.0/stigg/generated/archive_customer.py
--rw-r--r--   0        0        0     7303 2023-07-31 05:00:36.935977 stigg_api_client_v2-0.514.0/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0    70891 2023-07-31 05:00:37.195980 stigg_api_client_v2-0.514.0/stigg/generated/async_client.py
--rw-r--r--   0        0        0     2731 2023-07-31 05:00:31.087908 stigg_api_client_v2-0.514.0/stigg/generated/base_client.py
--rw-r--r--   0        0        0     1951 2023-07-31 05:00:36.935977 stigg_api_client_v2-0.514.0/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-07-31 05:00:35.843963 stigg_api_client_v2-0.514.0/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-07-31 05:00:35.863964 stigg_api_client_v2-0.514.0/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    70464 2023-07-31 05:00:31.339911 stigg_api_client_v2-0.514.0/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-07-31 05:00:35.891964 stigg_api_client_v2-0.514.0/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0    24198 2023-07-31 05:00:33.155932 stigg_api_client_v2-0.514.0/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-07-31 05:00:35.851963 stigg_api_client_v2-0.514.0/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-07-31 05:00:35.859964 stigg_api_client_v2-0.514.0/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-07-31 05:00:36.935977 stigg_api_client_v2-0.514.0/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    58974 2023-07-31 05:00:36.935977 stigg_api_client_v2-0.514.0/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-07-31 05:00:35.923964 stigg_api_client_v2-0.514.0/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-07-31 05:00:35.931964 stigg_api_client_v2-0.514.0/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-07-31 05:00:35.915964 stigg_api_client_v2-0.514.0/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-07-31 05:00:35.979965 stigg_api_client_v2-0.514.0/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-07-31 05:00:35.951965 stigg_api_client_v2-0.514.0/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-07-31 05:00:35.943965 stigg_api_client_v2-0.514.0/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-07-31 05:00:35.987965 stigg_api_client_v2-0.514.0/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-07-31 05:00:35.939964 stigg_api_client_v2-0.514.0/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-07-31 05:00:35.959965 stigg_api_client_v2-0.514.0/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-07-31 05:00:35.971965 stigg_api_client_v2-0.514.0/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-07-31 05:00:35.803963 stigg_api_client_v2-0.514.0/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-07-31 05:00:35.799963 stigg_api_client_v2-0.514.0/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-07-31 05:00:35.827963 stigg_api_client_v2-0.514.0/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   127277 2023-07-31 05:00:35.711962 stigg_api_client_v2-0.514.0/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-07-31 05:00:35.899964 stigg_api_client_v2-0.514.0/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-07-31 05:00:35.791963 stigg_api_client_v2-0.514.0/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-07-31 05:00:35.823963 stigg_api_client_v2-0.514.0/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-07-31 05:00:35.883964 stigg_api_client_v2-0.514.0/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-07-31 05:00:35.879964 stigg_api_client_v2-0.514.0/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-07-31 05:00:35.871964 stigg_api_client_v2-0.514.0/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-07-31 05:00:36.943977 stigg_api_client_v2-0.514.0/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-07-31 05:00:35.811963 stigg_api_client_v2-0.514.0/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-07-31 05:00:35.835963 stigg_api_client_v2-0.514.0/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      445 2023-07-31 05:00:35.995965 stigg_api_client_v2-0.514.0/stigg/generated/usage_history.py
--rw-r--r--   0        0        0     2075 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.514.0/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-07-31 10:12:25.415652 stigg_api_client_v2-0.515.3/README.md
+-rw-r--r--   0        0        0      452 2023-07-31 10:13:08.553031 stigg_api_client_v2-0.515.3/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-31 10:12:25.415652 stigg_api_client_v2-0.515.3/stigg/__init__.py
+-rw-r--r--   0        0        0     4711 2023-07-31 10:12:25.415652 stigg_api_client_v2-0.515.3/stigg/client.py
+-rw-r--r--   0        0        0      932 2023-07-31 10:12:25.415652 stigg_api_client_v2-0.515.3/stigg/edge_utils.py
+-rw-r--r--   0        0        0    40986 2023-07-31 10:13:06.896977 stigg_api_client_v2-0.515.3/stigg/generated/__init__.py
+-rw-r--r--   0        0        0      460 2023-07-31 10:13:05.508933 stigg_api_client_v2-0.515.3/stigg/generated/archive_customer.py
+-rw-r--r--   0        0        0     7303 2023-07-31 10:13:06.412962 stigg_api_client_v2-0.515.3/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0    70891 2023-07-31 10:13:06.632969 stigg_api_client_v2-0.515.3/stigg/generated/async_client.py
+-rw-r--r--   0        0        0     2731 2023-07-31 10:13:01.336801 stigg_api_client_v2-0.515.3/stigg/generated/base_client.py
+-rw-r--r--   0        0        0     1951 2023-07-31 10:13:06.412962 stigg_api_client_v2-0.515.3/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-07-31 10:13:05.452931 stigg_api_client_v2-0.515.3/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-07-31 10:13:05.468932 stigg_api_client_v2-0.515.3/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    70464 2023-07-31 10:13:01.556808 stigg_api_client_v2-0.515.3/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-07-31 10:13:05.496933 stigg_api_client_v2-0.515.3/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0    24198 2023-07-31 10:13:03.152859 stigg_api_client_v2-0.515.3/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-07-31 10:13:05.456931 stigg_api_client_v2-0.515.3/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-07-31 10:13:05.464932 stigg_api_client_v2-0.515.3/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-07-31 10:13:06.412962 stigg_api_client_v2-0.515.3/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    58974 2023-07-31 10:13:06.408961 stigg_api_client_v2-0.515.3/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-07-31 10:13:05.524933 stigg_api_client_v2-0.515.3/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-07-31 10:13:05.532934 stigg_api_client_v2-0.515.3/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-07-31 10:13:05.512933 stigg_api_client_v2-0.515.3/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-07-31 10:13:05.572935 stigg_api_client_v2-0.515.3/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-07-31 10:13:05.548934 stigg_api_client_v2-0.515.3/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-07-31 10:13:05.544934 stigg_api_client_v2-0.515.3/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-07-31 10:13:05.580935 stigg_api_client_v2-0.515.3/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-07-31 10:13:05.536934 stigg_api_client_v2-0.515.3/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-07-31 10:13:05.556934 stigg_api_client_v2-0.515.3/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-07-31 10:13:05.568935 stigg_api_client_v2-0.515.3/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-07-31 10:13:05.416930 stigg_api_client_v2-0.515.3/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-07-31 10:13:05.408930 stigg_api_client_v2-0.515.3/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-07-31 10:13:05.440931 stigg_api_client_v2-0.515.3/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   127287 2023-07-31 10:13:05.392929 stigg_api_client_v2-0.515.3/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-07-31 10:13:05.500933 stigg_api_client_v2-0.515.3/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-07-31 10:13:05.404930 stigg_api_client_v2-0.515.3/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-07-31 10:13:05.432931 stigg_api_client_v2-0.515.3/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-07-31 10:13:05.488932 stigg_api_client_v2-0.515.3/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-07-31 10:13:05.484932 stigg_api_client_v2-0.515.3/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-07-31 10:13:05.480932 stigg_api_client_v2-0.515.3/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-07-31 10:13:06.416962 stigg_api_client_v2-0.515.3/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-07-31 10:13:05.424930 stigg_api_client_v2-0.515.3/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-07-31 10:13:05.444931 stigg_api_client_v2-0.515.3/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-07-31 10:13:05.588935 stigg_api_client_v2-0.515.3/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0     2075 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.515.3/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.514.0/README.md` & `stigg_api_client_v2-0.515.3/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.514.0/stigg/client.py` & `stigg_api_client_v2-0.515.3/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.514.0/stigg/edge_utils.py` & `stigg_api_client_v2-0.515.3/stigg/edge_utils.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/__init__.py` & `stigg_api_client_v2-0.515.3/stigg/generated/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 
 from .archive_customer import ArchiveCustomer, ArchiveCustomerArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .async_client import AsyncClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.515.3/stigg/generated/async_base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/async_client.py` & `stigg_api_client_v2-0.515.3/stigg/generated/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/base_client.py` & `stigg_api_client_v2-0.515.3/stigg/generated/base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 
 import json
 from typing import Any, Dict, Optional, TypeVar, cast
 
 import httpx
 from pydantic import BaseModel
 from pydantic.json import pydantic_encoder
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/base_model.py` & `stigg_api_client_v2-0.515.3/stigg/generated/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.515.3/stigg/generated/cancel_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/client.py` & `stigg_api_client_v2-0.515.3/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .base_client import BaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.515.3/stigg/generated/create_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/enums.py` & `stigg_api_client_v2-0.515.3/stigg/generated/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerIsArchived = "CustomerIsArchived"
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.515.3/stigg/generated/estimate_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.515.3/stigg/generated/estimate_subscription_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.515.3/stigg/generated/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/fragments.py` & `stigg_api_client_v2-0.515.3/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -125,14 +125,25 @@
     status: SyncStatus
 
 
 class CouponFragmentCustomers(BaseModel):
     id: str
 
 
+class SlimCustomerFragment(BaseModel):
+    id: str
+    name: Optional[str]
+    email: Optional[str]
+    created_at: Optional[Any] = Field(alias="createdAt")
+    updated_at: Any = Field(alias="updatedAt")
+    ref_id: str = Field(alias="refId")
+    billing_id: Optional[str] = Field(alias="billingId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class PromotionalEntitlementFragment(BaseModel):
     status: PromotionalEntitlementStatus
     usage_limit: Optional[float] = Field(alias="usageLimit")
     feature_id: str = Field(alias="featureId")
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
     end_date: Optional[Any] = Field(alias="endDate")
@@ -147,25 +158,14 @@
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     ref_id: str = Field(alias="refId")
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
 
 
-class SlimCustomerFragment(BaseModel):
-    id: str
-    name: Optional[str]
-    email: Optional[str]
-    created_at: Optional[Any] = Field(alias="createdAt")
-    updated_at: Any = Field(alias="updatedAt")
-    ref_id: str = Field(alias="refId")
-    billing_id: Optional[str] = Field(alias="billingId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class CustomerFragment(SlimCustomerFragment):
     has_payment_method: bool = Field(alias="hasPaymentMethod")
     has_active_subscription: bool = Field(alias="hasActiveSubscription")
     default_payment_expiration_month: Optional[int] = Field(
         alias="defaultPaymentExpirationMonth"
     )
     default_payment_expiration_year: Optional[int] = Field(
@@ -342,21 +342,14 @@
     end_date: Optional[Any] = Field(alias="endDate")
 
 
 class CustomerResourceFragment(BaseModel):
     resource_id: str = Field(alias="resourceId")
 
 
-class CustomerPortalSubscriptionAddon(BaseModel):
-    addon_id: str = Field(alias="addonId")
-    description: Optional[str]
-    display_name: str = Field(alias="displayName")
-    quantity: int
-
-
 class CustomerPortalSubscriptionPriceFragment(BaseModel):
     billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
     billing_model: Optional[BillingModel] = Field(alias="billingModel")
     price: Optional["CustomerPortalSubscriptionPriceFragmentPrice"]
     feature: Optional["CustomerPortalSubscriptionPriceFragmentFeature"]
 
 
@@ -421,14 +414,21 @@
     BaseModel
 ):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
+class CustomerPortalSubscriptionAddon(BaseModel):
+    addon_id: str = Field(alias="addonId")
+    description: Optional[str]
+    display_name: str = Field(alias="displayName")
+    quantity: int
+
+
 class CustomerPortalSubscriptionFragment(BaseModel):
     subscription_id: str = Field(alias="subscriptionId")
     plan_name: str = Field(alias="planName")
     pricing_type: PricingType = Field(alias="pricingType")
     prices: List["CustomerPortalSubscriptionFragmentPrices"]
     pricing: "CustomerPortalSubscriptionFragmentPricing"
     status: SubscriptionStatus
@@ -548,87 +548,14 @@
     pass
 
 
 class CustomerPortalFragmentResource(CustomerResourceFragment):
     pass
 
 
-class ProductFragment(BaseModel):
-    ref_id: str = Field(alias="refId")
-    display_name: Optional[str] = Field(alias="displayName")
-    description: Optional[str]
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-    product_settings: "ProductFragmentProductSettings" = Field(alias="productSettings")
-
-
-class ProductFragmentProductSettings(BaseModel):
-    downgrade_plan: Optional["ProductFragmentProductSettingsDowngradePlan"] = Field(
-        alias="downgradePlan"
-    )
-
-
-class ProductFragmentProductSettingsDowngradePlan(BaseModel):
-    ref_id: str = Field(alias="refId")
-    display_name: str = Field(alias="displayName")
-
-
-class PlanFragment(BaseModel):
-    id: str
-    ref_id: str = Field(alias="refId")
-    display_name: str = Field(alias="displayName")
-    description: Optional[str]
-    billing_id: Optional[str] = Field(alias="billingId")
-    version_number: int = Field(alias="versionNumber")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-    product: "PlanFragmentProduct"
-    base_plan: Optional["PlanFragmentBasePlan"] = Field(alias="basePlan")
-    entitlements: Optional[List["PlanFragmentEntitlements"]]
-    inherited_entitlements: Optional[List["PlanFragmentInheritedEntitlements"]] = Field(
-        alias="inheritedEntitlements"
-    )
-    compatible_addons: Optional[List["PlanFragmentCompatibleAddons"]] = Field(
-        alias="compatibleAddons"
-    )
-    prices: Optional[List["PlanFragmentPrices"]]
-    pricing_type: Optional[PricingType] = Field(alias="pricingType")
-    default_trial_config: Optional["PlanFragmentDefaultTrialConfig"] = Field(
-        alias="defaultTrialConfig"
-    )
-
-
-class PlanFragmentProduct(ProductFragment):
-    pass
-
-
-class PlanFragmentBasePlan(BaseModel):
-    ref_id: str = Field(alias="refId")
-    display_name: str = Field(alias="displayName")
-
-
-class PlanFragmentEntitlements(PackageEntitlementFragment):
-    pass
-
-
-class PlanFragmentInheritedEntitlements(PackageEntitlementFragment):
-    pass
-
-
-class PlanFragmentCompatibleAddons(AddonFragment):
-    pass
-
-
-class PlanFragmentPrices(PriceFragment):
-    pass
-
-
-class PlanFragmentDefaultTrialConfig(BaseModel):
-    duration: float
-    units: TrialPeriodUnits
-
-
 class SubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
     target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
@@ -719,14 +646,87 @@
 
 class SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables(BaseModel):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
+class ProductFragment(BaseModel):
+    ref_id: str = Field(alias="refId")
+    display_name: Optional[str] = Field(alias="displayName")
+    description: Optional[str]
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+    product_settings: "ProductFragmentProductSettings" = Field(alias="productSettings")
+
+
+class ProductFragmentProductSettings(BaseModel):
+    downgrade_plan: Optional["ProductFragmentProductSettingsDowngradePlan"] = Field(
+        alias="downgradePlan"
+    )
+
+
+class ProductFragmentProductSettingsDowngradePlan(BaseModel):
+    ref_id: str = Field(alias="refId")
+    display_name: str = Field(alias="displayName")
+
+
+class PlanFragment(BaseModel):
+    id: str
+    ref_id: str = Field(alias="refId")
+    display_name: str = Field(alias="displayName")
+    description: Optional[str]
+    billing_id: Optional[str] = Field(alias="billingId")
+    version_number: int = Field(alias="versionNumber")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+    product: "PlanFragmentProduct"
+    base_plan: Optional["PlanFragmentBasePlan"] = Field(alias="basePlan")
+    entitlements: Optional[List["PlanFragmentEntitlements"]]
+    inherited_entitlements: Optional[List["PlanFragmentInheritedEntitlements"]] = Field(
+        alias="inheritedEntitlements"
+    )
+    compatible_addons: Optional[List["PlanFragmentCompatibleAddons"]] = Field(
+        alias="compatibleAddons"
+    )
+    prices: Optional[List["PlanFragmentPrices"]]
+    pricing_type: Optional[PricingType] = Field(alias="pricingType")
+    default_trial_config: Optional["PlanFragmentDefaultTrialConfig"] = Field(
+        alias="defaultTrialConfig"
+    )
+
+
+class PlanFragmentProduct(ProductFragment):
+    pass
+
+
+class PlanFragmentBasePlan(BaseModel):
+    ref_id: str = Field(alias="refId")
+    display_name: str = Field(alias="displayName")
+
+
+class PlanFragmentEntitlements(PackageEntitlementFragment):
+    pass
+
+
+class PlanFragmentInheritedEntitlements(PackageEntitlementFragment):
+    pass
+
+
+class PlanFragmentCompatibleAddons(AddonFragment):
+    pass
+
+
+class PlanFragmentPrices(PriceFragment):
+    pass
+
+
+class PlanFragmentDefaultTrialConfig(BaseModel):
+    duration: float
+    units: TrialPeriodUnits
+
+
 class TotalPriceFragment(BaseModel):
     sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
     total: "TotalPriceFragmentTotal"
 
 
 class TotalPriceFragmentSubTotal(BaseModel):
     amount: float
@@ -1407,17 +1407,17 @@
 PackageEntitlementFragmentFeature.update_forward_refs()
 AddonFragment.update_forward_refs()
 AddonFragmentEntitlements.update_forward_refs()
 AddonFragmentPrices.update_forward_refs()
 CouponFragment.update_forward_refs()
 CouponFragmentSyncStates.update_forward_refs()
 CouponFragmentCustomers.update_forward_refs()
+SlimCustomerFragment.update_forward_refs()
 PromotionalEntitlementFragment.update_forward_refs()
 PromotionalEntitlementFragmentFeature.update_forward_refs()
-SlimCustomerFragment.update_forward_refs()
 CustomerFragment.update_forward_refs()
 CustomerFragmentTrialedPlans.update_forward_refs()
 CustomerFragmentExperimentInfo.update_forward_refs()
 CustomerFragmentCoupon.update_forward_refs()
 CustomerFragmentEligibleForTrial.update_forward_refs()
 CustomerFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalBillingInformation.update_forward_refs()
@@ -1433,23 +1433,23 @@
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
 CustomerPortalPromotionalEntitlement.update_forward_refs()
 CustomerResourceFragment.update_forward_refs()
-CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionPriceFragment.update_forward_refs()
 CustomerPortalSubscriptionPriceFragmentPrice.update_forward_refs()
 CustomerPortalSubscriptionPriceFragmentFeature.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
+CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
 CustomerPortalSubscriptionFragmentPrices.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricing.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingFeature.update_forward_refs()
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
@@ -1461,35 +1461,35 @@
 CustomerPortalFragment.update_forward_refs()
 CustomerPortalFragmentSubscriptions.update_forward_refs()
 CustomerPortalFragmentEntitlements.update_forward_refs()
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
+SubscriptionScheduledUpdateData.update_forward_refs()
+SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
+SubscriptionFutureUpdateData.update_forward_refs()
+SubscriptionFutureUpdateDataTargetPackage.update_forward_refs()
+SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
+SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
+SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 ProductFragment.update_forward_refs()
 ProductFragmentProductSettings.update_forward_refs()
 ProductFragmentProductSettingsDowngradePlan.update_forward_refs()
 PlanFragment.update_forward_refs()
 PlanFragmentProduct.update_forward_refs()
 PlanFragmentBasePlan.update_forward_refs()
 PlanFragmentEntitlements.update_forward_refs()
 PlanFragmentInheritedEntitlements.update_forward_refs()
 PlanFragmentCompatibleAddons.update_forward_refs()
 PlanFragmentPrices.update_forward_refs()
 PlanFragmentDefaultTrialConfig.update_forward_refs()
-SubscriptionScheduledUpdateData.update_forward_refs()
-SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
-SubscriptionFutureUpdateData.update_forward_refs()
-SubscriptionFutureUpdateDataTargetPackage.update_forward_refs()
-SubscriptionFutureUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
-SubscriptionFutureUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
-SubscriptionFutureUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 TotalPriceFragment.update_forward_refs()
 TotalPriceFragmentSubTotal.update_forward_refs()
 TotalPriceFragmentTotal.update_forward_refs()
 SubscriptionFragment.update_forward_refs()
 SubscriptionFragmentResource.update_forward_refs()
 SubscriptionFragmentExperimentInfo.update_forward_refs()
 SubscriptionFragmentPrices.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.515.3/stigg/generated/get_active_subscriptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.515.3/stigg/generated/get_coupons.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.515.3/stigg/generated/get_customer_by_id.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.515.3/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.515.3/stigg/generated/get_mock_paywall.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/get_products.py` & `stigg_api_client_v2-0.515.3/stigg/generated/get_products.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.515.3/stigg/generated/get_sdk_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/input_types.py` & `stigg_api_client_v2-0.515.3/stigg/generated/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -2649,15 +2649,15 @@
     idempotency_key: str = Field(alias="idempotencyKey")
     resource_id: Optional[str] = Field(alias="resourceId")
     timestamp: Optional[Any]
 
 
 class UsageEventsInput(BaseModel):
     environment_id: str = Field(alias="environmentId")
-    filters: List["MeterFilterDefinitionInput"]
+    filters: Optional[List["MeterFilterDefinitionInput"]]
 
 
 class UsageEventsReportInput(BaseModel):
     environment_id: Optional[str] = Field(alias="environmentId")
     usage_events: List["UsageEventReportInput"] = Field(alias="usageEvents")
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.515.3/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.515.3/stigg/generated/provision_customer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.515.3/stigg/generated/provision_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.515.3/stigg/generated/report_usage.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.514.0/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.515.3/stigg/generated/update_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-31 05:00
+# Generated by ariadne-codegen on 2023-07-31 10:13
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.514.0/PKG-INFO` & `stigg_api_client_v2-0.515.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.514.0
+Version: 0.515.3
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

