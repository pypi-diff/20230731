# Comparing `tmp/lunchable-0.8.0.tar.gz` & `tmp/lunchable-0.8.1.tar.gz`

## Comparing `lunchable-0.8.0.tar` & `lunchable-0.8.1.tar`

### file list

```diff
@@ -1,136 +1,136 @@
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 lunchable-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 lunchable-0.8.0/.releaserc.js
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 lunchable-0.8.0/Dockerfile
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 lunchable-0.8.0/docker-compose.yaml
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 lunchable-0.8.0/.github/FUNDING.yaml
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 lunchable-0.8.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 lunchable-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 lunchable-0.8.0/.github/dependabot.yaml
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 lunchable-0.8.0/.github/labels.yaml
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 lunchable-0.8.0/.github/release-drafter.yaml
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 lunchable-0.8.0/.github/matchers/flake8.json
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 lunchable-0.8.0/.github/matchers/mypy.json
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 lunchable-0.8.0/.github/matchers/python.json
--rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 lunchable-0.8.0/.github/semantic_release/package-lock.json
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 lunchable-0.8.0/.github/semantic_release/package.json
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 lunchable-0.8.0/.github/semantic_release/release_notes.hbs
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 lunchable-0.8.0/.github/workflows/docker.yaml
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 lunchable-0.8.0/.github/workflows/labeler.yaml
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 lunchable-0.8.0/.github/workflows/lint.yaml
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 lunchable-0.8.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 lunchable-0.8.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 lunchable-0.8.0/.github/workflows/tests.yaml
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 lunchable-0.8.0/docs/Makefile
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 lunchable-0.8.0/docs/README.md
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 lunchable-0.8.0/docs/requirements.txt
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 lunchable-0.8.0/docs/source/cli.md
--rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 lunchable-0.8.0/docs/source/cli.rst
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 lunchable-0.8.0/docs/source/conf.py
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 lunchable-0.8.0/docs/source/contributing.md
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 lunchable-0.8.0/docs/source/index.rst
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 lunchable-0.8.0/docs/source/lunchable.rst
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 lunchable-0.8.0/docs/source/plugins.rst
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 lunchable-0.8.0/docs/source/primelunch.md
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 lunchable-0.8.0/docs/source/pushlunch.rst
--rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 lunchable-0.8.0/docs/source/splitlunch.rst
--rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 lunchable-0.8.0/docs/source/usage.rst
--rw-r--r--   0        0        0   124987 2020-02-02 00:00:00.000000 lunchable-0.8.0/docs/source/_static/lunchable.png
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/__main__.py
--rw-r--r--   0        0        0    13223 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/_cli.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/_version.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/py.typed
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/_config/__init__.py
--rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/_config/api_config.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/_config/file_config.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/_config/logging_config.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/models/__init__.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/models/_base.py
--rw-r--r--   0        0        0     6260 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/models/_core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/models/_lunchmoney.py
--rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/models/assets.py
--rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/models/budgets.py
--rw-r--r--   0        0        0    15170 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/models/categories.py
--rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/models/crypto.py
--rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/models/plaid_accounts.py
--rw-r--r--   0        0        0     6855 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/models/recurring_expenses.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/models/tags.py
--rw-r--r--   0        0        0    32885 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/models/transactions.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/models/user.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/plugins/__init__.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/plugins/base/__init__.py
--rw-r--r--   0        0        0    12118 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/plugins/base/base_app.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/plugins/base/pandas_app.py
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/plugins/primelunch/README.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/plugins/primelunch/__init__.py
--rw-r--r--   0        0        0    14911 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/plugins/primelunch/primelunch.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/plugins/pushlunch/README.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/plugins/pushlunch/__init__.py
--rw-r--r--   0        0        0    11673 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/plugins/pushlunch/pushover.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/plugins/splitlunch/README.md
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/plugins/splitlunch/__init__.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/plugins/splitlunch/_config.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/plugins/splitlunch/exceptions.py
--rw-r--r--   0        0        0    49340 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/plugins/splitlunch/lunchmoney_splitwise.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 lunchable-0.8.0/lunchable/plugins/splitlunch/models.py
--rw-r--r--   0        0        0    66093 2020-02-02 00:00:00.000000 lunchable-0.8.0/requirements/dev.txt
--rw-r--r--   0        0        0    17968 2020-02-02 00:00:00.000000 lunchable-0.8.0/requirements/prod.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/conftest.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/test_cli.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/test_assets.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/test_budgets.py
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/test_categories.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/test_crypto.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/test_plaid_accounts.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/test_recurring_expenses.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/test_tags.py
--rw-r--r--   0        0        0     4181 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/test_transactions.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/test_user.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_add_to_category_group.yaml
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_create_and_delete_transaction_group.yaml
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_create_asset.yaml
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_create_category.yaml
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_create_category_group.yaml
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_delete_budget.yaml
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_delete_category.yaml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_delete_category_force.yaml
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_get_assets.yaml
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_get_budgets.yaml
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_get_categories.yaml
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_get_category.yaml
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_get_crypto.yaml
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_get_plaid_accounts.yaml
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_get_recurring_expenses.yaml
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_get_tags.yaml
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_get_transaction.yaml
--rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_get_transactions.yaml
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_get_user.yaml
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_insert_transactions.yaml
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_split_transaction.yaml
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_unsplit_transaction.yaml
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_update_asset.yaml
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_update_category.yaml
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_update_crypto.yaml
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_update_transaction.yaml
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/models/cassettes/test_upsert_budget.yaml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/plugins/__init__.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/plugins/pushlunch/__init__.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/plugins/pushlunch/test_pushlunch.py
--rw-r--r--   0        0        0    10630 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/plugins/pushlunch/cassettes/test_post_transaction.yaml
--rw-r--r--   0        0        0     9985 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/plugins/pushlunch/cassettes/test_send_notification.yaml
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/plugins/splitlunch/__init__.py
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/plugins/splitlunch/test_splitwise.py
--rw-r--r--   0        0        0    14089 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/plugins/splitlunch/cassettes/test_update_balance.yaml
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/plugins/splitlunch/data/splitwise_non_involved_expense.json
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/plugins/splitlunch/data/splitwise_non_involved_transfer.json
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/plugins/splitlunch/data/splitwise_non_user_paid_expense.json
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/plugins/splitlunch/data/splitwise_non_user_paid_transfer.json
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/plugins/splitlunch/data/splitwise_user_paid_expense.json
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 lunchable-0.8.0/tests/plugins/splitlunch/data/splitwise_user_paid_transfer.json
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 lunchable-0.8.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 lunchable-0.8.0/LICENSE
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 lunchable-0.8.0/README.md
--rw-r--r--   0        0        0     5574 2020-02-02 00:00:00.000000 lunchable-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 lunchable-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 lunchable-0.8.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 lunchable-0.8.1/.releaserc.js
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 lunchable-0.8.1/Dockerfile
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 lunchable-0.8.1/docker-compose.yaml
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 lunchable-0.8.1/.github/FUNDING.yaml
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 lunchable-0.8.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 lunchable-0.8.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 lunchable-0.8.1/.github/dependabot.yaml
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 lunchable-0.8.1/.github/labels.yaml
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 lunchable-0.8.1/.github/release-drafter.yaml
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 lunchable-0.8.1/.github/matchers/flake8.json
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 lunchable-0.8.1/.github/matchers/mypy.json
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 lunchable-0.8.1/.github/matchers/python.json
+-rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 lunchable-0.8.1/.github/semantic_release/package-lock.json
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 lunchable-0.8.1/.github/semantic_release/package.json
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 lunchable-0.8.1/.github/semantic_release/release_notes.hbs
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 lunchable-0.8.1/.github/workflows/docker.yaml
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 lunchable-0.8.1/.github/workflows/labeler.yaml
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 lunchable-0.8.1/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 lunchable-0.8.1/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 lunchable-0.8.1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 lunchable-0.8.1/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 lunchable-0.8.1/docs/Makefile
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 lunchable-0.8.1/docs/README.md
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 lunchable-0.8.1/docs/requirements.txt
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 lunchable-0.8.1/docs/source/cli.md
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 lunchable-0.8.1/docs/source/cli.rst
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 lunchable-0.8.1/docs/source/conf.py
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 lunchable-0.8.1/docs/source/contributing.md
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 lunchable-0.8.1/docs/source/index.rst
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 lunchable-0.8.1/docs/source/lunchable.rst
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 lunchable-0.8.1/docs/source/plugins.rst
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 lunchable-0.8.1/docs/source/primelunch.md
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 lunchable-0.8.1/docs/source/pushlunch.rst
+-rw-r--r--   0        0        0     4638 2020-02-02 00:00:00.000000 lunchable-0.8.1/docs/source/splitlunch.rst
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 lunchable-0.8.1/docs/source/usage.rst
+-rw-r--r--   0        0        0   124987 2020-02-02 00:00:00.000000 lunchable-0.8.1/docs/source/_static/lunchable.png
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/__main__.py
+-rw-r--r--   0        0        0    13223 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/_cli.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/_version.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/py.typed
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/_config/__init__.py
+-rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/_config/api_config.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/_config/file_config.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/_config/logging_config.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/models/__init__.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/models/_base.py
+-rw-r--r--   0        0        0     6260 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/models/_core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/models/_lunchmoney.py
+-rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/models/assets.py
+-rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/models/budgets.py
+-rw-r--r--   0        0        0    15170 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/models/categories.py
+-rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/models/crypto.py
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/models/plaid_accounts.py
+-rw-r--r--   0        0        0     6855 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/models/recurring_expenses.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/models/tags.py
+-rw-r--r--   0        0        0    32885 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/models/transactions.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/models/user.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/plugins/__init__.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/plugins/base/__init__.py
+-rw-r--r--   0        0        0    12118 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/plugins/base/base_app.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/plugins/base/pandas_app.py
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/plugins/primelunch/README.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/plugins/primelunch/__init__.py
+-rw-r--r--   0        0        0    14911 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/plugins/primelunch/primelunch.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/plugins/pushlunch/README.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/plugins/pushlunch/__init__.py
+-rw-r--r--   0        0        0    11673 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/plugins/pushlunch/pushover.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/plugins/splitlunch/README.md
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/plugins/splitlunch/__init__.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/plugins/splitlunch/_config.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/plugins/splitlunch/exceptions.py
+-rw-r--r--   0        0        0    49345 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/plugins/splitlunch/lunchmoney_splitwise.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 lunchable-0.8.1/lunchable/plugins/splitlunch/models.py
+-rw-r--r--   0        0        0    66093 2020-02-02 00:00:00.000000 lunchable-0.8.1/requirements/dev.txt
+-rw-r--r--   0        0        0    17968 2020-02-02 00:00:00.000000 lunchable-0.8.1/requirements/prod.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/__init__.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/conftest.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/test_cli.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/test_assets.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/test_budgets.py
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/test_categories.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/test_crypto.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/test_plaid_accounts.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/test_recurring_expenses.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/test_tags.py
+-rw-r--r--   0        0        0     4181 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/test_transactions.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/test_user.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_add_to_category_group.yaml
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_create_and_delete_transaction_group.yaml
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_create_asset.yaml
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_create_category.yaml
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_create_category_group.yaml
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_delete_budget.yaml
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_delete_category.yaml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_delete_category_force.yaml
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_get_assets.yaml
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_get_budgets.yaml
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_get_categories.yaml
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_get_category.yaml
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_get_crypto.yaml
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_get_plaid_accounts.yaml
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_get_recurring_expenses.yaml
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_get_tags.yaml
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_get_transaction.yaml
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_get_transactions.yaml
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_get_user.yaml
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_insert_transactions.yaml
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_split_transaction.yaml
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_unsplit_transaction.yaml
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_update_asset.yaml
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_update_category.yaml
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_update_crypto.yaml
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_update_transaction.yaml
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/models/cassettes/test_upsert_budget.yaml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/plugins/__init__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/plugins/pushlunch/__init__.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/plugins/pushlunch/test_pushlunch.py
+-rw-r--r--   0        0        0    10630 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/plugins/pushlunch/cassettes/test_post_transaction.yaml
+-rw-r--r--   0        0        0     9985 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/plugins/pushlunch/cassettes/test_send_notification.yaml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/plugins/splitlunch/__init__.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/plugins/splitlunch/test_splitwise.py
+-rw-r--r--   0        0        0    14089 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/plugins/splitlunch/cassettes/test_update_balance.yaml
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/plugins/splitlunch/data/splitwise_non_involved_expense.json
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/plugins/splitlunch/data/splitwise_non_involved_transfer.json
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/plugins/splitlunch/data/splitwise_non_user_paid_expense.json
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/plugins/splitlunch/data/splitwise_non_user_paid_transfer.json
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/plugins/splitlunch/data/splitwise_user_paid_expense.json
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 lunchable-0.8.1/tests/plugins/splitlunch/data/splitwise_user_paid_transfer.json
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 lunchable-0.8.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 lunchable-0.8.1/LICENSE
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 lunchable-0.8.1/README.md
+-rw-r--r--   0        0        0     5574 2020-02-02 00:00:00.000000 lunchable-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 lunchable-0.8.1/PKG-INFO
```

