# Comparing `tmp/django-dynamic-model-0.3.0.tar.gz` & `tmp/django_dynamic_model-0.4.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-dynamic-model-0.3.0.tar", last modified: Mon Sep 21 23:35:55 2020, max compression
+gzip compressed data, was "django_dynamic_model-0.4.0rc0.tar", max compression
```

## Comparing `django-dynamic-model-0.3.0.tar` & `django_dynamic_model-0.4.0rc0.tar`

### file list

```diff
@@ -1,26 +1,19 @@
-drwxr-xr-x   0 rvinzent   (502) staff       (20)        0 2020-09-21 23:35:55.000000 django-dynamic-model-0.3.0/
--rw-r--r--   0 rvinzent   (502) staff       (20)     2235 2020-09-21 23:35:55.000000 django-dynamic-model-0.3.0/PKG-INFO
-drwxr-xr-x   0 rvinzent   (502) staff       (20)        0 2020-09-21 23:35:55.000000 django-dynamic-model-0.3.0/dynamic_models/
-drwxr-xr-x   0 rvinzent   (502) staff       (20)        0 2020-09-21 23:35:55.000000 django-dynamic-model-0.3.0/dynamic_models/migrations/
--rw-r--r--   0 rvinzent   (502) staff       (20)        0 2020-05-17 01:47:58.000000 django-dynamic-model-0.3.0/dynamic_models/migrations/__init__.py
--rw-r--r--   0 rvinzent   (502) staff       (20)      332 2020-09-21 04:35:14.000000 django-dynamic-model-0.3.0/dynamic_models/migrations/0002_remove_modelschema__modified.py
--rw-r--r--   0 rvinzent   (502) staff       (20)     1561 2020-09-21 00:53:16.000000 django-dynamic-model-0.3.0/dynamic_models/migrations/0001_initial.py
--rw-r--r--   0 rvinzent   (502) staff       (20)      665 2020-09-21 04:13:52.000000 django-dynamic-model-0.3.0/dynamic_models/config.py
--rw-r--r--   0 rvinzent   (502) staff       (20)     5032 2020-09-21 04:57:29.000000 django-dynamic-model-0.3.0/dynamic_models/models.py
--rw-r--r--   0 rvinzent   (502) staff       (20)      486 2020-09-21 04:41:35.000000 django-dynamic-model-0.3.0/dynamic_models/cache.py
--rw-r--r--   0 rvinzent   (502) staff       (20)       22 2020-09-21 23:34:30.000000 django-dynamic-model-0.3.0/dynamic_models/__init__.py
--rw-r--r--   0 rvinzent   (502) staff       (20)      138 2020-09-21 04:38:08.000000 django-dynamic-model-0.3.0/dynamic_models/apps.py
--rw-r--r--   0 rvinzent   (502) staff       (20)     3887 2020-09-21 04:57:29.000000 django-dynamic-model-0.3.0/dynamic_models/factory.py
--rw-r--r--   0 rvinzent   (502) staff       (20)     2202 2020-09-21 04:57:29.000000 django-dynamic-model-0.3.0/dynamic_models/utils.py
--rw-r--r--   0 rvinzent   (502) staff       (20)      729 2020-09-21 04:57:29.000000 django-dynamic-model-0.3.0/dynamic_models/exceptions.py
--rw-r--r--   0 rvinzent   (502) staff       (20)     1824 2020-05-17 10:04:27.000000 django-dynamic-model-0.3.0/dynamic_models/schema.py
--rw-r--r--   0 rvinzent   (502) staff       (20)       76 2020-09-21 04:13:52.000000 django-dynamic-model-0.3.0/pyproject.toml
--rw-r--r--   0 rvinzent   (502) staff       (20)     1493 2020-09-21 04:13:52.000000 django-dynamic-model-0.3.0/README.md
-drwxr-xr-x   0 rvinzent   (502) staff       (20)        0 2020-09-21 23:35:55.000000 django-dynamic-model-0.3.0/django_dynamic_model.egg-info/
--rw-r--r--   0 rvinzent   (502) staff       (20)     2235 2020-09-21 23:35:55.000000 django-dynamic-model-0.3.0/django_dynamic_model.egg-info/PKG-INFO
--rw-r--r--   0 rvinzent   (502) staff       (20)      623 2020-09-21 23:35:55.000000 django-dynamic-model-0.3.0/django_dynamic_model.egg-info/SOURCES.txt
--rw-r--r--   0 rvinzent   (502) staff       (20)       12 2020-09-21 23:35:55.000000 django-dynamic-model-0.3.0/django_dynamic_model.egg-info/requires.txt
--rw-r--r--   0 rvinzent   (502) staff       (20)       15 2020-09-21 23:35:55.000000 django-dynamic-model-0.3.0/django_dynamic_model.egg-info/top_level.txt
--rw-r--r--   0 rvinzent   (502) staff       (20)        1 2020-09-21 23:35:55.000000 django-dynamic-model-0.3.0/django_dynamic_model.egg-info/dependency_links.txt
--rw-r--r--   0 rvinzent   (502) staff       (20)      999 2020-09-21 23:32:47.000000 django-dynamic-model-0.3.0/setup.py
--rw-r--r--   0 rvinzent   (502) staff       (20)       38 2020-09-21 23:35:55.000000 django-dynamic-model-0.3.0/setup.cfg
+-rw-r--r--   0        0        0     1065 2022-05-09 19:19:15.260400 django_dynamic_model-0.4.0rc0/LICENSE
+-rw-r--r--   0        0        0       25 2023-07-31 18:41:48.865861 django_dynamic_model-0.4.0rc0/dynamic_models/__init__.py
+-rw-r--r--   0        0        0      138 2022-05-21 08:54:04.930289 django_dynamic_model-0.4.0rc0/dynamic_models/apps.py
+-rw-r--r--   0        0        0      158 2023-07-31 18:41:48.866999 django_dynamic_model-0.4.0rc0/dynamic_models/compat.py
+-rw-r--r--   0        0        0      665 2022-05-09 19:19:15.261895 django_dynamic_model-0.4.0rc0/dynamic_models/config.py
+-rw-r--r--   0        0        0      622 2023-07-31 18:41:48.868375 django_dynamic_model-0.4.0rc0/dynamic_models/exceptions.py
+-rw-r--r--   0        0        0     2728 2023-07-31 18:41:48.869442 django_dynamic_model-0.4.0rc0/dynamic_models/factory.py
+-rw-r--r--   0        0        0     2269 2022-05-21 08:47:49.008429 django_dynamic_model-0.4.0rc0/dynamic_models/migrations/0001_initial.py
+-rw-r--r--   0        0        0      332 2022-05-21 08:47:49.009688 django_dynamic_model-0.4.0rc0/dynamic_models/migrations/0002_remove_modelschema__modified.py
+-rw-r--r--   0        0        0     2208 2022-05-21 08:47:49.011223 django_dynamic_model-0.4.0rc0/dynamic_models/migrations/0003_add_classname_remove_datatype.py
+-rw-r--r--   0        0        0      428 2022-05-21 08:47:49.012449 django_dynamic_model-0.4.0rc0/dynamic_models/migrations/0004_modelschema_db_name.py
+-rw-r--r--   0        0        0      746 2023-07-31 18:41:48.870235 django_dynamic_model-0.4.0rc0/dynamic_models/migrations/0005_add_model_db_name.py
+-rw-r--r--   0        0        0        0 2022-05-09 19:19:15.263354 django_dynamic_model-0.4.0rc0/dynamic_models/migrations/__init__.py
+-rw-r--r--   0        0        0     6596 2023-07-31 18:41:48.871439 django_dynamic_model-0.4.0rc0/dynamic_models/models.py
+-rw-r--r--   0        0        0     2394 2022-05-21 08:47:49.014491 django_dynamic_model-0.4.0rc0/dynamic_models/schema.py
+-rw-r--r--   0        0        0     1635 2023-07-31 18:41:48.873359 django_dynamic_model-0.4.0rc0/dynamic_models/utils.py
+-rw-r--r--   0        0        0     1357 2023-07-31 19:38:07.346396 django_dynamic_model-0.4.0rc0/pyproject.toml
+-rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 django_dynamic_model-0.4.0rc0/setup.py
+-rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 django_dynamic_model-0.4.0rc0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-dynamic-model-0.3.0/dynamic_models/migrations/0001_initial.py` & `django_dynamic_model-0.4.0rc0/dynamic_models/migrations/0001_initial.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,68 @@
 # Generated by Django 2.2 on 2020-05-17 08:18
 
