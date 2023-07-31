# Comparing `tmp/Products.Formulator-2.0.dev0.tar.gz` & `tmp/Products.Formulator-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Products.Formulator-2.0.dev0.tar", last modified: Tue Mar 14 14:13:26 2023, max compression
+gzip compressed data, was "Products.Formulator-2.1.tar", last modified: Mon Jul 31 06:31:40 2023, max compression
```

## Comparing `Products.Formulator-2.0.dev0.tar` & `Products.Formulator-2.1.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-14 14:13:26.056872 Products.Formulator-2.0.dev0/
--rw-r--r--   0 mac        (513) staff       (20)    26510 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)     3301 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/CREDITS.rst
--rw-r--r--   0 mac        (513) staff       (20)     1490 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      440 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)    31307 2023-03-14 14:13:26.057048 Products.Formulator-2.0.dev0/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      869 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      420 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/buildout-base.cfg
--rw-r--r--   0 mac        (513) staff       (20)      121 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/buildout.cfg
--rw-r--r--   0 mac        (513) staff       (20)      110 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/buildout4.cfg
--rw-r--r--   0 mac        (513) staff       (20)      989 2023-03-14 14:13:26.057700 Products.Formulator-2.0.dev0/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     1954 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-14 14:13:26.013305 Products.Formulator-2.0.dev0/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-14 14:13:26.019767 Products.Formulator-2.0.dev0/src/Products/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-14 14:13:26.032379 Products.Formulator-2.0.dev0/src/Products/Formulator/
--rw-r--r--   0 mac        (513) staff       (20)     1163 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/DummyField.py
--rw-r--r--   0 mac        (513) staff       (20)     1317 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/EmailLinesField.py
--rw-r--r--   0 mac        (513) staff       (20)     1177 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/Errors.py
--rw-r--r--   0 mac        (513) staff       (20)     3289 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/FSForm.py
--rw-r--r--   0 mac        (513) staff       (20)    24577 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/Field.py
--rw-r--r--   0 mac        (513) staff       (20)     5278 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/FieldRegistry.py
--rw-r--r--   0 mac        (513) staff       (20)    41774 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/Form.py
--rw-r--r--   0 mac        (513) staff       (20)     4429 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/FormToXML.py
--rw-r--r--   0 mac        (513) staff       (20)     4738 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/FormulatorFormFile.py
--rw-r--r--   0 mac        (513) staff       (20)      334 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/HelperFields.py
--rw-r--r--   0 mac        (513) staff       (20)     4703 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/INSTALL.txt
--rw-r--r--   0 mac        (513) staff       (20)     2253 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/InterfaceField.py
--rw-r--r--   0 mac        (513) staff       (20)     2138 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/ListTextAreaField.py
--rw-r--r--   0 mac        (513) staff       (20)     2586 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/MethodField.py
--rw-r--r--   0 mac        (513) staff       (20)     4528 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/PatternChecker.py
--rw-r--r--   0 mac        (513) staff       (20)     5315 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/ProductForm.py
--rw-r--r--   0 mac        (513) staff       (20)     9877 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/StandardFields.py
--rw-r--r--   0 mac        (513) staff       (20)     2051 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/TALESField.py
--rw-r--r--   0 mac        (513) staff       (20)    33008 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/Validator.py
--rw-r--r--   0 mac        (513) staff       (20)    42683 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/Widget.py
--rw-r--r--   0 mac        (513) staff       (20)     2877 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/XMLObjects.py
--rw-r--r--   0 mac        (513) staff       (20)     5974 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/XMLToForm.py
--rw-r--r--   0 mac        (513) staff       (20)     3958 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      780 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/configure.zcml
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-14 14:13:26.037759 Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/
--rw-r--r--   0 mac        (513) staff       (20)     1152 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/fieldAdd.dtml
--rw-r--r--   0 mac        (513) staff       (20)     2223 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/fieldEdit.dtml
--rw-r--r--   0 mac        (513) staff       (20)      434 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/fieldListHeader.dtml
--rw-r--r--   0 mac        (513) staff       (20)      582 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/fieldMessages.dtml
--rw-r--r--   0 mac        (513) staff       (20)     1325 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/fieldOverride.dtml
--rw-r--r--   0 mac        (513) staff       (20)     1507 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/fieldTales.dtml
--rw-r--r--   0 mac        (513) staff       (20)     1335 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/fieldTest.dtml
--rw-r--r--   0 mac        (513) staff       (20)     1393 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/formAdd.dtml
--rw-r--r--   0 mac        (513) staff       (20)     4063 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/formOrder.dtml
--rw-r--r--   0 mac        (513) staff       (20)     1246 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/formSettings.dtml
--rw-r--r--   0 mac        (513) staff       (20)     1877 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/formTest.dtml
--rw-r--r--   0 mac        (513) staff       (20)      522 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/formXML.dtml
--rw-r--r--   0 mac        (513) staff       (20)      297 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/ftesting.zcml
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-14 14:13:26.043717 Products.Formulator-2.0.dev0/src/Products/Formulator/help/
--rw-r--r--   0 mac        (513) staff       (20)     1084 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/help/BasicForm.py
--rw-r--r--   0 mac        (513) staff       (20)     5259 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/help/Field.py
--rw-r--r--   0 mac        (513) staff       (20)     8623 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/help/Form.py
--rw-r--r--   0 mac        (513) staff       (20)      794 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/help/ZMIForm.py
--rw-r--r--   0 mac        (513) staff       (20)     6066 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/help/dogfood.txt
--rw-r--r--   0 mac        (513) staff       (20)     2510 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/help/fieldEdit.txt
--rw-r--r--   0 mac        (513) staff       (20)      332 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/help/fieldMessages.txt
--rw-r--r--   0 mac        (513) staff       (20)     2067 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/help/fieldOverride.txt
--rw-r--r--   0 mac        (513) staff       (20)     3809 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/help/fieldTales.txt
--rw-r--r--   0 mac        (513) staff       (20)      905 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/help/fieldTest.txt
--rw-r--r--   0 mac        (513) staff       (20)      816 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/help/formContents.txt
--rw-r--r--   0 mac        (513) staff       (20)     3425 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/help/formOrder.txt
--rw-r--r--   0 mac        (513) staff       (20)     1524 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/help/formSettings.txt
--rw-r--r--   0 mac        (513) staff       (20)     1033 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/help/formTest.txt
--rw-r--r--   0 mac        (513) staff       (20)      670 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/help/formXML.txt
--rw-r--r--   0 mac        (513) staff       (20)    10039 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/help/formulator_howto.txt
--rw-r--r--   0 mac        (513) staff       (20)      219 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/help/formulator_motto.txt
--rw-r--r--   0 mac        (513) staff       (20)     1710 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/helpers.py
--rw-r--r--   0 mac        (513) staff       (20)     1899 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/homepage.html
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-14 14:13:26.044456 Products.Formulator-2.0.dev0/src/Products/Formulator/i18n/
--rw-r--r--   0 mac        (513) staff       (20)      641 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/i18n/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-14 14:13:26.014423 Products.Formulator-2.0.dev0/src/Products/Formulator/i18n/de/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-14 14:13:26.044798 Products.Formulator-2.0.dev0/src/Products/Formulator/i18n/de/LC_MESSAGES/
--rw-r--r--   0 mac        (513) staff       (20)     2428 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/i18n/de/LC_MESSAGES/formulator.po
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-14 14:13:26.014753 Products.Formulator-2.0.dev0/src/Products/Formulator/i18n/en/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-14 14:13:26.045138 Products.Formulator-2.0.dev0/src/Products/Formulator/i18n/en/LC_MESSAGES/
--rw-r--r--   0 mac        (513) staff       (20)     1630 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/i18n/en/LC_MESSAGES/formulator.po
--rw-r--r--   0 mac        (513) staff       (20)     1630 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/i18n/formulator.pot
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-14 14:13:26.015077 Products.Formulator-2.0.dev0/src/Products/Formulator/i18n/fr/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-14 14:13:26.045478 Products.Formulator-2.0.dev0/src/Products/Formulator/i18n/fr/LC_MESSAGES/
--rw-r--r--   0 mac        (513) staff       (20)     2235 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/i18n/fr/LC_MESSAGES/formulator.po
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-14 14:13:26.015405 Products.Formulator-2.0.dev0/src/Products/Formulator/i18n/nl/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-14 14:13:26.045816 Products.Formulator-2.0.dev0/src/Products/Formulator/i18n/nl/LC_MESSAGES/
--rw-r--r--   0 mac        (513) staff       (20)     2257 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/i18n/nl/LC_MESSAGES/formulator.po
--rw-r--r--   0 mac        (513) staff       (20)      279 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)      710 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/monkey.py
--rw-r--r--   0 mac        (513) staff       (20)     1859 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/testing.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-14 14:13:26.049005 Products.Formulator-2.0.dev0/src/Products/Formulator/tests/
--rw-r--r--   0 mac        (513) staff       (20)      154 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     2799 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/tests/test_field_ids.py
--rw-r--r--   0 mac        (513) staff       (20)    22199 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/tests/test_form.py
--rw-r--r--   0 mac        (513) staff       (20)     1651 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/tests/test_pattern_checker.py
--rw-r--r--   0 mac        (513) staff       (20)    21973 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/tests/test_serialize.py
--rw-r--r--   0 mac        (513) staff       (20)    29425 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/tests/test_validators.py
--rw-r--r--   0 mac        (513) staff       (20)     3338 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/tests/test_widgets.py
--rw-r--r--   0 mac        (513) staff       (20)     5050 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/tests/test_zeam.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-14 14:13:26.056534 Products.Formulator-2.0.dev0/src/Products/Formulator/www/
--rw-r--r--   0 mac        (513) staff       (20)      899 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/www/BasicField.gif
--rw-r--r--   0 mac        (513) staff       (20)      901 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/www/CheckBoxField.gif
--rw-r--r--   0 mac        (513) staff       (20)      877 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/www/DateTimeField.gif
--rw-r--r--   0 mac        (513) staff       (20)      898 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/www/EmailField.gif
--rw-r--r--   0 mac        (513) staff       (20)      907 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/www/FileField.gif
--rw-r--r--   0 mac        (513) staff       (20)      902 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/www/FloatField.gif
--rw-r--r--   0 mac        (513) staff       (20)      875 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/www/Form.gif
--rw-r--r--   0 mac        (513) staff       (20)      895 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/www/IntegerField.gif
--rw-r--r--   0 mac        (513) staff       (20)      899 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/www/LabelField.gif
--rw-r--r--   0 mac        (513) staff       (20)      907 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/www/LinesField.gif
--rw-r--r--   0 mac        (513) staff       (20)      907 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/www/LinkField.gif
--rw-r--r--   0 mac        (513) staff       (20)      899 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/www/ListField.gif
--rw-r--r--   0 mac        (513) staff       (20)      877 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/www/MethodField.gif
--rw-r--r--   0 mac        (513) staff       (20)      919 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/www/MultiCheckBoxField.gif
--rw-r--r--   0 mac        (513) staff       (20)      118 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/www/MultiListField.gif
--rw-r--r--   0 mac        (513) staff       (20)      898 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/www/MultipleListField.gif
--rw-r--r--   0 mac        (513) staff       (20)      881 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/www/PasswordField.gif
--rw-r--r--   0 mac        (513) staff       (20)      905 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/www/PatternField.gif
--rw-r--r--   0 mac        (513) staff       (20)       92 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/www/RadioField.gif
--rw-r--r--   0 mac        (513) staff       (20)      906 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/www/RangedIntegerField.gif
--rw-r--r--   0 mac        (513) staff       (20)      899 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/www/StringField.gif
--rw-r--r--   0 mac        (513) staff       (20)      901 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/www/TextAreaField.gif
--rw-r--r--   0 mac        (513) staff       (20)     7436 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/Formulator/zeamsupport.py
--rw-r--r--   0 mac        (513) staff       (20)      342 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-14 14:13:26.022145 Products.Formulator-2.0.dev0/src/Products.Formulator.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)    31307 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products.Formulator.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     4622 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products.Formulator.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products.Formulator.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        9 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products.Formulator.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products.Formulator.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      308 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products.Formulator.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        9 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/src/Products.Formulator.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1661 2023-03-14 14:13:25.000000 Products.Formulator-2.0.dev0/tox.ini
+drwxr-xr-x   0 sallner   (1000) users      (100)        0 2023-07-31 06:31:40.599222 Products.Formulator-2.1/
+-rw-r--r--   0 sallner   (1000) users      (100)    26710 2023-07-31 06:31:36.000000 Products.Formulator-2.1/CHANGES.rst
+-rw-r--r--   0 sallner   (1000) users      (100)     3301 2023-07-31 06:31:36.000000 Products.Formulator-2.1/CREDITS.rst
+-rw-r--r--   0 sallner   (1000) users      (100)     1490 2023-07-31 06:31:36.000000 Products.Formulator-2.1/LICENSE.txt
+-rw-r--r--   0 sallner   (1000) users      (100)      440 2023-07-31 06:31:36.000000 Products.Formulator-2.1/MANIFEST.in
+-rw-r--r--   0 sallner   (1000) users      (100)    31774 2023-07-31 06:31:40.599222 Products.Formulator-2.1/PKG-INFO
+-rw-r--r--   0 sallner   (1000) users      (100)      869 2023-07-31 06:31:36.000000 Products.Formulator-2.1/README.rst
+-rw-r--r--   0 sallner   (1000) users      (100)      420 2023-07-31 06:31:36.000000 Products.Formulator-2.1/buildout-base.cfg
+-rw-r--r--   0 sallner   (1000) users      (100)      268 2023-07-31 06:31:36.000000 Products.Formulator-2.1/buildout.cfg
+-rw-r--r--   0 sallner   (1000) users      (100)      188 2023-07-31 06:31:36.000000 Products.Formulator-2.1/buildout4.cfg
+-rw-r--r--   0 sallner   (1000) users      (100)     1032 2023-07-31 06:31:40.599222 Products.Formulator-2.1/setup.cfg
+-rw-r--r--   0 sallner   (1000) users      (100)     2494 2023-07-31 06:31:36.000000 Products.Formulator-2.1/setup.py
+drwxr-xr-x   0 sallner   (1000) users      (100)        0 2023-07-31 06:31:40.575889 Products.Formulator-2.1/src/
+drwxr-xr-x   0 sallner   (1000) users      (100)        0 2023-07-31 06:31:40.579222 Products.Formulator-2.1/src/Products/
+drwxr-xr-x   0 sallner   (1000) users      (100)        0 2023-07-31 06:31:40.589222 Products.Formulator-2.1/src/Products/Formulator/
+-rw-r--r--   0 sallner   (1000) users      (100)     1163 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/DummyField.py
+-rw-r--r--   0 sallner   (1000) users      (100)     1317 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/EmailLinesField.py
+-rw-r--r--   0 sallner   (1000) users      (100)     1177 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/Errors.py
+-rw-r--r--   0 sallner   (1000) users      (100)     3289 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/FSForm.py
+-rw-r--r--   0 sallner   (1000) users      (100)    24598 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/Field.py
+-rw-r--r--   0 sallner   (1000) users      (100)     5318 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/FieldRegistry.py
+-rw-r--r--   0 sallner   (1000) users      (100)    41744 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/Form.py
+-rw-r--r--   0 sallner   (1000) users      (100)     4611 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/FormToXML.py
+-rw-r--r--   0 sallner   (1000) users      (100)     4738 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/FormulatorFormFile.py
+-rw-r--r--   0 sallner   (1000) users      (100)      334 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/HelperFields.py
+-rw-r--r--   0 sallner   (1000) users      (100)     4703 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/INSTALL.txt
+-rw-r--r--   0 sallner   (1000) users      (100)     2253 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/InterfaceField.py
+-rw-r--r--   0 sallner   (1000) users      (100)     2250 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/ListTextAreaField.py
+-rw-r--r--   0 sallner   (1000) users      (100)     2586 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/MethodField.py
+-rw-r--r--   0 sallner   (1000) users      (100)     4528 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/PatternChecker.py
+-rw-r--r--   0 sallner   (1000) users      (100)     5315 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/ProductForm.py
+-rw-r--r--   0 sallner   (1000) users      (100)     9906 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/StandardFields.py
+-rw-r--r--   0 sallner   (1000) users      (100)     2051 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/TALESField.py
+-rw-r--r--   0 sallner   (1000) users      (100)    33144 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/Validator.py
+-rw-r--r--   0 sallner   (1000) users      (100)    42673 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/Widget.py
+-rw-r--r--   0 sallner   (1000) users      (100)     2877 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/XMLObjects.py
+-rw-r--r--   0 sallner   (1000) users      (100)     6045 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/XMLToForm.py
+-rw-r--r--   0 sallner   (1000) users      (100)     4165 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/__init__.py
+-rw-r--r--   0 sallner   (1000) users      (100)      780 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/configure.zcml
+drwxr-xr-x   0 sallner   (1000) users      (100)        0 2023-07-31 06:31:40.589222 Products.Formulator-2.1/src/Products/Formulator/dtml/
+-rw-r--r--   0 sallner   (1000) users      (100)     1152 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/dtml/fieldAdd.dtml
+-rw-r--r--   0 sallner   (1000) users      (100)     2212 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/dtml/fieldEdit.dtml
+-rw-r--r--   0 sallner   (1000) users      (100)      434 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/dtml/fieldListHeader.dtml
+-rw-r--r--   0 sallner   (1000) users      (100)      582 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/dtml/fieldMessages.dtml
+-rw-r--r--   0 sallner   (1000) users      (100)     1317 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/dtml/fieldOverride.dtml
+-rw-r--r--   0 sallner   (1000) users      (100)     1499 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/dtml/fieldTales.dtml
+-rw-r--r--   0 sallner   (1000) users      (100)     1335 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/dtml/fieldTest.dtml
+-rw-r--r--   0 sallner   (1000) users      (100)     1393 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/dtml/formAdd.dtml
+-rw-r--r--   0 sallner   (1000) users      (100)     4063 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/dtml/formOrder.dtml
+-rw-r--r--   0 sallner   (1000) users      (100)     1246 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/dtml/formSettings.dtml
+-rw-r--r--   0 sallner   (1000) users      (100)     1877 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/dtml/formTest.dtml
+-rw-r--r--   0 sallner   (1000) users      (100)      522 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/dtml/formXML.dtml
+-rw-r--r--   0 sallner   (1000) users      (100)      297 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/ftesting.zcml
+drwxr-xr-x   0 sallner   (1000) users      (100)        0 2023-07-31 06:31:40.592555 Products.Formulator-2.1/src/Products/Formulator/help/
+-rw-r--r--   0 sallner   (1000) users      (100)     1084 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/help/BasicForm.py
+-rw-r--r--   0 sallner   (1000) users      (100)     5259 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/help/Field.py
+-rw-r--r--   0 sallner   (1000) users      (100)     8623 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/help/Form.py
+-rw-r--r--   0 sallner   (1000) users      (100)      794 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/help/ZMIForm.py
+-rw-r--r--   0 sallner   (1000) users      (100)     6066 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/help/dogfood.txt
+-rw-r--r--   0 sallner   (1000) users      (100)     2510 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/help/fieldEdit.txt
+-rw-r--r--   0 sallner   (1000) users      (100)      332 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/help/fieldMessages.txt
+-rw-r--r--   0 sallner   (1000) users      (100)     2067 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/help/fieldOverride.txt
+-rw-r--r--   0 sallner   (1000) users      (100)     3809 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/help/fieldTales.txt
+-rw-r--r--   0 sallner   (1000) users      (100)      905 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/help/fieldTest.txt
+-rw-r--r--   0 sallner   (1000) users      (100)      816 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/help/formContents.txt
+-rw-r--r--   0 sallner   (1000) users      (100)     3425 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/help/formOrder.txt
+-rw-r--r--   0 sallner   (1000) users      (100)     1524 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/help/formSettings.txt
+-rw-r--r--   0 sallner   (1000) users      (100)     1033 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/help/formTest.txt
+-rw-r--r--   0 sallner   (1000) users      (100)      670 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/help/formXML.txt
+-rw-r--r--   0 sallner   (1000) users      (100)    10039 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/help/formulator_howto.txt
+-rw-r--r--   0 sallner   (1000) users      (100)      219 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/help/formulator_motto.txt
+-rw-r--r--   0 sallner   (1000) users      (100)     1835 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/helpers.py
+-rw-r--r--   0 sallner   (1000) users      (100)     1899 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/homepage.html
+drwxr-xr-x   0 sallner   (1000) users      (100)        0 2023-07-31 06:31:40.592555 Products.Formulator-2.1/src/Products/Formulator/i18n/
+-rw-r--r--   0 sallner   (1000) users      (100)      641 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/i18n/__init__.py
+drwxr-xr-x   0 sallner   (1000) users      (100)        0 2023-07-31 06:31:40.575889 Products.Formulator-2.1/src/Products/Formulator/i18n/de/
+drwxr-xr-x   0 sallner   (1000) users      (100)        0 2023-07-31 06:31:40.592555 Products.Formulator-2.1/src/Products/Formulator/i18n/de/LC_MESSAGES/
+-rw-r--r--   0 sallner   (1000) users      (100)     2428 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/i18n/de/LC_MESSAGES/formulator.po
+drwxr-xr-x   0 sallner   (1000) users      (100)        0 2023-07-31 06:31:40.575889 Products.Formulator-2.1/src/Products/Formulator/i18n/en/
+drwxr-xr-x   0 sallner   (1000) users      (100)        0 2023-07-31 06:31:40.592555 Products.Formulator-2.1/src/Products/Formulator/i18n/en/LC_MESSAGES/
+-rw-r--r--   0 sallner   (1000) users      (100)     1630 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/i18n/en/LC_MESSAGES/formulator.po
+-rw-r--r--   0 sallner   (1000) users      (100)     1630 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/i18n/formulator.pot
+drwxr-xr-x   0 sallner   (1000) users      (100)        0 2023-07-31 06:31:40.575889 Products.Formulator-2.1/src/Products/Formulator/i18n/fr/
+drwxr-xr-x   0 sallner   (1000) users      (100)        0 2023-07-31 06:31:40.592555 Products.Formulator-2.1/src/Products/Formulator/i18n/fr/LC_MESSAGES/
+-rw-r--r--   0 sallner   (1000) users      (100)     2235 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/i18n/fr/LC_MESSAGES/formulator.po
+drwxr-xr-x   0 sallner   (1000) users      (100)        0 2023-07-31 06:31:40.575889 Products.Formulator-2.1/src/Products/Formulator/i18n/nl/
+drwxr-xr-x   0 sallner   (1000) users      (100)        0 2023-07-31 06:31:40.595889 Products.Formulator-2.1/src/Products/Formulator/i18n/nl/LC_MESSAGES/
+-rw-r--r--   0 sallner   (1000) users      (100)     2257 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/i18n/nl/LC_MESSAGES/formulator.po
+-rw-r--r--   0 sallner   (1000) users      (100)      279 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/interfaces.py
+-rw-r--r--   0 sallner   (1000) users      (100)      710 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/monkey.py
+-rw-r--r--   0 sallner   (1000) users      (100)     1857 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/testing.py
+drwxr-xr-x   0 sallner   (1000) users      (100)        0 2023-07-31 06:31:40.595889 Products.Formulator-2.1/src/Products/Formulator/tests/
+-rw-r--r--   0 sallner   (1000) users      (100)      154 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/tests/__init__.py
+-rw-r--r--   0 sallner   (1000) users      (100)     2787 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/tests/test_field_ids.py
+-rw-r--r--   0 sallner   (1000) users      (100)    22170 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/tests/test_form.py
+-rw-r--r--   0 sallner   (1000) users      (100)     1597 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/tests/test_pattern_checker.py
+-rw-r--r--   0 sallner   (1000) users      (100)    22079 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/tests/test_serialize.py
+-rw-r--r--   0 sallner   (1000) users      (100)    29404 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/tests/test_validators.py
+-rw-r--r--   0 sallner   (1000) users      (100)     3375 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/tests/test_widgets.py
+-rw-r--r--   0 sallner   (1000) users      (100)     5050 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/tests/test_zeam.py
+drwxr-xr-x   0 sallner   (1000) users      (100)        0 2023-07-31 06:31:40.599222 Products.Formulator-2.1/src/Products/Formulator/www/
+-rw-r--r--   0 sallner   (1000) users      (100)      899 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/www/BasicField.gif
+-rw-r--r--   0 sallner   (1000) users      (100)      901 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/www/CheckBoxField.gif
+-rw-r--r--   0 sallner   (1000) users      (100)      877 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/www/DateTimeField.gif
+-rw-r--r--   0 sallner   (1000) users      (100)      898 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/www/EmailField.gif
+-rw-r--r--   0 sallner   (1000) users      (100)      907 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/www/FileField.gif
+-rw-r--r--   0 sallner   (1000) users      (100)      902 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/www/FloatField.gif
+-rw-r--r--   0 sallner   (1000) users      (100)      875 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/www/Form.gif
+-rw-r--r--   0 sallner   (1000) users      (100)      895 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/www/IntegerField.gif
+-rw-r--r--   0 sallner   (1000) users      (100)      899 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/www/LabelField.gif
+-rw-r--r--   0 sallner   (1000) users      (100)      907 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/www/LinesField.gif
+-rw-r--r--   0 sallner   (1000) users      (100)      907 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/www/LinkField.gif
+-rw-r--r--   0 sallner   (1000) users      (100)      899 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/www/ListField.gif
+-rw-r--r--   0 sallner   (1000) users      (100)      877 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/www/MethodField.gif
+-rw-r--r--   0 sallner   (1000) users      (100)      919 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/www/MultiCheckBoxField.gif
+-rw-r--r--   0 sallner   (1000) users      (100)      118 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/www/MultiListField.gif
+-rw-r--r--   0 sallner   (1000) users      (100)      898 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/www/MultipleListField.gif
+-rw-r--r--   0 sallner   (1000) users      (100)      881 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/www/PasswordField.gif
+-rw-r--r--   0 sallner   (1000) users      (100)      905 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/www/PatternField.gif
+-rw-r--r--   0 sallner   (1000) users      (100)       92 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/www/RadioField.gif
+-rw-r--r--   0 sallner   (1000) users      (100)      906 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/www/RangedIntegerField.gif
+-rw-r--r--   0 sallner   (1000) users      (100)      899 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/www/StringField.gif
+-rw-r--r--   0 sallner   (1000) users      (100)      901 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/www/TextAreaField.gif
+-rw-r--r--   0 sallner   (1000) users      (100)     7454 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/Formulator/zeamsupport.py
+-rw-r--r--   0 sallner   (1000) users      (100)      342 2023-07-31 06:31:36.000000 Products.Formulator-2.1/src/Products/__init__.py
+drwxr-xr-x   0 sallner   (1000) users      (100)        0 2023-07-31 06:31:40.582555 Products.Formulator-2.1/src/Products.Formulator.egg-info/
+-rw-r--r--   0 sallner   (1000) users      (100)    31774 2023-07-31 06:31:39.000000 Products.Formulator-2.1/src/Products.Formulator.egg-info/PKG-INFO
+-rw-r--r--   0 sallner   (1000) users      (100)     4622 2023-07-31 06:31:40.000000 Products.Formulator-2.1/src/Products.Formulator.egg-info/SOURCES.txt
+-rw-r--r--   0 sallner   (1000) users      (100)        1 2023-07-31 06:31:39.000000 Products.Formulator-2.1/src/Products.Formulator.egg-info/dependency_links.txt
+-rw-r--r--   0 sallner   (1000) users      (100)        9 2023-07-31 06:31:40.000000 Products.Formulator-2.1/src/Products.Formulator.egg-info/namespace_packages.txt
+-rw-r--r--   0 sallner   (1000) users      (100)        1 2023-07-31 06:31:39.000000 Products.Formulator-2.1/src/Products.Formulator.egg-info/not-zip-safe
+-rw-r--r--   0 sallner   (1000) users      (100)      399 2023-07-31 06:31:40.000000 Products.Formulator-2.1/src/Products.Formulator.egg-info/requires.txt
+-rw-r--r--   0 sallner   (1000) users      (100)        9 2023-07-31 06:31:40.000000 Products.Formulator-2.1/src/Products.Formulator.egg-info/top_level.txt
+-rw-r--r--   0 sallner   (1000) users      (100)     2276 2023-07-31 06:31:36.000000 Products.Formulator-2.1/tox.ini
```

### Comparing `Products.Formulator-2.0.dev0/CHANGES.rst` & `Products.Formulator-2.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,27 @@
 Changes
 =======
 
