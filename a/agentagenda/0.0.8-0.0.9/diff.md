# Comparing `tmp/agentagenda-0.0.8.tar.gz` & `tmp/agentagenda-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentagenda-0.0.8.tar", last modified: Sun Jul 30 12:57:48 2023, max compression
+gzip compressed data, was "agentagenda-0.0.9.tar", last modified: Mon Jul 31 00:56:08 2023, max compression
```

## Comparing `agentagenda-0.0.8.tar` & `agentagenda-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:57:48.890134 agentagenda-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-30 12:57:35.000000 agentagenda-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-30 12:57:48.886134 agentagenda-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-07-30 12:57:35.000000 agentagenda-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:57:48.886134 agentagenda-0.0.8/agentagenda/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-30 12:57:35.000000 agentagenda-0.0.8/agentagenda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16577 2023-07-30 12:57:35.000000 agentagenda-0.0.8/agentagenda/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-07-30 12:57:35.000000 agentagenda-0.0.8/agentagenda/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:57:48.886134 agentagenda-0.0.8/agentagenda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-30 12:57:48.000000 agentagenda-0.0.8/agentagenda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-30 12:57:48.000000 agentagenda-0.0.8/agentagenda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 12:57:48.000000 agentagenda-0.0.8/agentagenda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-30 12:57:48.000000 agentagenda-0.0.8/agentagenda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-30 12:57:48.000000 agentagenda-0.0.8/agentagenda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 12:57:48.890134 agentagenda-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-30 12:57:35.000000 agentagenda-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:56:08.627672 agentagenda-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-31 00:55:56.000000 agentagenda-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-07-31 00:56:08.623672 agentagenda-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-31 00:55:56.000000 agentagenda-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:56:08.623672 agentagenda-0.0.9/agentagenda/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-31 00:55:56.000000 agentagenda-0.0.9/agentagenda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16899 2023-07-31 00:55:56.000000 agentagenda-0.0.9/agentagenda/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-07-31 00:55:56.000000 agentagenda-0.0.9/agentagenda/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:56:08.623672 agentagenda-0.0.9/agentagenda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-07-31 00:56:08.000000 agentagenda-0.0.9/agentagenda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-31 00:56:08.000000 agentagenda-0.0.9/agentagenda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 00:56:08.000000 agentagenda-0.0.9/agentagenda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-31 00:56:08.000000 agentagenda-0.0.9/agentagenda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 00:56:08.000000 agentagenda-0.0.9/agentagenda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 00:56:08.627672 agentagenda-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-31 00:55:56.000000 agentagenda-0.0.9/setup.py
```

### Comparing `agentagenda-0.0.8/LICENSE` & `agentagenda-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `agentagenda-0.0.8/PKG-INFO` & `agentagenda-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentagenda
-Version: 0.0.8
+Version: 0.0.9
 Summary: A task manager for your agent.
 Home-page: https://github.com/AutonomousResearchGroup/agentagenda
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
@@ -41,81 +41,105 @@
 print(task)
 
 # Complete the task
 finish_task(task)
 ```
 
 ### 1. Creating a Task:
+
 To create a task, use the `create_task` method. You can optionally specify a plan and steps.
+
 ```python
 task = create_task("Finish the project", plan="Plan for the project")
 print(task)
 ```
 
 ### 2. List All Tasks:
+
 Retrieve a list of all tasks that are in progress using the `list_tasks` method.
+
 ```python
 tasks = list_tasks()
 print(tasks)
 ```
 
 ### 3. Search for Tasks:
+
 You can search for specific tasks using the `search_tasks` method.
+
 ```python
 tasks = search_tasks("project")
 print(tasks)
 ```
 
 ### 4. Deleting a Task:
+
 To delete a task, use the `delete_task` method.
+
 ```python
 delete_task(task)
 ```
 
 ### 5. Completing a Task:
+
 Mark a task as complete using the `finish_task` method.
+
 ```python
 finish_task(task)
 ```
 
 ### 6. Cancelling a Task:
+
 If you want to cancel a task, use the `cancel_task` method.
+
 ```python
 cancel_task(task)
 ```
 
 ### 7. Retrieve Task ID:
+
 To get the ID of a specific task, use the `get_task_id` method.
+
 ```python
 task_id = get_task_id(task)
 print(task_id)
 ```
 
 ### 8. Working with Plans:
+
 - To create a plan for a specific goal, use the `create_plan` method.
+
 ```python
 plan = create_plan("Finish the project")
 print(plan)
 ```
+
 - To update the plan of a specific task, use the `update_plan` method.
+
 ```python
 update_plan(task, "New plan for the project")
 ```
 
 ### 9. Working with Steps:
+
 - To create a list of steps based on a given goal and plan, use the `create_steps` method.