-from django.db import migrations, models
 import django.db.models.deletion
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
-    dependencies = [
-    ]
+    dependencies = []
 
     operations = [
         migrations.CreateModel(
-            name='ModelSchema',
+            name="ModelSchema",
             fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(max_length=32, unique=True)),
-                ('_modified', models.DateTimeField(auto_now=True)),
+                (
+                    "id",
+                    models.AutoField(
+                        auto_created=True, primary_key=True, serialize=False, verbose_name="ID"
+                    ),
+                ),
+                ("name", models.CharField(max_length=32, unique=True)),
+                ("_modified", models.DateTimeField(auto_now=True)),
             ],
         ),
         migrations.CreateModel(
-            name='FieldSchema',
+            name="FieldSchema",
             fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(max_length=63)),
-                ('data_type', models.CharField(choices=[('character', 'character'), ('text', 'text'), ('integer', 'integer'), ('float', 'float'), ('boolean', 'boolean'), ('date', 'date')], editable=False, max_length=16)),
-                ('null', models.BooleanField(default=False)),
-                ('unique', models.BooleanField(default=False)),
-                ('max_length', models.PositiveIntegerField(null=True)),
-                ('model_schema', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='fields', to='dynamic_models.ModelSchema')),
+                (
+                    "id",
+                    models.AutoField(
+                        auto_created=True, primary_key=True, serialize=False, verbose_name="ID"
+                    ),
+                ),
+                ("name", models.CharField(max_length=63)),
+                (
+                    "data_type",
+                    models.CharField(
+                        choices=[
+                            ("character", "character"),
+                            ("text", "text"),
+                            ("integer", "integer"),
+                            ("float", "float"),
+                            ("boolean", "boolean"),
+                            ("date", "date"),
+                        ],
+                        editable=False,
+                        max_length=16,
+                    ),
+                ),
+                ("null", models.BooleanField(default=False)),
+                ("unique", models.BooleanField(default=False)),
+                ("max_length", models.PositiveIntegerField(null=True)),
+                (
+                    "model_schema",
+                    models.ForeignKey(
+                        on_delete=django.db.models.deletion.CASCADE,
+                        related_name="fields",
+                        to="dynamic_models.ModelSchema",
+                    ),
+                ),
             ],
             options={
-                'unique_together': {('name', 'model_schema')},
+                "unique_together": {("name", "model_schema")},
             },
         ),
     ]