-2.0 (unreleased)
------------------
+2.1 (2023-07-31)
+----------------
+
+- Port to Python 3, supporting Python 3.7 up to 3.11.
+
+
+2.0.1 (2023-03-28)
+------------------
+
+Bug fixes
++++++++++
+
+- Fix HTML quoting for values containing ``"``.
+
+
+2.0 (2023-03-14)
+----------------
 
 Backwards incompatible changes
 ++++++++++++++++++++++++++++++
 
 - Remove support for Zope 2 help system.
 
 - Stop testing Zope 2 compatibility. This release should still work with Zope 2
```

### Comparing `Products.Formulator-2.0.dev0/CREDITS.rst` & `Products.Formulator-2.1/CREDITS.rst`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/LICENSE.txt` & `Products.Formulator-2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/PKG-INFO` & `Products.Formulator-2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: Products.Formulator
-Version: 2.0.dev0
+Version: 2.1
 Summary: Form library for Zope 4
 Home-page: https://github.com/infrae/Products.Formulator
 Author: Martijn Faassen and community
 Author-email: info@infrae.com
 License: BSD
 Keywords: form generator zope4
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Zope :: 4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: test
 License-File: LICENSE.txt
 
 Formulator
 ==========
 
@@ -167,16 +173,31 @@
 Also a thank you to those few valiant souls who suffered through the
 bugs of ZFormulator, the previous implementation. Let's hope this
 one's better!
 
 Changes
 =======
 
-2.0 (unreleased)
------------------
+2.1 (2023-07-31)
+----------------
+
+- Port to Python 3, supporting Python 3.7 up to 3.11.
+
+
+2.0.1 (2023-03-28)
+------------------
+
+Bug fixes
++++++++++
+
+- Fix HTML quoting for values containing ``"``.
+
+
+2.0 (2023-03-14)
+----------------
 
 Backwards incompatible changes
 ++++++++++++++++++++++++++++++
 
 - Remove support for Zope 2 help system.
 
 - Stop testing Zope 2 compatibility. This release should still work with Zope 2
@@ -1061,7 +1082,9 @@
   documentation.
 
 0.9 (2001/04/30)
 ----------------
 
 - Initial public release of Formulator.
 
+
+
```

### Comparing `Products.Formulator-2.0.dev0/README.rst` & `Products.Formulator-2.1/README.rst`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/setup.cfg` & `Products.Formulator-2.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 htmldir = parts/flake8
 per-file-ignores = 
 	src/Products/Formulator/HelperFields.py: F401
 	src/Products/Formulator/Field.py: E301
 	src/Products/Formulator/Form.py: E301
 	src/Products/Formulator/FormulatorFormFile.py: E301
 	src/Products/Formulator/ProductForm.py: E301
+	src/Products/Formulator/__init__.py: E402
 extend-ignore = F821
 
 [check-manifest]
 ignore = 
 	.editorconfig
 	.meta.toml
 ignore-bad-ideas =
```

### Comparing `Products.Formulator-2.0.dev0/setup.py` & `Products.Formulator-2.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 # Copyright (c) 2008-2013 Infrae. All rights reserved.
 # See also LICENSE.txt
 
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = '2.0.dev0'
+version = '2.1'
 
 
 tests_require = [
+    'Products.PythonScripts',
     'Products.PythonScripts < 5.0; python_version=="2.7"',
     'plone.testing',
 ]
 
 
 def read_file(filename):
     with open(filename) as data:
