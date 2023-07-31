# Comparing `tmp/aws_iam_tester-1.0.3.tar.gz` & `tmp/aws_iam_tester-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_iam_tester-1.0.3.tar", max compression
+gzip compressed data, was "aws_iam_tester-1.0.5.tar", max compression
```

## Comparing `aws_iam_tester-1.0.3.tar` & `aws_iam_tester-1.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2020-06-08 19:14:08.315887 aws_iam_tester-1.0.3/LICENSE
--rw-r--r--   0        0        0    11058 2022-05-16 11:38:15.732588 aws_iam_tester-1.0.3/README.md
--rw-r--r--   0        0        0      157 2021-03-04 11:59:21.240784 aws_iam_tester-1.0.3/aws_iam_tester/__init__.py
--rw-r--r--   0        0        0       27 2020-10-23 20:18:53.274166 aws_iam_tester-1.0.3/aws_iam_tester/__main__.py
--rwxr-xr-x   0        0        0     8494 2021-04-29 08:47:07.038228 aws_iam_tester-1.0.3/aws_iam_tester/cli.py
--rw-r--r--   0        0        0       40 2020-10-23 09:25:43.704372 aws_iam_tester-1.0.3/aws_iam_tester/lib/__init__.py
--rw-r--r--   0        0        0    30411 2022-12-09 08:12:00.858109 aws_iam_tester-1.0.3/aws_iam_tester/lib/aws_iam_tester.py
--rw-r--r--   0        0        0     1128 2023-05-23 06:45:21.893223 aws_iam_tester-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    12419 1970-01-01 00:00:00.000000 aws_iam_tester-1.0.3/setup.py
--rw-r--r--   0        0        0    12266 1970-01-01 00:00:00.000000 aws_iam_tester-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2020-06-08 19:14:08.315887 aws_iam_tester-1.0.5/LICENSE
+-rw-r--r--   0        0        0    11058 2022-05-16 11:38:15.732588 aws_iam_tester-1.0.5/README.md
+-rw-r--r--   0        0        0      157 2021-03-04 11:59:21.240784 aws_iam_tester-1.0.5/aws_iam_tester/__init__.py
+-rw-r--r--   0        0        0       27 2020-10-23 20:18:53.274166 aws_iam_tester-1.0.5/aws_iam_tester/__main__.py
+-rwxr-xr-x   0        0        0     8494 2021-04-29 08:47:07.038228 aws_iam_tester-1.0.5/aws_iam_tester/cli.py
+-rw-r--r--   0        0        0       40 2020-10-23 09:25:43.704372 aws_iam_tester-1.0.5/aws_iam_tester/lib/__init__.py
+-rw-r--r--   0        0        0    30550 2023-06-07 12:21:52.950875 aws_iam_tester-1.0.5/aws_iam_tester/lib/aws_iam_tester.py
+-rw-r--r--   0        0        0     1128 2023-07-31 08:22:40.267168 aws_iam_tester-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    12419 1970-01-01 00:00:00.000000 aws_iam_tester-1.0.5/setup.py
+-rw-r--r--   0        0        0    12266 1970-01-01 00:00:00.000000 aws_iam_tester-1.0.5/PKG-INFO
```

### Comparing `aws_iam_tester-1.0.3/LICENSE` & `aws_iam_tester-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_iam_tester-1.0.3/README.md` & `aws_iam_tester-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `aws_iam_tester-1.0.3/aws_iam_tester/cli.py` & `aws_iam_tester-1.0.5/aws_iam_tester/cli.py`

 * *Files identical despite different names*

### Comparing `aws_iam_tester-1.0.3/aws_iam_tester/lib/aws_iam_tester.py` & `aws_iam_tester-1.0.5/aws_iam_tester/lib/aws_iam_tester.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,18 @@
                 # convert key to CamelCase
                 if isinstance(key, str):
                     new_key = ''.join(x.capitalize() or '_' for x in key.split('_'))
                     result[new_key] = value
 
                     # the ContextKeyValues should be a list
                     if new_key == 'ContextKeyValues':
-                        result[new_key] = [value]
+                        if isinstance(value, list):
+                            result[new_key] = value
+                        else:    
+                         result[new_key] = [value]
                 else:
                     result[key] = value
 
             # convert boolean values to strings
             if result['ContextKeyType'] == 'boolean':
                 result['ContextKeyValues'] = [str(x).lower() for x in result['ContextKeyValues']]