### Comparing `lunchable-0.8.0/.pre-commit-config.yaml` & `lunchable-0.8.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/.releaserc.js` & `lunchable-0.8.1/.releaserc.js`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/Dockerfile` & `lunchable-0.8.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/docker-compose.yaml` & `lunchable-0.8.1/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/.github/PULL_REQUEST_TEMPLATE.md` & `lunchable-0.8.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/.github/dependabot.yaml` & `lunchable-0.8.1/.github/dependabot.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/.github/labels.yaml` & `lunchable-0.8.1/.github/labels.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/.github/release-drafter.yaml` & `lunchable-0.8.1/.github/release-drafter.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/.github/semantic_release/package-lock.json` & `lunchable-0.8.1/.github/semantic_release/package-lock.json`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/.github/semantic_release/release_notes.hbs` & `lunchable-0.8.1/.github/semantic_release/release_notes.hbs`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/.github/workflows/docker.yaml` & `lunchable-0.8.1/.github/workflows/docker.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/.github/workflows/labeler.yaml` & `lunchable-0.8.1/.github/workflows/labeler.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/.github/workflows/lint.yaml` & `lunchable-0.8.1/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/.github/workflows/publish.yaml` & `lunchable-0.8.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/.github/workflows/release.yaml` & `lunchable-0.8.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/.github/workflows/tests.yaml` & `lunchable-0.8.1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/docs/Makefile` & `lunchable-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/docs/source/cli.rst` & `lunchable-0.8.1/docs/source/cli.rst`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/docs/source/conf.py` & `lunchable-0.8.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/docs/source/contributing.md` & `lunchable-0.8.1/docs/source/contributing.md`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/docs/source/index.rst` & `lunchable-0.8.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/docs/source/primelunch.md` & `lunchable-0.8.1/docs/source/primelunch.md`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/docs/source/pushlunch.rst` & `lunchable-0.8.1/docs/source/pushlunch.rst`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/docs/source/splitlunch.rst` & `lunchable-0.8.1/docs/source/splitlunch.rst`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/docs/source/usage.rst` & `lunchable-0.8.1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/docs/source/_static/lunchable.png` & `lunchable-0.8.1/docs/source/_static/lunchable.png`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/__init__.py` & `lunchable-0.8.1/lunchable/__init__.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/_cli.py` & `lunchable-0.8.1/lunchable/_cli.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/_config/api_config.py` & `lunchable-0.8.1/lunchable/_config/api_config.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/_config/logging_config.py` & `lunchable-0.8.1/lunchable/_config/logging_config.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/models/__init__.py` & `lunchable-0.8.1/lunchable/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/models/_core.py` & `lunchable-0.8.1/lunchable/models/_core.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/models/_lunchmoney.py` & `lunchable-0.8.1/lunchable/models/_lunchmoney.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/models/assets.py` & `lunchable-0.8.1/lunchable/models/assets.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/models/budgets.py` & `lunchable-0.8.1/lunchable/models/budgets.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/models/categories.py` & `lunchable-0.8.1/lunchable/models/categories.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/models/crypto.py` & `lunchable-0.8.1/lunchable/models/crypto.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/models/plaid_accounts.py` & `lunchable-0.8.1/lunchable/models/plaid_accounts.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/models/recurring_expenses.py` & `lunchable-0.8.1/lunchable/models/recurring_expenses.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/models/tags.py` & `lunchable-0.8.1/lunchable/models/tags.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/models/transactions.py` & `lunchable-0.8.1/lunchable/models/transactions.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/models/user.py` & `lunchable-0.8.1/lunchable/models/user.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/plugins/base/base_app.py` & `lunchable-0.8.1/lunchable/plugins/base/base_app.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/plugins/base/pandas_app.py` & `lunchable-0.8.1/lunchable/plugins/base/pandas_app.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/plugins/primelunch/README.md` & `lunchable-0.8.1/lunchable/plugins/primelunch/README.md`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/plugins/primelunch/primelunch.py` & `lunchable-0.8.1/lunchable/plugins/primelunch/primelunch.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/plugins/pushlunch/README.md` & `lunchable-0.8.1/lunchable/plugins/pushlunch/README.md`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/plugins/pushlunch/pushover.py` & `lunchable-0.8.1/lunchable/plugins/pushlunch/pushover.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/plugins/splitlunch/README.md` & `lunchable-0.8.1/lunchable/plugins/splitlunch/README.md`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/lunchable/plugins/splitlunch/lunchmoney_splitwise.py` & `lunchable-0.8.1/lunchable/plugins/splitlunch/lunchmoney_splitwise.py`

 * *Files 0% similar despite different names*