@@ -30,32 +31,43 @@
       ),
       classifiers=[
           "Development Status :: 5 - Production/Stable",
           "Framework :: Zope :: 4",
           "License :: OSI Approved :: BSD License",
           "Programming Language :: Python",
           "Programming Language :: Python :: 2.7",
+          "Programming Language :: Python :: 3.7",
+          "Programming Language :: Python :: 3.8",
+          "Programming Language :: Python :: 3.9",
+          "Programming Language :: Python :: 3.10",
+          "Programming Language :: Python :: 3.11",
           "Topic :: Software Development :: Libraries :: Python Modules",
       ],
       keywords='form generator zope4',
       author='Martijn Faassen and community',
       author_email='info@infrae.com',
       url='https://github.com/infrae/Products.Formulator',
       license='BSD',
       packages=find_packages('src'),
       package_dir={'': 'src'},
       namespace_packages=['Products'],
       include_package_data=True,
       zip_safe=False,
       install_requires=[
+          'AccessControl',
           'grokcore.chameleon < 4.0; python_version=="2.7"',  # transitive
+          'DocumentTemplate',
+          'DocumentTemplate < 4.0; python_version=="2.7"',
+          'grokcore.component < 4.0; python_version=="2.7"',
           'grokcore.component',
           'grokcore.component < 4.0; python_version=="2.7"',
           'grokcore.view < 4.0; python_version=="2.7"',  # transitive
+          'martian < 2.0; python_version=="2.7"',  # transitive
           'setuptools',
+          'six',
           'zope.component',
           'zope.i18nmessageid',
           'zope.interface',
           'zope.cachedescriptors',
           'zeam.form.base',
           'zeam.form.base < 1.4; python_version=="2.7"',
       ],
```

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/DummyField.py` & `Products.Formulator-2.1/src/Products/Formulator/DummyField.py`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/EmailLinesField.py` & `Products.Formulator-2.1/src/Products/Formulator/EmailLinesField.py`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/Errors.py` & `Products.Formulator-2.1/src/Products/Formulator/Errors.py`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/FSForm.py` & `Products.Formulator-2.1/src/Products/Formulator/FSForm.py`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/Field.py` & `Products.Formulator-2.1/src/Products/Formulator/Field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2013  Infrae. All rights reserved.
 # See also LICENSE.txt
 
+import six
+
 import Acquisition
 import OFS.SimpleItem
 import zope.cachedescriptors.property
+import zope.interface
 from AccessControl import ClassSecurityInfo
 from AccessControl.class_init import InitializeClass
 from Acquisition import aq_inner
 from Acquisition import aq_parent
 from Acquisition.interfaces import IAcquirer
 from App.special_dtml import DTMLFile
 from Persistence import Persistent
 from Products.PageTemplates.Expressions import SecureModuleImporter
 from zope.i18nmessageid import MessageFactory
-from zope.interface import implements
 
 from Products.Formulator.Errors import ValidationError
 from Products.Formulator.helpers import convert_unicode
 from Products.Formulator.helpers import id_value_re
 from Products.Formulator.helpers import key_to_id_re
 from Products.Formulator.interfaces import IField
 from Products.Formulator.Widget import MultiItemsWidget
 
 
+@zope.interface.implementer(IField)
 class Field:
     """Base class of all fields.
     A field is an object consisting of a widget and a validator.
     """
     security = ClassSecurityInfo()
-    implements(IField)
 
     # this is a field
     is_field = 1
     # this is not an internal field (can be overridden by subclass)
     internal_field = 0
     # can alternatively render this field with Zope's :record syntax
     # this will be the record's name
@@ -282,15 +284,15 @@
                 result = getattr(self.validator, name)
             else:
                 result = "Unknown error: %s" % name
             # if we don't want message id, strip it off
             if not want_message_id:
                 try:
                     # convert message id into unicode string
-                    result = unicode(result)
+                    result = six.text_type(result)
                 except AttributeError:
                     pass
             return result
         else:
             if want_message_id:
                 # we do want a message id, so construct one from form domain
                 result = MessageFactory(self.get_i18n_domain())(result)
@@ -587,15 +589,15 @@
         """Change message texts.
         """
         messages = self.message_values
         unicode_mode = self.get_unicode_mode()
         for message_key in self.get_error_names():
             message = REQUEST[message_key]
             if unicode_mode:
-                message = unicode(message, 'UTF-8')
+                message = six.text_type(message, 'UTF-8')
             # only save message if we're indeed changing from original
             if getattr(self.validator, message_key) != message:
                 messages[message_key] = message
 
         self.message_values = messages
         if REQUEST:
             message = "Content changed."
```

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/FieldRegistry.py` & `Products.Formulator-2.1/src/Products/Formulator/FieldRegistry.py`

 * *Files 9% similar despite different names*

```diff
@@ -59,16 +59,16 @@
 FieldRegistry = FieldRegistry()
 
 
 def initializeFieldForm(field_class):
     """Initialize the properties (fields and values) on a particular
     field class. Also add the tales and override methods.
     """
-    from DummyField import fields
-    from Form import BasicForm
+    from Products.Formulator.DummyField import fields
+    from Products.Formulator.Form import BasicForm
 
     form = BasicForm()
     override_form = BasicForm()
     tales_form = BasicForm()
     for field in getPropertyFields(field_class.widget):
         group = field.get_value("group") or "widget"
         form.add_field(field, group)
```

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/Form.py` & `Products.Formulator-2.1/src/Products/Formulator/Form.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2013  Infrae. All rights reserved.
 # See also LICENSE.txt
 
-import string
-from urllib import quote
+from six import StringIO
+from six.moves import range
+from six.moves.urllib.parse import quote
 
 import Acquisition
-# Zope
 from AccessControl import ClassSecurityInfo
 from AccessControl.class_init import InitializeClass
 from Acquisition import aq_base
 from App.special_dtml import DTMLFile
 from ComputedAttribute import ComputedAttribute
 from OFS.ObjectManager import ObjectManager
 from OFS.PropertyManager import PropertyManager
 from OFS.role import RoleManager
 from OFS.SimpleItem import Item
 from Persistence import Persistent
-# String
-from StringIO import StringIO
-from zope.interface import implements
+from zope.interface import implementer
 
 from Products.Formulator.DummyField import fields
 from Products.Formulator.Errors import FieldDisabledError
 from Products.Formulator.Errors import FormValidationError
 from Products.Formulator.Errors import ValidationError
 from Products.Formulator.FieldRegistry import FieldRegistry
 from Products.Formulator.FormToXML import formToXML
 from Products.Formulator.helpers import ensure_unicode
 from Products.Formulator.interfaces import IForm
 from Products.Formulator.Widget import render_tag
 from Products.Formulator.XMLToForm import XMLToForm
 
 
+@implementer(IForm)
 class Form:
     """Form base class.
     """
     security = ClassSecurityInfo()
-    implements(IForm)
 
     # need to make settings form upgrade
     encoding = 'UTF-8'
     stored_encoding = 'ISO-8859-1'
     unicode_mode = 0
     i18n_domain = ''
 
@@ -782,15 +780,15 @@
         """Add a new field to the form.
         id        -- the id of the field to add
         title     -- the title of the field to add; this will be used in
                      displays of the field on forms
         fieldname -- the name of the field (meta_type) to add
         Result    -- empty string
         """
-        title = string.strip(title)
+        title = title.strip()
         if not title:
             title = id  # title is always required, use id if not provided
         if self.get_unicode_mode():
             # ZMI input is UTF-8 always (?)
             title = ensure_unicode(title)
         # get the field class we want to add
         field_class = FieldRegistry.get_field_class(fieldname)
@@ -837,18 +835,18 @@
     security.declareProtected('Change Formulator Forms', 'manage_settings')
     def manage_settings(self, REQUEST):
         """Change settings in settings screen.
         """
         try:
             result = self.settings_form.validate_all(REQUEST)
         except FormValidationError as e:
-            message = "Validation error(s).<br />" + string.join(
-                map(lambda error: "%s: %s" % (
+            message = "Validation error(s).<br />" + "<br />".join(
+                ["%s: %s" % (
                     error.field.get_value('title'),
-                    error.error_text), e.errors), "<br />")
+                    error.error_text) for error in e.errors])
             return self.formSettings(self, REQUEST,
                                      manage_tabs_message=message)
         # if we need to switch encoding, get xml representation before setting
         if result['unicode_mode'] != self.unicode_mode:
             xml = self.get_xml()
         # now set the form settings
 
@@ -899,15 +897,15 @@
                               'get_group_rows')
     def get_group_rows(self):
         """Get the groups in rows (for the order screen).
         """
         row_length = self.row_length
         groups = self.get_groups(include_empty=1)
         # get the amount of rows
-        rows = len(groups) / row_length
+        rows = len(groups) // row_length
         # if we would have extra groups not in a row, add a row
         if len(groups) % self.row_length != 0:
             rows = rows + 1
         # now create a list of group lists and return it
         result = []
         for i in range(rows):
             start = i * row_length
@@ -958,29 +956,29 @@
                               'manage_move_group')
     def manage_move_group(self, group, to_group, REQUEST):
         """Moves fields to a different group.
         """
         field_ids = self._get_field_ids(group, REQUEST)
         if (to_group != 'Move to:' and
                 self.move_field_group(field_ids, group, to_group)):
-            fields = string.join(field_ids, ", ")
+            fields = ", ".join(field_ids)
             message = "Fields %s transferred from %s to %s." % (fields,
                                                                 group,
                                                                 to_group)
         else:
             message = "Can't transfer fields."
         return self.formOrder(self, REQUEST,
                               manage_tabs_message=message)
 
     security.declareProtected('Change Formulator Forms',
                               'manage_add_group')
     def manage_add_group(self, new_group, REQUEST):
         """Adds a new group.
         """
-        group = string.strip(new_group)
+        group = new_group.strip()
         if (group and group != 'Select group' and
                 self.add_group(group)):
             message = "Group %s created." % (group)
         else:
             message = "Can't create group."
         return self.formOrder(self, REQUEST,
                               manage_tabs_message=message)
@@ -999,15 +997,15 @@
 
     security.declareProtected('Change Formulator Forms',
                               'manage_rename_group')
     def manage_rename_group(self, group, REQUEST):
         """Renames group.
         """
         if 'new_name' in REQUEST:
-            new_name = string.strip(REQUEST['new_name'])
+            new_name = REQUEST['new_name'].strip()
             if self.rename_group(group, new_name):
                 message = "Group %s renamed to %s." % (group, new_name)
             else:
                 message = "Can't rename group."
         else:
             message = "No new name supplied."
```

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/FormToXML.py` & `Products.Formulator-2.1/src/Products/Formulator/FormToXML.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2013  Infrae. All rights reserved.
 # See also LICENSE.txt
-import types
-from cgi import escape
+try:
+    from html import escape
+except ImportError:
+    from cgi import escape  # PY2
+
+import six
+from six import StringIO
 
 from DateTime import DateTime
-from StringIO import StringIO
 from zope.interface.interfaces import IInterface
 
 
 def formToXML(form, prologue=1):
     """Takes a formulator form and serializes it to an XML representation.
     """
     f = StringIO()
@@ -62,47 +66,49 @@
                 elif callable(value):
                     write('          <%s type="method">%s</%s>\n' %
                           (key, escape(str(value.method_name)), key))
                 elif isinstance(value, DateTime):
                     write('          <%s type="datetime">%s</%s>\n' %
                           (key, escape(str(value)), key))
                 else:
-                    if type(value) not in (
-                            types.StringType, types.UnicodeType):
+                    if not isinstance(
+                            value, (six.binary_type, six.text_type)):
                         value = str(value)
                     write('          <%s>%s</%s>\n'
                           % (key, escape(value), key))
             write('        </values>\n')
 
             write('        <tales>\n')
-            items = field.tales.items()
-            items.sort()
+            items = sorted(field.tales.items())
             for key, value in items:
                 if value:
                     write('          <%s>%s</%s>\n' %
                           (key, escape(str(value._text)), key))
             write('        </tales>\n')
 
             write('        <messages>\n')
             for message_key in field.get_error_names():
                 # get message text, don't want a MessageId as we
                 # don't want to trigger translation in serialization
                 message_text = field.get_error_message(message_key,
                                                        want_message_id=False)
+                message_text = escape(message_text)
+                message_key = escape(message_key)
                 # we don't want unicode here
                 if not form.unicode_mode:
-                    if isinstance(message_text, unicode):
+                    if six.PY2 and isinstance(message_text, six.text_type):
                         message_text = message_text.encode(
                             form.stored_encoding)
                 write('          <message name="%s">%s</message>\n' %
-                      (escape(message_key), escape(message_text)))
+                      (message_key, message_text))
             write('        </messages>\n')
             write('      </field>\n')
         write('      </fields>\n')
         write('    </group>\n')
     write('  </groups>\n')
     write('</form>')
 
-    if form.unicode_mode:
+    if six.PY3:
+        return f.getvalue()
+    elif form.unicode_mode:
         return f.getvalue().encode('UTF-8')