```

### Comparing `aws_iam_tester-1.0.3/pyproject.toml` & `aws_iam_tester-1.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-iam-tester"
-version = "1.0.3"
+version = "1.0.5"
 description = "AWS IAM tester - simple command-line tool to check permissions handed out to IAM users and roles."
 authors = ["Gerco Grandia <gerco.grandia@4synergy.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/gercograndia/aws-iam-tester"
 repository = "https://github.com/gercograndia/aws-iam-tester"
 documentation = "https://github.com/gercograndia/aws-iam-tester/blob/master/README.md"
```

### Comparing `aws_iam_tester-1.0.3/setup.py` & `aws_iam_tester-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'termcolor>=2.1.0,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['aws-iam-tester = aws_iam_tester.cli:cli']}
 
 setup_kwargs = {
     'name': 'aws-iam-tester',
-    'version': '1.0.3',
+    'version': '1.0.5',
     'description': 'AWS IAM tester - simple command-line tool to check permissions handed out to IAM users and roles.',
     'long_description': '# Testing AWS IAM policies\n\n## Introduction\n\nAWS IAM policies are notouriously complex, it is too easy to add some unintended permissions and it is surprisingly difficult to identify these in heavily used AWS accounts.\n\nThankfully AWS has provided an [IAM simulator](https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies_testing-policies.html) that allows you to evaluate existing or new policies for its behavior. Which is very nice, but doing this manually is quite time consuming and it is unrealistic to test the entire environment for what you are trying to do.\n\nHowever, in good AWS spirit the simulator has an API and this tool provides automation on top of it. It allows you to define the complete list of actions you want to evaluate against what resources, which allows you to run these tests on a regular basis or (better) integrate it in your CI/CD pipeline.\n\n## Testing approach\n\nThe testing leverages AWS\' [IAM simulator (api)](https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies_testing-policies.html), that basically includes the same IAM evaluation logic that is applied when working in the console or using the cli. The beneits of this approach are:\n\n- It takes all different levels of policies into account. Think about permission boundaries, service control policies and so on.\n- It is an official service from AWS, so you can expect this to kept up to date over time.\n- The actual actions are evaluated, but NOT executed. Hence no need for cleaning up resources after testing.\n\n# Quick testing\n\nFor convenience, you can use this tool to quickly test whether a user has a specific permission on a particular resource:\n\n```bash\n$ aws-iam-tester access -u the_user -a \'glue:DeleteTable\'\nTest:\nSource:     arn:aws:iam::208912673223:user/the_user\nAction:     glue:DeleteTable\nResource:   *\nResult:     allowed\n\nMatched statements:\nPolicy:     admin_permissions\nType:       IAM Policy\nStart:      L3:C17\nEnd:        L8:C6\n```\n\nOr to see who has access to a particular resource and action by omitting both `user` and `role`:\n\n```bash\n$ aws-iam-tester access -a "s3:PutObject"\n..............\n\nSummary:\n\n| Source                                                   | Action       | Resource   | Decision   | Policies            |\n|----------------------------------------------------------|--------------|------------|------------|---------------------|\n| arn:aws:iam::XXXXXXXXXXXX:user/the_user                  | s3:PutObject | *          | allowed    | admins_permissions  |\n| arn:aws:iam::xxxxxxxxxxxx:role/the_role                  | s3:PutObject | *          | allowed    | AdministratorAccess |\n```\n\n## Finding out who has access to a particular action/resource combination\n\nIt might be useful to check your highly senstive resources and find out who exactly can access these. \n\n```bash\n$ aws-iam-tester access -a "s3:PutObject" -R "arn:aws:s3:::my-strictly-confidential-data"\n..............\n\nSummary:\n\n| Source                                                   | Action       | Resource                                   | Decision   | Policies            |\n|----------------------------------------------------------|--------------|--------------------------------------------|------------|---------------------|\n| arn:aws:iam::XXXXXXXXXXXX:user/the_user                  | s3:PutObject | arn:aws:s3:::my-strictly-confidential-data | allowed    | admins_permissions  |\n| arn:aws:iam::xxxxxxxxxxxx:role/the_role                  | s3:PutObject | arn:aws:s3:::my-strictly-confidential-data | allowed    | AdministratorAccess |\n```\n\n# Account testing\n\nHowever, the initial purpose of this tool is to check an entire account whether there are no users and/or roles having permissons which they should not have.\n\n## Configuration\n\nIn order to run, a configuration of the tests to run is required.\n\nA sample configuration (with only one test) is shown, in various steps.\n\nFirst there is a global section where you define settings which are applied to all tests (unless overruled, more on that later).\n\n```yaml\n---\nuser_landing_account: 0123456789 # ID of AWS Account that is allowed to assume roles in the test account\nglobal_exemptions: # The roles and/or users below will be ignored in all tests. Regular expressions are supported\n- "^arn:aws:iam::(\\\\d{12}):user/(.*)(ADMIN|admin)(.*)$"\n- "^arn:aws:iam::(\\\\d{12}):role/(.*)(ADMIN|admin)(.*)$"\n- "^arn:aws:iam::(\\\\d{12}):role/AWSCloudFormationStackSetExecutionRole$"\n```\n\nThen you define a list of tests, each consisting at least of a set of:\n- actions\n- resources\n- the expected result (should it fail or succeed)\n\n```yaml\n# List of tests to execute. In general the configurations follow the rules of the AWS IAM Policy Simulator.\n# For more information: https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies_testing-policies.html\ntests: \n- actions: # list of actions to validate\n  - "*:*"\n  - iam:*\n  - iam:AddUser*\n  - iam:Attach*\n  - iam:Create*\n  - iam:Delete*\n  - iam:Detach*\n  - iam:Pass*\n  - iam:Put*\n  - iam:Remove*\n  - iam:UpdateAccountPasswordPolicy\n  - sts:AssumeRole\n  - sts:AssumeRoleWithSAML\n  expected_result: fail # \'fail\' or \'succeed\'\n  resources: # list of resources to validate against\n  - "*"\n```\n\nRather than using all users and roles (without exemptions) you can also limit your test to a particular set of users and roles.\n\nThe test below does that, including defining a custom context that specifies multi factor authentication is disabled when running the test. By default the context under which the simulations are run assumes MFA is enabled, but you can override that with the `custom_context` element. For more information see the [AWS documentation](https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies_testing-policies.html).\n\n```yaml\n- actions: # Same list of actions, but now check (with a custom context) whether\n  - "*:*"\n  - iam:*\n  - iam:AddUser*\n  - iam:Attach*\n  - iam:Create*\n  - iam:Delete*\n  - iam:Detach*\n  - iam:Pass*\n  - iam:Put*\n  - iam:Remove*\n  - iam:UpdateAccountPasswordPolicy\n  - sts:AssumeRole\n  - sts:AssumeRoleWithSAML\n  expected_result: fail # \'fail\' or \'succeed\'\n  resources: # list of resources to validate against\n  - "*"\n  limit_to: # check this list for the admin users\n  - "^arn:aws:iam::(\\\\d*):user/(.*)(ADMIN|admin)(.*)$"\n  - "^arn:aws:iam::(\\\\d*):role/(.*)(ADMIN|admin)(.*)$"\n  # test if the admins are required to use multi factor authentication\n  custom_context: \n    - context_key_name: aws:MultiFactorAuthPresent\n      context_key_values: false\n      context_key_type: boolean\n```\n\nOr if you want to do that for **all** tests you can use the `global_limit_to`:\n\n```yaml\n---\nuser_landing_account: 0123456789 # ID of AWS Account that is allowed to assume roles in the test account\nglobal_limit_to: # These roles and/or users below will be u. Regular expressions are supported\n- "^arn:aws:iam::(\\\\d{12}):user/(.*)(ENGINEER|engineer)(.*)$"\n- "^arn:aws:iam::(\\\\d{12}):role/(.*)(SCIENTIST|scientist)(.*)$"\n```\n\nBelow an example where an additional set of roles is exempt from testing:\n\n```yaml\n- actions: # list of data centric actions\n  - redshift:GetClusterCredentials\n  - redshift:JoinGroup\n  - rds:Create*\n  - rds:Delete*\n  - rds:Modify*\n  - rds-db:connect\n  - s3:BypassGovernanceRetention\n  - s3:CreateBucket\n  - s3:DeleteBucket\n  - s3:DeleteBucketPolicy\n  - s3:PutBucketAcl\n  - s3:PutBucketPolicy\n  - s3:PutEncryptionConfiguration\n  - s3:ReplicateDelete\n  expected_result: fail # \'fail\' or \'succeed\'\n  resources: # list of resources to validate against\n  - "*"\n  exemptions: [\n  - "^arn:aws:iam::(\\\\d{12}):role/(.*)_worker$" # ignore this for the worker roles\n  ]\n```\n\nIf you want to run positive tests (i.e. tests that you need to succeed rather than fail), these `exemptions` don\'t work that well.\n\nIn that case you can limit your tests to a set of roles and users:\n\n```yaml\n- actions:\n  - s3:PutObject\n  expected_result: succeed\n  resources:\n  - "arn:aws:s3:::my_bucket/xyz/*"\n  limit_to: # if you specify this, test will only be performed for the sources below\n  - "^arn:aws:iam::(\\\\d{12}):role/my_worker$"\n```\n\n> Note that the exemptions are ignored when using a `limit_to` list.\n\n### Using a dynamic account id in the resource arn\n\nIn case you **need** to specify the `account id` in the resource arn, you can specificy this as follows:\n\n```yaml\n- actions:\n  - "secretsmanager:GetSecretValue"\n  expected_result: succeed\n  resources:\n  - "arn:aws:secretsmanager:eu-central-1:{account_id}:secret:my-secret/*"\n```\n\n### Using regular expressions for user and role matching\n\nRegular expressions can be used when checking the users and/or roles that need to be included in the tests. Hence they are supported for the following elements in the config file:\n\n- limit_to (the filtered list of users/roles to be used for a particular test)\n- global_limit_to (the filtered list of users/roles to be used for all tests)\n- exemptions (the filtered list of users/roles that should be excluded from a particular test)\n- global_exemptions (the filtered list of users/roles that should be excluded from all tests)\n\n> For all other elements, regular expression matching is NOT supported!\n\n## How to use\n\nAssuming you have define a config.yml in your local directory, then to run and write the outputs to the local `./results` directory:\n\n```bash\naws-iam-tester --write-to-file\n```\n\nUsing a specific config file:\n\n```bash\naws-iam-tester --config-file my-config.yml\n```\n\nUsing a specific output location:\n\n```bash\naws-iam-tester --output-location /tmp\n```\n\nOr write to s3:\n\n```bash\naws-iam-tester --output-location s3://my-bucket/my-prefix\n```\n\nInclude only roles that can be assumed by human beings:\n\n```bash\naws-iam-tester --no-include-system-roles\n```\n\n> Note: including system roles does NOT include the aws service roles.\n\nOr print debug output:\n\n```bash\naws-iam-tester --debug\n```\n\nTo run a limited number of evaluations (which helps speeding things up, and avoiding API throttling issues):\n\n```bash\naws-iam-tester --number-of-runs 10\n```\n\nFor more information, run `aws-iam-tester --help` for more instructions.\n\n## Return codes\n\nThe tester returns the following return codes:\n\n- 0 upon successful completion with NO findings\n- 1 upon successful completion with findings\n- 2 (or higher) on failures\n\n## Required permissions\n\nObviously the client has to run under an AWS security context that has sufficient permissions to query the IAM resources and run the simulator.\n\nThe following permissions are needed at the minimum:\n\n```yaml\n- sts:GetCallerIdentity\n- iam:ListAccountAliases\n- iam:ListRoles\n- iam:ListUsers\n- iam:SimulatePrincipalPolicy\n```\n\nAnd if you want to write the output to an s3 location, then obviously you need write access (`s3:PutObject`) to that particular location as well.\n\n## Unit testing\n\n`pytest` is being used for testing the various options.\n\nAs long as the `aws-iam-tester` module is installed, you can run the [tests](./tests).\n\n```console\npytest -vsx\n\n# or, alternatively\npoetry run pytest -vsx\n```\n\nAfter installing `tox`, you can also simply run `$ tox`.',
     'author': 'Gerco Grandia',
     'author_email': 'gerco.grandia@4synergy.nl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/gercograndia/aws-iam-tester',
```

### Comparing `aws_iam_tester-1.0.3/PKG-INFO` & `aws_iam_tester-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-iam-tester
-Version: 1.0.3
+Version: 1.0.5
 Summary: AWS IAM tester - simple command-line tool to check permissions handed out to IAM users and roles.
 Home-page: https://github.com/gercograndia/aws-iam-tester
 License: MIT
 Keywords: AWS,IAM,Policy,Tester,Evaluation,Simulator
 Author: Gerco Grandia
 Author-email: gerco.grandia@4synergy.nl
 Requires-Python: >=3.7.2,<4.0.0
```