+
 ```python
 steps = create_steps("Finish the project", "Plan for the project")
 print(steps)
 ```
+
 - To add a new step to a task, use the `add_step` method.
+
 ```python
 add_step(task, "New step for the project")
 ```
+
 - To mark a specific step of a task as complete, use the `finish_step` method.
+
 ```python
 finish_step(task, "Step to complete")
 ```
 
 ## Documentation
 
 **`create_task(goal: str, plan: str = None, steps: dict = None) -> dict`**
@@ -315,22 +339,22 @@
 
     *Example:*
 
     ```python
     cancel_step(task, "Step to cancel")
     ```
 
-**`get_task_as_formatted_string(task: dict, include_plan: bool = True, include_status: bool = True, include_steps: bool = True) -> str`**
+**`get_task_as_formatted_string(task: dict, include_plan: bool = True, include_current_step: bool = True, include_status: bool = True, include_steps: bool = True) -> str`**
 
     Returns a string representation of the task, including the plan, status, and steps based on the arguments provided.
 
     *Example:*
 
     ```python
-    task_string = get_task_as_formatted_string(task, include_plan=True, include_status=True, include_steps=True)
+    task_string = get_task_as_formatted_string(task, include_plan=True, include_current_step=True, include_status=True, include_steps=True)
     print(task_string)
     ```
 
 **`list_tasks_as_formatted_string() -> str`**
 
     Retrieves and formats a list of all current tasks. Returns a string containing details of all current tasks.
```

### Comparing `agentagenda-0.0.8/README.md` & `agentagenda-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -25,81 +25,105 @@
 print(task)
 
 # Complete the task
 finish_task(task)
 ```
 
 ### 1. Creating a Task:
+
 To create a task, use the `create_task` method. You can optionally specify a plan and steps.
+
 ```python
 task = create_task("Finish the project", plan="Plan for the project")
 print(task)
 ```
 
 ### 2. List All Tasks:
+
 Retrieve a list of all tasks that are in progress using the `list_tasks` method.
+
 ```python
 tasks = list_tasks()
 print(tasks)
 ```
 
 ### 3. Search for Tasks:
+
 You can search for specific tasks using the `search_tasks` method.
+
 ```python
 tasks = search_tasks("project")
 print(tasks)
 ```
 
 ### 4. Deleting a Task:
+
 To delete a task, use the `delete_task` method.
+
 ```python
 delete_task(task)
 ```
 
 ### 5. Completing a Task:
+
 Mark a task as complete using the `finish_task` method.
+
 ```python
 finish_task(task)
 ```
 
 ### 6. Cancelling a Task:
+
 If you want to cancel a task, use the `cancel_task` method.
+
 ```python
 cancel_task(task)
 ```
 
 ### 7. Retrieve Task ID:
+
 To get the ID of a specific task, use the `get_task_id` method.
+
 ```python
 task_id = get_task_id(task)
 print(task_id)
 ```
 
 ### 8. Working with Plans:
+
 - To create a plan for a specific goal, use the `create_plan` method.
+
 ```python
 plan = create_plan("Finish the project")
 print(plan)
 ```
+
 - To update the plan of a specific task, use the `update_plan` method.
+
 ```python
 update_plan(task, "New plan for the project")
 ```
 
 ### 9. Working with Steps:
+
 - To create a list of steps based on a given goal and plan, use the `create_steps` method.
+
 ```python
 steps = create_steps("Finish the project", "Plan for the project")
 print(steps)
 ```
+
 - To add a new step to a task, use the `add_step` method.
+
 ```python
 add_step(task, "New step for the project")
 ```
+
 - To mark a specific step of a task as complete, use the `finish_step` method.
+
 ```python
 finish_step(task, "Step to complete")
 ```
 
 ## Documentation
 
 **`create_task(goal: str, plan: str = None, steps: dict = None) -> dict`**
@@ -299,22 +323,22 @@
 
     *Example:*
 
     ```python
     cancel_step(task, "Step to cancel")
     ```
 
-**`get_task_as_formatted_string(task: dict, include_plan: bool = True, include_status: bool = True, include_steps: bool = True) -> str`**
+**`get_task_as_formatted_string(task: dict, include_plan: bool = True, include_current_step: bool = True, include_status: bool = True, include_steps: bool = True) -> str`**
 
     Returns a string representation of the task, including the plan, status, and steps based on the arguments provided.
 
     *Example:*
 
     ```python
-    task_string = get_task_as_formatted_string(task, include_plan=True, include_status=True, include_steps=True)
+    task_string = get_task_as_formatted_string(task, include_plan=True, include_current_step=True, include_status=True, include_steps=True)
     print(task_string)
     ```
 
 **`list_tasks_as_formatted_string() -> str`**
 
     Retrieves and formats a list of all current tasks. Returns a string containing details of all current tasks.
```