-    else:
-        return unicode(f.getvalue(), form.stored_encoding).encode('UTF-8')
+    return six.text_type(f.getvalue(), form.stored_encoding).encode('UTF-8')
```

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/FormulatorFormFile.py` & `Products.Formulator-2.1/src/Products/Formulator/FormulatorFormFile.py`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/INSTALL.txt` & `Products.Formulator-2.1/src/Products/Formulator/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/InterfaceField.py` & `Products.Formulator-2.1/src/Products/Formulator/InterfaceField.py`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/ListTextAreaField.py` & `Products.Formulator-2.1/src/Products/Formulator/ListTextAreaField.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2013  Infrae. All rights reserved.
 # See also LICENSE.txt
 
+import six
+
 from Products.Formulator import Validator
 from Products.Formulator import Widget
 from Products.Formulator.DummyField import fields
 from Products.Formulator.Field import ZMIField
 
 
 def split_value(value):
     result = []
     for line in value:
-        elements = line.split("|")
+        if isinstance(line, bytes):
+            elements = line.split(b"|")
+        else:
+            elements = line.split("|")
         if len(elements) >= 2:
             text, value = elements[:2]
         else:
             text = line
             value = line
         text = text.strip()
         value = value.strip()
@@ -28,15 +33,15 @@
                                        title='Default',
                                        default=[],
                                        required=0)
 
     def render(self, field, key, value, REQUEST):
         if value is None:
             value = field.get_value('default')
-        if isinstance(value, basestring):
+        if isinstance(value, six.string_types):
             # This happens while redisplaying a value from the request
             # i.e. _get_default(field, None, request)
             value = split_value(value.splitlines())
         lines = []
         for element_text, element_value in value:
             lines.append("%s | %s" % (element_text, element_value))
         lines = '\n'.join(lines)
```

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/MethodField.py` & `Products.Formulator-2.1/src/Products/Formulator/MethodField.py`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/PatternChecker.py` & `Products.Formulator-2.1/src/Products/Formulator/PatternChecker.py`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/ProductForm.py` & `Products.Formulator-2.1/src/Products/Formulator/ProductForm.py`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/StandardFields.py` & `Products.Formulator-2.1/src/Products/Formulator/StandardFields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2013  Infrae. All rights reserved.
 # See also LICENSE.txt
 
+from six.moves import range
+
 from DateTime import DateTime
 
 from Products.Formulator import Validator
 from Products.Formulator import Widget
 from Products.Formulator.Field import ZMIField
 from Products.Formulator.Form import BasicForm
 from Products.Formulator.MethodField import BoundMethod
```

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/TALESField.py` & `Products.Formulator-2.1/src/Products/Formulator/TALESField.py`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/Validator.py` & `Products.Formulator-2.1/src/Products/Formulator/Validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2013  Infrae. All rights reserved.
 # See also LICENSE.txt
 import re
 from threading import Thread
-from types import StringTypes
-from urllib import urlopen
+
+import six
+from six.moves.urllib.parse import urljoin
+from six.moves.urllib.request import urlopen
 
 from AccessControl.tainted import TaintedString
 from DateTime import DateTime
-from urlparse import urljoin
 
 from Products.Formulator import PatternChecker
 from Products.Formulator.DummyField import fields
 from Products.Formulator.Errors import ValidationError
 from Products.Formulator.helpers import ensure_unicode
 from Products.Formulator.i18n import translate as _
 
@@ -69,15 +70,15 @@
         """
         pass  # override in subclass
 
     def deserializeValue(self, field, value, context=None):
         """Given a field, a value and a context, unserialize the XML
         value for the field.
         """
-        if isinstance(value, basestring):
+        if isinstance(value, six.string_types):
             data = value
         else:
             # We have an lxml node
             data = value.text
             if data is None:
                 # Try for subvalues
                 data = []
@@ -157,15 +158,15 @@
             field=field,
             value=REQUEST.get(key, ""),
             failover=key + '_novalidate' in REQUEST)
 
     def serializeValue(self, field, value, producer):
         # if our value is not a string type, the SAX lib won't eat it,
         # therefore convert to string first
-        if type(value) not in (str, unicode):
+        if not isinstance(value, six.string_types):
             value = str(value)
         producer.characters(value)
 
 
 class StringValidator(StringBaseValidator):
     property_names = StringBaseValidator.property_names +\
         ['unicode', 'max_length', 'truncate']
@@ -298,15 +299,15 @@
         if value:
             value_string = 'True'
         else:
             value_string = 'False'
         producer.characters(value_string)
 
     def deserializeValue(self, field, value, context=None):
-        if not isinstance(value, basestring):
+        if not isinstance(value, six.string_types):
             value = value.text
         if value == 'True':
             return True
         return False
 
 
 BooleanValidatorInstance = BooleanValidator()
@@ -483,15 +484,18 @@
 
         # Check whether the entire input is too long
         max_length = field.get_value('max_length') or 0
         if max_length and len(value) > max_length:
             self.raise_error('too_long', field)
 
         # split input into separate lines
-        value = value.split("\n")
+        if isinstance(value, bytes):
+            value = value.split(b"\n")
+        else:
+            value = value.split("\n")
         return self.check(field, value, key + '_novalidate' in REQUEST)
 
     def serializeValue(self, field, value, producer):
         value_string = '\n'.join(value)
         producer.characters(value_string)
 
 
@@ -602,15 +606,15 @@
                 self.raise_error('required_not_found', field)
             return []
 
         convert = field.get_value('unicode')
         encoding = field.get_form_encoding()
 
         # Convert everything to unicode if necessary
-        value = map(lambda v: ensure_unicode(v, convert, encoding), value)
+        value = [ensure_unicode(v, convert, encoding) for v in value]
 
         if not failover:
             # Possible values
             items = set()
             for item in field.get_value('items'):
                 if isinstance(item, (tuple, list)):
                     _, candidate = item
@@ -663,15 +667,15 @@
         description=(
             "Checked if the field is required; the user has to supply a"
             " file."),
         default=0)
 
     def validate(self, field, key, REQUEST):
         f = REQUEST.get(key, None)
-        if type(f) in StringTypes:
+        if isinstance(f, six.string_types):
             self.raise_error('incorrect_enctype', field)
         if field.get_value('required'):
             if f.filename == '':
                 # I think we can assume that if the filename part
                 # of the content-disposition header is empty, then
                 # no file was uploaded.  I suppose we should also check to
                 # see if the file is of zero length, too.
@@ -891,15 +895,15 @@
 
     def serializeValue(self, field, value, producer):
         if value is not None:
             value_string = DateTime(value).HTML4()
             producer.characters(value_string)
 
     def deserializeValue(self, field, value, context=None):
-        if isinstance(value, basestring):
+        if isinstance(value, six.string_types):
             value = value.strip()
         else:
             value = value.text
             if value:
                 value.strip()
         if value:
             return DateTime(value)
```

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/Widget.py` & `Products.Formulator-2.1/src/Products/Formulator/Widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2013  Infrae. All rights reserved.
 # See also LICENSE.txt
-import cgi
 import operator
-import string
+
+import six
 
 from DateTime import DateTime
+from DocumentTemplate.html_quote import html_quote
 
 from Products.Formulator.DummyField import fields
 from Products.Formulator.helpers import id_value_re
 from Products.Formulator.helpers import is_sequence
 
 
 class Widget:
@@ -245,15 +246,15 @@
         height = field.get_value('height')
         extra = field.get_value('extra')
         css_class = field.get_value('css_class')
         kw = {'name': key,
               'css_class': css_class,
               'cols': width,
               'rows': height,
-              'contents': cgi.escape(value)}
+              'contents': html_quote(value)}
         if not extra or not id_value_re.search(extra):
             kw['id'] = field.generate_field_html_id(key)
         contents = render_element("textarea", **kw)
         return render_element("div", contents=contents, css_class=css_class)
 
     def render_view(self, field, value):
         return render_value(value)
@@ -284,15 +285,15 @@
         width=20,
         default='<br />\n',
         whitespace_preserve=1,
         required=1)
 
     def render(self, field, key, value, REQUEST):
         if is_sequence(value):
-            value = string.join(value, "\n")
+            value = "\n".join(value)
         return TextAreaWidget.render(self, field, key, value, REQUEST)
 
     def render_view(self, field, value):
         return render_value(value, field.get_value('view_separator'))
 
     def render_hidden(self, field, key, value, REQUEST):
         if value is None:
