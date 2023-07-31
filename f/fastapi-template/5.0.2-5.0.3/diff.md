# Comparing `tmp/fastapi_template-5.0.2.tar.gz` & `tmp/fastapi_template-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_template-5.0.2.tar", max compression
+gzip compressed data, was "fastapi_template-5.0.3.tar", max compression
```

## Comparing `fastapi_template-5.0.2.tar` & `fastapi_template-5.0.3.tar`

### file list

```diff
@@ -1,159 +1,159 @@
--rw-r--r--   0        0        0     1069 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/LICENSE
--rw-r--r--   0        0        0     4436 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/README.md
--rw-r--r--   0        0        0        0 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/__init__.py
--rw-r--r--   0        0        0     1209 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/__main__.py
--rw-r--r--   0        0        0    21165 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/cli.py
--rw-r--r--   0        0        0     8230 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/input_model.py
--rw-r--r--   0        0        0     1292 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/hooks/__init__.py
--rw-r--r--   0        0        0     2583 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/hooks/post_gen_project.py
--rw-r--r--   0        0        0       28 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/hooks/pre_gen_project.py
--rw-r--r--   0        0        0     2086 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/.dockerignore
--rw-r--r--   0        0        0      463 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/.editorconfig
--rw-r--r--   0        0        0      272 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/.env
--rw-r--r--   0        0        0     2428 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/.flake8
--rw-r--r--   0        0        0     5369 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/.github/workflows/tests.yml
--rw-r--r--   0        0        0     2070 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/.gitignore
--rw-r--r--   0        0        0     3206 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/.gitlab-ci.yml
--rw-r--r--   0        0        0     1743 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0     7290 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0      960 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/alembic.ini
--rw-r--r--   0        0        0     8799 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/conditional_files.json
--rw-r--r--   0        0        0     1006 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/Dockerfile
--rw-r--r--   0        0        0      569 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.dev.yml
--rw-r--r--   0        0        0      565 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.otlp.yml
--rw-r--r--   0        0        0     8154 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.yml
--rw-r--r--   0        0        0     2718 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/app.yml
--rw-r--r--   0        0        0     3002 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/db.yml
--rw-r--r--   0        0        0       87 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/namespace.yml
--rw-r--r--   0        0        0     1242 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/rabbit.yml
--rw-r--r--   0        0        0     1022 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/redis.yml
--rw-r--r--   0        0        0      509 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/otel-collector-config.yml
--rw-r--r--   0        0        0     6903 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      305 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/replaceable_files.json
--rw-r--r--   0        0        0       45 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/__init__.py
--rw-r--r--   0        0        0     2768 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/__main__.py
--rw-r--r--   0        0        0    14107 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/conftest.py
--rw-r--r--   0        0        0      254 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/base.py
--rw-r--r--   0        0        0      134 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/config.py
--rw-r--r--   0        0        0       19 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/dao/__init__.py
--rw-r--r--   0        0        0     1119 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/dao/dummy_dao.py
--rw-r--r--   0        0        0       46 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/meta.py
--rw-r--r--   0        0        0       26 2023-07-23 09:18:44.976941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/__init__.py
--rw-r--r--   0        0        0     2309 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/env.py
--rw-r--r--   0        0        0      510 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/script.py.mako
--rw-r--r--   0        0        0      302 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/versions/2021-08-16-16-53_819cbf6e030b.py
--rw-r--r--   0        0        0      800 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/versions/2021-08-16-16-55_2b7380507a71.py
--rw-r--r--   0        0        0        0 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/versions/__init__.py
--rw-r--r--   0        0        0      421 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/models/__init__.py
--rw-r--r--   0        0        0      308 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/models/dummy_model.py
--rw-r--r--   0        0        0     2762 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/utils.py
--rw-r--r--   0        0        0      532 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/app_conf.py
--rw-r--r--   0        0        0       42 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/dao/__init__.py
--rw-r--r--   0        0        0     1115 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/dao/dummy_dao.py
--rw-r--r--   0        0        0     1067 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/migrations/2022-04-16T17-38-51-672827.py
--rw-r--r--   0        0        0        0 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/migrations/__init__.py
--rw-r--r--   0        0        0       44 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/models/__init__.py
--rw-r--r--   0        0        0      177 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/models/dummy_model.py
--rw-r--r--   0        0        0     2676 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_psycopg/dao/dummy_dao.py
--rw-r--r--   0        0        0      491 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_psycopg/dependencies.py
--rw-r--r--   0        0        0      125 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_psycopg/models/dummy_model.py
--rw-r--r--   0        0        0      182 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/base.py
--rw-r--r--   0        0        0       19 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/dao/__init__.py
--rw-r--r--   0        0        0     1562 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/dao/dummy_dao.py
--rw-r--r--   0        0        0      688 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/dependencies.py
--rw-r--r--   0        0        0       46 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/meta.py
--rw-r--r--   0        0        0       26 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/__init__.py
--rw-r--r--   0        0        0     2486 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/env.py
--rw-r--r--   0        0        0      510 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/script.py.mako
--rw-r--r--   0        0        0      302 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/versions/2021-08-16-16-53_819cbf6e030b.py
--rw-r--r--   0        0        0      819 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/versions/2021-08-16-16-55_2b7380507a71.py
--rw-r--r--   0        0        0        0 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/versions/__init__.py
--rw-r--r--   0        0        0      421 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/models/__init__.py
--rw-r--r--   0        0        0      391 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/models/dummy_model.py
--rw-r--r--   0        0        0     3019 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/utils.py
--rw-r--r--   0        0        0      568 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/config.py
--rw-r--r--   0        0        0       19 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/dao/__init__.py
--rw-r--r--   0        0        0     1082 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/dao/dummy_dao.py
--rw-r--r--   0        0        0      261 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/0_20210928165300_init_mysql.sql
--rw-r--r--   0        0        0      228 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/0_20210928165300_init_pg.sql
--rw-r--r--   0        0        0      242 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/0_20210928165300_init_sqlite.sql
--rw-r--r--   0        0        0      239 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/1_20210928165300_init_dummy_mysql.sql
--rw-r--r--   0        0        0      231 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/1_20210928165300_init_dummy_pg.sql
--rw-r--r--   0        0        0      216 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/1_20210928165300_init_dummy_sqlite.sql
--rw-r--r--   0        0        0       48 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/models/__init__.py
--rw-r--r--   0        0        0      255 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/models/dummy_model.py
--rw-r--r--   0        0        0     2208 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/gunicorn_runner.py
--rw-r--r--   0        0        0     3497 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/logging.py
--rw-r--r--   0        0        0      674 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/piccolo_conf.py
--rw-r--r--   0        0        0       50 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/__init__.py
--rw-r--r--   0        0        0       21 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/kafka/__init__.py
--rw-r--r--   0        0        0      492 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/kafka/dependencies.py
--rw-r--r--   0        0        0      961 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/kafka/lifetime.py
--rw-r--r--   0        0        0       24 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/rabbit/__init__.py
--rw-r--r--   0        0        0      507 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/rabbit/dependencies.py
--rw-r--r--   0        0        0     1656 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/rabbit/lifetime.py
--rw-r--r--   0        0        0       21 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/redis/__init__.py
--rw-r--r--   0        0        0      898 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/redis/dependency.py
--rw-r--r--   0        0        0      583 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/redis/lifetime.py
--rw-r--r--   0        0        0     5489 2023-07-23 09:18:44.980941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/settings.py
--rw-r--r--   0        0        0  1034247 2023-07-23 09:18:44.984941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/redoc.standalone.js
--rw-r--r--   0        0        0  1436263 2023-07-23 09:18:44.992941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/swagger-ui-bundle.js
--rw-r--r--   0        0        0   150945 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/swagger-ui.css
--rw-r--r--   0        0        0       47 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/__init__.py
--rw-r--r--   0        0        0     3265 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_dummy.py
--rw-r--r--   0        0        0     1233 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_echo.py
--rw-r--r--   0        0        0     1706 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_kafka.py
--rw-r--r--   0        0        0     3291 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_rabbit.py
--rw-r--r--   0        0        0     3084 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_redis.py
--rw-r--r--   0        0        0      479 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_{{cookiecutter.project_name}}.py
--rw-r--r--   0        0        0     1091 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tkq.py
--rw-r--r--   0        0        0       49 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/__init__.py
--rw-r--r--   0        0        0       49 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/__init__.py
--rw-r--r--   0        0        0      126 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/docs/__init__.py
--rw-r--r--   0        0        0     1425 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/docs/views.py
--rw-r--r--   0        0        0      114 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/dummy/__init__.py
--rw-r--r--   0        0        0      558 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/dummy/schema.py
--rw-r--r--   0        0        0     1320 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/dummy/views.py
--rw-r--r--   0        0        0      106 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/echo/__init__.py
--rw-r--r--   0        0        0      109 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/echo/schema.py
--rw-r--r--   0        0        0      405 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/echo/views.py
--rw-r--r--   0        0        0      125 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/kafka/__init__.py
--rw-r--r--   0        0        0      131 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/kafka/schema.py
--rw-r--r--   0        0        0      662 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/kafka/views.py
--rw-r--r--   0        0        0      135 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/monitoring/__init__.py
--rw-r--r--   0        0        0      203 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/monitoring/views.py
--rw-r--r--   0        0        0      129 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/rabbit/__init__.py
--rw-r--r--   0        0        0      177 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/rabbit/schema.py
--rw-r--r--   0        0        0     1044 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/rabbit/views.py
--rw-r--r--   0        0        0      108 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/redis/__init__.py
--rw-r--r--   0        0        0      181 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/redis/schema.py
--rw-r--r--   0        0        0     1272 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/redis/views.py
--rw-r--r--   0        0        0     1742 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/router.py
--rw-r--r--   0        0        0     3757 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/application.py
--rw-r--r--   0        0        0       49 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/__init__.py
--rw-r--r--   0        0        0     2541 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/context.py
--rw-r--r--   0        0        0      207 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/__init__.py
--rw-r--r--   0        0        0     1130 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/mutation.py
--rw-r--r--   0        0        0     1388 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/query.py
--rw-r--r--   0        0        0      186 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/schema.py
--rw-r--r--   0        0        0      189 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/echo/__init__.py
--rw-r--r--   0        0        0      350 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/echo/mutation.py
--rw-r--r--   0        0        0      341 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/echo/query.py
--rw-r--r--   0        0        0      136 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/kafka/__init__.py
--rw-r--r--   0        0        0      735 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/kafka/mutation.py
--rw-r--r--   0        0        0      135 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/kafka/schema.py
--rw-r--r--   0        0        0      140 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/rabbit/__init__.py
--rw-r--r--   0        0        0     1133 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/rabbit/mutation.py
--rw-r--r--   0        0        0      166 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/rabbit/schema.py
--rw-r--r--   0        0        0      192 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/__init__.py
--rw-r--r--   0        0        0      870 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/mutation.py
--rw-r--r--   0        0        0      867 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/query.py
--rw-r--r--   0        0        0      273 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/schema.py
--rw-r--r--   0        0        0     1735 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/router.py
--rw-r--r--   0        0        0    11104 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/lifetime.py
--rw-r--r--   0        0        0     2638 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/tests/conftest.py
--rw-r--r--   0        0        0     4903 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/tests/test_generator.py
--rw-r--r--   0        0        0     1769 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/fastapi_template/tests/utils.py
--rw-r--r--   0        0        0     1222 2023-07-23 09:18:44.996941 fastapi_template-5.0.2/pyproject.toml
--rw-r--r--   0        0        0     5416 1970-01-01 00:00:00.000000 fastapi_template-5.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/LICENSE
+-rw-r--r--   0        0        0     4436 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/__init__.py
+-rw-r--r--   0        0        0     1209 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/__main__.py
+-rw-r--r--   0        0        0    21382 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/cli.py
+-rw-r--r--   0        0        0     8230 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/input_model.py
+-rw-r--r--   0        0        0     1292 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/hooks/__init__.py
+-rw-r--r--   0        0        0     2583 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/hooks/post_gen_project.py
+-rw-r--r--   0        0        0       28 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0     2086 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/.dockerignore
+-rw-r--r--   0        0        0      463 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/.editorconfig
+-rw-r--r--   0        0        0      272 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/.env
+-rw-r--r--   0        0        0     2428 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/.flake8
+-rw-r--r--   0        0        0     5369 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     2070 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/.gitignore
+-rw-r--r--   0        0        0     3206 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1743 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     7290 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0      960 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/alembic.ini
+-rw-r--r--   0        0        0     8799 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/conditional_files.json
+-rw-r--r--   0        0        0     1006 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/Dockerfile
+-rw-r--r--   0        0        0      569 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.dev.yml
+-rw-r--r--   0        0        0      565 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.otlp.yml
+-rw-r--r--   0        0        0     8154 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.yml
+-rw-r--r--   0        0        0     2718 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/app.yml
+-rw-r--r--   0        0        0     3002 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/db.yml
+-rw-r--r--   0        0        0       87 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/namespace.yml
+-rw-r--r--   0        0        0     1242 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/rabbit.yml
+-rw-r--r--   0        0        0     1022 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/redis.yml
+-rw-r--r--   0        0        0      509 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/otel-collector-config.yml
+-rw-r--r--   0        0        0     6903 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      305 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/replaceable_files.json
+-rw-r--r--   0        0        0       45 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/__init__.py
+-rw-r--r--   0        0        0     2768 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/__main__.py
+-rw-r--r--   0        0        0    14107 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/conftest.py
+-rw-r--r--   0        0        0      254 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/base.py
+-rw-r--r--   0        0        0      134 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/config.py
+-rw-r--r--   0        0        0       19 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/dao/__init__.py
+-rw-r--r--   0        0        0     1119 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/dao/dummy_dao.py
+-rw-r--r--   0        0        0       46 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/meta.py
+-rw-r--r--   0        0        0       26 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/__init__.py
+-rw-r--r--   0        0        0     2309 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/env.py
+-rw-r--r--   0        0        0      510 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/script.py.mako
+-rw-r--r--   0        0        0      302 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/versions/2021-08-16-16-53_819cbf6e030b.py
+-rw-r--r--   0        0        0      800 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/versions/2021-08-16-16-55_2b7380507a71.py
+-rw-r--r--   0        0        0        0 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/versions/__init__.py
+-rw-r--r--   0        0        0      421 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/models/__init__.py
+-rw-r--r--   0        0        0      308 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/models/dummy_model.py
+-rw-r--r--   0        0        0     2762 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/utils.py
+-rw-r--r--   0        0        0      532 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/app_conf.py
+-rw-r--r--   0        0        0       42 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/dao/__init__.py
+-rw-r--r--   0        0        0     1115 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/dao/dummy_dao.py
+-rw-r--r--   0        0        0     1067 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/migrations/2022-04-16T17-38-51-672827.py
+-rw-r--r--   0        0        0        0 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/migrations/__init__.py
+-rw-r--r--   0        0        0       44 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/models/__init__.py
+-rw-r--r--   0        0        0      177 2023-07-31 11:34:07.758992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/models/dummy_model.py
+-rw-r--r--   0        0        0     2676 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_psycopg/dao/dummy_dao.py
+-rw-r--r--   0        0        0      491 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_psycopg/dependencies.py
+-rw-r--r--   0        0        0      125 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_psycopg/models/dummy_model.py
+-rw-r--r--   0        0        0      182 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/base.py
+-rw-r--r--   0        0        0       19 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/dao/__init__.py
+-rw-r--r--   0        0        0     1562 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/dao/dummy_dao.py
+-rw-r--r--   0        0        0      688 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/dependencies.py
+-rw-r--r--   0        0        0       46 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/meta.py
+-rw-r--r--   0        0        0       26 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/__init__.py
+-rw-r--r--   0        0        0     2486 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/env.py
+-rw-r--r--   0        0        0      510 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/script.py.mako
+-rw-r--r--   0        0        0      302 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/versions/2021-08-16-16-53_819cbf6e030b.py
+-rw-r--r--   0        0        0      819 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/versions/2021-08-16-16-55_2b7380507a71.py
+-rw-r--r--   0        0        0        0 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/versions/__init__.py
+-rw-r--r--   0        0        0      421 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/models/__init__.py
+-rw-r--r--   0        0        0      391 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/models/dummy_model.py
+-rw-r--r--   0        0        0     3019 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/utils.py
+-rw-r--r--   0        0        0      568 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/config.py
+-rw-r--r--   0        0        0       19 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/dao/__init__.py
+-rw-r--r--   0        0        0     1082 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/dao/dummy_dao.py
+-rw-r--r--   0        0        0      261 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/0_20210928165300_init_mysql.sql
+-rw-r--r--   0        0        0      228 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/0_20210928165300_init_pg.sql
+-rw-r--r--   0        0        0      242 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/0_20210928165300_init_sqlite.sql
+-rw-r--r--   0        0        0      239 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/1_20210928165300_init_dummy_mysql.sql
+-rw-r--r--   0        0        0      231 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/1_20210928165300_init_dummy_pg.sql
+-rw-r--r--   0        0        0      216 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/migrations/models/1_20210928165300_init_dummy_sqlite.sql
+-rw-r--r--   0        0        0       48 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/models/__init__.py
+-rw-r--r--   0        0        0      255 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/models/dummy_model.py
+-rw-r--r--   0        0        0     2208 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/gunicorn_runner.py
+-rw-r--r--   0        0        0     3497 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/logging.py
+-rw-r--r--   0        0        0      674 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/piccolo_conf.py
+-rw-r--r--   0        0        0       50 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/__init__.py
+-rw-r--r--   0        0        0       21 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/kafka/__init__.py
+-rw-r--r--   0        0        0      492 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/kafka/dependencies.py
+-rw-r--r--   0        0        0      961 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/kafka/lifetime.py
+-rw-r--r--   0        0        0       24 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/rabbit/__init__.py
+-rw-r--r--   0        0        0      507 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/rabbit/dependencies.py
+-rw-r--r--   0        0        0     1656 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/rabbit/lifetime.py
+-rw-r--r--   0        0        0       21 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/redis/__init__.py
+-rw-r--r--   0        0        0      898 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/redis/dependency.py
+-rw-r--r--   0        0        0      583 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/redis/lifetime.py
+-rw-r--r--   0        0        0     5489 2023-07-31 11:34:07.762992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/settings.py
+-rw-r--r--   0        0        0  1034247 2023-07-31 11:34:07.766992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/redoc.standalone.js
+-rw-r--r--   0        0        0  1436263 2023-07-31 11:34:07.774992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/swagger-ui-bundle.js
+-rw-r--r--   0        0        0   150945 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/swagger-ui.css
+-rw-r--r--   0        0        0       47 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/__init__.py
+-rw-r--r--   0        0        0     3265 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_dummy.py
+-rw-r--r--   0        0        0     1233 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_echo.py
+-rw-r--r--   0        0        0     1706 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_kafka.py
+-rw-r--r--   0        0        0     3291 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_rabbit.py
+-rw-r--r--   0        0        0     3084 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_redis.py
+-rw-r--r--   0        0        0      479 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_{{cookiecutter.project_name}}.py
+-rw-r--r--   0        0        0     1091 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tkq.py
+-rw-r--r--   0        0        0       49 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/__init__.py
+-rw-r--r--   0        0        0       49 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/__init__.py
+-rw-r--r--   0        0        0      126 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/docs/__init__.py
+-rw-r--r--   0        0        0     1425 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/docs/views.py
+-rw-r--r--   0        0        0      114 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/dummy/__init__.py
+-rw-r--r--   0        0        0      558 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/dummy/schema.py
+-rw-r--r--   0        0        0     1320 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/dummy/views.py
+-rw-r--r--   0        0        0      106 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/echo/__init__.py
+-rw-r--r--   0        0        0      109 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/echo/schema.py
+-rw-r--r--   0        0        0      405 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/echo/views.py
+-rw-r--r--   0        0        0      125 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/kafka/__init__.py
+-rw-r--r--   0        0        0      131 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/kafka/schema.py
+-rw-r--r--   0        0        0      662 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/kafka/views.py
+-rw-r--r--   0        0        0      135 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/monitoring/__init__.py
+-rw-r--r--   0        0        0      203 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/monitoring/views.py
+-rw-r--r--   0        0        0      129 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/rabbit/__init__.py
+-rw-r--r--   0        0        0      177 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/rabbit/schema.py
+-rw-r--r--   0        0        0     1044 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/rabbit/views.py
+-rw-r--r--   0        0        0      108 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/redis/__init__.py
+-rw-r--r--   0        0        0      181 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/redis/schema.py
+-rw-r--r--   0        0        0     1272 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/redis/views.py
+-rw-r--r--   0        0        0     1742 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/router.py
+-rw-r--r--   0        0        0     3757 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/application.py
+-rw-r--r--   0        0        0       49 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/__init__.py
+-rw-r--r--   0        0        0     2541 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/context.py
+-rw-r--r--   0        0        0      207 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/__init__.py
+-rw-r--r--   0        0        0     1130 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/mutation.py
+-rw-r--r--   0        0        0     1388 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/query.py
+-rw-r--r--   0        0        0      186 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/schema.py
+-rw-r--r--   0        0        0      189 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/echo/__init__.py
+-rw-r--r--   0        0        0      350 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/echo/mutation.py
+-rw-r--r--   0        0        0      341 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/echo/query.py
+-rw-r--r--   0        0        0      136 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/kafka/__init__.py
+-rw-r--r--   0        0        0      735 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/kafka/mutation.py
+-rw-r--r--   0        0        0      135 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/kafka/schema.py
+-rw-r--r--   0        0        0      140 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/rabbit/__init__.py
+-rw-r--r--   0        0        0     1133 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/rabbit/mutation.py
+-rw-r--r--   0        0        0      166 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/rabbit/schema.py
+-rw-r--r--   0        0        0      192 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/__init__.py
+-rw-r--r--   0        0        0      870 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/mutation.py
+-rw-r--r--   0        0        0      867 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/query.py
+-rw-r--r--   0        0        0      273 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/schema.py
+-rw-r--r--   0        0        0     1735 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/router.py
+-rw-r--r--   0        0        0    11104 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/lifetime.py
+-rw-r--r--   0        0        0     2638 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/tests/conftest.py
+-rw-r--r--   0        0        0     4903 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/tests/test_generator.py
+-rw-r--r--   0        0        0     1769 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/fastapi_template/tests/utils.py
+-rw-r--r--   0        0        0     1222 2023-07-31 11:34:07.778992 fastapi_template-5.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5416 1970-01-01 00:00:00.000000 fastapi_template-5.0.3/PKG-INFO
```

### Comparing `fastapi_template-5.0.2/LICENSE` & `fastapi_template-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/README.md` & `fastapi_template-5.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/__main__.py` & `fastapi_template-5.0.3/fastapi_template/__main__.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/cli.py` & `fastapi_template-5.0.3/fastapi_template/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,14 +309,20 @@
     title="Additional tweaks",
     code="features",
     description="Additional project features",
     multiselect=True,
     before_ask=do_not_ask_features_if_quite,
     entries=[
         MenuEntry(
+            code="pydanticv1",
+            cli_name="pydantic-v1",
+            user_view="Use older version of pydantic",
+            description="Use pydantic version ^1 instead of ^2",
+        ),
+        MenuEntry(
             code="enable_redis",
             cli_name="redis",
             user_view="Add redis support",
             description=(
                 "{name} is a cool and lightweight in-memory key-value store.\n"
                 "It's good for {purpose1} or {purpose2}.".format(
                     name=colored(
```

### Comparing `fastapi_template-5.0.2/fastapi_template/input_model.py` & `fastapi_template-5.0.3/fastapi_template/input_model.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/cookiecutter.json` & `fastapi_template-5.0.3/fastapi_template/template/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/hooks/post_gen_project.py` & `fastapi_template-5.0.3/fastapi_template/template/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/.dockerignore` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/.dockerignore`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/.flake8` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/.flake8`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/.github/workflows/tests.yml` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/.gitignore` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/.gitlab-ci.yml` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/.pre-commit-config.yaml` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/README.md` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/alembic.ini` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/alembic.ini`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/conditional_files.json` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/conditional_files.json`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/Dockerfile` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/Dockerfile`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.dev.yml` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.dev.yml`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.otlp.yml` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.otlp.yml`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.yml` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/app.yml` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/app.yml`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/db.yml` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/db.yml`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/rabbit.yml` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/rabbit.yml`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/redis.yml` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/deploy/kube/redis.yml`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/pyproject.toml` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/__main__.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/__main__.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/conftest.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/conftest.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/dao/dummy_dao.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/dao/dummy_dao.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/env.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/versions/2021-08-16-16-55_2b7380507a71.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/migrations/versions/2021-08-16-16-55_2b7380507a71.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/utils.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_ormar/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/app_conf.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/app_conf.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/dao/dummy_dao.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/dao/dummy_dao.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/migrations/2022-04-16T17-38-51-672827.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_piccolo/migrations/2022-04-16T17-38-51-672827.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_psycopg/dao/dummy_dao.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_psycopg/dao/dummy_dao.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/dao/dummy_dao.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/dao/dummy_dao.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/dependencies.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/dependencies.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/env.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/versions/2021-08-16-16-55_2b7380507a71.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/migrations/versions/2021-08-16-16-55_2b7380507a71.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/utils.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_sa/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/config.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/config.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/dao/dummy_dao.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/db_tortoise/dao/dummy_dao.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/gunicorn_runner.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/gunicorn_runner.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/logging.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/logging.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/piccolo_conf.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/piccolo_conf.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/kafka/lifetime.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/kafka/lifetime.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/rabbit/lifetime.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/rabbit/lifetime.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/redis/dependency.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/redis/dependency.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/redis/lifetime.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/services/redis/lifetime.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/settings.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/settings.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/redoc.standalone.js` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/redoc.standalone.js`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/swagger-ui-bundle.js` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/swagger-ui.css` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/static/docs/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_dummy.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_dummy.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_echo.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_echo.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_kafka.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_kafka.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_rabbit.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_rabbit.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_redis.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tests/test_redis.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tkq.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/tkq.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/docs/views.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/docs/views.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/dummy/schema.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/dummy/schema.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/dummy/views.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/dummy/views.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/kafka/views.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/kafka/views.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/rabbit/views.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/rabbit/views.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/redis/views.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/redis/views.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/router.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/api/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/application.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/application.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/context.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/context.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/mutation.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/mutation.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/query.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/dummy/query.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/kafka/mutation.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/kafka/mutation.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/rabbit/mutation.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/rabbit/mutation.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/mutation.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/mutation.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/query.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/redis/query.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/router.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/gql/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/lifetime.py` & `fastapi_template-5.0.3/fastapi_template/template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/web/lifetime.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/tests/conftest.py` & `fastapi_template-5.0.3/fastapi_template/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/tests/test_generator.py` & `fastapi_template-5.0.3/fastapi_template/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/fastapi_template/tests/utils.py` & `fastapi_template-5.0.3/fastapi_template/tests/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_template-5.0.2/pyproject.toml` & `fastapi_template-5.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi_template"
-version = "5.0.2"
+version = "5.0.3"
 description = "Feature-rich robust FastAPI template"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 packages = [{ include = "fastapi_template" }]
 repository = "https://github.com/s3rius/FastAPI-template"
 homepage = "https://github.com/s3rius/FastAPI-template"
 readme = "README.md"
 keywords = ["FastAPI", "Cookiecutter", "Template"]
```

### Comparing `fastapi_template-5.0.2/PKG-INFO` & `fastapi_template-5.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-template
-Version: 5.0.2
+Version: 5.0.3
 Summary: Feature-rich robust FastAPI template
 Home-page: https://github.com/s3rius/FastAPI-template
 Keywords: FastAPI,Cookiecutter,Template
 Author: Pavel Kirilin
 Author-email: win10@list.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-template Version: 5.0.2 Summary: Feature-
+Metadata-Version: 2.1 Name: fastapi-template Version: 5.0.3 Summary: Feature-
 rich robust FastAPI template Home-page: https://github.com/s3rius/FastAPI-
 template Keywords: FastAPI,Cookiecutter,Template Author: Pavel Kirilin Author-
 email: win10@list.ru Requires-Python: >=3.8,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: cookiecutter
```