```

### Comparing `django-dynamic-model-0.3.0/dynamic_models/config.py` & `django_dynamic_model-0.4.0rc0/dynamic_models/config.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-model-0.3.0/dynamic_models/models.py` & `django_dynamic_model-0.4.0rc0/dynamic_models/models.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,47 @@
-from django.core.exceptions import FieldDoesNotExist
+from django.core.exceptions import FieldDoesNotExist, ValidationError
 from django.db import models
+from django.db.utils import DEFAULT_DB_ALIAS
 from django.utils.text import slugify
 
-from dynamic_models import config, cache
-from dynamic_models.factory import ModelFactory, FieldFactory
-from dynamic_models.exceptions import NullFieldChangedError, InvalidFieldNameError
-from dynamic_models.schema import ModelSchemaEditor, FieldSchemaEditor
+from dynamic_models import compat, config
+from dynamic_models.exceptions import InvalidFieldNameError, NullFieldChangedError
+from dynamic_models.factory import ModelFactory
+from dynamic_models.schema import FieldSchemaEditor, ModelSchemaEditor
 from dynamic_models.utils import ModelRegistry
 
 
 class ModelSchema(models.Model):
-    name = models.CharField(max_length=32, unique=True)
+    name = models.CharField(max_length=250, unique=True)
+    db_name = models.CharField(max_length=32, default=DEFAULT_DB_ALIAS)
+    managed = models.BooleanField(default=True)
+    db_table_name = models.CharField(null=True, max_length=250)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._registry = ModelRegistry(self.app_label)
         self._initial_name = self.name
         initial_model = self.get_registered_model()