@@ -569,15 +570,15 @@
     def render(self, field, key, value, REQUEST):
         rendered_items = self.render_items(field, key, value, REQUEST)
 
         extra = field.get_value('extra')
         kw = {'name': key,
               'css_class': field.get_value('css_class'),
               'size': field.get_value('size'),
-              'contents': string.join(rendered_items, "\n"),
+              'contents': "\n".join(rendered_items),
               'extra': extra}
         if not extra or not id_value_re.search(extra):
             kw['id'] = field.generate_field_html_id(key)
         return render_element('select', **kw)
 
     def render_item(self, text, value, key, css_class, extra_item, html_id):
         return render_element('option', contents=text, value=value,
@@ -618,15 +619,15 @@
         rendered_items = self.render_items(field, key, value, REQUEST)
 
         extra = field.get_value('extra')
         kw = {'name': key,
               'multiple': None,
               'css_class': field.get_value('css_class'),
               'size': field.get_value('size'),
-              'contents': string.join(rendered_items, "\n"),
+              'contents': "\n".join(rendered_items),
               'extra': extra}
         if not extra or not id_value_re.search(extra):
             kw['id'] = field.generate_field_html_id(key)
         return render_element('select', **kw)
 
     def render_item(self, text, value, key, css_class, extra_item, html_id):
         return render_element('option', contents=text, value=value,
@@ -670,17 +671,17 @@
 
     has_html_id = False
 
     def render(self, field, key, value, REQUEST):
         rendered_items = self.render_items(field, key, value, REQUEST)
         orientation = field.get_value('orientation')
         if orientation == 'horizontal':
-            return string.join(rendered_items, "&nbsp;&nbsp;")
+            return "&nbsp;&nbsp;".join(rendered_items)
         else:
-            return string.join(rendered_items, "<br />")
+            return "<br />".join(rendered_items)
 
     def render_item(self, text, value, key, css_class, extra_item, html_id):
         kw = {'type': "radio",
               'css_class': css_class,
               'name': key,
               'value': value,
               'extra': extra_item}
@@ -735,17 +736,17 @@
 
     has_html_id = False
 
     def render(self, field, key, value, REQUEST):
         rendered_items = self.render_items(field, key, value, REQUEST)
         orientation = field.get_value('orientation')
         if orientation == 'horizontal':
-            return string.join(rendered_items, "&nbsp;&nbsp;")
+            return "&nbsp;&nbsp;".join(rendered_items)
         else:
-            return string.join(rendered_items, "<br />")
+            return "<br />".join(rendered_items)
 
     def render_item(self, text, value, key, css_class, extra_item, html_id):
         kw = {'type': "checkbox",
               'css_class': css_class,
               'name': key,
               'value': value,
               'extra': extra_item}
@@ -949,15 +950,15 @@
                 sub_field = field.sub_form.get_field(sub_field_name)
                 hidden_day_part = sub_field.widget.\
                     render_hidden(sub_field, sub_key,
                                   dayvalue, REQUEST)
             else:
                 result.append(field.render_sub_field(sub_field_name,
                                                      sub_field_value, REQUEST))
-        date_result = string.join(result, field.get_value('date_separator'))
+        date_result = field.get_value('date_separator').join(result)
 
         day_id = field.sub_form.get_field('day').generate_field_html_id(
             "subfield_" + field.id + "_day")
         month_id = field.sub_form.get_field('month').generate_field_html_id(
             "subfield_" + field.id + "_month")
         year_id = field.sub_form.get_field('year').generate_field_html_id(
             "subfield_" + field.id + "_year")
@@ -1106,15 +1107,15 @@
         order = field.get_value('input_order')
         if order == 'ymd':
             output = [year, month, day]
         elif order == 'dmy':
             output = [day, month, year]
         elif order == 'mdy':
             output = [month, day, year]
-        date_result = string.join(output, field.get_value('date_separator'))
+        date_result = field.get_value('date_separator').join(output)
 
         if not field.get_value('date_only'):
             time_result = hour + field.get_value('time_separator') + minute
             if use_ampm:
                 time_result += '&nbsp;' + ampm
             return date_result + '&nbsp;&nbsp;&nbsp;' + time_result
         else:
@@ -1148,18 +1149,18 @@
         return field.get_value('default')
 
 
 LabelWidgetInstance = LabelWidget()
 
 
 def render_unicode(value):
-    if not isinstance(value, unicode):
+    if not isinstance(value, six.text_type):
         if isinstance(value, str):
             return value.decode('utf-8', 'replace')
-        return unicode(value)
+        return six.text_type(value)
     return value
 
 
 def render_tag(tag, css_class=None, extra=None, **attributes):
     result = [tag]
 
     # special case handling for css_class
@@ -1192,11 +1193,11 @@
 
 def render_value(value, separator=None):
     """Default helper to render a value, paying attention to unicode.
     """
     if value is None:
         return u''
     if separator is not None and isinstance(value, (list, tuple)):
-        if not isinstance(separator, unicode):
-            separator = unicode(separator, 'utf-8')
+        if not isinstance(separator, six.text_type):
+            separator = six.text_type(separator, 'utf-8')
         value = separator.join(value)
-    return cgi.escape(render_unicode(value))
+    return html_quote(render_unicode(value))
```

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/XMLObjects.py` & `Products.Formulator-2.1/src/Products/Formulator/XMLObjects.py`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/XMLToForm.py` & `Products.Formulator-2.1/src/Products/Formulator/XMLToForm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2013  Infrae. All rights reserved.
 # See also LICENSE.txt
+import six
+
 from DateTime import DateTime
 from zope.component import getUtility
 from zope.interface.interfaces import IInterface
 
 from Products.Formulator import XMLObjects
 from Products.Formulator.MethodField import Method
 from Products.Formulator.TALESField import TALESMethod
@@ -67,15 +69,17 @@
             has_default = 1
         form.add_group(group_title)
         # create fields in group
         if not hasattr(group.first.fields.elements, 'field'):
             # empty <fields> element
             continue
         for entry in group.first.fields.elements.field:
-            id = str(encode(entry.first.id.text, encoding))
+            id = encode(entry.first.id.text, encoding)
+            if six.PY2:
+                id = str(id)
             meta_type = encode(entry.first.type.text, encoding)
             try:
                 form._delObject(id)
             except (KeyError, AttributeError):
                 pass
             form.manage_addField(id, '', meta_type)
             field = form._getOb(id)
@@ -143,11 +147,11 @@
     old_ids = [x for x in form.objectIds()
                if x not in form.get_field_ids(include_disabled=1)]
     if old_ids:
         form.manage_delObjects(old_ids)
 
 
 def encode(text, encoding):
-    if encoding is None:
+    if six.PY3 or encoding is None:
         return text
     else:
         return text.encode(encoding)
```

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/__init__.py` & `Products.Formulator-2.1/src/Products/Formulator/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2013  Infrae. All rights reserved.
 # See also LICENSE.txt
 
+import warnings
+
+
+# ignore some annoying warning in the test run:
+warnings.filterwarnings(
+    "ignore",
+    message="Deprecated call to `pkg_resources.declare_namespace",
+    category=DeprecationWarning)
+
+
 from AccessControl import allow_module
 
 from Products.Formulator import EmailLinesField
 from Products.Formulator import Errors  # noqa: F401 imported but unused
 from Products.Formulator import Form
 from Products.Formulator import HelperFields
 from Products.Formulator import InterfaceField
```

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/configure.zcml` & `Products.Formulator-2.1/src/Products/Formulator/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/fieldAdd.dtml` & `Products.Formulator-2.1/src/Products/Formulator/dtml/fieldAdd.dtml`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/fieldEdit.dtml` & `Products.Formulator-2.1/src/Products/Formulator/dtml/fieldEdit.dtml`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 <dtml-in "form.get_groups()">
 <dtml-let group=sequence-item fields="form.get_fields_in_group(group)">
 
 <dtml-if fields>
 <tr>
 <td colspan="4" class="form-title">
-  <dtml-var "_.string.capitalize(group)"> properties
+  <dtml-var "group.capitalize()"> properties
 </td>
 </tr>
 
 <dtml-var fieldListHeader>
 
 <dtml-in fields>
 <dtml-let field=sequence-item field_id="field.id"
@@ -67,10 +67,7 @@
     </td>
   </tr>
 </table>
 </form>
 
 </dtml-let>
 <dtml-var manage_page_footer>
-
-
-
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 
 Edit  properties here.
 This field's HTML name is:
 This field's HTML ID is:
 NOTE: for multi-item inputs (e.g. Radios and Checkboxes), individual input
 field keys use field's HTML ID + item index. E.g. the second checkbox would be
 2.
-_.string.capitalize(group)"> properties
+group.capitalize()"> properties
 field.widget.has_html_id"> field.render field.meta_type"> field.get_value
 html_id">">                (value)">                      ('description')">
 tales or override">[
 field.title()">
 field.has_value
 ('required') and
 field.get_value
```

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/fieldMessages.dtml` & `Products.Formulator-2.1/src/Products/Formulator/dtml/fieldMessages.dtml`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/fieldOverride.dtml` & `Products.Formulator-2.1/src/Products/Formulator/dtml/fieldOverride.dtml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 <dtml-in "override_form.get_groups()">
 <dtml-let group=sequence-item fields="override_form.get_fields_in_group(group)">
 
 <dtml-if fields>
 <tr>
 <td colspan="3" class="form-title">
-  <dtml-var "_.string.capitalize(group)"> properties
+  <dtml-var "group.capitalize()"> properties
 </td>
 </tr>
 
 <dtml-var fieldListHeader>
 
 <dtml-let current_field="this()">
 <dtml-in fields>
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
 
 Edit  method overrides here.
-_.string.capitalize(group)"> properties
+group.capitalize()"> properties
 field.title()"> field.render(value)"> current_field.form.get_field
                                       (field.id).meta_type">
 [Save Changes]
```

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/fieldTales.dtml` & `Products.Formulator-2.1/src/Products/Formulator/dtml/fieldTales.dtml`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 <dtml-in "override_form.get_groups()">
 <dtml-let group=sequence-item fields="tales_form.get_fields_in_group(group)">
 
 <dtml-if fields>
 <tr>
 <td colspan="3" class="form-title">
-  <dtml-var "_.string.capitalize(group)"> properties
+  <dtml-var "group.capitalize()"> properties
 </td>
 </tr>
 
 <dtml-var fieldListHeader>
 
 <dtml-let current_field="this()">
 <dtml-in fields>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 
 Edit  method TALES expressions here. not isTALESAvailable()">
  Zope Page Templates and therefore TALES is not installed. This tab can
 therefore not be used.
-_.string.capitalize(group)"> properties
+group.capitalize()"> properties
 field.title()"> field.render(value)"> current_field.form.get_field
                                       (field.id).meta_type">
 [Save Changes]
```

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/fieldTest.dtml` & `Products.Formulator-2.1/src/Products/Formulator/dtml/fieldTest.dtml`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/formAdd.dtml` & `Products.Formulator-2.1/src/Products/Formulator/dtml/formAdd.dtml`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/formOrder.dtml` & `Products.Formulator-2.1/src/Products/Formulator/dtml/formOrder.dtml`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/formSettings.dtml` & `Products.Formulator-2.1/src/Products/Formulator/dtml/formSettings.dtml`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/formTest.dtml` & `Products.Formulator-2.1/src/Products/Formulator/dtml/formTest.dtml`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/dtml/formXML.dtml` & `Products.Formulator-2.1/src/Products/Formulator/dtml/formXML.dtml`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/help/BasicForm.py` & `Products.Formulator-2.1/src/Products/Formulator/help/BasicForm.py`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/help/Field.py` & `Products.Formulator-2.1/src/Products/Formulator/help/Field.py`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/help/Form.py` & `Products.Formulator-2.1/src/Products/Formulator/help/Form.py`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/help/ZMIForm.py` & `Products.Formulator-2.1/src/Products/Formulator/help/ZMIForm.py`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/help/dogfood.txt` & `Products.Formulator-2.1/src/Products/Formulator/help/dogfood.txt`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/help/fieldEdit.txt` & `Products.Formulator-2.1/src/Products/Formulator/help/fieldEdit.txt`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/help/fieldOverride.txt` & `Products.Formulator-2.1/src/Products/Formulator/help/fieldOverride.txt`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/help/fieldTales.txt` & `Products.Formulator-2.1/src/Products/Formulator/help/fieldTales.txt`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/help/fieldTest.txt` & `Products.Formulator-2.1/src/Products/Formulator/help/fieldTest.txt`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/help/formContents.txt` & `Products.Formulator-2.1/src/Products/Formulator/help/formContents.txt`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/help/formOrder.txt` & `Products.Formulator-2.1/src/Products/Formulator/help/formOrder.txt`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/help/formSettings.txt` & `Products.Formulator-2.1/src/Products/Formulator/help/formSettings.txt`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/help/formTest.txt` & `Products.Formulator-2.1/src/Products/Formulator/help/formTest.txt`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/help/formXML.txt` & `Products.Formulator-2.1/src/Products/Formulator/help/formXML.txt`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/help/formulator_howto.txt` & `Products.Formulator-2.1/src/Products/Formulator/help/formulator_howto.txt`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/helpers.py` & `Products.Formulator-2.1/src/Products/Formulator/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2013  Infrae. All rights reserved.
 # See also LICENSE.txt
 import re
 
+import six
+
 from Acquisition import aq_base
 
 
-seq_types = [type([]), type(())]
+seq_types = [list, tuple]
 
 
 def ensure_unicode(value, convert=True, encoding='utf-8'):
-    if convert:
-        if not isinstance(value, unicode):
-            if not isinstance(value, str):
+    if six.PY3 or convert:
+        if not isinstance(value, six.text_type):
+            if not isinstance(value, six.binary_type):
                 value = str(value)
-            value = unicode(value, encoding)
-    elif isinstance(value, unicode):
+            else:
+                value = six.text_type(value, encoding)
+    elif isinstance(value, six.text_type):
         value = value.encode(encoding)
-    elif not isinstance(value, basestring):
-        value = str(value)
+    elif not isinstance(value, (six.binary_type, six.text_type)):
+        value = str(value).encode(encoding)
     return value
 
 
 def is_sequence(v):
     return type(aq_base(v)) in seq_types
 
 
 def convert_unicode(struct, encoding):
     """ convert all strings of a possibly deeply nested structure
     of lists from utf-8 to unicode
     in case of a dictionary only converts the values, not the keys
     """
 
-    if isinstance(struct, str):
-        return unicode(struct, encoding)
+    if isinstance(struct, six.binary_type):
+        return six.text_type(struct, encoding)
 
     if isinstance(struct, list):
         return [convert_unicode(x, encoding) for x in struct]
 
     if isinstance(struct, tuple):
         return tuple([convert_unicode(x, encoding) for x in struct])
```

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/homepage.html` & `Products.Formulator-2.1/src/Products/Formulator/homepage.html`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/i18n/__init__.py` & `Products.Formulator-2.1/src/Products/Formulator/i18n/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/i18n/de/LC_MESSAGES/formulator.po` & `Products.Formulator-2.1/src/Products/Formulator/i18n/de/LC_MESSAGES/formulator.po`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/i18n/en/LC_MESSAGES/formulator.po` & `Products.Formulator-2.1/src/Products/Formulator/i18n/en/LC_MESSAGES/formulator.po`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/i18n/formulator.pot` & `Products.Formulator-2.1/src/Products/Formulator/i18n/formulator.pot`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/i18n/fr/LC_MESSAGES/formulator.po` & `Products.Formulator-2.1/src/Products/Formulator/i18n/fr/LC_MESSAGES/formulator.po`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/i18n/nl/LC_MESSAGES/formulator.po` & `Products.Formulator-2.1/src/Products/Formulator/i18n/nl/LC_MESSAGES/formulator.po`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/monkey.py` & `Products.Formulator-2.1/src/Products/Formulator/monkey.py`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/testing.py` & `Products.Formulator-2.1/src/Products/Formulator/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2013  Infrae. All rights reserved.
 # See also LICENSE.txt
-
-
 import importlib
 
 import plone.testing.zope
 from plone.testing.layer import Layer
 from plone.testing.zca import ZCMLSandbox
 from plone.testing.zope import WSGI_SERVER
 from Testing.makerequest import makerequest
```

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/tests/test_field_ids.py` & `Products.Formulator-2.1/src/Products/Formulator/tests/test_field_ids.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,52 +24,52 @@
         self.form = self.root.form
         factory = self.form.manage_addProduct['Formulator']
         factory.manage_addField('text', 'Text Field', 'StringField')
 
     def test_field_html_id(self):
         # test standard use-case
         sf = self.form.text
-        self.assertEquals('field-text', sf.generate_field_html_id())
-        self.assertEquals('field-text', sf.html_id)
+        self.assertEqual('field-text', sf.generate_field_html_id())
+        self.assertEqual('field-text', sf.html_id)
 
     def test_html_id_with_field_record(self):
         # SilvaMetadata uses a 'field_record' to add uniqueness
         # to the field key, so test that as well
         sf = self.form.text
-        self.assertEquals('field-text', sf.generate_field_html_id())
+        self.assertEqual('field-text', sf.generate_field_html_id())
 
         sf.field_record = 'silva-extra'
-        self.assertEquals('silva-extra-text-record',
-                          sf.generate_field_html_id())
+        self.assertEqual('silva-extra-text-record',
+                         sf.generate_field_html_id())
 
         sf.field_record = None
 
     def test_html_id_with_field_record_bis(self):
         # the form name can be used to add uniqueness as well
         # to the field key, so test that as well
         sf = self.form.text
-        self.assertEquals('field-text', sf.generate_field_html_id())
+        self.assertEqual('field-text', sf.generate_field_html_id())
 
         self.form.name = 'test'
-        self.assertEquals('testfield-text', sf.generate_field_html_id())
+        self.assertEqual('testfield-text', sf.generate_field_html_id())
         self.form.name = ''
 
     def test_html_id_in_extra(self):
         # verify that an html id specified in the "extra" parameter
         # is used if present.  Also test the regular expression
         sf = self.form.text
         sf.values['extra'] = 'id="HTML"'
-        self.assertEquals('HTML', sf.generate_field_html_id())
+        self.assertEqual('HTML', sf.generate_field_html_id())
         sf.values['extra'] = "id='HTML'"
-        self.assertEquals('HTML', sf.generate_field_html_id())
+        self.assertEqual('HTML', sf.generate_field_html_id())
         sf.values['extra'] = 'class="blah123" id="HTML"'
-        self.assertEquals('HTML', sf.generate_field_html_id())
+        self.assertEqual('HTML', sf.generate_field_html_id())
         sf.values['extra'] = 'formid="asdf" id="HTML"'
-        self.assertEquals('HTML', sf.generate_field_html_id())
+        self.assertEqual('HTML', sf.generate_field_html_id())
         sf.values['extra'] = 'id="HTML" formid="asdf"'
-        self.assertEquals('HTML', sf.generate_field_html_id())
+        self.assertEqual('HTML', sf.generate_field_html_id())
 
 
 def test_suite():
     suite = unittest.TestSuite()
     suite.addTest(unittest.makeSuite(FieldIdsTestCase))
     return suite
```

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/tests/test_form.py` & `Products.Formulator-2.1/src/Products/Formulator/tests/test_form.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,41 +68,41 @@
         items1 = list_field.render()
 
         # test TALES
         list_field.tales['items'] = TALESMethod("python:['ok', 'no']")
         items2 = list_field.render()
 
         # test render
-        self.assertEquals(items1, items2)
+        self.assertEqual(items1, items2)
         # test render_view
-        self.assertEquals('ok', list_field.render_view('ok'))
+        self.assertEqual('ok', list_field.render_view('ok'))
         # test validation ... fake request with a dictionary ...
         list_field.validate({'field_list_field': 'ok'})
 
         # test override (most probably superfluous)
         del list_field.tales['items']
         list_field.overrides['items'] = Method('override_test')
         items2 = list_field.render()
 
-        self.assertEquals(items1, items2)
+        self.assertEqual(items1, items2)
 
         # missing: if returning a list of int,
         # rendering does work here, but validation fails.
         # maybe it should fail, but on the other hand this is a FAQ on the list
         # ...
         del list_field.overrides['items']
         # test when TALES returns a list of e.g. int
         list_field.values['items'] = [('42', '42'), ('88', '88')]
 
         items1 = list_field.render()
 
         list_field.tales['items'] = TALESMethod("python:[42, 88]")
         items2 = list_field.render()
 
-        self.assertEquals(items1, items2)
+        self.assertEqual(items1, items2)
 
         list_field.validate({'field_list_field': '42'})
 
     def test_items_is_sequence(self):
         """ test that a multi list widget renders correctly,
         even if the items consist out of a tuple.
         this has bugged in some earlier version
@@ -117,22 +117,22 @@
         list_field = self.form.list_field
         list_field.values['items'] = [('foo', 'foo'), ('bar', 'bar')]
 
         items1 = list_field.render(('foo',))
 
         list_field.tales['items'] = TALESMethod("python:('foo', 'bar')")
 
-        self.assertEquals(('foo', 'bar'), list_field.get_value('items'))
+        self.assertEqual(('foo', 'bar'), list_field.get_value('items'))
 
         items2 = list_field.render(('foo',))
 
         # test render
-        self.assertEquals(items1, items2)
+        self.assertEqual(items1, items2)
         # test render_view
-        self.assertEquals("foo", list_field.render_view(('foo',)))
+        self.assertEqual("foo", list_field.render_view(('foo',)))
 
     def test_items_is_sequence_bis(self):
         """ test that a multi list values widget renders correctly,
             if the value from the request contains a list of non-ascii values
         """
         self.form.manage_addField(
             'list_boxes',
@@ -141,25 +141,25 @@
         self.encoding = "utf-8"
         self.form.unicode_mode = 1
         list_boxes = self.form.list_boxes
         list_boxes.values['unicode'] = 1
         list_boxes.values['items'] = \
             [(u'\xe4', u'A uml'), (u'\xfc', u'U uml')]
         request = TestRequest()
-        request.form['key'] = ['\xc3\xa4', '\xc3\xbc']
+        request.form['key'] = [b'\xc3\xa4', b'\xc3\xbc']
         items = list_boxes._get_default(key='key', value=None,
                                         REQUEST=request)
-        self.assertEquals([u'\xe4', u'\xfc'], items)
+        self.assertEqual([u'\xe4', u'\xfc'], items)
 
         # same with latin-1 (we should not hardcode utf-8)
         self.form.encoding = "latin-1"
         request.form['key'] = ['\xe4', '\xfc']
         items = list_boxes._get_default(key='key', value=None,
                                         REQUEST=request)
-        self.assertEquals([u'\xe4', u'\xfc'], items)
+        self.assertEqual([u'\xe4', u'\xfc'], items)
 
     def test_lines_field_rendering(self):
         """ line fields should both accept lists / tuples
         of strings and single strings with whitespace.
         If they would not accept the second case, render_from_request
         would be broken.
         """
@@ -181,15 +181,15 @@
         textareas = [child for child in divs[0].childNodes
                      if child.nodeType == child.ELEMENT_NODE]
         self.assertEqual(len(textareas), 1)
         self.assertEqual(textareas[0].nodeName, 'textarea')
         text = [child for child in textareas[0].childNodes
                 if child.nodeType == child.TEXT_NODE]
 
-        self.assertEquals('Text', ''.join(map(lambda n: n.nodeValue, text)))
+        self.assertEqual('Text', ''.join([n.nodeValue for n in text]))
 
         field.values['hidden'] = 'checked'
         rendered = field.render(REQUEST=request)
 
     def test_labels(self):
         """ test that labels do not influence validation """
         self.form.manage_addField(
@@ -198,15 +198,15 @@
         self.form.label_field.overrides['default'] = "Some label"
 
         self.form.manage_addField(
             'int_field', 'Test integer field', 'IntegerField')
 
         result = self.form.validate_all(
             {'field_int_field': '3'})
-        self.assertEquals({'int_field': 3}, result)
+        self.assertEqual({'int_field': 3}, result)
 
     def test_labels_with_direct_validation(self):
         """ PloneFormMailer calls validate() directly on each field,
         this used to give a KeyError as 'external_validator' wasn't
         known for a label field.
         """
         self.form.manage_addField(
@@ -220,93 +220,93 @@
         self.form.manage_addProduct['Formulator']\
                  .manage_addField('date_time', 'Test Field', 'DateTimeField')
         field = self.form.date_time
 
         css_matcher = re.compile('class="([^"]*)"')
 
         # initially no css class is set
-        self.assertEquals(0, len(css_matcher.findall(field.render())))
+        self.assertEqual(0, len(css_matcher.findall(field.render())))
 
         # edit the field, bypassing validation ...
         field._edit({'css_class': 'some_class'})
 
         # now we should have five matches for the five subfields ...
         css_matches = css_matcher.findall(field.render())
-        self.assertEquals(10, len(css_matches))
+        self.assertEqual(10, len(css_matches))
         # ... and all have the given value:
         for m in css_matches:
-            self.assertEquals('some_class', m)
+            self.assertEqual('some_class', m)
 
         # change the input style: the css needs to be
         # propagated to the newly created subfields
         current_style = field['input_style']
         other_style = {'list': 'text', 'text': 'list'}[current_style]
         field._edit({'input_style': other_style})
 
         # still the css classes should remain the same
         css_matches = css_matcher.findall(field.render())
-        self.assertEquals(7, len(css_matches))
+        self.assertEqual(7, len(css_matches))
         for m in css_matches:
-            self.assertEquals('some_class', m)
+            self.assertEqual('some_class', m)
 
         # now just change to another value:
         field._edit({'css_class': 'other_class'})
         css_matches = css_matcher.findall(field.render())
-        self.assertEquals(7, len(css_matches))
+        self.assertEqual(7, len(css_matches))
         for m in css_matches:
-            self.assertEquals('other_class', m)
+            self.assertEqual('other_class', m)
 
         # and clear the css_class field:
         field._edit({'css_class': ''})
         css_matches = css_matcher.findall(field.render())
-        self.assertEquals(0, len(css_matches))
+        self.assertEqual(0, len(css_matches))
 
     def _helper_render_datetime(
             self,
             expected_values,
             rendered,
             type='hidden'):
         # heper to check if the generated HTML from render or render_hidden
         # meets the expectations
         dom = parseString('<dummy>%s</dummy>' % rendered)
         elements = [child for child in dom.documentElement.childNodes
                     if child.nodeType == child.ELEMENT_NODE]
         if type != 'hidden':
             # They are wrapped in divs if not hidden
-            self.assertEquals(len(elements), len(expected_values))
+            self.assertEqual(len(elements), len(expected_values))
             inputs = []
             for element in elements:
                 inputs.extend([child for child in element.childNodes
                                if child.nodeType == child.ELEMENT_NODE])
         else:
             inputs = elements
 
-        self.assertEquals(len(expected_values.keys()), len(inputs))
+        self.assertEqual(len(list(expected_values.keys())), len(inputs))
         values = {}
         for input in inputs:
-            self.assertEquals('input', input.nodeName)
-            self.assertEquals(type, input.getAttribute('type'))
+            self.assertEqual('input', input.nodeName)
+            self.assertEqual(type, input.getAttribute('type'))
             self.assertFalse(input.childNodes)
             values[input.getAttribute('name')] = input.getAttribute('value')
-        self.assertEquals(expected_values, values)
+        self.assertEqual(expected_values, values)
 
     def _helper_render_hidden_list(self, expected_name, expected_values,
                                    rendered):
         # heper to check if the generated HTML from render_hidden
         # meets the expectations
         dom = parseString('<dummy>%s</dummy>' % rendered)
         elements = [child for child in dom.documentElement.childNodes
                     if child.nodeType == child.ELEMENT_NODE]
-        self.assertEquals(len(expected_values), len(elements))
+        self.assertEqual(len(expected_values), len(elements))
         for child in elements:
-            self.assertEquals('input', child.nodeName)
-            self.assertEquals('hidden', child.getAttribute('type'))
-            self.assertEquals(expected_name, child.getAttribute('name'))
-            self.assertEquals(expected_values.pop(0),
-                              child.getAttribute('value'))
+            self.assertEqual('input', child.nodeName)
+            self.assertEqual('hidden', child.getAttribute('type'))
+            self.assertEqual(expected_name, child.getAttribute('name'))
+            self.assertEqual(expected_values.pop(0),
+                             child.getAttribute('value'))
             self.assertFalse(child.childNodes)
 
     def test_render_hidden(self):
         # test that rendering fields hidden does produce
         # meaningful results; i.e. such which may still lead to successful
         # validation when submitting a form with hidden fields
         # this has been broken for DateTimeFields, and fields
@@ -389,26 +389,26 @@
         self.form.manage_addProduct['Formulator']\
                  .manage_addField('radio', 'Test Field', 'RadioField')
 
         for field in self.form.single_list, self.form.radio:
             field.values['items'] = [('Alpha', 'a'),
                                      ('Beta', 'b'),
                                      ('Gamma', 'c'), ]
-            self.assertEquals('Gamma', field.render_view('c'), msg=field.id)
+            self.assertEqual('Gamma', field.render_view('c'), msg=field.id)
 
         for field in self.form.multi_list, self.form.check_boxes:
             field.values['items'] = [('Alpha', 'a'),
                                      ('Beta', 'b'),
                                      ('Gamma', 'c'), ]
 
             field.values['view_separator'] = '|||'
-            self.assertEquals('Gamma', field.render_view(['c']))
-            self.assertEquals('|||'.join(('Alpha', 'Gamma')),
-                              field.render_view(['a', 'c']))
-            self.assertEquals('', field.render_view([]))
+            self.assertEqual('Gamma', field.render_view(['c']))
+            self.assertEqual('|||'.join(('Alpha', 'Gamma')),
+                             field.render_view(['a', 'c']))
+            self.assertEqual('', field.render_view([]))
 
     def test_default_to_now_does_not_overwrite_request_values(self):
         self.form.manage_addField(
             'date_field',
             'Test DateTime Field',
             'DateTimeField')
         date_field = self.form.date_field
@@ -438,23 +438,23 @@
             'Test Checkbox',
             'CheckBoxField')
         checkbox_field = self.form.checkbox_field
 
         checkbox_field.values['default'] = 1
 
         rendered = checkbox_field.render()
-        self.assert_(-1 != rendered.find('checked="checked"'))
+        self.assertNotEqual(-1, rendered.find('checked="checked"'))
 
         request = TestRequest()
         rendered = checkbox_field.render_from_request(request)
-        self.assert_(-1 != rendered.find('checked="checked"'))
+        self.assertNotEqual(-1, rendered.find('checked="checked"'))
 
         request.form['formulator_submission'] = '1'
         rendered = checkbox_field.render_from_request(request)
-        self.assertEquals(-1, rendered.find('checked="checked"'))
+        self.assertEqual(-1, rendered.find('checked="checked"'))
 
     def test_edit_listitem(self):
         """ if eding a list item via ZMI (or xml rpc) in unicode mode
         this has blown because some lists of strings have
         not been converted properly
         """
         self.form.unicode_mode = 1
@@ -462,74 +462,74 @@
         self.form.manage_addField(
             'lines_field',
             'Test Linesfield',
             'LinesField')
         list_field = self.form.list_field
         lines_field = self.form.lines_field
         # just to make sure
-        self.assert_(list_field.get_unicode_mode())
+        self.assertTrue(list_field.get_unicode_mode())
 
         # the list field has the most complicated setting:
         # a list of 2-tuples for the 'items'
         request = TestRequest(form={
-            'field_title': 'Title\xc3\xbc',
-            'field_default': 'item\xc3\xbc',
-            'field_items': 'item\xc3\xbc | item_ue\nitem2 | item2',
+            'field_title': b'Title\xc3\xbc',
+            'field_default': b'item\xc3\xbc',
+            'field_items': b'item\xc3\xbc | item_ue\nitem2 | item2',
             'field_size': '7',
         })
         list_field.manage_edit(request)
-        self.assertEquals(u'item\xfc',
-                          list_field.get_value('default'))
+        self.assertEqual(u'item\xfc',
+                         list_field.get_value('default'))
         expected_items = [(u'item\xfc', u'item_ue'), ('item2', 'item2')]
-        self.assertEquals(expected_items,
-                          list_field.get_value('items'))
+        self.assertEqual(expected_items,
+                         list_field.get_value('items'))
 
-        self.assertEquals(7, list_field.get_value('size'))
+        self.assertEqual(7, list_field.get_value('size'))
 
         # the lines field has a plain list of string as 'default'
         request = TestRequest(form={
-            'field_title': 'Title\xc3\xbc',
-            'field_default': 'item\xc3\xbc\nitem2',
+            'field_title': b'Title\xc3\xbc',
+            'field_default': b'item\xc3\xbc\nitem2',
             'field_width': '40',
             'field_height': '5',
-            'field_view_separator': 'sep \xc3\xbc',
+            'field_view_separator': b'sep \xc3\xbc',
         })
         lines_field.manage_edit(request)
-        self.assertEquals(u'Title\xfc',
-                          lines_field.get_value('title'))
-        self.assertEquals([u'item\xfc', u'item2'],
-                          lines_field.get_value('default'))
+        self.assertEqual(u'Title\xfc',
+                         lines_field.get_value('title'))
+        self.assertEqual([u'item\xfc', u'item2'],
+                         lines_field.get_value('default'))
 
     def test_tales_none(self):
         # test that a TALES default of None is rendered
         # as the empty string in the field's value attribute
         # and not as "value"
         self.form.manage_addField('text', 'Text Field', 'StringField')
         text = self.form.text
         text.tales['default'] = TALESMethod('nothing')
-        self.assertEquals(1, text.render().count('value=""'))
+        self.assertEqual(1, text.render().count('value=""'))
 
     def test_add_unicode_form(self):
         # test bugfix when adding a form with a non-ascii title
         # and the unicode flag set
         self.root.manage_addProduct['Formulator'].manage_add(
-            'form2', 'Test Form b\xef\xbf\xbdr', unicode_mode=1)
+            'form2', b'Test Form b\xef\xbf\xbdr', unicode_mode=1)
         form2 = self.root.form2
-        self.assertEquals(1, form2.get_unicode_mode())
-        self.assertEquals(type(u' '), type(form2.title))
-        self.assertEquals(u'Test Form b\ufffdr', form2.title)
+        self.assertEqual(1, form2.get_unicode_mode())
+        self.assertEqual(type(u' '), type(form2.title))
+        self.assertEqual(u'Test Form b\ufffdr', form2.title)
 
     def test_add_unicode_field(self):
         # test bugfix when adding a field with a non-ascii title
         # to a form with the unicode flag set
         self.root.manage_addProduct['Formulator'].manage_add(
             'form2', 'Test Form b\xef\xbf\xbdr', unicode_mode=1)
         form2 = self.root.form2
-        self.assertEquals(1, form2.get_unicode_mode())
+        self.assertEqual(1, form2.get_unicode_mode())
 
-        form2.manage_addField('testfield', 'Test field b\xef\xbf\xbdr',
+        form2.manage_addField('testfield', b'Test field b\xef\xbf\xbdr',
                               'StringField')
-        self.assertEquals(type(u' '), type(form2.testfield.title()))
-        self.assertEquals(u'Test field b\ufffdr', form2.testfield.title())
-        self.assertEquals(
+        self.assertEqual(type(u' '), type(form2.testfield.title()))
+        self.assertEqual(u'Test field b\ufffdr', form2.testfield.title())
+        self.assertEqual(
             u'Test field b\ufffdr',
             form2.testfield.get_value('title'))
```

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/tests/test_pattern_checker.py` & `Products.Formulator-2.1/src/Products/Formulator/tests/test_pattern_checker.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,20 +10,18 @@
 
 class PatternCheckerTest(unittest.TestCase):
 
     def setUp(self):
         self.val = PatternChecker()
 
     def assertValueMatches(self, patterns, value):
-        self.assertEquals(value,
-                          self.val.validate_value(patterns, value))
+        self.assertEqual(value, self.val.validate_value(patterns, value))
 
     def assertValueChanged(self, patterns, value, result):
-        self.assertEquals(result,
-                          self.val.validate_value(patterns, value))
+        self.assertEqual(result, self.val.validate_value(patterns, value))
 
     def test_some_patterns(self):
         vOk = self.assertValueMatches
         mOk = self.assertValueChanged
 
         # American long ZIP
         vOk(['ddddd-dddd'], '34567-1298')
```

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/tests/test_serialize.py` & `Products.Formulator-2.1/src/Products/Formulator/tests/test_serialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2013  Infrae. All rights reserved.
 # See also LICENSE.txt
 
 import re
 import unittest
 
+import six
+
 from DateTime import DateTime
 
 from Products.Formulator.Errors import FormValidationError
 from Products.Formulator.Errors import ValidationError
 from Products.Formulator.Form import ZMIForm
 from Products.Formulator.FormToXML import formToXML
 from Products.Formulator.MethodField import Method
@@ -117,54 +119,54 @@
         </tales>
       </field>
       </fields>
     </group>
   </groups>
 </form>'''  # noqa: E501 line too long
         XMLToForm(xml, form)
-        s = formToXML(form)
+        b = formToXML(form)
         f = open('output1.txt', 'w')
-        f.write(s)
+        f.write(b)
         f.close()
         form2 = ZMIForm('another', 'Something')
         XMLToForm(xml, form2)
         f = open('output2.txt', 'w')
         f.write(formToXML(form2))
         f.close()
 
     def assertEqualForms(self, form1, form2):
         """ test that the two forms are equal (except for their ids) """
         # in case of failures the messages could be nicer ...
 
-        self.assertEquals(map(lambda x: x.getId(), form1.get_fields()),
-                          map(lambda x: x.getId(), form2.get_fields()))
+        self.assertEqual([x.getId() for x in form1.get_fields()],
+                         [x.getId() for x in form2.get_fields()])
         for field in form1.get_fields():
-            self.assert_(form2.has_field(field.getId()))
+            self.assertTrue(form2.has_field(field.getId()))
             field2 = getattr(form2, field.getId())
             # test if values are the same
-            self.assertEquals(field.values, field2.values)
+            self.assertEqual(field.values, field2.values)
             # test if default renderings are the same
-            self.assertEquals(field.render(), field2.render())
+            self.assertEqual(field.render(), field2.render())
 
-        self.assertEquals(form1.title, form2.title)
-        # self.assertEquals(form1.row_lenght, form2.row_lenght) # not
+        self.assertEqual(form1.title, form2.title)
+        # self.assertEqual(form1.row_lenght, form2.row_lenght) # not
         # initialized ?
-        self.assertEquals(form1.name, form2.name)
-        self.assertEquals(form1.action, form2.action)
-        self.assertEquals(form1.method, form2.method)
-        self.assertEquals(form1.enctype, form2.enctype)
-        self.assertEquals(form1.encoding, form2.encoding)
-        self.assertEquals(form1.stored_encoding, form2.stored_encoding)
-        self.assertEquals(form1.unicode_mode, form2.unicode_mode)
-        self.assertEquals(form1.i18n_domain, form2.i18n_domain)
+        self.assertEqual(form1.name, form2.name)
+        self.assertEqual(form1.action, form2.action)
+        self.assertEqual(form1.method, form2.method)
+        self.assertEqual(form1.enctype, form2.enctype)
+        self.assertEqual(form1.encoding, form2.encoding)
+        self.assertEqual(form1.stored_encoding, form2.stored_encoding)
+        self.assertEqual(form1.unicode_mode, form2.unicode_mode)
+        self.assertEqual(form1.i18n_domain, form2.i18n_domain)
 
-        self.assertEquals(form1.get_groups(), form2.get_groups())
+        self.assertEqual(form1.get_groups(), form2.get_groups())
 
         # if we have forgotten something, this will usually remind us ;-)
-        self.assertEquals(form1.render(), form2.render())
+        self.assertEqual(form1.render(), form2.render())
 
     def test_escaping(self):
         """ test if the necessary elements are escaped in the XML.
         (Actually this test is very incomplete)
         """
         form = ZMIForm('test', '<EncodingTest>')
         # XXX don't test escaping of name, as needs to be javascript
@@ -209,25 +211,25 @@
         # print xml
 
         request = TestRequest(form={'field_int_field': 'not a number'})
         try:
             form.validate_all(request)
             self.fail('form should fail in validation')
         except FormValidationError as e:
-            self.assertEquals(1, len(e.errors))
+            self.assertEqual(1, len(e.errors))
             text1 = e.errors[0].error_text
 
         try:
             form2.validate_all(request)
             self.fail('form2 should fail in validation')
         except FormValidationError as e:
-            self.assertEquals(1, len(e.errors))
+            self.assertEqual(1, len(e.errors))
             text2 = e.errors[0].error_text
 
-        self.assertEquals(unicode(text1), unicode(text2))
+        self.assertEqual(six.text_type(text1), six.text_type(text2))
 
     def test_fieldValueTypes(self):
         """ test checking if the field values are of the proper type.
         after reading from XML some field values may not have the right type,
         if they have a special type (only for "int" and "list" yet).
         Also tests if rendering and validation are the same
         between the original form and the one after one form -> xml -> form
@@ -347,21 +349,21 @@
 
         try:
             result2 = form2.validate_all(request)
         except FormValidationError as e:
             # XXX only render first error ...
             self.fail('error when editing form1, field %s; error message: %s' %
                       (e.errors[0].field_id, e.errors[0].error_text))
-        self.assertEquals(result1, result2)
-        self.assertEquals(42, result2['int_field'])
-        self.assertEquals(2.71828, result2['float_field'])
+        self.assertEqual(result1, result2)
+        self.assertEqual(42, result2['int_field'])
+        self.assertEqual(2.71828, result2['float_field'])
 
         # check link field timeout value
-        self.assertEquals(link_field.get_value('check_timeout'),
-                          form2.link_field.get_value('check_timeout'))
+        self.assertEqual(link_field.get_value('check_timeout'),
+                         form2.link_field.get_value('check_timeout'))
 
         # XXX not tested: equal form validation failure on invalid input
 
     def test_emptyGroup(self):
         """ test bugfix: empty groups are allowed in the XMLForm """
         form = ZMIForm('test', 'GroupTest')
         form.add_group('empty')
@@ -380,40 +382,44 @@
 
         self.root.manage_addDTMLMethod('test_dtml', 'Test DTML', 'ok')
 
         form.manage_addField('string_field', '<string> Field', 'StringField')
         form.string_field.values['external_validator'] = Method('test_dtml')
 
         # test that the override works:
-        self.assertEquals('ok',
-                          form.string_field.get_value('external_validator')())
+        self.assertEqual('ok',
+                         form.string_field.get_value('external_validator')())
 
         # now serialize it:
         xml = formToXML(form)
 
         # get the external validator from the output
         # XXX this could be more elegant, I guess ...
-        for line in xml.split('\n'):
+        if six.PY2:
+            xml_decoded = xml.decode('utf-8')
+        else:
+            xml_decoded = xml
+        for line in xml_decoded.split('\n'):
             m = re.match(
                 r'\s*<external_validator type="method">(.*?)'
                 r'</external_validator>\s*',
                 line)
             if m:
                 break
         else:
             self.fail('external_validator not found in xml')
-        self.assertEquals('test_dtml', m.group(1))
+        self.assertEqual('test_dtml', m.group(1))
 
         # deserialize it
         self.root.manage_addProduct['Formulator'] \
             .manage_add('form2', 'Test Form')
         form2 = self.root.form2
         XMLToForm(xml, form2)
-        self.assertEquals('ok',
-                          form2.string_field.get_value('external_validator')())
+        self.assertEqual('ok',
+                         form2.string_field.get_value('external_validator')())
 
     def test_serializeDateTimeValues(self):
         form = ZMIForm('test', 'DateTime')
 
         form.manage_addField('date_field', 'Date Field', 'DateTimeField')
         form.date_field.values['start_datetime'] = DateTime(
             '2004/01/01 12:01:00')
```

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/tests/test_validators.py` & `Products.Formulator-2.1/src/Products/Formulator/tests/test_validators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2013  Infrae. All rights reserved.
 # See also LICENSE.txt
 
 import unittest
 
+import six
+from six.moves import range
+
 from AccessControl.tainted import TaintedString
 from DateTime import DateTime
 
 from Products.Formulator import Validator
 from Products.Formulator.StandardFields import DateTimeField
 from Products.Formulator.testing import FunctionalLayer
 
@@ -75,16 +78,16 @@
     def test_htmlquotes(self):
         result = self.v.validate(
             TestField('f', max_length=0, truncate=0, required=0, unicode=0),
             'f', {'f': '<html>'})
         self.assertEqual('<html>', result)
 
     def test_encoding(self):
-        utf8_string = 'M\303\274ller'  # this is a M&uuml;ller
-        unicode_string = unicode(utf8_string, 'utf-8')
+        utf8_string = b'M\303\274ller'  # this is a M&uuml;ller
+        unicode_string = six.text_type(utf8_string, 'utf-8')
         result = self.v.validate(
             TestField('f', max_length=0, truncate=0, required=0, unicode=1),
             'f', {'f': utf8_string})
         self.assertEqual(unicode_string, result)
 
     def test_strip_whitespace(self):
         result = self.v.validate(
@@ -155,46 +158,46 @@
         self.assertEqual('<foo>', result)
 
     def test_serializeValue(self):
         handler = FakeSaxHandler()
         string = 'This is the string value'
         field = TestField('f', max_length=0, truncate=0, required=0, unicode=1)
         self.v.serializeValue(field, string, handler)
-        self.assertEquals('This is the string value', handler.getXml())
+        self.assertEqual('This is the string value', handler.getXml())
 
     def test_deserializeValue(self):
         field = TestField('f', max_length=0, truncate=0, required=0, unicode=1)
-        self.assertEquals(
+        self.assertEqual(
             'This is the string value',
             self.v.deserializeValue(field, 'This is the string value'))
 
     def test_serializeNonStringValues(self):
         not_a_string = 0
         handler = FakeSaxHandler()
         field = TestField('f', max_length=0, truncate=0, required=0, unicode=1)
         self.v.serializeValue(field, not_a_string, handler)
-        self.assertEquals('0', handler.getXml())
+        self.assertEqual('0', handler.getXml())
 
 
 class LinesValidatorTestVase(ValidatorTestCase):
 
     def setUp(self):
         self.v = Validator.LinesValidatorInstance
 
     def test_whitespace_preserve(self):
         result = self.v.validate(
             TestField('f', max_length=0, truncate=0, required=1, unicode=0),
             'f', {'f': 'Two Lines \n of Text'})
-        self.assertEquals(['Two Lines', 'of Text'], result)
+        self.assertEqual(['Two Lines', 'of Text'], result)
         # without stripping whitespace
         result = self.v.validate(
             TestField('f', max_lenght=0, whitespace_preserve=1,
                       truncate=0, required=1, unicode=0),
             'f', {'f': 'Two Lines \n of Text'})
-        self.assertEquals(['Two Lines ', ' of Text'], result)
+        self.assertEqual(['Two Lines ', ' of Text'], result)
 
     def test_maxlength(self):
         # currently the validator checks the max lenght before
         # stripping whitespace from each line (and includes the
         # linebreaks)
         self.assertValidatorRaises(
             Validator.ValidationError, 'too_long',
@@ -239,15 +242,15 @@
         field = TestField(
             'f',
             max_length=0,
             truncate=0,
             whitespace_preserve=1,
             required=0,
             unicode=1)
-        self.assertEquals(
+        self.assertEqual(
             ['Two Lines ', ' of Text'],
             self.v.deserializeValue(field, string))
 
 
 class SelectionValidatorTestCase(ValidatorTestCase):
 
     def setUp(self):
@@ -255,106 +258,106 @@
 
     def test_items(self):
         result = self.v.validate(
             TestField(
                 'f', required=1, unicode=True, items=[
                     ('Some A here', 'a'), ('Some B then', 'b')]),
             'f', {'f': 'b'})
-        self.assertEquals('b', result)
+        self.assertEqual('b', result)
         # With single items
         result = self.v.validate(
             TestField('f', required=1, unicode=True, items=[('ab', 'bb')]),
             'f', {'f': 'bb'})
-        self.assertEquals('bb', result)
+        self.assertEqual('bb', result)
         # Empty
         result = self.v.validate(
             TestField(
                 'f', required=0, unicode=True, items=[
                     ('Some A here', 'a'), ('Some B then', 'b')]),
             'f', {})
-        self.assertEquals(u'', result)
+        self.assertEqual(u'', result)
 
     def test_integer_items(self):
         result = self.v.validate(
             TestField(
                 'f', required=1, unicode=True, items=[
                     ('Un', 1), ('Deux', 2)]),
             'f', {'f': '1'})
-        self.assertEquals(1, result)
+        self.assertEqual(1, result)
 
     def test_unicode_items(self):
         result = self.v.validate(
             TestField(
                 'f', required=1, unicode=True, items=[
                     (u'Some \xc3\x84 here', u'\xe4'), (u'Some B then', u'b')]),
-            'f', {'f': '\xc3\xa4'})
-        self.assertEquals(u'\xe4', result)
+            'f', {'f': b'\xc3\xa4'})
+        self.assertEqual(u'\xe4', result)
 
     def test_invalid_items(self):
         with self.assertRaises(Validator.ValidationError) as error:
             self.v.validate(
                 TestField(
                     'f', required=1, unicode=True, items=[
                         ('Some A here', 'a'), ('Some B then', 'b')]),
                 'f', {'f': 'c'})
-        self.assertEquals('unknown_selection', error.exception.error_key)
+        self.assertEqual('unknown_selection', error.exception.error_key)
 
 
 class MultiSelectionValidatorTestCase(ValidatorTestCase):
 
     def setUp(self):
         self.v = Validator.MultiSelectionValidatorInstance
 
     def test_items(self):
         result = self.v.validate(
             TestField(
                 'f', required=1, unicode=True, items=[
                     ('Some A here', 'a'), ('Some B then', 'b')]),
             'f', {'f': 'b'})
-        self.assertEquals(['b'], result)
+        self.assertEqual(['b'], result)
         # Empty
         result = self.v.validate(
             TestField(
                 'f', required=0, unicode=True, items=[
                     ('Some A here', 'a'), ('Some B then', 'b')]),
             'f', {})
-        self.assertEquals([], result)
+        self.assertEqual([], result)
 
     def test_unicode_items(self):
         result = self.v.validate(
             TestField(
                 'f', required=1, unicode=True, items=[
                     (u'Some \xc3\x84 here', u'\xe4'), (u'Some B then', u'b')]),
-            'f', {'f': '\xc3\xa4'})
-        self.assertEquals([u'\xe4'], result)
+            'f', {'f': b'\xc3\xa4'})
+        self.assertEqual([u'\xe4'], result)
 
     def test_invalid_items(self):
         with self.assertRaises(Validator.ValidationError) as error:
             self.v.validate(
                 TestField(
                     'f', required=1, unicode=True, items=[
                         ('Some A here', 'a'), ('Some B then', 'b')]),
                 'f', {'f': ['a', 'c']})
-        self.assertEquals('unknown_selection', error.exception.error_key)
+        self.assertEqual('unknown_selection', error.exception.error_key)
 
 
 class EmailValidatorTestCase(ValidatorTestCase):
 
     def setUp(self):
         self.v = Validator.EmailValidatorInstance
 
     def test_basic(self):
         result = self.v.validate(
             TestField('f', max_length=0, truncate=0, required=1, unicode=0),
             'f', {'f': 'foo@bar.com'})
-        self.assertEquals('foo@bar.com', result)
+        self.assertEqual('foo@bar.com', result)
         result = self.v.validate(
             TestField('f', max_length=0, truncate=0, required=1, unicode=0),
             'f', {'f': 'm.faassen@vet.uu.nl'})
-        self.assertEquals('m.faassen@vet.uu.nl', result)
+        self.assertEqual('m.faassen@vet.uu.nl', result)
 
     def test_error_not_email(self):
         # a few wrong email addresses should raise error
         self.assertValidatorRaises(
             Validator.ValidationError, 'not_email',
             self.v.validate,
             TestField('f', max_length=0, truncate=0, required=1, unicode=0),
@@ -378,15 +381,15 @@
         string = 'eric@infrae.com'
         field = TestField('f', max_length=0, truncate=0, required=0, unicode=1)
         self.v.serializeValue(field, string, handler)
         self.assertEqual('eric@infrae.com', handler.getXml())
 
     def test_deserializeValue(self):
         field = TestField('f', max_length=0, truncate=0, required=0, unicode=1)
-        self.assertEquals(
+        self.assertEqual(
             'eric@infrae.com',
             self.v.deserializeValue(field, 'eric@infrae.com'))
 
 
 class PatternValidatorTestCase(ValidatorTestCase):
 
     def setUp(self):
@@ -398,101 +401,101 @@
         pattern = 'f-f'
         value = 'd-1'
 
         field = \
             TestField('f', max_length=0, truncate=0, required=1, unicode=0,
                       pattern=pattern)
         result = self.v.validate(field, 'f', {'f': value})
-        self.assertEquals(value, result)
+        self.assertEqual(value, result)
 
 
 class BooleanValidatorTestCase(ValidatorTestCase):
 
     def setUp(self):
         self.v = Validator.BooleanValidatorInstance
 
     def test_basic(self):
         result = self.v.validate(
             TestField('f'),
             'f', {'f': ''})
-        self.assertEquals(0, result)
+        self.assertEqual(0, result)
         result = self.v.validate(
             TestField('f'),
             'f', {'f': 1})
-        self.assertEquals(1, result)
+        self.assertEqual(1, result)
         result = self.v.validate(
             TestField('f'),
             'f', {'f': 0})
-        self.assertEquals(0, result)
+        self.assertEqual(0, result)
         result = self.v.validate(
             TestField('f'),
             'f', {})
-        self.assertEquals(0, result)
+        self.assertEqual(0, result)
 
     def test_serializeValue(self):
         handler = FakeSaxHandler()
         value = False
         field = TestField('f', max_length=0, truncate=0, required=0, unicode=1)
         self.v.serializeValue(field, value, handler)
         self.assertEqual('False', handler.getXml())
         handler2 = FakeSaxHandler()
         value = True
         self.v.serializeValue(field, value, handler2)
         self.assertEqual('True', handler2.getXml())
 
     def test_deserializeValue(self):
         field = TestField('f', max_length=0, truncate=0, required=0, unicode=1)
-        self.assertEquals(
+        self.assertEqual(
             False,
             self.v.deserializeValue(field, 'False'))
-        self.assertEquals(
+        self.assertEqual(
             True,
             self.v.deserializeValue(field, 'True'))
 
 
 class IntegerValidatorTestCase(ValidatorTestCase):
     def setUp(self):
         self.v = Validator.IntegerValidatorInstance
 
     def test_basic(self):
         result = self.v.validate(
             TestField('f', max_length=0, truncate=0,
                       required=0, start="", end=""),
             'f', {'f': '15'})
-        self.assertEquals(15, result)
+        self.assertEqual(15, result)
 
         result = self.v.validate(
             TestField('f', max_length=0, truncate=0,
                       required=0, start="", end=""),
             'f', {'f': '0'})
-        self.assertEquals(0, result)
+        self.assertEqual(0, result)
 
         result = self.v.validate(
             TestField('f', max_length=0, truncate=0,
                       required=0, start="", end=""),
             'f', {'f': '-1'})
-        self.assertEquals(-1, result)
+        self.assertEqual(-1, result)
 
     def test_no_entry(self):
         # result should be empty string if nothing entered
         result = self.v.validate(
             TestField('f', max_length=0, truncate=0,
                       required=0, start="", end=""),
             'f', {'f': ''})
-        self.assertEquals("", result)
+        self.assertEqual("", result)
 
     def test_ranges(self):
         # first check whether everything that should be in range is
         # in range
         for i in range(0, 100):
             result = self.v.validate(
                 TestField('f', max_length=0, truncate=0, required=1,
                           start=0, end=100),
                 'f', {'f': str(i)})
-            self.assertEquals(i, result)
+            self.assertEqual(i, result)
         # now check out of range errors
         self.assertValidatorRaises(
             Validator.ValidationError, 'integer_out_of_range',
             self.v.validate,
             TestField('f', max_length=0, truncate=0, required=1,
                       start=0, end=100),
             'f', {'f': '100'})
@@ -585,15 +588,15 @@
             'f',
             max_length=0,
             truncate=0,
             required=0,
             unicode=1,
             start=0,
             end=2000)
-        self.assertEquals(
+        self.assertEqual(
             1337,
             self.v.deserializeValue(field, '1337'))
 
 
 class FloatValidatorTestCase(ValidatorTestCase):
     def setUp(self):
         self.v = Validator.FloatValidatorInstance
@@ -637,15 +640,15 @@
             'f',
             max_length=0,
             truncate=0,
             required=0,
             unicode=1,
             start=0,
             end=2000)
-        self.assertEquals(
+        self.assertEqual(
             1.00001,
             self.v.deserializeValue(field, string))
 
 
 class DateTimeValidatorTestCase(ValidatorTestCase):
     def setUp(self):
         self.v = Validator.DateTimeValidatorInstance
@@ -654,48 +657,48 @@
         result = self.v.validate(
             DateTimeField('f'),
             'f', {'subfield_f_year': '2002',
                   'subfield_f_month': '12',
                   'subfield_f_day': '1',
                   'subfield_f_hour': '10',
                   'subfield_f_minute': '30'})
-        self.assertEquals(2002, result.year())
-        self.assertEquals(12, result.month())
-        self.assertEquals(1, result.day())
-        self.assertEquals(10, result.hour())
-        self.assertEquals(30, result.minute())
+        self.assertEqual(2002, result.year())
+        self.assertEqual(12, result.month())
+        self.assertEqual(1, result.day())
+        self.assertEqual(10, result.hour())
+        self.assertEqual(30, result.minute())
 
     def test_ampm(self):
         result = self.v.validate(
             DateTimeField('f', ampm_time_style=1),
             'f', {'subfield_f_year': '2002',
                   'subfield_f_month': '12',
                   'subfield_f_day': '1',
                   'subfield_f_hour': '10',
                   'subfield_f_minute': '30',
                   'subfield_f_ampm': 'am'})
-        self.assertEquals(2002, result.year())
-        self.assertEquals(12, result.month())
-        self.assertEquals(1, result.day())
-        self.assertEquals(10, result.hour())
-        self.assertEquals(30, result.minute())
+        self.assertEqual(2002, result.year())
+        self.assertEqual(12, result.month())
+        self.assertEqual(1, result.day())
+        self.assertEqual(10, result.hour())
+        self.assertEqual(30, result.minute())
 
         result = self.v.validate(
             DateTimeField('f', ampm_time_style=1),
             'f', {'subfield_f_year': '2002',
                   'subfield_f_month': '12',
                   'subfield_f_day': '1',
                   'subfield_f_hour': '10',
                   'subfield_f_minute': '30',
                   'subfield_f_ampm': 'pm'})
-        self.assertEquals(2002, result.year())
-        self.assertEquals(12, result.month())
-        self.assertEquals(1, result.day())
-        self.assertEquals(22, result.hour())
-        self.assertEquals(30, result.minute())
+        self.assertEqual(2002, result.year())
+        self.assertEqual(12, result.month())
+        self.assertEqual(1, result.day())
+        self.assertEqual(22, result.hour())
+        self.assertEqual(30, result.minute())
 
         self.assertValidatorRaises(
             Validator.ValidationError, 'not_datetime',
             self.v.validate,
             DateTimeField('f', ampm_time_style=1),
             'f', {'subfield_f_year': '2002',
                   'subfield_f_month': '12',
@@ -705,62 +708,62 @@
 
     def test_date_only(self):
         result = self.v.validate(
             DateTimeField('f', date_only=1),
             'f', {'subfield_f_year': '2002',
                   'subfield_f_month': '12',
                   'subfield_f_day': '1'})
-        self.assertEquals(2002, result.year())
-        self.assertEquals(12, result.month())
-        self.assertEquals(1, result.day())
-        self.assertEquals(0, result.hour())
-        self.assertEquals(0, result.minute())
+        self.assertEqual(2002, result.year())
+        self.assertEqual(12, result.month())
+        self.assertEqual(1, result.day())
+        self.assertEqual(0, result.hour())
+        self.assertEqual(0, result.minute())
 
         result = self.v.validate(
             DateTimeField('f', date_only=1),
             'f', {'subfield_f_year': '2002',
                   'subfield_f_month': '12',
                   'subfield_f_day': '1',
                   'subfield_f_hour': '10',
                   'subfield_f_minute': '30'})
-        self.assertEquals(2002, result.year())
-        self.assertEquals(12, result.month())
-        self.assertEquals(1, result.day())
-        self.assertEquals(0, result.hour())
-        self.assertEquals(0, result.minute())
+        self.assertEqual(2002, result.year())
+        self.assertEqual(12, result.month())
+        self.assertEqual(1, result.day())
+        self.assertEqual(0, result.hour())
+        self.assertEqual(0, result.minute())
 
     def test_allow_empty_time(self):
         result = self.v.validate(
             DateTimeField('f', allow_empty_time=1),
             'f', {'subfield_f_year': '2002',
                   'subfield_f_month': '12',
                   'subfield_f_day': '1'})
-        self.assertEquals(2002, result.year())
-        self.assertEquals(12, result.month())
-        self.assertEquals(1, result.day())
-        self.assertEquals(0, result.hour())
-        self.assertEquals(0, result.minute())
+        self.assertEqual(2002, result.year())
+        self.assertEqual(12, result.month())
+        self.assertEqual(1, result.day())
+        self.assertEqual(0, result.hour())
+        self.assertEqual(0, result.minute())
 
         result = self.v.validate(
             DateTimeField('f', allow_empty_time=1),
             'f', {'subfield_f_year': '2002',
                   'subfield_f_month': '12',
                   'subfield_f_day': '1',
                   'subfield_f_hour': '10',
                   'subfield_f_minute': '30'})
-        self.assertEquals(2002, result.year())
-        self.assertEquals(12, result.month())
-        self.assertEquals(1, result.day())
-        self.assertEquals(10, result.hour())
-        self.assertEquals(30, result.minute())
+        self.assertEqual(2002, result.year())
+        self.assertEqual(12, result.month())
+        self.assertEqual(1, result.day())
+        self.assertEqual(10, result.hour())
+        self.assertEqual(30, result.minute())
 
     def test_allow_empty_time2(self):
         result = self.v.validate(
             DateTimeField('f', allow_empty_time=1, required=0), 'f', {})
-        self.assertEquals(None, result)
+        self.assertEqual(None, result)
 
     def test_date_failure(self):
         self.assertValidatorRaises(
             Validator.ValidationError, 'not_datetime',
             self.v.validate,
             DateTimeField('f'),
             'f', {'subfield_f_year': '2002',
@@ -792,10 +795,10 @@
         field = DateTimeField('f')
         self.v.serializeValue(field, value, handler)
         self.assertEqual('2002-12-01T09:30:00Z', handler.getXml())
 
     def test_deserializeValue(self):
         string = '2004-04-23T16:13:40Z'
         field = TestField('f', max_length=0, truncate=0, required=0, unicode=1)
-        self.assertEquals(
+        self.assertEqual(
             DateTime('2004-04-23T16:13:40Z'),
             self.v.deserializeValue(field, string))
```

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/tests/test_widgets.py` & `Products.Formulator-2.1/src/Products/Formulator/tests/test_widgets.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,17 +43,17 @@
     def test_string_escape_html(self):
         """Create a regular TextField and render an unicode value
         containing HTML entities.
         """
         self.root.form.manage_addField('text_field', 'Name', 'StringField')
         self.assertEqual(
             self.root.form.text_field.render(
-                value=u"<élèves />"),
+                value=u'<élève"s />'),
             u'<div><input id="field-text-field" name="field_text_field"'
-            u' size="20" type="text" value="&lt;élèves /&gt;" /></div>')
+            u' size="20" type="text" value="&lt;élève&quot;s /&gt;" /></div>')
         self.assertEqual(
             self.root.form.text_field.render_view(value=u"<élèves />"),
             u'&lt;élèves /&gt;')
 
     def test_string_unicode(self):
         """Create a regular TextField and render an unicode value.
         """
@@ -70,14 +70,15 @@
     def test_textarea_escape_html(self):
         """Create a regular TextAreaField and render an unicode value
         containing HTML entities.
         """
         self.root.form.manage_addField('life_field', 'Life', 'TextAreaField')
         self.assertEqual(
             self.root.form.life_field.render(
-                value=u"<b>élèves</b>"),
+                value=u'<b>élèv"es"</b>'),
             u'<div><textarea cols="40" id="field-life-field"'
-            u' name="field_life_field" rows="5">&lt;b&gt;élèves&lt;/b&gt;'
+            u' name="field_life_field" rows="5">'
+            u'&lt;b&gt;élèv&quot;es&quot;&lt;/b&gt;'
             u'</textarea></div>')
         self.assertEqual(
             self.root.form.life_field.render_view(value=u"<b>élèves</b>"),
             u'&lt;b&gt;élèves&lt;/b&gt;')
```

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/tests/test_zeam.py` & `Products.Formulator-2.1/src/Products/Formulator/tests/test_zeam.py`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/www/BasicField.gif` & `Products.Formulator-2.1/src/Products/Formulator/www/BasicField.gif`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/www/CheckBoxField.gif` & `Products.Formulator-2.1/src/Products/Formulator/www/CheckBoxField.gif`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/www/DateTimeField.gif` & `Products.Formulator-2.1/src/Products/Formulator/www/DateTimeField.gif`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/www/EmailField.gif` & `Products.Formulator-2.1/src/Products/Formulator/www/EmailField.gif`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/www/FileField.gif` & `Products.Formulator-2.1/src/Products/Formulator/www/FileField.gif`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/www/FloatField.gif` & `Products.Formulator-2.1/src/Products/Formulator/www/FloatField.gif`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/www/Form.gif` & `Products.Formulator-2.1/src/Products/Formulator/www/Form.gif`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/www/IntegerField.gif` & `Products.Formulator-2.1/src/Products/Formulator/www/IntegerField.gif`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/www/LabelField.gif` & `Products.Formulator-2.1/src/Products/Formulator/www/LabelField.gif`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/www/LinesField.gif` & `Products.Formulator-2.1/src/Products/Formulator/www/LinesField.gif`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/www/LinkField.gif` & `Products.Formulator-2.1/src/Products/Formulator/www/LinkField.gif`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/www/ListField.gif` & `Products.Formulator-2.1/src/Products/Formulator/www/ListField.gif`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/www/MethodField.gif` & `Products.Formulator-2.1/src/Products/Formulator/www/MethodField.gif`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/www/MultiCheckBoxField.gif` & `Products.Formulator-2.1/src/Products/Formulator/www/MultiCheckBoxField.gif`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/www/MultipleListField.gif` & `Products.Formulator-2.1/src/Products/Formulator/www/MultipleListField.gif`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/www/PasswordField.gif` & `Products.Formulator-2.1/src/Products/Formulator/www/PasswordField.gif`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/www/PatternField.gif` & `Products.Formulator-2.1/src/Products/Formulator/www/PatternField.gif`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/www/RangedIntegerField.gif` & `Products.Formulator-2.1/src/Products/Formulator/www/RangedIntegerField.gif`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/www/StringField.gif` & `Products.Formulator-2.1/src/Products/Formulator/www/StringField.gif`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/www/TextAreaField.gif` & `Products.Formulator-2.1/src/Products/Formulator/www/TextAreaField.gif`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/src/Products/Formulator/zeamsupport.py` & `Products.Formulator-2.1/src/Products/Formulator/zeamsupport.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) 2013  Infrae. All rights reserved.
 # See also LICENSE.txt
 
 
+import six
+
 import grokcore.component as grok
 from zeam.form.base import NO_VALUE
 from zeam.form.base import Error
 from zeam.form.base import Field
 from zeam.form.base import interfaces
 from zeam.form.base.markers import getValue
 from zope.interface import Attribute
@@ -19,18 +21,18 @@
 from Products.Formulator.interfaces import IForm
 
 
 def decode(value):
     """Helper to ensure we have unicode everywhere, as Formulator use
     it in an optional fashion.
     """
-    if not isinstance(value, unicode):
-        if isinstance(value, str):
+    if not isinstance(value, six.text_type):
+        if isinstance(value, bytes):
             return value.decode('utf-8')
-        return unicode(value)
+        return six.text_type(value)
     return value
 
 
 class CustomizedField(object):
     """Proxy around a native Formulator field to be able to
     programmatically change values retrieved with get_value.
     """
@@ -56,16 +58,16 @@
         """
 
 
 class IFormulatorWidget(interfaces.IFieldWidget):
     pass
 
 
+@grok.implementer(IFormulatorField)
 class FormulatorField(Field):
-    grok.implements(IFormulatorField)
 
     def __init__(self, field, form):
         self._form = form
         self._field = field
         self._customizations = {}
         required = bool(self._getValue('required', False))
         readonly = bool(self._getValue('readonly', False))
@@ -100,18 +102,18 @@
         return Specification(
             (implementedBy(self.__class__), providedBy(self._field)))
 
     def customize(self, customizations):
         self._customizations.update(customizations)
 
 
+@grok.implementer(IFormulatorWidget)
 class FormulatorWidget(object):
     """Bind a Formulator field to a data.
     """
-    grok.implements(IFormulatorWidget)
     order = 0
     alternateLayout = False
     defaultHtmlAttributes = set([])
     defaultHtmlClass = ['field']
 
     def __init__(self, component, form, request):
         field = component._field.__of__(form.context)
@@ -202,16 +204,16 @@
 grok.global_adapter(
     FormulatorDisplayWidget,
     (IFormulatorField, interfaces.IFormData, Interface),
     interfaces.IWidget,
     name=u"display")
 
 
+@grok.implementer(interfaces.IWidgetExtractor)
 class FormulatorExtractor(grok.MultiAdapter):
-    grok.implements(interfaces.IWidgetExtractor)
     grok.provides(interfaces.IWidgetExtractor)
     grok.adapts(
         IFormulatorField,
         interfaces.IFieldExtractionValueSetting,
         Interface)
 
     def __init__(self, component, form, request):
@@ -227,16 +229,16 @@
         except ValidationError as error:
             return (None, Error(error.error_text, self.identifier))
 
     def extractRaw(self):
         return {}
 
 
+@grok.implementer(interfaces.IFieldFactory)
 class FormulatorFieldFactory(grok.Adapter):
-    grok.implements(interfaces.IFieldFactory)
     grok.context(IForm)
 
     def __init__(self, form):
         self.form = form
 
     def produce(self):
         for field in self.form.get_fields():
```

### Comparing `Products.Formulator-2.0.dev0/src/Products.Formulator.egg-info/PKG-INFO` & `Products.Formulator-2.1/src/Products.Formulator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: Products.Formulator
-Version: 2.0.dev0
+Version: 2.1
 Summary: Form library for Zope 4
 Home-page: https://github.com/infrae/Products.Formulator
 Author: Martijn Faassen and community
 Author-email: info@infrae.com
 License: BSD
 Keywords: form generator zope4
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Zope :: 4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: test
 License-File: LICENSE.txt
 
 Formulator
 ==========
 
@@ -167,16 +173,31 @@
 Also a thank you to those few valiant souls who suffered through the
 bugs of ZFormulator, the previous implementation. Let's hope this
 one's better!
 
 Changes
 =======
 
-2.0 (unreleased)
------------------
+2.1 (2023-07-31)
+----------------
+
+- Port to Python 3, supporting Python 3.7 up to 3.11.
+
+
+2.0.1 (2023-03-28)
+------------------
+
+Bug fixes
++++++++++
+
+- Fix HTML quoting for values containing ``"``.
+
+
+2.0 (2023-03-14)
+----------------
 
 Backwards incompatible changes
 ++++++++++++++++++++++++++++++
 
 - Remove support for Zope 2 help system.
 
 - Stop testing Zope 2 compatibility. This release should still work with Zope 2
@@ -1061,7 +1082,9 @@
   documentation.
 
 0.9 (2001/04/30)
 ----------------
 
 - Initial public release of Formulator.
 
+
+
```

### Comparing `Products.Formulator-2.0.dev0/src/Products.Formulator.egg-info/SOURCES.txt` & `Products.Formulator-2.1/src/Products.Formulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Products.Formulator-2.0.dev0/tox.ini` & `Products.Formulator-2.1/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,48 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/zope-product
 [tox]
 minversion = 3.18
 envlist =
     lint
     py27
+    py37
+    py38
+    py39
+    py310
+    py311
     coverage
 
 [testenv]
 skip_install = true
 setenv =
     TZ = CET
 deps =
-    zc.buildout == 2.13.8
+    zc.buildout > 3
     wheel > 0.37
+    pudb
+    py27: pip==20.3.4
 commands_pre =
-    {envbindir}/buildout -nc {toxinidir}/buildout4.cfg buildout:directory={envdir} buildout:develop={toxinidir} install test
+    {envbindir}/buildout -nc {toxinidir}/buildout.cfg buildout:directory={envdir} buildout:develop={toxinidir} install test
 commands =
     {envbindir}/test {posargs:-cv}
 
+# Only these Pyhton versions are supported by Zope 4, newer ones need Zope 5:
+[testenv:py27]
+commands_pre =
+    {envbindir}/buildout -nc {toxinidir}/buildout4.cfg buildout:directory={envdir} buildout:develop={toxinidir} install test
+[testenv:py37]
+commands_pre =
+    {envbindir}/buildout -nc {toxinidir}/buildout4.cfg buildout:directory={envdir} buildout:develop={toxinidir} install test
+[testenv:py38]
+commands_pre =
+    {envbindir}/buildout -nc {toxinidir}/buildout4.cfg buildout:directory={envdir} buildout:develop={toxinidir} install test
+
 [testenv:lint]
-basepython = python3.7
+basepython = python3.9
 commands_pre =
     mkdir -p {toxinidir}/parts/flake8
 allowlist_externals =
     mkdir
 commands =
     isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
     flake8 {toxinidir}/src {toxinidir}/setup.py
@@ -42,27 +60,27 @@
 commands_pre =
 deps =
     isort
 commands =
     isort {toxinidir}/src {toxinidir}/setup.py []
 
 [testenv:coverage]
-basepython = python2.7
+basepython = python3.9
 skip_install = true
 allowlist_externals =
     mkdir
 deps =
     {[testenv]deps}
     coverage
     coverage-python-version
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run {envbindir}/test {posargs:-cv}
     coverage html
-    coverage report -m --fail-under=76
+    coverage report -m --fail-under=77
 
 [coverage:run]
 branch = True
 plugins = coverage_python_version
 source = Products.Formulator
 
 [coverage:report]
```