#### html2text {}

```diff
@@ -81,19 +81,21 @@
 specified step of the specified task as complete. The task can be specified as
 a dictionary (as returned by `create_task`), an integer ID, or a string ID.
 *Example:* ```python finish_step(task, "Step to complete") ``` **`cancel_step
 (task: Union[dict, int, str], step: str) -> dict`** Cancels the specified step
 of the specified task. The task can be specified as a dictionary (as returned
 by `create_task`), an integer ID, or a string ID. *Example:* ```python
 cancel_step(task, "Step to cancel") ``` **`get_task_as_formatted_string(task:
-dict, include_plan: bool = True, include_status: bool = True, include_steps:
-bool = True) -> str`** Returns a string representation of the task, including
-the plan, status, and steps based on the arguments provided. *Example:
-* ```python task_string = get_task_as_formatted_string(task, include_plan=True,
-include_status=True, include_steps=True) print(task_string) ```
-**`list_tasks_as_formatted_string() -> str`** Retrieves and formats a list of
-all current tasks. Returns a string containing details of all current tasks.
-*Example:* ```python tasks_string = list_tasks_as_formatted_string() print
-(tasks_string) ``` # Contributions Welcome If you like this library and want to
-contribute in any way, please feel free to submit a PR and I will review it.
-Please note that the goal here is simplicity and accesibility, using common
-language and few dependencies. [resources/youcreatethefuture.jpg]
+dict, include_plan: bool = True, include_current_step: bool = True,
+include_status: bool = True, include_steps: bool = True) -> str`** Returns a
+string representation of the task, including the plan, status, and steps based
+on the arguments provided. *Example:* ```python task_string =
+get_task_as_formatted_string(task, include_plan=True,
+include_current_step=True, include_status=True, include_steps=True) print
+(task_string) ``` **`list_tasks_as_formatted_string() -> str`** Retrieves and
+formats a list of all current tasks. Returns a string containing details of all
+current tasks. *Example:* ```python tasks_string =
+list_tasks_as_formatted_string() print(tasks_string) ``` # Contributions
+Welcome If you like this library and want to contribute in any way, please feel
+free to submit a PR and I will review it. Please note that the goal here is
+simplicity and accesibility, using common language and few dependencies.
+[resources/youcreatethefuture.jpg]
```

### Comparing `agentagenda-0.0.8/agentagenda/main.py` & `agentagenda-0.0.9/agentagenda/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
         steps = response["arguments"]["steps"]
 
         step_items = []
 
         for step in steps:
             step_items.append({"content": step, "completed": False})
-        
+
         steps = step_items
 
     # if steps is a dict, json stringify it
     if isinstance(steps, dict) or isinstance(steps, list):
         steps = json.dumps(steps)
 
     # get timestamp