-        self._schema_editor = ModelSchemaEditor(initial_model)
+        self._schema_editor = (
+            ModelSchemaEditor(initial_model=initial_model, db_name=self.db_name)
+            if self.managed
+            else None
+        )
 
     def save(self, **kwargs):
         super().save(**kwargs)
-        cache.update_last_modified(self.model_name)
-        cache.update_last_modified(self.initial_model_name)
-        self._schema_editor.update_table(self._factory.make_model())
+        if self._schema_editor:
+            self._schema_editor.update_table(self._factory.get_model())
+
         self._initial_name = self.name
 
     def delete(self, **kwargs):
-        self._schema_editor.drop_table(self.as_model())
+        if self._schema_editor:
+            self._schema_editor.drop_table(self.as_model())
         self._factory.destroy_model()
-        cache.clear_last_modified(self.initial_model_name)
         super().delete(**kwargs)
 
     def get_registered_model(self):
         return self._registry.get_model(self.model_name)
 
     @property
     def _factory(self):
@@ -53,55 +61,101 @@
 
     @classmethod
     def get_model_name(cls, name):
         return name.title().replace(" ", "")
 
     @property
     def db_table(self):
-        parts = (self.app_label, slugify(self.name).replace("-", "_"))
-        return "_".join(parts)
+        return self.db_table_name if self.db_table_name else self._default_db_table_name()
+
+    def _default_db_table_name(self):
+        safe_name = slugify(self.name).replace("-", "_")
+        return f"{self.app_label}_{safe_name}"
 
     def as_model(self):
         return self._factory.get_model()
 
 
+class FieldKwargsJSON(compat.JSONField):
+    description = "A field that handles storing models.Field kwargs as JSON"
+
+    def to_python(self, value):
+        raw_value = super().to_python(value)
+        try:
+            return self._convert_on_delete_to_function(raw_value)
+        except AttributeError as err:
+            raise ValidationError("Invalid value for 'on_delete'") from err
+
+    def from_db_value(self, value, expression, connection):
+        # django.contrib.postgres.fields.JSONField does not implement from_db_value
+        # for some reason. In that version, value is already a dict
+        try:
+            db_value = super().from_db_value(value, expression, connection)
+        except AttributeError:
+            db_value = value
+        return self._convert_on_delete_to_function(db_value)
+
+    def get_prep_value(self, value):
+        prep_value = self._convert_on_delete_to_string(value)
+        return super().get_prep_value(prep_value)
+
+    def _convert_on_delete_to_function(self, raw_value):
+        if raw_value is None or "on_delete" not in raw_value:
+            return raw_value
+
+        raw_on_delete = raw_value["on_delete"]
+        if isinstance(raw_on_delete, str):
+            raw_value["on_delete"] = getattr(models, raw_on_delete)
+
+        return raw_value
+
+    def _convert_on_delete_to_string(self, raw_value):
+        if raw_value is None or "on_delete" not in raw_value:
+            return raw_value
+
+        raw_on_delete = raw_value["on_delete"]
+        if callable(raw_on_delete):
+            raw_value["on_delete"] = raw_on_delete.__name__
+
+        return raw_value
+
+
 class FieldSchema(models.Model):
     _PROHIBITED_NAMES = ("__module__", "_declared")
-    _MAX_LENGTH_DATA_TYPES = ("character",)
 
     name = models.CharField(max_length=63)
     model_schema = models.ForeignKey(ModelSchema, on_delete=models.CASCADE, related_name="fields")