```diff
@@ -874,15 +874,15 @@
                 notes=notes,
                 # financial_impact for self-paid transactions will be negative
                 amount=round(
                     transaction.amount - abs(new_transaction.financial_impact), 2
                 ),
             )
             reimbursement_object = split_object.copy()
-            reimbursement_object.amount = new_transaction.financial_impact
+            reimbursement_object.amount = abs(new_transaction.financial_impact)
             reimbursement_object.category_id = self.reimbursement_category.id
             logger.debug(
                 f"Transaction split by Splitwise: {transaction.amount} -> "
                 f"({split_object.amount}, {reimbursement_object.amount})"
             )
             update_response = self.lunchable.update_transaction(
                 transaction_id=transaction.id,
```

### Comparing `lunchable-0.8.0/lunchable/plugins/splitlunch/models.py` & `lunchable-0.8.1/lunchable/plugins/splitlunch/models.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/requirements/dev.txt` & `lunchable-0.8.1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/requirements/prod.txt` & `lunchable-0.8.1/requirements/prod.txt`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/conftest.py` & `lunchable-0.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/test_assets.py` & `lunchable-0.8.1/tests/models/test_assets.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/test_budgets.py` & `lunchable-0.8.1/tests/models/test_budgets.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/test_categories.py` & `lunchable-0.8.1/tests/models/test_categories.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/test_crypto.py` & `lunchable-0.8.1/tests/models/test_crypto.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/test_plaid_accounts.py` & `lunchable-0.8.1/tests/models/test_plaid_accounts.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/test_recurring_expenses.py` & `lunchable-0.8.1/tests/models/test_recurring_expenses.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/test_tags.py` & `lunchable-0.8.1/tests/models/test_tags.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/test_transactions.py` & `lunchable-0.8.1/tests/models/test_transactions.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_add_to_category_group.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_add_to_category_group.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_create_and_delete_transaction_group.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_create_and_delete_transaction_group.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_create_asset.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_create_asset.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_create_category.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_create_category.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_create_category_group.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_create_category_group.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_delete_budget.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_delete_budget.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_delete_category.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_delete_category.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_delete_category_force.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_delete_category_force.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_get_assets.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_get_assets.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_get_budgets.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_get_budgets.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_get_categories.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_get_categories.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_get_category.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_get_category.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_get_crypto.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_get_crypto.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_get_plaid_accounts.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_get_plaid_accounts.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_get_recurring_expenses.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_get_recurring_expenses.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_get_tags.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_get_tags.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_get_transaction.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_get_transaction.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_get_transactions.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_get_transactions.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_get_user.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_get_user.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_insert_transactions.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_insert_transactions.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_split_transaction.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_split_transaction.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_unsplit_transaction.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_unsplit_transaction.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_update_asset.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_update_asset.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_update_category.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_update_category.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_update_crypto.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_update_crypto.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_update_transaction.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_update_transaction.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/models/cassettes/test_upsert_budget.yaml` & `lunchable-0.8.1/tests/models/cassettes/test_upsert_budget.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/plugins/pushlunch/test_pushlunch.py` & `lunchable-0.8.1/tests/plugins/pushlunch/test_pushlunch.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/plugins/pushlunch/cassettes/test_post_transaction.yaml` & `lunchable-0.8.1/tests/plugins/pushlunch/cassettes/test_post_transaction.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/plugins/pushlunch/cassettes/test_send_notification.yaml` & `lunchable-0.8.1/tests/plugins/pushlunch/cassettes/test_send_notification.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/plugins/splitlunch/test_splitwise.py` & `lunchable-0.8.1/tests/plugins/splitlunch/test_splitwise.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/plugins/splitlunch/cassettes/test_update_balance.yaml` & `lunchable-0.8.1/tests/plugins/splitlunch/cassettes/test_update_balance.yaml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/plugins/splitlunch/data/splitwise_non_involved_expense.json` & `lunchable-0.8.1/tests/plugins/splitlunch/data/splitwise_non_involved_expense.json`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/plugins/splitlunch/data/splitwise_non_involved_transfer.json` & `lunchable-0.8.1/tests/plugins/splitlunch/data/splitwise_non_involved_transfer.json`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/plugins/splitlunch/data/splitwise_non_user_paid_expense.json` & `lunchable-0.8.1/tests/plugins/splitlunch/data/splitwise_non_user_paid_expense.json`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/plugins/splitlunch/data/splitwise_non_user_paid_transfer.json` & `lunchable-0.8.1/tests/plugins/splitlunch/data/splitwise_non_user_paid_transfer.json`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/plugins/splitlunch/data/splitwise_user_paid_expense.json` & `lunchable-0.8.1/tests/plugins/splitlunch/data/splitwise_user_paid_expense.json`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/tests/plugins/splitlunch/data/splitwise_user_paid_transfer.json` & `lunchable-0.8.1/tests/plugins/splitlunch/data/splitwise_user_paid_transfer.json`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/.gitignore` & `lunchable-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/LICENSE` & `lunchable-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/README.md` & `lunchable-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/pyproject.toml` & `lunchable-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lunchable-0.8.0/PKG-INFO` & `lunchable-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lunchable
-Version: 0.8.0
+Version: 0.8.1
 Summary: A simple Python SDK around the Lunch Money Developer API
 Project-URL: Changelog, https://github.com/juftin/lunchable/releases
 Project-URL: Discussions, https://github.com/juftin/lunchable/discussions
 Project-URL: Docker, https://hub.docker.com/r/juftin/lunchable
 Project-URL: Documentation, https://github.com/juftin/lunchable#readme
 Project-URL: Issues, https://github.com/juftin/lunchable/issues
 Project-URL: Source, https://github.com/juftin/lunchable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lunchable Version: 0.8.0 Summary: A simple Python
+Metadata-Version: 2.1 Name: lunchable Version: 0.8.1 Summary: A simple Python
 SDK around the Lunch Money Developer API Project-URL: Changelog, https://
 github.com/juftin/lunchable/releases Project-URL: Discussions, https://
 github.com/juftin/lunchable/discussions Project-URL: Docker, https://
 hub.docker.com/r/juftin/lunchable Project-URL: Documentation, https://
 github.com/juftin/lunchable#readme Project-URL: Issues, https://github.com/
 juftin/lunchable/issues Project-URL: Source, https://github.com/juftin/
 lunchable Author-email: Justin Flannery
```