@@ -472,15 +472,15 @@
         The updated task after marking the step as completed.
     """
     task_id = get_task_id(task)
     task = get_memory("task", task_id)
     metadata = task["metadata"]
     steps = json.loads(metadata["steps"])
     for s in steps:
-        if s["content"].includes(step):
+        if step.lower() in s["content"].lower() or s["content"].lower() in step.lower():
             s["completed"] = True
     metadata["steps"] = json.dumps(steps)
     log(
         "Finishing step for task: {}\nSteps are: {}".format(task, metadata["steps"]),
         log=debug,
     )
     metadata["updated_at"] = datetime.timestamp(datetime.now())
@@ -535,15 +535,19 @@
             return step
 
     # If all steps are completed, return None
     return None
 
 
 def get_task_as_formatted_string(
-    task, include_plan=True, include_status=True, include_steps=True
+    task,
+    include_current_step=True,
+    include_plan=True,
+    include_status=True,
+    include_steps=True,
 ):
     """
     This function will return a string representation of the task,
     including the plan, status and steps based on the arguments provided
     """
 
     # Define an empty list to store the task details
@@ -552,18 +556,24 @@
     # Append each detail to the list based on the arguments
     if include_plan:
         task_details.append("Plan: {}".format(task["metadata"]["plan"]))
 
     if include_status:
         task_details.append("Status: {}".format(task["metadata"]["status"]))
 
-    if include_steps:
-        # For the steps, since it's a list, we need to format each step separately
-        steps = json.loads(task["metadata"]["steps"])
+    # For the steps, since it's a list, we need to format each step separately
+    steps = json.loads(task["metadata"]["steps"])
 
+    if include_current_step:
+        # find the first step that isn't completed
+        current_step = get_next_step(task)
+        if current_step is not None:
+            task_details.append("Current Step: {}".format(current_step["content"]))
+
+    if include_steps:
         formatted_steps = ", ".join(
             [
                 "{}: {}".format(
                     step["content"],
                     "Completed" if step["completed"] else "Not completed",
                 )
                 for step in steps
```

### Comparing `agentagenda-0.0.8/agentagenda/test.py` & `agentagenda-0.0.9/agentagenda/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,14 +233,15 @@
         }
     }
 
     task_string = get_task_as_formatted_string(task)
     expected_string = (
         "Plan: Plan 1\n"
         "Status: in_progress\n"
+        "Current Step: Step 1\n"
         "Steps: Step 1: Not completed, Step 2: Not completed"
     )
     assert task_string == expected_string
 
 
 def test_list_tasks_as_formatted_string():
     # Setup: Create multiple tasks
```

### Comparing `agentagenda-0.0.8/agentagenda.egg-info/PKG-INFO` & `agentagenda-0.0.9/agentagenda.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentagenda
-Version: 0.0.8
+Version: 0.0.9
 Summary: A task manager for your agent.
 Home-page: https://github.com/AutonomousResearchGroup/agentagenda
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
@@ -41,81 +41,105 @@
 print(task)
 
 # Complete the task
 finish_task(task)
 ```
 
 ### 1. Creating a Task:
+
 To create a task, use the `create_task` method. You can optionally specify a plan and steps.
+
 ```python
 task = create_task("Finish the project", plan="Plan for the project")
 print(task)
 ```
 
 ### 2. List All Tasks:
+
 Retrieve a list of all tasks that are in progress using the `list_tasks` method.
+
 ```python
 tasks = list_tasks()
 print(tasks)
 ```
 
 ### 3. Search for Tasks:
+
 You can search for specific tasks using the `search_tasks` method.
+
 ```python
 tasks = search_tasks("project")
 print(tasks)
 ```
 
 ### 4. Deleting a Task:
+
 To delete a task, use the `delete_task` method.
+
 ```python
 delete_task(task)
 ```
 
 ### 5. Completing a Task:
+
 Mark a task as complete using the `finish_task` method.
+
 ```python
 finish_task(task)
 ```
 
 ### 6. Cancelling a Task:
+
 If you want to cancel a task, use the `cancel_task` method.
+
 ```python
 cancel_task(task)
 ```
 
 ### 7. Retrieve Task ID:
+
 To get the ID of a specific task, use the `get_task_id` method.
+
 ```python
 task_id = get_task_id(task)
 print(task_id)
 ```
 
 ### 8. Working with Plans:
+
 - To create a plan for a specific goal, use the `create_plan` method.
+
 ```python
 plan = create_plan("Finish the project")
 print(plan)
 ```
+
 - To update the plan of a specific task, use the `update_plan` method.
+
 ```python
 update_plan(task, "New plan for the project")
 ```
 
 ### 9. Working with Steps:
+
 - To create a list of steps based on a given goal and plan, use the `create_steps` method.
+
 ```python
 steps = create_steps("Finish the project", "Plan for the project")
 print(steps)
 ```
+
 - To add a new step to a task, use the `add_step` method.
+
 ```python
 add_step(task, "New step for the project")
 ```
+
 - To mark a specific step of a task as complete, use the `finish_step` method.
+
 ```python
 finish_step(task, "Step to complete")
 ```
 
 ## Documentation
 
 **`create_task(goal: str, plan: str = None, steps: dict = None) -> dict`**
@@ -315,22 +339,22 @@
 
     *Example:*
 
     ```python
     cancel_step(task, "Step to cancel")
     ```
 
-**`get_task_as_formatted_string(task: dict, include_plan: bool = True, include_status: bool = True, include_steps: bool = True) -> str`**
+**`get_task_as_formatted_string(task: dict, include_plan: bool = True, include_current_step: bool = True, include_status: bool = True, include_steps: bool = True) -> str`**
 
     Returns a string representation of the task, including the plan, status, and steps based on the arguments provided.
 
     *Example:*
 
     ```python
-    task_string = get_task_as_formatted_string(task, include_plan=True, include_status=True, include_steps=True)
+    task_string = get_task_as_formatted_string(task, include_plan=True, include_current_step=True, include_status=True, include_steps=True)
     print(task_string)
     ```
 
 **`list_tasks_as_formatted_string() -> str`**
 
     Retrieves and formats a list of all current tasks. Returns a string containing details of all current tasks.
```

### Comparing `agentagenda-0.0.8/setup.py` & `agentagenda-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
     long_description = "\n".join(long_description)
 
 
 setup(
     name="agentagenda",
-    version="0.0.8",
+    version="0.0.9",
     description="A task manager for your agent.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/agentagenda",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