-    data_type = models.CharField(
-        max_length=16, choices=FieldFactory.data_type_choices(), editable=False
-    )
-    null = models.BooleanField(default=False)
-    unique = models.BooleanField(default=False)
-    max_length = models.PositiveIntegerField(null=True)
+    class_name = models.TextField()
+    kwargs = FieldKwargsJSON(default=dict)
 
     class Meta:
         unique_together = (("name", "model_schema"),)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._initial_name = self.name
         self._initial_null = self.null
         self._initial_field = self.get_registered_model_field()
-        self._schema_editor = FieldSchemaEditor(self._initial_field)
+        self._schema_editor = (
+            FieldSchemaEditor(initial_field=self._initial_field, db_name=self.model_schema.db_name)
+            if self.model_schema.managed
+            else None
+        )
 
     def save(self, **kwargs):
         self.validate()
         super().save(**kwargs)
-        self.update_last_modified()
         model, field = self._get_model_with_field()
-        self._schema_editor.update_column(model, field)
+        if self._schema_editor:
+            self._schema_editor.update_column(model, field)
 
     def delete(self, **kwargs):
         model, field = self._get_model_with_field()
-        self._schema_editor.drop_column(model, field)
-        self.update_last_modified()
+        if self._schema_editor:
+            self._schema_editor.drop_column(model, field)
         super().delete(**kwargs)
 
     def validate(self):
         if self._initial_null and not self.null:
             raise NullFieldChangedError(f"Cannot change NULL field '{self.name}' to NOT NULL")
 
         if self.name in self.get_prohibited_names():
@@ -116,33 +170,28 @@
                 pass
 
     @classmethod
     def get_prohibited_names(cls):
         # TODO: return prohbited names based on backend
         return cls._PROHIBITED_NAMES
 
-    @classmethod
-    def get_data_types(cls):
-        return FieldFactory.get_data_types()
-
     @property
     def db_column(self):
         return slugify(self.name).replace("-", "_")
 
-    def requires_max_length(self):
-        return self.data_type in self.__class__._MAX_LENGTH_DATA_TYPES
+    @property
+    def null(self):
+        return self.kwargs.get("null", False)
 
-    def update_last_modified(self):
-        cache.update_last_modified(self.model_schema.initial_model_name)
+    @null.setter
+    def null(self, value):
+        self.kwargs["null"] = value
 
     def get_options(self):
-        options = {"null": self.null, "unique": self.unique}
-        if self.requires_max_length():
-            options["max_length"] = self.max_length or config.default_charfield_max_length()
-        return options
+        return self.kwargs.copy()
 
     def _get_model_with_field(self):
         model = self.model_schema.as_model()
         try:
             field = model._meta.get_field(self.db_column)
         except FieldDoesNotExist:
             field = None
```

### Comparing `django-dynamic-model-0.3.0/dynamic_models/factory.py` & `django_dynamic_model-0.4.0rc0/dynamic_models/factory.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,46 @@
+import importlib
+
 from django.db import models
-from django.utils import timezone
 
 from dynamic_models import config
-from dynamic_models.exceptions import OutdatedModelError, UnsavedSchemaError
-from dynamic_models.utils import ModelRegistry, is_current_model
+from dynamic_models.exceptions import UnsavedSchemaError
+from dynamic_models.utils import ModelRegistry
+
+
+class DynamicModelBase(models.base.ModelBase):
+    def __instancecheck__(cls, instance):
+        if issubclass(type(instance.__class__), DynamicModelBase):
+            return cls._class_descriptor(instance.__class__) == cls._class_descriptor(cls)
+
+        return super().__instancecheck__(instance)
+
+    @staticmethod
+    def _class_descriptor(class_):
+        return (class_.__module__, class_.__qualname__)
 
 
 class ModelFactory:
     def __init__(self, model_schema):
         self.schema = model_schema
         self.registry = ModelRegistry(model_schema.app_label)
 
     def get_model(self):
-        registered = self.get_registered_model()
-        if registered and is_current_model(registered):
-            return registered
-        return self.make_model()
-
-    def make_model(self):
         if not self.schema.pk:
             raise UnsavedSchemaError(
                 f"Cannot create a model for schema '{self.schema.name}'"
                 " because it has not been saved to the database"
             )
+
         self.unregister_model()
-        model = type(self.schema.model_name, (models.Model,), self.get_properties())
-        _connect_schema_checker(model)
-        return model
+        return DynamicModelBase(self.schema.model_name, (models.Model,), self.get_properties())
 
     def destroy_model(self):
-        last_model = self.get_registered_model()
-        if last_model:
-            _disconnect_schema_checker(last_model)
+        registered_model = self.get_registered_model()
+        if registered_model is not None:
             self.unregister_model()
 
     def get_registered_model(self):
         return self.registry.get_model(self.schema.initial_model_name)
 
     def unregister_model(self):
         try:
@@ -49,82 +54,37 @@
             **config.default_fields(),
             **self._custom_fields(),
         }
 
     def _base_properties(self):
         return {
             "__module__": "{}.models".format(self.schema.app_label),
-            "_declared": timezone.now(),
             "Meta": self._model_meta(),
         }
 
     def _custom_fields(self):
-        fields = {}
-        for field_schema in self.schema.fields.all():
-            model_field = FieldFactory(field_schema).make_field()
-            fields[field_schema.db_column] = model_field
-        return fields
+        return {
+            field.db_column: FieldFactory(field).make_field() for field in self.schema.fields.all()
+        }
 
     def _model_meta(self):
         class Meta:
             app_label = self.schema.app_label
             db_table = self.schema.db_table
             verbose_name = self.schema.name
 
         return Meta
 
 
 class FieldFactory:
-    DATA_TYPES = {
-        "character": models.CharField,
-        "text": models.TextField,
-        "integer": models.IntegerField,
-        "float": models.FloatField,
-        "boolean": models.BooleanField,
-        "date": models.DateTimeField,
-    }
-
     def __init__(self, field_schema):
         self.schema = field_schema
 
     def make_field(self):
         options = self.schema.get_options()
-        constructor = self.get_constructor()
-        return constructor(**options)
-
-    def get_constructor(self):
-        return self.DATA_TYPES[self.schema.data_type]
-
-    @classmethod
-    def data_type_choices(cls):
-        return [(dt, dt) for dt in cls.get_data_types()]
-
-    @classmethod
-    def get_data_types(cls):
-        return cls.DATA_TYPES
-
-
-def check_model_schema(sender, instance, **kwargs):
-    """
-    Check that the schema being used is the most up-to-date.
-
-    Called on pre_save to guard against the possibility of a model schema change
-    between instance instantiation and record save.
-    """
-    if not is_current_model(sender):
-        raise OutdatedModelError(f"model {sender.__name__} has changed")
-
-
-def _connect_schema_checker(model):
-    models.signals.pre_save.connect(
-        check_model_schema, sender=model, dispatch_uid=_get_signal_uid(model.__name__)
-    )
-
-
-def _disconnect_schema_checker(model):
-    models.signals.pre_save.disconnect(
-        check_model_schema, sender=model, dispatch_uid=_get_signal_uid(model.__name__)
-    )
-
+        field_class = self.get_field_class()
+        return field_class(**options)
 
-def _get_signal_uid(model_name):
-    return "{}_model_schema".format(model_name)
+    def get_field_class(self):
+        module_name, class_name = self.schema.class_name.rsplit(".", maxsplit=1)
+        module = importlib.import_module(module_name)
+        return getattr(module, class_name)
```

### Comparing `django-dynamic-model-0.3.0/dynamic_models/utils.py` & `django_dynamic_model-0.4.0rc0/dynamic_models/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from contextlib import contextmanager
 
-from django.db import connection
 from django.apps import apps
 from django.core.exceptions import FieldDoesNotExist
-
-from dynamic_models import cache
+from django.db import connection
 
 
 def db_table_exists(table_name):
     with _db_cursor() as c:
         table_names = connection.introspection.table_names(c)
         return table_name in table_names
 
@@ -34,27 +32,14 @@
 @contextmanager
 def _db_cursor():
     cursor = connection.cursor()
     yield cursor
     cursor.close()
 
 
-def receiver_is_connected(receiver_name, signal, sender):
-    receivers = signal._live_receivers(sender)
-    receiver_strings = ["{}.{}".format(r.__module__, r.__name__) for r in receivers]
-    return receiver_name in receiver_strings
-
-
-def is_current_model(model):
-    # if there is no cache entry, the model schema has not been updated since
-    # restarting the server and the current schema is fine
-    last_modified = cache.get_last_modified(model.__name__)
-    return last_modified is None or last_modified < model._declared
-
-
 class ModelRegistry:
     def __init__(self, app_label):
         self.app_label = app_label
 
     def is_registered(self, model_name):
         return model_name.lower() in apps.all_models[self.app_label]
```

### Comparing `django-dynamic-model-0.3.0/dynamic_models/exceptions.py` & `django_dynamic_model-0.4.0rc0/dynamic_models/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,14 @@
 """
 
 
 class DynamicModelError(Exception):
     """Base exception for use in dynamic models."""
 
 
-class OutdatedModelError(DynamicModelError):
-    """Raised when a model's schema is outdated on save."""
-
-
 class NullFieldChangedError(DynamicModelError):
     """Raised when a field is attempted to be change from NULL to NOT NULL."""
 
 
 class InvalidFieldNameError(DynamicModelError):
     """Raised when a field name is invalid."""
```

### Comparing `django-dynamic-model-0.3.0/dynamic_models/schema.py` & `django_dynamic_model-0.4.0rc0/dynamic_models/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,62 @@
 """Wrapper functions for performing runtime schema changes."""
-from django.db import connection
+from django.db import connections
+from django.db.utils import DEFAULT_DB_ALIAS, ProgrammingError
 
 
 class ModelSchemaEditor:
-    def __init__(self, initial_model=None):
+    def __init__(self, initial_model=None, db_name=DEFAULT_DB_ALIAS):
         self.initial_model = initial_model
+        self.db_name = db_name
 
     def update_table(self, new_model):
         if self.initial_model and self.initial_model != new_model:
             self.alter_table(new_model)
         elif not self.initial_model:
             self.create_table(new_model)
         self.initial_model = new_model
 
     def create_table(self, new_model):
-        with connection.schema_editor() as editor:
-            editor.create_model(new_model)
+        try:
+            with connections[self.db_name].schema_editor() as editor:
+                editor.create_model(new_model)
+        except ProgrammingError:
+            # TODO: I couldn't figure out why sometimes despite the
+            # fact that the model exists, the initial_model is None and
+            # therefore this method will be called which leads to this
+            # error
+            pass
 
     def alter_table(self, new_model):
         old_name = self.initial_model._meta.db_table
         new_name = new_model._meta.db_table
-        with connection.schema_editor() as editor:
+        with connections[self.db_name].schema_editor() as editor:
             editor.alter_db_table(new_model, old_name, new_name)
 
     def drop_table(self, model):
-        with connection.schema_editor() as editor:
+        with connections[self.db_name].schema_editor() as editor:
             editor.delete_model(model)
 
 
 class FieldSchemaEditor:
-    def __init__(self, initial_field=None):
+    def __init__(self, initial_field=None, db_name=DEFAULT_DB_ALIAS):
         self.initial_field = initial_field
+        self.db_name = db_name
 
     def update_column(self, model, new_field):
         if self.initial_field and self.initial_field != new_field:
             self.alter_column(model, new_field)
         elif not self.initial_field:
             self.add_column(model, new_field)
         self.initial_field = new_field
 
     def add_column(self, model, field):
-        with connection.schema_editor() as editor:
+        with connections[self.db_name].schema_editor() as editor:
             editor.add_field(model, field)
 
     def alter_column(self, model, new_field):
-        with connection.schema_editor() as editor:
+        with connections[self.db_name].schema_editor() as editor:
             editor.alter_field(model, self.initial_field, new_field)
 
     def drop_column(self, model, field):
-        with connection.schema_editor() as editor:
+        with connections[self.db_name].schema_editor() as editor:
             editor.remove_field(model, field)
```

