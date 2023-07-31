# Comparing `tmp/django-daiquiri-0.4.2.tar.gz` & `tmp/django-daiquiri-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-daiquiri-0.4.2.tar", last modified: Thu Jul 20 09:24:15 2023, max compression
+gzip compressed data, was "django-daiquiri-0.4.3.tar", last modified: Mon Jul 31 14:32:01 2023, max compression
```

## Comparing `django-daiquiri-0.4.2.tar` & `django-daiquiri-0.4.3.tar`

### file list

```diff
@@ -1,798 +1,799 @@
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.426122 django-daiquiri-0.4.2/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      451 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/AUTHORS
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    11359 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/LICENSE
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)       92 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/MANIFEST.in
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     7407 2023-07-19 07:53:11.000000 django-daiquiri-0.4.2/NOTICE
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6177 2023-07-20 09:24:15.426122 django-daiquiri-0.4.2/PKG-INFO
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5302 2023-07-20 09:22:46.000000 django-daiquiri-0.4.2/README.md
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      249 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/__init__.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.386123 django-daiquiri-0.4.2/daiquiri/auth/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/auth/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1571 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/auth/adapter.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      432 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/admin.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      208 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/apps.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3695 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/auth/forms.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4902 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/handlers.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.386123 django-daiquiri-0.4.2/daiquiri/auth/migrations/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2089 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0001_profile_model.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      486 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0002_profile_attributes.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      526 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0003_view_permission.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      522 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0004_view_permission_typo.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      535 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0005_view_permission_fix.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      581 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0006_profile_ordering.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      459 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0007_profile_is_confirmed.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      625 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0008_profile_is_pending.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      366 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0009_delete_detailkey.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      556 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0010_profile_consent.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      774 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0011_meta.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      448 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0012_django2.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      439 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0013_alter_profile_id.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      567 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/0014_use_django_jsonfield.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/migrations/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2358 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/auth/models.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      367 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/permissions.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2055 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/serializers.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      145 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/settings.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      266 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/auth/signals.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.378123 django-daiquiri-0.4.2/daiquiri/auth/static/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.378123 django-daiquiri-0.4.2/daiquiri/auth/static/auth/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.386123 django-daiquiri-0.4.2/daiquiri/auth/static/auth/css/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/static/auth/css/users.scss
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.386123 django-daiquiri-0.4.2/daiquiri/auth/static/auth/js/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1724 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/static/auth/js/users.js
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.378123 django-daiquiri-0.4.2/daiquiri/auth/templates/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.386123 django-daiquiri-0.4.2/daiquiri/auth/templates/account/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      178 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/account_inactive.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      309 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/account_pending.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1124 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/account_profile.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      588 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/account_token.html
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      308 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/activation_message.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)       55 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/activation_subject.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      392 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/email_confirmation_message.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)       62 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/email_confirmation_subject.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      308 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/notify_activation_message.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)       46 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/notify_activation_subject.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      372 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/notify_confirmation_message.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)       46 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/notify_confirmation_subject.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      247 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/notify_password_changed_message.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)       44 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/notify_password_changed_subject.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      354 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/notify_rejection_message.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)       45 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/notify_rejection_subject.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      556 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/password_reset_key_message.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)       43 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/password_reset_key_subject.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      411 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/request_activation_message.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)       55 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/request_activation_subject.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      407 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/request_confirmation_message.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)       54 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/request_confirmation_subject.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2783 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      975 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/email_confirm.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      224 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/login.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1594 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/login_form.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      546 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/logout.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      383 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/logout_form.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      550 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/password_change.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      254 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/password_change_done.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      532 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/password_reset.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      473 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/password_reset_done.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      853 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/password_reset_from_key.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      341 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/password_reset_from_key_done.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      511 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/password_set.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      247 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/password_set_done.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3164 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/signup.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      201 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/signup_closed.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)       17 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/terms_of_use.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      365 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/verification_sent.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      769 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/account/verified_email_required.html
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/auth/templates/auth/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6370 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1054 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_activate_user.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1050 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_confirm_user.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1050 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_disable_user.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1038 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_enable_user.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1044 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_reject_user.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3020 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_show_user.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3331 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_update_user.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2167 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_options.html
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/auth/templates/socialaccount/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      303 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/socialaccount/authentication_error.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1879 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/socialaccount/connections.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      766 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/socialaccount/login.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      435 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/socialaccount/login_cancelled.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3294 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/socialaccount/signup.html
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/auth/templates/socialaccount/snippets/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      904 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/templates/socialaccount/snippets/provider_list.html
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/auth/tests/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/tests/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6328 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/auth/tests/test_accounts.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2301 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/auth/tests/test_honeypot.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      552 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/auth/tests/test_views.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2728 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/auth/tests/test_viewset_group.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     7451 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/auth/tests/test_viewset_profile.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      968 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/auth/urls_accounts.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      447 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/urls_auth.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2350 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/utils.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      760 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/auth/validators.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3472 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/auth/views.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3114 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/auth/viewsets.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/conesearch/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/conesearch/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5814 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/conesearch/adapter.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      171 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/conesearch/apps.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      270 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/conesearch/permissions.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      354 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/conesearch/renderers.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      273 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/conesearch/settings.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.378123 django-daiquiri-0.4.2/daiquiri/conesearch/templates/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/conesearch/templates/conesearch/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      508 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/conesearch/templates/conesearch/root.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      563 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/conesearch/urls.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      652 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/conesearch/views.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1347 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/conesearch/viewsets.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3198 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/conesearch/vo.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/contact/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/contact/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      314 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/admin.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      158 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/apps.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      476 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/filters.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      815 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/contact/forms.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/contact/migrations/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1441 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/migrations/0001_initial.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      755 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/migrations/0002_meta.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      582 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/migrations/0003_add_permissions.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      584 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/migrations/0004_meta.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      440 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/migrations/0005_django2.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      449 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/migrations/0006_alter_contactmessage_id.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/migrations/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1376 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/contact/models.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      571 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/serializers.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.378123 django-daiquiri-0.4.2/daiquiri/contact/static/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.378123 django-daiquiri-0.4.2/daiquiri/contact/static/contact/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/contact/static/contact/css/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/static/contact/css/messages.scss
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/contact/static/contact/js/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1556 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/static/contact/js/messages.js
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/contact/templates/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.390123 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      959 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/contact.html
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.394122 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/email/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      104 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/email/contact_template.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      407 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/email/new_message_admin_message.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)       48 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/email/new_message_admin_subject.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      326 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/email/new_message_user_message.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)       49 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/email/new_message_user_subject.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5319 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/messages.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      283 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/messages_mailto.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1986 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/messages_modal_show.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1028 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/messages_options.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      247 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/templates/contact/thanks.html
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.394122 django-daiquiri-0.4.2/daiquiri/contact/tests/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/tests/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2336 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/contact/tests/test_views.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3477 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/contact/tests/test_viewset_contact_messages.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1104 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/contact/tests/test_viewset_status.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      541 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/urls.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      822 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/contact/utils.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1546 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/contact/views.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1215 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/contact/viewsets.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.394122 django-daiquiri-0.4.2/daiquiri/core/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/__init__.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.394122 django-daiquiri-0.4.2/daiquiri/core/adapter/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      303 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/adapter/__init__.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.394122 django-daiquiri-0.4.2/daiquiri/core/adapter/database/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/adapter/database/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    12923 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/core/adapter/database/base.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1266 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/adapter/database/mariadb.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     8216 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/adapter/database/mysql.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    12800 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/core/adapter/database/postgres.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.394122 django-daiquiri-0.4.2/daiquiri/core/adapter/download/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/adapter/download/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5237 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/core/adapter/download/base.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1011 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/adapter/download/mysqldump.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1618 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/adapter/download/pgdump.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1100 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/adapter/stream.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      936 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/core/celery.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1707 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/core/constants.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      219 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/encoders.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2584 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/env.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      101 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/exceptions.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    14347 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/core/generators.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1346 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/hashers.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      118 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/http.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.394122 django-daiquiri-0.4.2/daiquiri/core/management/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/management/__init__.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.394122 django-daiquiri-0.4.2/daiquiri/core/management/commands/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      586 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/activate_user.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      244 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/create_admin_user.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      246 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/daiquiri_path.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2417 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/delete_users.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      295 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/deploy.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5286 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/find_users.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      606 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/promote_user.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      679 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/rabbitcreate.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1021 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/runworker.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      434 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/setup_groups.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      223 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/show_databases.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4661 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/sqlcreate.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1718 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/core/management/commands/workers.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1338 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/managers.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      675 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/middleware.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      164 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/paginations.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2058 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/permissions.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.394122 django-daiquiri-0.4.2/daiquiri/core/renderers/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2636 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/renderers/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6120 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/renderers/datacite.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1596 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/renderers/dublincore.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3960 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/renderers/voresource.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6832 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/renderers/vosi.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      118 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/responses.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2007 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/routers.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1158 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/serializers.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.394122 django-daiquiri-0.4.2/daiquiri/core/settings/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/settings/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      805 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/settings/daiquiri.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     7551 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/core/settings/django.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3471 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/settings/logging.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4462 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/settings/vendor.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/core/static/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/core/static/core/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.398122 django-daiquiri-0.4.2/daiquiri/core/static/core/css/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    11581 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/css/base.scss
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1874 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/css/browser.scss
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4889 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/css/codehilite.scss
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      153 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/css/codemirror.scss
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      827 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/css/fonts.scss
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1350 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/css/list.scss
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/css/style.scss
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4551 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/css/table.scss
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1665 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/css/variables.scss
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.398122 django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/
--rwxr-xr-x   0 kmakan    (1002) kmakan    (1003)    42480 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSans-Bold.ttf
--rwxr-xr-x   0 kmakan    (1002) kmakan    (1003)    41028 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSans.ttf
--rwxr-xr-x   0 kmakan    (1002) kmakan    (1003)   117072 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSansMono.ttf
--rwxr-xr-x   0 kmakan    (1002) kmakan    (1003)    48880 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSerif-Bold.ttf
--rwxr-xr-x   0 kmakan    (1002) kmakan    (1003)    45652 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSerif-BoldItalic.ttf
--rwxr-xr-x   0 kmakan    (1002) kmakan    (1003)    40416 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSerif-Italic.ttf
--rwxr-xr-x   0 kmakan    (1002) kmakan    (1003)    43648 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSerif.ttf
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.398122 django-daiquiri-0.4.2/daiquiri/core/static/core/html/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1759 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/browser.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      457 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_checkbox.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      417 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_codemirror.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      421 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_date.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      471 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_file.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1115 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_multicheckbox.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      428 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_number.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      472 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_radio.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      848 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_select.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      862 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_selectnumber.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      444 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_text.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      461 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_textarea.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      486 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_textareasplit.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      383 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/html/order-list.html
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.398122 django-daiquiri-0.4.2/daiquiri/core/static/core/img/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    19025 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/img/daiquiri.jpg
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      380 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/img/daiquiri32.png
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1406 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/img/favicon.ico
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      459 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/img/favicon.png
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.398122 django-daiquiri-0.4.2/daiquiri/core/static/core/js/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     9139 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/js/browser.js
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      653 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/js/byNumber.js
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4597 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/js/core.js
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1435 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/js/filter.js
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      917 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/js/formgroup.js
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2740 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/js/list.js
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1303 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/js/multiCheckbox.js
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1606 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/js/polling.js
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1839 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/js/stream.js
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    14578 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/core/static/core/js/table.js
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      224 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/tasks.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/core/templates/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.398122 django-daiquiri-0.4.2/daiquiri/core/templates/core/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      188 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/400.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      177 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/403.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      185 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/404.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      192 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/500.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      396 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/base.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/base_analytics.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/base_footer.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1024 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/base_head.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1801 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/base_navigation.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      568 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/base_navigation_account.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      208 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/base_navigation_admin.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1391 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/base_navigation_management.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      156 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/home.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      341 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/page.html
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1903 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/form_field.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      189 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/form_fields.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      322 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1390 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table_footer.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      352 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table_header.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2637 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table_modal.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      665 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table_pagination.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5391 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table_pane.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      463 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table_search.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1007 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table_tooltip.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      183 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templates/core/wide.html
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/core/templatetags/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/templatetags/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1495 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/templatetags/core_tags.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/core/tests/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/tests/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1862 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/tests/test_adapter.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      384 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/tests/test_views.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    12749 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/core/utils.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2720 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/views.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2092 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/core/viewsets.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      319 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/core/vo.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/cutout/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/cutout/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      269 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/cutout/adapter.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      154 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/cutout/apps.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      266 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/cutout/permissions.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      350 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/cutout/renderers.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)       88 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/cutout/settings.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      191 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/cutout/urls.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1326 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/cutout/viewsets.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/datalink/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/datalink/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     9541 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/datalink/adapter.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      162 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/apps.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4909 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/constants.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/datalink/management/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/management/__init__.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/datalink/management/commands/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/management/commands/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      579 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/management/commands/rebuild_datalink_table.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/datalink/migrations/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1320 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/migrations/0001_initial.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      426 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/migrations/0002_alter_datalink_content_length.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      450 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/datalink/migrations/0003_alter_datalink_content_length.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/migrations/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1209 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/datalink/models.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1724 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/serializers.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)       91 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/settings.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/datalink/templates/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/datalink/templates/datalink/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1719 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/datalink/templates/datalink/datalink.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      507 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/templates/datalink/root.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      690 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/datalink/urls.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      959 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/utils.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      697 2023-04-27 21:33:15.000000 django-daiquiri-0.4.2/daiquiri/datalink/views.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1728 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/viewsets.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2789 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/datalink/vo.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/files/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      349 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/files/admin.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      371 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/files/apps.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/files/migrations/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1355 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/files/migrations/0001_initial.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      670 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/files/migrations/0002_depth.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      660 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/files/migrations/0003_python3.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      410 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/files/migrations/0004_django2.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      496 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/files/migrations/0005_directory_layout.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      451 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/files/migrations/0006_alter_directory_id.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      473 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/files/migrations/0007_alter_directory_layout.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/files/migrations/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1470 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/models.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5211 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/files/search.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      217 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/settings.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/files/templates/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/files/templates/files/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      194 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/files/templates/files/layout.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1409 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/templates/files/list-results.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      261 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/templates/files/search-input.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      220 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/templates/files/search-results.html
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/files/templatetags/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/templatetags/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      634 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/templatetags/search_highlight.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.402122 django-daiquiri-0.4.2/daiquiri/files/tests/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/files/tests/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1891 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/tests/test_views.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      252 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/urls.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2991 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/utils.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2045 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/files/views.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.406122 django-daiquiri-0.4.2/daiquiri/jobs/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/jobs/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      898 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/jobs/admin.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      146 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/apps.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      101 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/exceptions.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      995 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/filters.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      454 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/managers.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.406122 django-daiquiri-0.4.2/daiquiri/jobs/migrations/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1705 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0001_job_model.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      473 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0002_execution_duration_default_0.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      586 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0003_owner_fk.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      874 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0004_phases_to_char.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      583 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0005_owner_null_true.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      596 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0006_owner_blank_true.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      466 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0007_creation_time.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      476 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0008_job_error_summary.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      505 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0009_meta.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      805 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0010_add_fields.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      465 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0011_job_client_ip.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      539 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0012_meta.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      456 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0013_job_error_summary.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      477 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0014_blank_run_id.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1088 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0015_job_index.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      400 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/0016_django2.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/migrations/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3378 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/jobs/models.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3038 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/renderers.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1041 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/jobs/routers.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2766 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/jobs/serializers.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      919 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/jobs/utils.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    11152 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/jobs/viewsets.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.406122 django-daiquiri-0.4.2/daiquiri/metadata/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1893 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/admin.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      215 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/apps.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3187 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/handlers.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.406122 django-daiquiri-0.4.2/daiquiri/metadata/management/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/management/__init__.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.406122 django-daiquiri-0.4.2/daiquiri/metadata/management/commands/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/management/commands/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      739 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/management/commands/dump_table.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1019 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/management/commands/update_access_level.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.410122 django-daiquiri-0.4.2/daiquiri/metadata/migrations/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4525 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0001_initial.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1073 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0002_published_for.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      877 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0003_groups.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      501 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0004_function_query_string.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3114 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0005_more_fields.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    11136 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0006_meta.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3913 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0007_access_level.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1162 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0008_refactoring.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      430 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0009_arraysize.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      563 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0010_meta.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1672 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0011_directory.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      412 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0012_remove_directory_metadata_access_level.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      499 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0013_remove_directory.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      563 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0014_rename_pid_to_doi.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      740 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0015_change_doi_to_char.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2266 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0016_rename_database_to_schema.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1307 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0017_rename_database_to_schema.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      583 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0018_meta.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      578 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0019_column_index_for.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      594 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0020_blank_index_for.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      513 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0021_table_nrows.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      507 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0022_table_size.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5264 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0023_python3.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1010 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0024_django2.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      974 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0025_add_published_updated.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1060 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0026_add_creators_and_contributors.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1798 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0027_auto_20201202_1625.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2392 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0028_add_related_identifiers.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1089 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0029_alter_ids.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      634 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0030_move_licenses_to_settings.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1059 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0031_change_order.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1714 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0032_data_migration.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     9659 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/0033_refactor_fields.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/migrations/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    12036 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/models.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.410122 django-daiquiri-0.4.2/daiquiri/metadata/serializers/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2218 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/serializers/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5021 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/metadata/serializers/datacite.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1965 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/serializers/dublincore.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2676 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/serializers/export.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      740 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/serializers/management.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2118 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/serializers/user.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1923 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/settings.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/metadata/static/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.410122 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/css/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      694 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/css/metadata.scss
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.410122 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1173 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by.png
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1768 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by_nc.png
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2069 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by_nc_nd.png
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2236 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by_nc_sa.png
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1515 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by_nd.png
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1755 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by_sa.png
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1230 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/cc0.png
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1331 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/nc.png
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1051 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/nd.png
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      985 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/pd.png
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1289 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/sa.png
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.410122 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/js/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     8560 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/js/metadata.js
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/metadata/templates/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.410122 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3508 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2916 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_display.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1484 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_delete_columns.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1492 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_delete_functions.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1717 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_delete_schemas.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1702 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_delete_tables.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     9346 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_columns.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4872 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_functions.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     8059 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_schemas.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1841 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_schemas_attribution.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3754 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_schemas_contributors.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3702 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_schemas_creators.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1866 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_schemas_description.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    10199 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_tables.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1835 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_tables_attribution.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3751 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_tables_contributors.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3699 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_tables_creators.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1860 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_tables_description.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1020 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_options.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1514 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/schema.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2228 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/table.html
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.410122 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/tags/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      442 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/tags/access_panel.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      501 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/tags/doi_panel.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      523 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/tags/license_panel.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      349 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/tags/schemas_menu.html
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.410122 django-daiquiri-0.4.2/daiquiri/metadata/templatetags/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/templatetags/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1710 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/templatetags/metadata_tags.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.410122 django-daiquiri-0.4.2/daiquiri/metadata/tests/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/tests/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      459 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/tests/test_tags.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3579 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/tests/test_views.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3975 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/tests/test_viewset_column.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4329 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/tests/test_viewset_function.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4355 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/tests/test_viewset_schema.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3922 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/tests/test_viewset_table.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1150 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/urls.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      727 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/metadata/utils.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2271 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/views.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     9261 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/metadata/viewsets.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.414122 django-daiquiri-0.4.2/daiquiri/oai/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/oai/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    15252 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/oai/adapter.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      142 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/apps.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.414122 django-daiquiri-0.4.2/daiquiri/oai/management/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/management/__init__.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.414122 django-daiquiri-0.4.2/daiquiri/oai/management/commands/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/management/commands/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2208 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/management/commands/rebuild_oai_schema.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.414122 django-daiquiri-0.4.2/daiquiri/oai/migrations/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1069 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/migrations/0001_initial.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      682 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/migrations/0002_resource_type.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      443 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/migrations/0003_record_set_spec.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      445 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/migrations/0004_alter_record_id.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      439 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/migrations/0005_alter_record_resource_id.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      507 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/migrations/0006_alter_record_resource_id.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/migrations/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1195 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/oai/models.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     7874 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/renderers.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1236 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/settings.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      141 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/urls.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2522 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/utils.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    11305 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/oai/views.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.414122 django-daiquiri-0.4.2/daiquiri/query/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1285 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/admin.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      523 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/apps.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      597 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/filters.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      692 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/handlers.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.414122 django-daiquiri-0.4.2/daiquiri/query/management/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/management/__init__.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.414122 django-daiquiri-0.4.2/daiquiri/query/management/commands/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/management/commands/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2482 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/management/commands/archive_query_jobs.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1915 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/management/commands/fix_query_jobs.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1808 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/management/commands/scrub_query_jobs.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1981 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/management/commands/scrub_user_tables.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      437 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/managers.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.418122 django-daiquiri-0.4.2/daiquiri/query/migrations/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1214 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0001_initial.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      502 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0002_meta.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1025 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0003_query_language_and_actual_query.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1149 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0004_table_name.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      702 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0005_meta.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1155 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0006_example.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      505 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0007_queryjob_metadata.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      463 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0008_queryjob_pid.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      613 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0009_remove_choices.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      476 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0010_queue_can_be_null.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      469 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0011_queryjob_native_query.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      469 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0012_query_language_length.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2222 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0013_refactoring.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1453 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0014_downloadjob.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1611 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0015_queryarchivejob.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      447 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0016_rename_database_to_schema.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      648 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0017_big_integer_fields.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      485 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0018_blank_metadata.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      516 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0019_remove_sync_jobs.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      669 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0020_python3.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1014 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0021_django2.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1277 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0022_blank_fields.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      422 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0023_queryjob_uploads.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      728 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0024_fix_jsonfield.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      446 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0025_alter_example_id.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      779 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0026_use_django_jsonfield.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      525 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/0027_rename_job_to_query_job.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/migrations/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    20749 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/query/models.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      265 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/permissions.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    13390 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/query/process.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6071 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/query/serializers.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3716 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/settings.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/query/static/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/query/static/query/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.418122 django-daiquiri-0.4.2/daiquiri/query/static/query/css/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)       35 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/css/examples.scss
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      214 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/css/jobs.scss
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)       89 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/css/plot.scss
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3784 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/css/query.scss
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/query/static/query/js/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.418122 django-daiquiri-0.4.2/daiquiri/query/static/query/js/apps/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      243 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/apps/examples.js
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      223 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/apps/jobs.js
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2010 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/apps/query.js
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.418122 django-daiquiri-0.4.2/daiquiri/query/static/query/js/downloads/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      634 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/downloads/archive.js
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.418122 django-daiquiri-0.4.2/daiquiri/query/static/query/js/dropdowns/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1207 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/dropdowns/simbad.js
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1893 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/dropdowns/vizier.js
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.418122 django-daiquiri-0.4.2/daiquiri/query/static/query/js/forms/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1254 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/forms/box.js
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1045 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/forms/cone.js
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4545 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/forms/sql.js
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      857 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/forms/upload.js
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.418122 django-daiquiri-0.4.2/daiquiri/query/static/query/js/services/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2970 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/services/download.js
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3109 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/services/examples.js
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3793 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/services/jobs.js
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    27091 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/services/plot.js
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    12546 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/query/static/query/js/services/query.js
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    12660 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/query/tasks.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/query/templates/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.418122 django-daiquiri-0.4.2/daiquiri/query/templates/query/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4903 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/examples.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1475 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/examples_modal_delete.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4918 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/examples_modal_form.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      349 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/examples_options.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6534 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/jobs.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4036 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/jobs_modal_show_job.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5289 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      409 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_download.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      572 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_download_archive.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      806 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_download_table.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      565 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_dropdown_columns.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      602 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_dropdown_examples.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      591 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_dropdown_functions.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      582 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_dropdown_schemas.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2282 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_dropdown_simbad.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2922 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_dropdown_vizier.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      188 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_form.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3657 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_form_box.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2560 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_form_cone.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3128 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_form_sql.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1945 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_form_upload.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1329 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_modal_abort_job.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1339 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_modal_archive_job.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1138 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_modal_logout.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1557 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_modal_update_job.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4684 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_overview.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2241 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_plot.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1478 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_plot_histogram.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4381 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_plot_scatter.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1836 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_plot_scatter_cmap.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)       62 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_results.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5899 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_sidebar.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/templates/query/query_sidebar_status_extra.html
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.418122 django-daiquiri-0.4.2/daiquiri/query/tests/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/query/tests/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2454 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/tests/test_permissions.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1169 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/tests/test_views.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1093 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/tests/test_viewset_download.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1076 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/tests/test_viewset_dropdown.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4394 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/tests/test_viewset_example.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1083 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/tests/test_viewset_form.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    12329 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/tests/test_viewset_job.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1122 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/tests/test_viewset_status.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1216 2022-08-19 10:23:10.000000 django-daiquiri-0.4.2/daiquiri/query/urls.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    10213 2023-04-24 07:48:40.000000 django-daiquiri-0.4.2/daiquiri/query/utils.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3242 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/query/validators.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1127 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/query/views.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    14163 2023-07-20 09:06:08.000000 django-daiquiri-0.4.2/daiquiri/query/viewsets.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/registry/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/registry/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      162 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/registry/apps.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1204 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/registry/serializers.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      135 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/registry/settings.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/registry/templates/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/registry/templates/registry/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1196 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/registry/templates/registry/root.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      551 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/registry/urls.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      956 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/registry/views.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4143 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/registry/vo.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/serve/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/serve/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      159 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/apps.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/serve/migrations/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/migrations/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      448 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/serializers.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)       48 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/settings.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/serve/static/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/serve/static/serve/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/serve/static/serve/css/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      114 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/static/serve/css/table.scss
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/serve/static/serve/js/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      191 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/static/serve/js/table.js
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      736 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/tasks.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/serve/templates/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/serve/templates/serve/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1441 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/templates/serve/table.html
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/serve/tests/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/tests/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2410 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/serve/tests/test_views.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4860 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/serve/tests/test_viewsets.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      609 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/serve/urls.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      218 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/utils.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      719 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/views.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3057 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/serve/viewsets.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/stats/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/stats/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      296 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/admin.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      150 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/apps.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/stats/migrations/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1291 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/migrations/0001_initial.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      927 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/migrations/0002_data_migration.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1050 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/migrations/0003_data_migration.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      603 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/migrations/0004_set_record_null.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      411 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/migrations/0005_django2.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      439 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/migrations/0006_alter_record_id.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      380 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/migrations/0007_use_django_jsonfield.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      461 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/migrations/0008_alter_record_resource.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/migrations/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      717 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/stats/models.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      405 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/settings.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/stats/templates/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/stats/templates/stats/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      730 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/templates/stats/management.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      174 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/urls.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      929 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/stats/views.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/tap/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/tap/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      142 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/apps.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    11624 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/tap/constants.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/tap/management/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/management/__init__.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/tap/management/commands/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/management/commands/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      524 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/management/commands/rebuild_tap_schema.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3212 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/management/commands/setup_tap_metadata.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/tap/migrations/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3204 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/migrations/0001_initial.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      856 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/migrations/0002_alter_ids.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/migrations/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1952 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/models.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1341 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/serializers.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      161 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/settings.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/tap/static/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/tap/static/tap/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/tap/static/tap/css/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)       50 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/static/tap/css/examples.scss
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/tap/templates/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/tap/templates/tap/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      928 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/templates/tap/examples.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      806 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/templates/tap/root.html
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/tap/tests/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/tests/__init__.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    27429 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/tap/tests/test_async.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4970 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/tap/tests/test_sync.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1464 2023-01-30 20:07:21.000000 django-daiquiri-0.4.2/daiquiri/tap/tests/test_views.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      883 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/urls.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5004 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/utils.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1039 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/views.py
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3771 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/tap/vo.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/uws/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/uws/__init__.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.382123 django-daiquiri-0.4.2/daiquiri/uws/templates/
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.422122 django-daiquiri-0.4.2/daiquiri/uws/templates/uws/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      122 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/uws/templates/uws/root.html
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      861 2022-06-16 09:10:03.000000 django-daiquiri-0.4.2/daiquiri/uws/urls.py
-drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-20 09:24:15.426122 django-daiquiri-0.4.2/django_daiquiri.egg-info/
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6177 2023-07-20 09:24:15.000000 django-daiquiri-0.4.2/django_daiquiri.egg-info/PKG-INFO
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)    28901 2023-07-20 09:24:15.000000 django-daiquiri-0.4.2/django_daiquiri.egg-info/SOURCES.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        1 2023-07-20 09:24:15.000000 django-daiquiri-0.4.2/django_daiquiri.egg-info/dependency_links.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      720 2023-07-20 09:24:15.000000 django-daiquiri-0.4.2/django_daiquiri.egg-info/requires.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)        9 2023-07-20 09:24:15.000000 django-daiquiri-0.4.2/django_daiquiri.egg-info/top_level.txt
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)      253 2023-07-20 09:24:15.426122 django-daiquiri-0.4.2/setup.cfg
--rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1376 2023-07-20 09:24:11.000000 django-daiquiri-0.4.2/setup.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.753205 django-daiquiri-0.4.3/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      451 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/AUTHORS
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    11359 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/LICENSE
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       92 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/MANIFEST.in
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     7407 2023-07-19 07:53:11.000000 django-daiquiri-0.4.3/NOTICE
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6177 2023-07-31 14:32:01.753205 django-daiquiri-0.4.3/PKG-INFO
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5302 2023-07-20 09:22:46.000000 django-daiquiri-0.4.3/README.md
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.713206 django-daiquiri-0.4.3/daiquiri/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      249 2023-07-31 14:30:28.000000 django-daiquiri-0.4.3/daiquiri/__init__.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.717206 django-daiquiri-0.4.3/daiquiri/auth/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/auth/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1571 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/auth/adapter.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      432 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/admin.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      208 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/apps.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3695 2023-04-24 07:48:40.000000 django-daiquiri-0.4.3/daiquiri/auth/forms.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4902 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/handlers.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.717206 django-daiquiri-0.4.3/daiquiri/auth/migrations/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2089 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/migrations/0001_profile_model.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      486 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/migrations/0002_profile_attributes.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      526 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/migrations/0003_view_permission.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      522 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/migrations/0004_view_permission_typo.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      535 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/migrations/0005_view_permission_fix.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      581 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/migrations/0006_profile_ordering.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      459 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/migrations/0007_profile_is_confirmed.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      625 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/migrations/0008_profile_is_pending.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      366 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/migrations/0009_delete_detailkey.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      556 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/migrations/0010_profile_consent.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      774 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/migrations/0011_meta.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      448 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/migrations/0012_django2.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      439 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/migrations/0013_alter_profile_id.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      567 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/migrations/0014_use_django_jsonfield.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/migrations/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2358 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/auth/models.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      367 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/permissions.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2055 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/serializers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      145 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/settings.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      266 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/auth/signals.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.709206 django-daiquiri-0.4.3/daiquiri/auth/static/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.709206 django-daiquiri-0.4.3/daiquiri/auth/static/auth/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.717206 django-daiquiri-0.4.3/daiquiri/auth/static/auth/css/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/static/auth/css/users.scss
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.717206 django-daiquiri-0.4.3/daiquiri/auth/static/auth/js/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1724 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/static/auth/js/users.js
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.709206 django-daiquiri-0.4.3/daiquiri/auth/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.717206 django-daiquiri-0.4.3/daiquiri/auth/templates/account/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      178 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/account_inactive.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      309 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/account_pending.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1124 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/account_profile.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      588 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/account_token.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.717206 django-daiquiri-0.4.3/daiquiri/auth/templates/account/email/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      308 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/email/activation_message.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       55 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/email/activation_subject.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      392 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/email/email_confirmation_message.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       62 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/email/email_confirmation_subject.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      308 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/email/notify_activation_message.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       46 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/email/notify_activation_subject.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      372 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/email/notify_confirmation_message.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       46 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/email/notify_confirmation_subject.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      247 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/email/notify_password_changed_message.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       44 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/email/notify_password_changed_subject.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      354 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/email/notify_rejection_message.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       45 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/email/notify_rejection_subject.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      556 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/email/password_reset_key_message.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       43 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/email/password_reset_key_subject.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      411 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/email/request_activation_message.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       55 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/email/request_activation_subject.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      407 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/email/request_confirmation_message.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       54 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/email/request_confirmation_subject.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2783 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/email.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      975 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/email_confirm.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      224 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/login.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1594 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/login_form.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      546 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/logout.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      383 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/logout_form.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      550 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/password_change.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      254 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/password_change_done.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      532 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/password_reset.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      473 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/password_reset_done.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      853 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/password_reset_from_key.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      341 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/password_reset_from_key_done.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      511 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/password_set.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      247 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/password_set_done.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3164 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/signup.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      201 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/signup_closed.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       17 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/terms_of_use.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      365 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/verification_sent.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      769 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/account/verified_email_required.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.721206 django-daiquiri-0.4.3/daiquiri/auth/templates/auth/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6370 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/auth/users.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1054 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/auth/users_modal_activate_user.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1050 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/auth/users_modal_confirm_user.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1050 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/auth/users_modal_disable_user.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1038 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/auth/users_modal_enable_user.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1044 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/auth/users_modal_reject_user.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3020 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/auth/users_modal_show_user.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3331 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/auth/users_modal_update_user.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2167 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/auth/users_options.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.721206 django-daiquiri-0.4.3/daiquiri/auth/templates/socialaccount/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      303 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/socialaccount/authentication_error.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1879 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/socialaccount/connections.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      766 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/socialaccount/login.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      435 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/socialaccount/login_cancelled.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3294 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/socialaccount/signup.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.721206 django-daiquiri-0.4.3/daiquiri/auth/templates/socialaccount/snippets/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      904 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/templates/socialaccount/snippets/provider_list.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.721206 django-daiquiri-0.4.3/daiquiri/auth/tests/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/tests/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6328 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/auth/tests/test_accounts.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2301 2023-04-24 07:48:40.000000 django-daiquiri-0.4.3/daiquiri/auth/tests/test_honeypot.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      552 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/auth/tests/test_views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2728 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/auth/tests/test_viewset_group.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     7451 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/auth/tests/test_viewset_profile.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      968 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/auth/urls_accounts.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      447 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/urls_auth.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2350 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/utils.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      760 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/auth/validators.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3472 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/auth/views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3114 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/auth/viewsets.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.721206 django-daiquiri-0.4.3/daiquiri/conesearch/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/conesearch/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5814 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/conesearch/adapter.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      171 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/conesearch/apps.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      270 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/conesearch/permissions.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      354 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/conesearch/renderers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      273 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/conesearch/settings.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.709206 django-daiquiri-0.4.3/daiquiri/conesearch/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.721206 django-daiquiri-0.4.3/daiquiri/conesearch/templates/conesearch/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      508 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/conesearch/templates/conesearch/root.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      563 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/conesearch/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      652 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/conesearch/views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1347 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/conesearch/viewsets.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3198 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/conesearch/vo.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.721206 django-daiquiri-0.4.3/daiquiri/contact/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/contact/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      314 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/admin.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      158 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/apps.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      476 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/filters.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      815 2023-04-24 07:48:40.000000 django-daiquiri-0.4.3/daiquiri/contact/forms.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.721206 django-daiquiri-0.4.3/daiquiri/contact/migrations/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1441 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/migrations/0001_initial.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      755 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/migrations/0002_meta.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      582 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/migrations/0003_add_permissions.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      584 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/migrations/0004_meta.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      440 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/migrations/0005_django2.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      449 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/migrations/0006_alter_contactmessage_id.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/migrations/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1376 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/contact/models.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      571 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/serializers.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.709206 django-daiquiri-0.4.3/daiquiri/contact/static/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.709206 django-daiquiri-0.4.3/daiquiri/contact/static/contact/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.721206 django-daiquiri-0.4.3/daiquiri/contact/static/contact/css/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/static/contact/css/messages.scss
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.721206 django-daiquiri-0.4.3/daiquiri/contact/static/contact/js/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1556 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/static/contact/js/messages.js
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.709206 django-daiquiri-0.4.3/daiquiri/contact/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.721206 django-daiquiri-0.4.3/daiquiri/contact/templates/contact/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      959 2023-04-24 07:48:40.000000 django-daiquiri-0.4.3/daiquiri/contact/templates/contact/contact.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.721206 django-daiquiri-0.4.3/daiquiri/contact/templates/contact/email/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      104 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/templates/contact/email/contact_template.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      407 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/templates/contact/email/new_message_admin_message.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       48 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/templates/contact/email/new_message_admin_subject.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      326 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/templates/contact/email/new_message_user_message.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       49 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/templates/contact/email/new_message_user_subject.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5319 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/templates/contact/messages.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      283 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/templates/contact/messages_mailto.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1986 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/templates/contact/messages_modal_show.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1028 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/templates/contact/messages_options.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      247 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/templates/contact/thanks.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.721206 django-daiquiri-0.4.3/daiquiri/contact/tests/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/tests/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2336 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/contact/tests/test_views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3477 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/contact/tests/test_viewset_contact_messages.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1104 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/contact/tests/test_viewset_status.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      541 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      822 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/contact/utils.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1546 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/contact/views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1215 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/contact/viewsets.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.725206 django-daiquiri-0.4.3/daiquiri/core/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/__init__.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.725206 django-daiquiri-0.4.3/daiquiri/core/adapter/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      303 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/adapter/__init__.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.725206 django-daiquiri-0.4.3/daiquiri/core/adapter/database/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/adapter/database/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    12923 2023-04-24 07:48:40.000000 django-daiquiri-0.4.3/daiquiri/core/adapter/database/base.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1266 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/adapter/database/mariadb.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     8216 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/core/adapter/database/mysql.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    12800 2023-04-24 07:48:40.000000 django-daiquiri-0.4.3/daiquiri/core/adapter/database/postgres.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.725206 django-daiquiri-0.4.3/daiquiri/core/adapter/download/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/adapter/download/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5237 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/core/adapter/download/base.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1011 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/adapter/download/mysqldump.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1618 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/adapter/download/pgdump.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1100 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/core/adapter/stream.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      936 2022-08-19 10:23:10.000000 django-daiquiri-0.4.3/daiquiri/core/celery.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1707 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/core/constants.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      219 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/encoders.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2584 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/env.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      101 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/exceptions.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    14347 2023-04-24 07:48:40.000000 django-daiquiri-0.4.3/daiquiri/core/generators.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1346 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/core/hashers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      118 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/http.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.725206 django-daiquiri-0.4.3/daiquiri/core/management/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/management/__init__.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.725206 django-daiquiri-0.4.3/daiquiri/core/management/commands/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/management/commands/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      586 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/management/commands/activate_user.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      244 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/management/commands/create_admin_user.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      246 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/core/management/commands/daiquiri_path.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2417 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/core/management/commands/delete_users.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      295 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/management/commands/deploy.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5286 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/core/management/commands/find_users.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      606 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/management/commands/promote_user.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      679 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/core/management/commands/rabbitcreate.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1021 2022-08-19 10:23:10.000000 django-daiquiri-0.4.3/daiquiri/core/management/commands/runworker.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      434 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/management/commands/setup_groups.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      223 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/management/commands/show_databases.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4661 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/core/management/commands/sqlcreate.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1718 2022-08-19 10:23:10.000000 django-daiquiri-0.4.3/daiquiri/core/management/commands/workers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1338 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/managers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      675 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/middleware.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      164 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/paginations.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2058 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/permissions.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.725206 django-daiquiri-0.4.3/daiquiri/core/renderers/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2636 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/core/renderers/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6349 2023-07-31 14:29:21.000000 django-daiquiri-0.4.3/daiquiri/core/renderers/datacite.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1596 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/renderers/dublincore.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3960 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/renderers/voresource.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6832 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/renderers/vosi.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      118 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/responses.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2007 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/routers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1158 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/serializers.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.725206 django-daiquiri-0.4.3/daiquiri/core/settings/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/settings/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      805 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/core/settings/daiquiri.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     7551 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/core/settings/django.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3471 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/settings/logging.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4462 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/core/settings/vendor.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.713206 django-daiquiri-0.4.3/daiquiri/core/static/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.713206 django-daiquiri-0.4.3/daiquiri/core/static/core/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.725206 django-daiquiri-0.4.3/daiquiri/core/static/core/css/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    11581 2022-08-19 10:23:10.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/css/base.scss
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1874 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/css/browser.scss
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4889 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/css/codehilite.scss
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      153 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/css/codemirror.scss
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      827 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/css/fonts.scss
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1350 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/css/list.scss
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/css/style.scss
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4551 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/css/table.scss
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1665 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/css/variables.scss
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.729206 django-daiquiri-0.4.3/daiquiri/core/static/core/fonts/
+-rwxr-xr-x   0 kmakan    (1002) kmakan    (1003)    42480 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/fonts/DroidSans-Bold.ttf
+-rwxr-xr-x   0 kmakan    (1002) kmakan    (1003)    41028 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/fonts/DroidSans.ttf
+-rwxr-xr-x   0 kmakan    (1002) kmakan    (1003)   117072 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/fonts/DroidSansMono.ttf
+-rwxr-xr-x   0 kmakan    (1002) kmakan    (1003)    48880 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/fonts/DroidSerif-Bold.ttf
+-rwxr-xr-x   0 kmakan    (1002) kmakan    (1003)    45652 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/fonts/DroidSerif-BoldItalic.ttf
+-rwxr-xr-x   0 kmakan    (1002) kmakan    (1003)    40416 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/fonts/DroidSerif-Italic.ttf
+-rwxr-xr-x   0 kmakan    (1002) kmakan    (1003)    43648 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/fonts/DroidSerif.ttf
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.729206 django-daiquiri-0.4.3/daiquiri/core/static/core/html/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1759 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/html/browser.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      457 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/html/formgroup_checkbox.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      417 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/html/formgroup_codemirror.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      421 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/html/formgroup_date.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      471 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/html/formgroup_file.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1115 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/html/formgroup_multicheckbox.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      428 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/html/formgroup_number.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      472 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/html/formgroup_radio.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      848 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/html/formgroup_select.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      862 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/html/formgroup_selectnumber.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      444 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/html/formgroup_text.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      461 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/html/formgroup_textarea.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      486 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/html/formgroup_textareasplit.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      383 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/html/order-list.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.729206 django-daiquiri-0.4.3/daiquiri/core/static/core/img/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    19025 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/img/daiquiri.jpg
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      380 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/img/daiquiri32.png
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1406 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/img/favicon.ico
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      459 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/img/favicon.png
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.729206 django-daiquiri-0.4.3/daiquiri/core/static/core/js/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     9139 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/js/browser.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      653 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/js/byNumber.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4597 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/js/core.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1435 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/js/filter.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      917 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/js/formgroup.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2740 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/js/list.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1303 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/js/multiCheckbox.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1606 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/js/polling.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1839 2022-08-19 10:23:10.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/js/stream.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    14578 2022-08-19 10:23:10.000000 django-daiquiri-0.4.3/daiquiri/core/static/core/js/table.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      224 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/tasks.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.713206 django-daiquiri-0.4.3/daiquiri/core/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.729206 django-daiquiri-0.4.3/daiquiri/core/templates/core/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      188 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/400.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      177 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/403.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      185 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/404.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      192 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/500.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      396 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/base.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/base_analytics.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/base_footer.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1024 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/base_head.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1801 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/base_navigation.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      568 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/base_navigation_account.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      208 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/base_navigation_admin.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1391 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/base_navigation_management.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      156 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/home.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      341 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/page.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.729206 django-daiquiri-0.4.3/daiquiri/core/templates/core/partials/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1903 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/partials/form_field.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      189 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/partials/form_fields.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      322 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/partials/table.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1390 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/partials/table_footer.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      352 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/partials/table_header.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2637 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/partials/table_modal.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      665 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/partials/table_pagination.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5391 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/partials/table_pane.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      463 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/partials/table_search.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1007 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/partials/table_tooltip.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      183 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templates/core/wide.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.729206 django-daiquiri-0.4.3/daiquiri/core/templatetags/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/templatetags/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1495 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/core/templatetags/core_tags.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.729206 django-daiquiri-0.4.3/daiquiri/core/tests/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/tests/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1862 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/core/tests/test_adapter.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      384 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/core/tests/test_views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    12749 2023-04-24 07:48:40.000000 django-daiquiri-0.4.3/daiquiri/core/utils.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2720 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/core/views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2092 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/core/viewsets.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      319 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/core/vo.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.733206 django-daiquiri-0.4.3/daiquiri/cutout/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/cutout/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      269 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/cutout/adapter.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      154 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/cutout/apps.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      266 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/cutout/permissions.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      350 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/cutout/renderers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       88 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/cutout/settings.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      191 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/cutout/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1326 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/cutout/viewsets.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.733206 django-daiquiri-0.4.3/daiquiri/datalink/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/datalink/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     9541 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/datalink/adapter.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      162 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/datalink/apps.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4909 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/datalink/constants.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.733206 django-daiquiri-0.4.3/daiquiri/datalink/management/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/datalink/management/__init__.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.733206 django-daiquiri-0.4.3/daiquiri/datalink/management/commands/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/datalink/management/commands/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      579 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/datalink/management/commands/rebuild_datalink_table.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.733206 django-daiquiri-0.4.3/daiquiri/datalink/migrations/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1320 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/datalink/migrations/0001_initial.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      426 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/datalink/migrations/0002_alter_datalink_content_length.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      450 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/datalink/migrations/0003_alter_datalink_content_length.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/datalink/migrations/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1209 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/datalink/models.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1724 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/datalink/serializers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       91 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/datalink/settings.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.713206 django-daiquiri-0.4.3/daiquiri/datalink/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.733206 django-daiquiri-0.4.3/daiquiri/datalink/templates/datalink/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1719 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/datalink/templates/datalink/datalink.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      507 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/datalink/templates/datalink/root.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      690 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/datalink/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      959 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/datalink/utils.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      697 2023-04-27 21:33:15.000000 django-daiquiri-0.4.3/daiquiri/datalink/views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1728 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/datalink/viewsets.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2789 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/datalink/vo.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.733206 django-daiquiri-0.4.3/daiquiri/files/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/files/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      349 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/files/admin.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      371 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/files/apps.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.733206 django-daiquiri-0.4.3/daiquiri/files/migrations/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1355 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/files/migrations/0001_initial.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      670 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/files/migrations/0002_depth.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      660 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/files/migrations/0003_python3.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      410 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/files/migrations/0004_django2.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      496 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/files/migrations/0005_directory_layout.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      451 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/files/migrations/0006_alter_directory_id.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      473 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/files/migrations/0007_alter_directory_layout.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/files/migrations/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1470 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/files/models.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5211 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/files/search.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      217 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/files/settings.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.713206 django-daiquiri-0.4.3/daiquiri/files/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.733206 django-daiquiri-0.4.3/daiquiri/files/templates/files/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      194 2022-08-19 10:23:10.000000 django-daiquiri-0.4.3/daiquiri/files/templates/files/layout.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1409 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/files/templates/files/list-results.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      261 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/files/templates/files/search-input.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      220 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/files/templates/files/search-results.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.733206 django-daiquiri-0.4.3/daiquiri/files/templatetags/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/files/templatetags/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      634 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/files/templatetags/search_highlight.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.733206 django-daiquiri-0.4.3/daiquiri/files/tests/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/files/tests/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1891 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/files/tests/test_views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      252 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/files/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2991 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/files/utils.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2045 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/files/views.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.733206 django-daiquiri-0.4.3/daiquiri/jobs/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/jobs/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      898 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/jobs/admin.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      146 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/jobs/apps.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      101 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/jobs/exceptions.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      995 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/jobs/filters.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      454 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/jobs/managers.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.737206 django-daiquiri-0.4.3/daiquiri/jobs/migrations/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1705 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/jobs/migrations/0001_job_model.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      473 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/jobs/migrations/0002_execution_duration_default_0.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      586 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/jobs/migrations/0003_owner_fk.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      874 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/jobs/migrations/0004_phases_to_char.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      583 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/jobs/migrations/0005_owner_null_true.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      596 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/jobs/migrations/0006_owner_blank_true.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      466 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/jobs/migrations/0007_creation_time.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      476 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/jobs/migrations/0008_job_error_summary.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      505 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/jobs/migrations/0009_meta.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      805 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/jobs/migrations/0010_add_fields.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      465 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/jobs/migrations/0011_job_client_ip.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      539 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/jobs/migrations/0012_meta.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      456 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/jobs/migrations/0013_job_error_summary.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      477 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/jobs/migrations/0014_blank_run_id.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1088 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/jobs/migrations/0015_job_index.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      400 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/jobs/migrations/0016_django2.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/jobs/migrations/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3378 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/jobs/models.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3038 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/jobs/renderers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1041 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/jobs/routers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2766 2022-08-19 10:23:10.000000 django-daiquiri-0.4.3/daiquiri/jobs/serializers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      919 2022-08-19 10:23:10.000000 django-daiquiri-0.4.3/daiquiri/jobs/utils.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    11152 2022-08-19 10:23:10.000000 django-daiquiri-0.4.3/daiquiri/jobs/viewsets.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.737206 django-daiquiri-0.4.3/daiquiri/metadata/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/metadata/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1893 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/metadata/admin.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      215 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/apps.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3187 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/handlers.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.737206 django-daiquiri-0.4.3/daiquiri/metadata/management/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/management/__init__.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.737206 django-daiquiri-0.4.3/daiquiri/metadata/management/commands/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/management/commands/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      739 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/management/commands/dump_table.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1019 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/metadata/management/commands/update_access_level.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.737206 django-daiquiri-0.4.3/daiquiri/metadata/migrations/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4525 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0001_initial.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1073 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0002_published_for.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      877 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0003_groups.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      501 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0004_function_query_string.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3114 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0005_more_fields.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    11136 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0006_meta.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3913 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0007_access_level.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1162 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0008_refactoring.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      430 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0009_arraysize.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      563 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0010_meta.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1672 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0011_directory.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      412 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0012_remove_directory_metadata_access_level.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      499 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0013_remove_directory.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      563 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0014_rename_pid_to_doi.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      740 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0015_change_doi_to_char.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2266 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0016_rename_database_to_schema.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1307 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0017_rename_database_to_schema.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      583 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0018_meta.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      578 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0019_column_index_for.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      594 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0020_blank_index_for.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      513 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0021_table_nrows.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      507 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0022_table_size.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5264 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0023_python3.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1010 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0024_django2.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      974 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0025_add_published_updated.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1060 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0026_add_creators_and_contributors.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1798 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0027_auto_20201202_1625.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2392 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0028_add_related_identifiers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1089 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0029_alter_ids.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      634 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0030_move_licenses_to_settings.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1059 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0031_change_order.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1714 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0032_data_migration.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     9659 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/0033_refactor_fields.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/migrations/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    12036 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/metadata/models.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.737206 django-daiquiri-0.4.3/daiquiri/metadata/serializers/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2406 2023-07-31 14:29:21.000000 django-daiquiri-0.4.3/daiquiri/metadata/serializers/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5021 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/metadata/serializers/datacite.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1965 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/serializers/dublincore.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2676 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/serializers/export.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      740 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/serializers/management.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2118 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/metadata/serializers/user.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1262 2023-07-31 14:29:21.000000 django-daiquiri-0.4.3/daiquiri/metadata/serializers/validators.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1923 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/metadata/settings.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.713206 django-daiquiri-0.4.3/daiquiri/metadata/static/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.713206 django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.737206 django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/css/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      694 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/css/metadata.scss
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.741206 django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/img/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1173 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/img/by.png
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1768 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/img/by_nc.png
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2069 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/img/by_nc_nd.png
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2236 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/img/by_nc_sa.png
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1515 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/img/by_nd.png
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1755 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/img/by_sa.png
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1230 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/img/cc0.png
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1331 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/img/nc.png
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1051 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/img/nd.png
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      985 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/img/pd.png
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1289 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/img/sa.png
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.741206 django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/js/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     8526 2023-07-31 14:29:21.000000 django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/js/metadata.js
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.713206 django-daiquiri-0.4.3/daiquiri/metadata/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.741206 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3508 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2916 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_display.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1484 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_delete_columns.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1492 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_delete_functions.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1717 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_delete_schemas.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1702 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_delete_tables.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     9346 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_form_columns.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4872 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_form_functions.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     8059 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_form_schemas.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1841 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_form_schemas_attribution.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3349 2023-07-31 14:29:21.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_form_schemas_contributors.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3301 2023-07-31 14:29:21.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_form_schemas_creators.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1866 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_form_schemas_description.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    10199 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_form_tables.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1835 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_form_tables_attribution.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3346 2023-07-31 14:29:21.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_form_tables_contributors.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3298 2023-07-31 14:29:21.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_form_tables_creators.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1860 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_form_tables_description.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1020 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_options.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1514 2022-08-19 10:23:10.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/schema.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2228 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/table.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.741206 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/tags/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      442 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/tags/access_panel.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      501 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/tags/doi_panel.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      523 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/tags/license_panel.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      349 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/tags/schemas_menu.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.741206 django-daiquiri-0.4.3/daiquiri/metadata/templatetags/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/templatetags/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1710 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/metadata/templatetags/metadata_tags.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.741206 django-daiquiri-0.4.3/daiquiri/metadata/tests/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/tests/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      459 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/metadata/tests/test_tags.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3579 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/metadata/tests/test_views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3975 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/metadata/tests/test_viewset_column.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4329 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/metadata/tests/test_viewset_function.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4355 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/metadata/tests/test_viewset_schema.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3922 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/metadata/tests/test_viewset_table.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1150 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      727 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/metadata/utils.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2271 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/metadata/views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     9261 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/metadata/viewsets.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.741206 django-daiquiri-0.4.3/daiquiri/oai/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/oai/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    15252 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/oai/adapter.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      142 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/oai/apps.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.741206 django-daiquiri-0.4.3/daiquiri/oai/management/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/oai/management/__init__.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.741206 django-daiquiri-0.4.3/daiquiri/oai/management/commands/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/oai/management/commands/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2208 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/oai/management/commands/rebuild_oai_schema.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.741206 django-daiquiri-0.4.3/daiquiri/oai/migrations/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1069 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/oai/migrations/0001_initial.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      682 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/oai/migrations/0002_resource_type.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      443 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/oai/migrations/0003_record_set_spec.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      445 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/oai/migrations/0004_alter_record_id.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      439 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/oai/migrations/0005_alter_record_resource_id.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      507 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/oai/migrations/0006_alter_record_resource_id.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/oai/migrations/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1195 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/oai/models.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     7874 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/oai/renderers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1236 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/oai/settings.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      141 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/oai/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2522 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/oai/utils.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    11305 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/oai/views.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.745205 django-daiquiri-0.4.3/daiquiri/query/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1285 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/admin.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      523 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/apps.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      597 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/filters.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      692 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/handlers.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.745205 django-daiquiri-0.4.3/daiquiri/query/management/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/management/__init__.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.745205 django-daiquiri-0.4.3/daiquiri/query/management/commands/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/management/commands/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2482 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/management/commands/archive_query_jobs.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1915 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/management/commands/fix_query_jobs.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1808 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/management/commands/scrub_query_jobs.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1981 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/management/commands/scrub_user_tables.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      437 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/managers.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.745205 django-daiquiri-0.4.3/daiquiri/query/migrations/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1214 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0001_initial.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      502 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0002_meta.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1025 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0003_query_language_and_actual_query.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1149 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0004_table_name.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      702 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0005_meta.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1155 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0006_example.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      505 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0007_queryjob_metadata.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      463 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0008_queryjob_pid.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      613 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0009_remove_choices.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      476 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0010_queue_can_be_null.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      469 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0011_queryjob_native_query.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      469 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0012_query_language_length.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2222 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0013_refactoring.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1453 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0014_downloadjob.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1611 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0015_queryarchivejob.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      447 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0016_rename_database_to_schema.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      648 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0017_big_integer_fields.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      485 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0018_blank_metadata.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      516 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0019_remove_sync_jobs.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      669 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0020_python3.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1014 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0021_django2.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1277 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0022_blank_fields.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      422 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0023_queryjob_uploads.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      728 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0024_fix_jsonfield.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      446 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0025_alter_example_id.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      779 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0026_use_django_jsonfield.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      525 2022-08-19 10:23:10.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/0027_rename_job_to_query_job.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/migrations/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    20749 2023-04-24 07:48:40.000000 django-daiquiri-0.4.3/daiquiri/query/models.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      265 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/permissions.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    13457 2023-07-31 14:29:21.000000 django-daiquiri-0.4.3/daiquiri/query/process.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6071 2022-08-19 10:23:10.000000 django-daiquiri-0.4.3/daiquiri/query/serializers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3716 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/settings.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.713206 django-daiquiri-0.4.3/daiquiri/query/static/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.713206 django-daiquiri-0.4.3/daiquiri/query/static/query/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.745205 django-daiquiri-0.4.3/daiquiri/query/static/query/css/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       35 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/static/query/css/examples.scss
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      214 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/static/query/css/jobs.scss
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       89 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/static/query/css/plot.scss
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3784 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/static/query/css/query.scss
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.713206 django-daiquiri-0.4.3/daiquiri/query/static/query/js/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.745205 django-daiquiri-0.4.3/daiquiri/query/static/query/js/apps/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      243 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/static/query/js/apps/examples.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      223 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/static/query/js/apps/jobs.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2010 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/query/static/query/js/apps/query.js
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.745205 django-daiquiri-0.4.3/daiquiri/query/static/query/js/downloads/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      634 2022-08-19 10:23:10.000000 django-daiquiri-0.4.3/daiquiri/query/static/query/js/downloads/archive.js
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.745205 django-daiquiri-0.4.3/daiquiri/query/static/query/js/dropdowns/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1207 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/static/query/js/dropdowns/simbad.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1893 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/static/query/js/dropdowns/vizier.js
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.745205 django-daiquiri-0.4.3/daiquiri/query/static/query/js/forms/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1254 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/static/query/js/forms/box.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1045 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/static/query/js/forms/cone.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4545 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/static/query/js/forms/sql.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      857 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/static/query/js/forms/upload.js
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.745205 django-daiquiri-0.4.3/daiquiri/query/static/query/js/services/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2970 2022-08-19 10:23:10.000000 django-daiquiri-0.4.3/daiquiri/query/static/query/js/services/download.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3109 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/static/query/js/services/examples.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3793 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/static/query/js/services/jobs.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    27091 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/static/query/js/services/plot.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    12546 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/query/static/query/js/services/query.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    12660 2023-04-24 07:48:40.000000 django-daiquiri-0.4.3/daiquiri/query/tasks.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.713206 django-daiquiri-0.4.3/daiquiri/query/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.749205 django-daiquiri-0.4.3/daiquiri/query/templates/query/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4903 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/examples.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1475 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/examples_modal_delete.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4918 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/examples_modal_form.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      349 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/examples_options.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6534 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/jobs.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4036 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/jobs_modal_show_job.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5289 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      409 2022-08-19 10:23:10.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_download.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      572 2022-08-19 10:23:10.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_download_archive.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      806 2022-08-19 10:23:10.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_download_table.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      565 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_dropdown_columns.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      602 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_dropdown_examples.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      591 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_dropdown_functions.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      582 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_dropdown_schemas.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2282 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_dropdown_simbad.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2922 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_dropdown_vizier.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      188 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_form.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3657 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_form_box.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2560 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_form_cone.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3128 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_form_sql.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1945 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_form_upload.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1329 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_modal_abort_job.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1339 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_modal_archive_job.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1138 2022-08-19 10:23:10.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_modal_logout.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1557 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_modal_update_job.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4684 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_overview.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2241 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_plot.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1478 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_plot_histogram.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4381 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_plot_scatter.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1836 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_plot_scatter_cmap.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       62 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_results.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5899 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_sidebar.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/templates/query/query_sidebar_status_extra.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.749205 django-daiquiri-0.4.3/daiquiri/query/tests/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/query/tests/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2454 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/tests/test_permissions.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1169 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/tests/test_views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1093 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/tests/test_viewset_download.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1076 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/tests/test_viewset_dropdown.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4394 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/tests/test_viewset_example.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1083 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/tests/test_viewset_form.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    12329 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/tests/test_viewset_job.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1122 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/tests/test_viewset_status.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1216 2022-08-19 10:23:10.000000 django-daiquiri-0.4.3/daiquiri/query/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    10213 2023-04-24 07:48:40.000000 django-daiquiri-0.4.3/daiquiri/query/utils.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3242 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/query/validators.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1127 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/query/views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    14163 2023-07-20 09:06:08.000000 django-daiquiri-0.4.3/daiquiri/query/viewsets.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.749205 django-daiquiri-0.4.3/daiquiri/registry/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/registry/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      162 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/registry/apps.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1204 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/registry/serializers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      135 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/registry/settings.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.713206 django-daiquiri-0.4.3/daiquiri/registry/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.749205 django-daiquiri-0.4.3/daiquiri/registry/templates/registry/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1196 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/registry/templates/registry/root.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      551 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/registry/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      956 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/registry/views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4143 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/registry/vo.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.749205 django-daiquiri-0.4.3/daiquiri/serve/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/serve/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      159 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/serve/apps.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.749205 django-daiquiri-0.4.3/daiquiri/serve/migrations/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/serve/migrations/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      448 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/serve/serializers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       48 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/serve/settings.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.713206 django-daiquiri-0.4.3/daiquiri/serve/static/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.713206 django-daiquiri-0.4.3/daiquiri/serve/static/serve/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.749205 django-daiquiri-0.4.3/daiquiri/serve/static/serve/css/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      114 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/serve/static/serve/css/table.scss
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.749205 django-daiquiri-0.4.3/daiquiri/serve/static/serve/js/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      191 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/serve/static/serve/js/table.js
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      736 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/serve/tasks.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.713206 django-daiquiri-0.4.3/daiquiri/serve/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.749205 django-daiquiri-0.4.3/daiquiri/serve/templates/serve/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1441 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/serve/templates/serve/table.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.749205 django-daiquiri-0.4.3/daiquiri/serve/tests/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/serve/tests/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     2410 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/serve/tests/test_views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4860 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/serve/tests/test_viewsets.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      609 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/serve/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      218 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/serve/utils.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      719 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/serve/views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3057 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/serve/viewsets.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.753205 django-daiquiri-0.4.3/daiquiri/stats/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/stats/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      296 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/stats/admin.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      150 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/stats/apps.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.753205 django-daiquiri-0.4.3/daiquiri/stats/migrations/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1291 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/stats/migrations/0001_initial.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      927 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/stats/migrations/0002_data_migration.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1050 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/stats/migrations/0003_data_migration.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      603 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/stats/migrations/0004_set_record_null.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      411 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/stats/migrations/0005_django2.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      439 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/stats/migrations/0006_alter_record_id.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      380 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/stats/migrations/0007_use_django_jsonfield.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      461 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/stats/migrations/0008_alter_record_resource.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/stats/migrations/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      717 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/stats/models.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      405 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/stats/settings.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.713206 django-daiquiri-0.4.3/daiquiri/stats/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.753205 django-daiquiri-0.4.3/daiquiri/stats/templates/stats/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      730 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/stats/templates/stats/management.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      174 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/stats/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      929 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/stats/views.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.753205 django-daiquiri-0.4.3/daiquiri/tap/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/tap/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      142 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/tap/apps.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    11624 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/tap/constants.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.753205 django-daiquiri-0.4.3/daiquiri/tap/management/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/tap/management/__init__.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.753205 django-daiquiri-0.4.3/daiquiri/tap/management/commands/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/tap/management/commands/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      524 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/tap/management/commands/rebuild_tap_schema.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3212 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/tap/management/commands/setup_tap_metadata.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.753205 django-daiquiri-0.4.3/daiquiri/tap/migrations/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3204 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/tap/migrations/0001_initial.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      856 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/tap/migrations/0002_alter_ids.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/tap/migrations/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1952 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/tap/models.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1341 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/tap/serializers.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      161 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/tap/settings.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.713206 django-daiquiri-0.4.3/daiquiri/tap/static/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.713206 django-daiquiri-0.4.3/daiquiri/tap/static/tap/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.753205 django-daiquiri-0.4.3/daiquiri/tap/static/tap/css/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)       50 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/tap/static/tap/css/examples.scss
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.713206 django-daiquiri-0.4.3/daiquiri/tap/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.753205 django-daiquiri-0.4.3/daiquiri/tap/templates/tap/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      928 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/tap/templates/tap/examples.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      806 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/tap/templates/tap/root.html
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.753205 django-daiquiri-0.4.3/daiquiri/tap/tests/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/tap/tests/__init__.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    27429 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/tap/tests/test_async.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     4970 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/tap/tests/test_sync.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1464 2023-01-30 20:07:21.000000 django-daiquiri-0.4.3/daiquiri/tap/tests/test_views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      883 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/tap/urls.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     5004 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/tap/utils.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1039 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/tap/views.py
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     3771 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/tap/vo.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.753205 django-daiquiri-0.4.3/daiquiri/uws/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        0 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/uws/__init__.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.713206 django-daiquiri-0.4.3/daiquiri/uws/templates/
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.753205 django-daiquiri-0.4.3/daiquiri/uws/templates/uws/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      122 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/uws/templates/uws/root.html
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      861 2022-06-16 09:10:03.000000 django-daiquiri-0.4.3/daiquiri/uws/urls.py
+drwxr-xr-x   0 kmakan    (1002) kmakan    (1003)        0 2023-07-31 14:32:01.753205 django-daiquiri-0.4.3/django_daiquiri.egg-info/
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     6177 2023-07-31 14:32:01.000000 django-daiquiri-0.4.3/django_daiquiri.egg-info/PKG-INFO
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)    28945 2023-07-31 14:32:01.000000 django-daiquiri-0.4.3/django_daiquiri.egg-info/SOURCES.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        1 2023-07-31 14:32:01.000000 django-daiquiri-0.4.3/django_daiquiri.egg-info/dependency_links.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      720 2023-07-31 14:32:01.000000 django-daiquiri-0.4.3/django_daiquiri.egg-info/requires.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)        9 2023-07-31 14:32:01.000000 django-daiquiri-0.4.3/django_daiquiri.egg-info/top_level.txt
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)      253 2023-07-31 14:32:01.753205 django-daiquiri-0.4.3/setup.cfg
+-rw-r--r--   0 kmakan    (1002) kmakan    (1003)     1376 2023-07-20 09:24:11.000000 django-daiquiri-0.4.3/setup.py
```

### Comparing `django-daiquiri-0.4.2/LICENSE` & `django-daiquiri-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/NOTICE` & `django-daiquiri-0.4.3/NOTICE`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/PKG-INFO` & `django-daiquiri-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-daiquiri
-Version: 0.4.2
+Version: 0.4.3
 Summary: Daiquiri is a framework for the publication of scientific databases.
 Home-page: https://github.com/django-daiquiri/daiquiri
 Author: Jochen Klar
 Author-email: mail@jochenklar.de
 Maintainer: Jochen Klar
 Maintainer-email: mail@jochenklar.de
 License: Apache-2.0
```

### Comparing `django-daiquiri-0.4.2/README.md` & `django-daiquiri-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/adapter.py` & `django-daiquiri-0.4.3/daiquiri/auth/adapter.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/forms.py` & `django-daiquiri-0.4.3/daiquiri/auth/forms.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/handlers.py` & `django-daiquiri-0.4.3/daiquiri/auth/handlers.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/migrations/0001_profile_model.py` & `django-daiquiri-0.4.3/daiquiri/auth/migrations/0001_profile_model.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/migrations/0003_view_permission.py` & `django-daiquiri-0.4.3/daiquiri/auth/migrations/0003_view_permission.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/migrations/0004_view_permission_typo.py` & `django-daiquiri-0.4.3/daiquiri/auth/migrations/0004_view_permission_typo.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/migrations/0005_view_permission_fix.py` & `django-daiquiri-0.4.3/daiquiri/auth/migrations/0005_view_permission_fix.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/migrations/0006_profile_ordering.py` & `django-daiquiri-0.4.3/daiquiri/auth/migrations/0006_profile_ordering.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/migrations/0008_profile_is_pending.py` & `django-daiquiri-0.4.3/daiquiri/auth/migrations/0008_profile_is_pending.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/migrations/0010_profile_consent.py` & `django-daiquiri-0.4.3/daiquiri/auth/migrations/0010_profile_consent.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/migrations/0011_meta.py` & `django-daiquiri-0.4.3/daiquiri/auth/migrations/0011_meta.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/migrations/0014_use_django_jsonfield.py` & `django-daiquiri-0.4.3/daiquiri/auth/migrations/0014_use_django_jsonfield.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/models.py` & `django-daiquiri-0.4.3/daiquiri/auth/models.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/serializers.py` & `django-daiquiri-0.4.3/daiquiri/auth/serializers.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/static/auth/js/users.js` & `django-daiquiri-0.4.3/daiquiri/auth/static/auth/js/users.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/account/account_profile.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/account/account_profile.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/account/account_token.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/account/account_token.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/account/email/password_reset_key_message.txt` & `django-daiquiri-0.4.3/daiquiri/auth/templates/account/email/password_reset_key_message.txt`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/account/email.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/account/email.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/account/email_confirm.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/account/login_form.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/account/login_form.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/account/logout.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/account/logout.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/account/password_change.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/account/password_change.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/account/password_reset.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/account/password_reset_from_key.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/account/signup.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/account/signup.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/account/verified_email_required.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/account/verified_email_required.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/auth/users.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_activate_user.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/auth/users_modal_activate_user.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_confirm_user.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/auth/users_modal_confirm_user.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_disable_user.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/auth/users_modal_disable_user.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_enable_user.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/auth/users_modal_enable_user.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_reject_user.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/auth/users_modal_reject_user.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_show_user.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/auth/users_modal_show_user.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_modal_update_user.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/auth/users_modal_update_user.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/auth/users_options.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/auth/users_options.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/socialaccount/connections.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/socialaccount/connections.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/socialaccount/login.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/socialaccount/login.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/socialaccount/signup.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/socialaccount/signup.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/templates/socialaccount/snippets/provider_list.html` & `django-daiquiri-0.4.3/daiquiri/auth/templates/socialaccount/snippets/provider_list.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/tests/test_accounts.py` & `django-daiquiri-0.4.3/daiquiri/auth/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/tests/test_honeypot.py` & `django-daiquiri-0.4.3/daiquiri/auth/tests/test_honeypot.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/tests/test_views.py` & `django-daiquiri-0.4.3/daiquiri/auth/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/tests/test_viewset_group.py` & `django-daiquiri-0.4.3/daiquiri/auth/tests/test_viewset_group.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/tests/test_viewset_profile.py` & `django-daiquiri-0.4.3/daiquiri/auth/tests/test_viewset_profile.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/urls_accounts.py` & `django-daiquiri-0.4.3/daiquiri/auth/urls_accounts.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/utils.py` & `django-daiquiri-0.4.3/daiquiri/auth/utils.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/validators.py` & `django-daiquiri-0.4.3/daiquiri/auth/validators.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/views.py` & `django-daiquiri-0.4.3/daiquiri/auth/views.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/auth/viewsets.py` & `django-daiquiri-0.4.3/daiquiri/auth/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/conesearch/adapter.py` & `django-daiquiri-0.4.3/daiquiri/conesearch/adapter.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/conesearch/urls.py` & `django-daiquiri-0.4.3/daiquiri/conesearch/urls.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/conesearch/views.py` & `django-daiquiri-0.4.3/daiquiri/conesearch/views.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/conesearch/viewsets.py` & `django-daiquiri-0.4.3/daiquiri/conesearch/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/conesearch/vo.py` & `django-daiquiri-0.4.3/daiquiri/conesearch/vo.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/contact/forms.py` & `django-daiquiri-0.4.3/daiquiri/contact/forms.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/contact/migrations/0001_initial.py` & `django-daiquiri-0.4.3/daiquiri/contact/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/contact/migrations/0002_meta.py` & `django-daiquiri-0.4.3/daiquiri/contact/migrations/0002_meta.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/contact/migrations/0003_add_permissions.py` & `django-daiquiri-0.4.3/daiquiri/contact/migrations/0003_add_permissions.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/contact/migrations/0004_meta.py` & `django-daiquiri-0.4.3/daiquiri/contact/migrations/0004_meta.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/contact/models.py` & `django-daiquiri-0.4.3/daiquiri/contact/models.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/contact/serializers.py` & `django-daiquiri-0.4.3/daiquiri/contact/serializers.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/contact/static/contact/js/messages.js` & `django-daiquiri-0.4.3/daiquiri/contact/static/contact/js/messages.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/contact/templates/contact/contact.html` & `django-daiquiri-0.4.3/daiquiri/contact/templates/contact/contact.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/contact/templates/contact/messages.html` & `django-daiquiri-0.4.3/daiquiri/contact/templates/contact/messages.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/contact/templates/contact/messages_modal_show.html` & `django-daiquiri-0.4.3/daiquiri/contact/templates/contact/messages_modal_show.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/contact/templates/contact/messages_options.html` & `django-daiquiri-0.4.3/daiquiri/contact/templates/contact/messages_options.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/contact/tests/test_views.py` & `django-daiquiri-0.4.3/daiquiri/contact/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/contact/tests/test_viewset_contact_messages.py` & `django-daiquiri-0.4.3/daiquiri/contact/tests/test_viewset_contact_messages.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/contact/tests/test_viewset_status.py` & `django-daiquiri-0.4.3/daiquiri/contact/tests/test_viewset_status.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/contact/urls.py` & `django-daiquiri-0.4.3/daiquiri/contact/urls.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/contact/utils.py` & `django-daiquiri-0.4.3/daiquiri/contact/utils.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/contact/views.py` & `django-daiquiri-0.4.3/daiquiri/contact/views.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/contact/viewsets.py` & `django-daiquiri-0.4.3/daiquiri/contact/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/adapter/database/base.py` & `django-daiquiri-0.4.3/daiquiri/core/adapter/database/base.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/adapter/database/mariadb.py` & `django-daiquiri-0.4.3/daiquiri/core/adapter/database/mariadb.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/adapter/database/mysql.py` & `django-daiquiri-0.4.3/daiquiri/core/adapter/database/mysql.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/adapter/database/postgres.py` & `django-daiquiri-0.4.3/daiquiri/core/adapter/database/postgres.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/adapter/download/base.py` & `django-daiquiri-0.4.3/daiquiri/core/adapter/download/base.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/adapter/download/mysqldump.py` & `django-daiquiri-0.4.3/daiquiri/core/adapter/download/mysqldump.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/adapter/download/pgdump.py` & `django-daiquiri-0.4.3/daiquiri/core/adapter/download/pgdump.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/adapter/stream.py` & `django-daiquiri-0.4.3/daiquiri/core/adapter/stream.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/celery.py` & `django-daiquiri-0.4.3/daiquiri/core/celery.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/constants.py` & `django-daiquiri-0.4.3/daiquiri/core/constants.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/env.py` & `django-daiquiri-0.4.3/daiquiri/core/env.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/generators.py` & `django-daiquiri-0.4.3/daiquiri/core/generators.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/hashers.py` & `django-daiquiri-0.4.3/daiquiri/core/hashers.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/management/commands/activate_user.py` & `django-daiquiri-0.4.3/daiquiri/core/management/commands/activate_user.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/management/commands/delete_users.py` & `django-daiquiri-0.4.3/daiquiri/core/management/commands/delete_users.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/management/commands/find_users.py` & `django-daiquiri-0.4.3/daiquiri/core/management/commands/find_users.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/management/commands/promote_user.py` & `django-daiquiri-0.4.3/daiquiri/core/management/commands/promote_user.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/management/commands/rabbitcreate.py` & `django-daiquiri-0.4.3/daiquiri/core/management/commands/rabbitcreate.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/management/commands/runworker.py` & `django-daiquiri-0.4.3/daiquiri/core/management/commands/runworker.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/management/commands/sqlcreate.py` & `django-daiquiri-0.4.3/daiquiri/core/management/commands/sqlcreate.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/management/commands/workers.py` & `django-daiquiri-0.4.3/daiquiri/core/management/commands/workers.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/managers.py` & `django-daiquiri-0.4.3/daiquiri/core/managers.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/middleware.py` & `django-daiquiri-0.4.3/daiquiri/core/middleware.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/permissions.py` & `django-daiquiri-0.4.3/daiquiri/core/permissions.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/renderers/__init__.py` & `django-daiquiri-0.4.3/daiquiri/core/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/renderers/datacite.py` & `django-daiquiri-0.4.3/daiquiri/core/renderers/datacite.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,21 @@
             orcid = person.get('orcid')
             if orcid:
                 self.node('nameIdentifier', {
                     'schemeURI': 'http://orcid.org/',
                     'nameIdentifierScheme': 'ORCID'
                 }, orcid)
 
+            ror = person.get('ror')
+            if ror:
+                self.node('nameIdentifier', {
+                    'schemeURI': 'http://ror.org/',
+                    'nameIdentifierScheme': 'ROR'
+                }, ror)
+
             affiliations = person.get('affiliations')
             if affiliations:
                 for affiliation in affiliations:
                     self.node('affiliation', {
                         'affiliationIdentifier': affiliation.get('affiliation_identifier'),
                         'affiliationIdentifierScheme': affiliation.get('affiliation_identifier_scheme'),
                         'schemeURI': affiliation.get('scheme_uri')
```

### Comparing `django-daiquiri-0.4.2/daiquiri/core/renderers/dublincore.py` & `django-daiquiri-0.4.3/daiquiri/core/renderers/dublincore.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/renderers/voresource.py` & `django-daiquiri-0.4.3/daiquiri/core/renderers/voresource.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/renderers/vosi.py` & `django-daiquiri-0.4.3/daiquiri/core/renderers/vosi.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/routers.py` & `django-daiquiri-0.4.3/daiquiri/core/routers.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/serializers.py` & `django-daiquiri-0.4.3/daiquiri/core/serializers.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/settings/daiquiri.py` & `django-daiquiri-0.4.3/daiquiri/core/settings/daiquiri.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/settings/django.py` & `django-daiquiri-0.4.3/daiquiri/core/settings/django.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/settings/logging.py` & `django-daiquiri-0.4.3/daiquiri/core/settings/logging.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/settings/vendor.py` & `django-daiquiri-0.4.3/daiquiri/core/settings/vendor.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/css/base.scss` & `django-daiquiri-0.4.3/daiquiri/core/static/core/css/base.scss`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/css/browser.scss` & `django-daiquiri-0.4.3/daiquiri/core/static/core/css/browser.scss`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/css/codehilite.scss` & `django-daiquiri-0.4.3/daiquiri/core/static/core/css/codehilite.scss`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/css/fonts.scss` & `django-daiquiri-0.4.3/daiquiri/core/static/core/css/fonts.scss`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/css/list.scss` & `django-daiquiri-0.4.3/daiquiri/core/static/core/css/list.scss`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/css/table.scss` & `django-daiquiri-0.4.3/daiquiri/core/static/core/css/table.scss`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/css/variables.scss` & `django-daiquiri-0.4.3/daiquiri/core/static/core/css/variables.scss`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSans-Bold.ttf` & `django-daiquiri-0.4.3/daiquiri/core/static/core/fonts/DroidSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSans.ttf` & `django-daiquiri-0.4.3/daiquiri/core/static/core/fonts/DroidSans.ttf`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSansMono.ttf` & `django-daiquiri-0.4.3/daiquiri/core/static/core/fonts/DroidSansMono.ttf`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSerif-Bold.ttf` & `django-daiquiri-0.4.3/daiquiri/core/static/core/fonts/DroidSerif-Bold.ttf`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSerif-BoldItalic.ttf` & `django-daiquiri-0.4.3/daiquiri/core/static/core/fonts/DroidSerif-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSerif-Italic.ttf` & `django-daiquiri-0.4.3/daiquiri/core/static/core/fonts/DroidSerif-Italic.ttf`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/fonts/DroidSerif.ttf` & `django-daiquiri-0.4.3/daiquiri/core/static/core/fonts/DroidSerif.ttf`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/html/browser.html` & `django-daiquiri-0.4.3/daiquiri/core/static/core/html/browser.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_multicheckbox.html` & `django-daiquiri-0.4.3/daiquiri/core/static/core/html/formgroup_multicheckbox.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_select.html` & `django-daiquiri-0.4.3/daiquiri/core/static/core/html/formgroup_select.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/html/formgroup_selectnumber.html` & `django-daiquiri-0.4.3/daiquiri/core/static/core/html/formgroup_selectnumber.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/img/daiquiri.jpg` & `django-daiquiri-0.4.3/daiquiri/core/static/core/img/daiquiri.jpg`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/img/favicon.ico` & `django-daiquiri-0.4.3/daiquiri/core/static/core/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/js/browser.js` & `django-daiquiri-0.4.3/daiquiri/core/static/core/js/browser.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/js/byNumber.js` & `django-daiquiri-0.4.3/daiquiri/core/static/core/js/byNumber.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/js/core.js` & `django-daiquiri-0.4.3/daiquiri/core/static/core/js/core.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/js/filter.js` & `django-daiquiri-0.4.3/daiquiri/core/static/core/js/filter.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/js/formgroup.js` & `django-daiquiri-0.4.3/daiquiri/core/static/core/js/formgroup.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/js/list.js` & `django-daiquiri-0.4.3/daiquiri/core/static/core/js/list.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/js/multiCheckbox.js` & `django-daiquiri-0.4.3/daiquiri/core/static/core/js/multiCheckbox.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/js/polling.js` & `django-daiquiri-0.4.3/daiquiri/core/static/core/js/polling.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/js/stream.js` & `django-daiquiri-0.4.3/daiquiri/core/static/core/js/stream.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/static/core/js/table.js` & `django-daiquiri-0.4.3/daiquiri/core/static/core/js/table.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/templates/core/base_head.html` & `django-daiquiri-0.4.3/daiquiri/core/templates/core/base_head.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/templates/core/base_navigation.html` & `django-daiquiri-0.4.3/daiquiri/core/templates/core/base_navigation.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/templates/core/base_navigation_account.html` & `django-daiquiri-0.4.3/daiquiri/core/templates/core/base_navigation_account.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/templates/core/base_navigation_management.html` & `django-daiquiri-0.4.3/daiquiri/core/templates/core/base_navigation_management.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/form_field.html` & `django-daiquiri-0.4.3/daiquiri/core/templates/core/partials/form_field.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table_footer.html` & `django-daiquiri-0.4.3/daiquiri/core/templates/core/partials/table_footer.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table_modal.html` & `django-daiquiri-0.4.3/daiquiri/core/templates/core/partials/table_modal.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table_pagination.html` & `django-daiquiri-0.4.3/daiquiri/core/templates/core/partials/table_pagination.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table_pane.html` & `django-daiquiri-0.4.3/daiquiri/core/templates/core/partials/table_pane.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/templates/core/partials/table_tooltip.html` & `django-daiquiri-0.4.3/daiquiri/core/templates/core/partials/table_tooltip.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/templatetags/core_tags.py` & `django-daiquiri-0.4.3/daiquiri/core/templatetags/core_tags.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/tests/test_adapter.py` & `django-daiquiri-0.4.3/daiquiri/core/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/utils.py` & `django-daiquiri-0.4.3/daiquiri/core/utils.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/views.py` & `django-daiquiri-0.4.3/daiquiri/core/views.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/core/viewsets.py` & `django-daiquiri-0.4.3/daiquiri/core/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/cutout/viewsets.py` & `django-daiquiri-0.4.3/daiquiri/cutout/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/datalink/adapter.py` & `django-daiquiri-0.4.3/daiquiri/datalink/adapter.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/datalink/constants.py` & `django-daiquiri-0.4.3/daiquiri/datalink/constants.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/datalink/management/commands/rebuild_datalink_table.py` & `django-daiquiri-0.4.3/daiquiri/datalink/management/commands/rebuild_datalink_table.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/datalink/migrations/0001_initial.py` & `django-daiquiri-0.4.3/daiquiri/datalink/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/datalink/models.py` & `django-daiquiri-0.4.3/daiquiri/datalink/models.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/datalink/serializers.py` & `django-daiquiri-0.4.3/daiquiri/datalink/serializers.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/datalink/templates/datalink/datalink.html` & `django-daiquiri-0.4.3/daiquiri/datalink/templates/datalink/datalink.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/datalink/urls.py` & `django-daiquiri-0.4.3/daiquiri/datalink/urls.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/datalink/utils.py` & `django-daiquiri-0.4.3/daiquiri/datalink/utils.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/datalink/views.py` & `django-daiquiri-0.4.3/daiquiri/datalink/views.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/datalink/viewsets.py` & `django-daiquiri-0.4.3/daiquiri/datalink/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/datalink/vo.py` & `django-daiquiri-0.4.3/daiquiri/datalink/vo.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/files/migrations/0001_initial.py` & `django-daiquiri-0.4.3/daiquiri/files/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/files/migrations/0002_depth.py` & `django-daiquiri-0.4.3/daiquiri/files/migrations/0002_depth.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/files/migrations/0003_python3.py` & `django-daiquiri-0.4.3/daiquiri/files/migrations/0003_python3.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/files/models.py` & `django-daiquiri-0.4.3/daiquiri/files/models.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/files/search.py` & `django-daiquiri-0.4.3/daiquiri/files/search.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/files/templates/files/list-results.html` & `django-daiquiri-0.4.3/daiquiri/files/templates/files/list-results.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/files/templatetags/search_highlight.py` & `django-daiquiri-0.4.3/daiquiri/files/templatetags/search_highlight.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/files/tests/test_views.py` & `django-daiquiri-0.4.3/daiquiri/files/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/files/utils.py` & `django-daiquiri-0.4.3/daiquiri/files/utils.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/files/views.py` & `django-daiquiri-0.4.3/daiquiri/files/views.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/jobs/admin.py` & `django-daiquiri-0.4.3/daiquiri/jobs/admin.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/jobs/filters.py` & `django-daiquiri-0.4.3/daiquiri/jobs/filters.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/jobs/migrations/0001_job_model.py` & `django-daiquiri-0.4.3/daiquiri/jobs/migrations/0001_job_model.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/jobs/migrations/0003_owner_fk.py` & `django-daiquiri-0.4.3/daiquiri/jobs/migrations/0003_owner_fk.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/jobs/migrations/0004_phases_to_char.py` & `django-daiquiri-0.4.3/daiquiri/jobs/migrations/0004_phases_to_char.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/jobs/migrations/0005_owner_null_true.py` & `django-daiquiri-0.4.3/daiquiri/jobs/migrations/0005_owner_null_true.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/jobs/migrations/0006_owner_blank_true.py` & `django-daiquiri-0.4.3/daiquiri/jobs/migrations/0006_owner_blank_true.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/jobs/migrations/0010_add_fields.py` & `django-daiquiri-0.4.3/daiquiri/jobs/migrations/0010_add_fields.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/jobs/migrations/0012_meta.py` & `django-daiquiri-0.4.3/daiquiri/jobs/migrations/0012_meta.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/jobs/migrations/0015_job_index.py` & `django-daiquiri-0.4.3/daiquiri/jobs/migrations/0015_job_index.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/jobs/models.py` & `django-daiquiri-0.4.3/daiquiri/jobs/models.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/jobs/renderers.py` & `django-daiquiri-0.4.3/daiquiri/jobs/renderers.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/jobs/routers.py` & `django-daiquiri-0.4.3/daiquiri/jobs/routers.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/jobs/serializers.py` & `django-daiquiri-0.4.3/daiquiri/jobs/serializers.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/jobs/utils.py` & `django-daiquiri-0.4.3/daiquiri/jobs/utils.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/jobs/viewsets.py` & `django-daiquiri-0.4.3/daiquiri/jobs/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/admin.py` & `django-daiquiri-0.4.3/daiquiri/metadata/admin.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/handlers.py` & `django-daiquiri-0.4.3/daiquiri/metadata/handlers.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/management/commands/dump_table.py` & `django-daiquiri-0.4.3/daiquiri/metadata/management/commands/dump_table.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/management/commands/update_access_level.py` & `django-daiquiri-0.4.3/daiquiri/metadata/management/commands/update_access_level.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0001_initial.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0002_published_for.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0002_published_for.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0003_groups.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0003_groups.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0005_more_fields.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0005_more_fields.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0006_meta.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0006_meta.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0007_access_level.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0007_access_level.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0008_refactoring.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0008_refactoring.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0010_meta.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0010_meta.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0011_directory.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0011_directory.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0014_rename_pid_to_doi.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0014_rename_pid_to_doi.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0015_change_doi_to_char.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0015_change_doi_to_char.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0016_rename_database_to_schema.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0016_rename_database_to_schema.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0017_rename_database_to_schema.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0017_rename_database_to_schema.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0018_meta.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0018_meta.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0019_column_index_for.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0019_column_index_for.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0020_blank_index_for.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0020_blank_index_for.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0021_table_nrows.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0021_table_nrows.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0023_python3.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0023_python3.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0024_django2.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0024_django2.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0025_add_published_updated.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0025_add_published_updated.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0026_add_creators_and_contributors.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0026_add_creators_and_contributors.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0027_auto_20201202_1625.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0027_auto_20201202_1625.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0028_add_related_identifiers.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0028_add_related_identifiers.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0029_alter_ids.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0029_alter_ids.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0030_move_licenses_to_settings.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0030_move_licenses_to_settings.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0031_change_order.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0031_change_order.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0032_data_migration.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0032_data_migration.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/migrations/0033_refactor_fields.py` & `django-daiquiri-0.4.3/daiquiri/metadata/migrations/0033_refactor_fields.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/models.py` & `django-daiquiri-0.4.3/daiquiri/metadata/models.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/serializers/__init__.py` & `django-daiquiri-0.4.3/daiquiri/metadata/serializers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from django.conf import settings
 from django.contrib.auth.models import Group
 
 from daiquiri.core.serializers import JSONListField
 
 from rest_framework import serializers
 
+from .validators import PersonListValidator
 from ..models import Schema, Table, Column, Function
 
 
 class GroupSerializer(serializers.ModelSerializer):
 
     class Meta:
         model = Group
@@ -56,28 +57,28 @@
 
 
 class TableSerializer(serializers.ModelSerializer):
 
     label = serializers.CharField(source='__str__', read_only=True)
 
     related_identifiers = JSONListField(required=False)
-    creators = JSONListField(required=False)
-    contributors = JSONListField(required=False)
+    creators = JSONListField(required=False, validators=[PersonListValidator()])
+    contributors = JSONListField(required=False, validators=[PersonListValidator()])
     license = serializers.ChoiceField(choices=settings.LICENSE_CHOICES, default='')
 
     class Meta:
         model = Table
         fields = '__all__'
 
 
 class SchemaSerializer(serializers.ModelSerializer):
 
     label = serializers.CharField(source='__str__', read_only=True)
 
     related_identifiers = JSONListField(required=False)
-    creators = JSONListField(required=False)
-    contributors = JSONListField(required=False)
+    creators = JSONListField(required=False, validators=[PersonListValidator()])
+    contributors = JSONListField(required=False, validators=[PersonListValidator()])
     license = serializers.ChoiceField(choices=settings.LICENSE_CHOICES, default='', initial='')
 
     class Meta:
         model = Schema
         fields = '__all__'
```

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/serializers/datacite.py` & `django-daiquiri-0.4.3/daiquiri/metadata/serializers/datacite.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/serializers/dublincore.py` & `django-daiquiri-0.4.3/daiquiri/metadata/serializers/dublincore.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/serializers/export.py` & `django-daiquiri-0.4.3/daiquiri/metadata/serializers/export.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/serializers/management.py` & `django-daiquiri-0.4.3/daiquiri/metadata/serializers/management.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/serializers/user.py` & `django-daiquiri-0.4.3/daiquiri/metadata/serializers/user.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/settings.py` & `django-daiquiri-0.4.3/daiquiri/metadata/settings.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/css/metadata.scss` & `django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/css/metadata.scss`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by.png` & `django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/img/by.png`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by_nc.png` & `django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/img/by_nc.png`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by_nc_nd.png` & `django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/img/by_nc_nd.png`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by_nc_sa.png` & `django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/img/by_nc_sa.png`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by_nd.png` & `django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/img/by_nd.png`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/by_sa.png` & `django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/img/by_sa.png`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/cc0.png` & `django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/img/cc0.png`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/nc.png` & `django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/img/nc.png`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/nd.png` & `django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/img/nd.png`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/pd.png` & `django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/img/pd.png`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/img/sa.png` & `django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/img/sa.png`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/static/metadata/js/metadata.js` & `django-daiquiri-0.4.3/daiquiri/metadata/static/metadata/js/metadata.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -62,16 +62,15 @@
                 };
             },
             persons: function() {
                 return {
                     name: '',
                     first_name: '',
                     last_name: '',
-                    orcid: '',
-                    affiliations: ''
+                    orcid: ''
                 }
             }
         };
 
         /* define service functions */
 
         service.init = function() {
```

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management.html` & `django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_display.html` & `django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_display.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_delete_columns.html` & `django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_delete_columns.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_delete_functions.html` & `django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_delete_functions.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_delete_schemas.html` & `django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_delete_schemas.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_delete_tables.html` & `django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_delete_tables.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_columns.html` & `django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_form_columns.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_functions.html` & `django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_form_functions.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_schemas.html` & `django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_form_schemas.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_schemas_attribution.html` & `django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_form_schemas_attribution.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_schemas_creators.html` & `django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_form_schemas_creators.html`

 * *Files 13% similar despite different names*

```diff
@@ -14,48 +14,42 @@
 
                 <div class="modal-body">
                     <div class="daiquiri-metadata-modal-person"
                         ng-repeat="creator in service.values.creators">
 
                         <div class="row">
                             <formgroup
-                                class="col-md-3"
+                                class="col-md-4"
                                 data-type="text"
                                 data-label="{% trans 'Name' %}"
                                 data-model="creator.name">
                             </formgroup>
                             <formgroup
-                                class="col-md-3"
+                                class="col-md-4"
                                 data-type="text"
                                 data-label="{% trans 'First name' %}"
                                 data-model="creator.first_name">
                             </formgroup>
                             <formgroup
-                                class="col-md-3"
+                                class="col-md-4"
                                 data-type="text"
                                 data-label="{% trans 'Last name' %}"
                                 data-model="creator.last_name">
                             </formgroup>
+                        </div>
+                        <div class="row">
                             <formgroup
-                                class="col-md-3"
+                                class="col-md-4"
                                 data-type="text"
                                 data-label="{% trans 'ORCID' %}"
                                 data-model="creator.orcid">
                             </formgroup>
-                        </div>
-                        <div class="row">
-                            <div class="col-md-9">
-                               <formgroup
-                                    data-type="textareasplit"
-                                    data-label="{% trans 'Affiliations' %}"
-                                    data-help="{% trans 'Seperate multiple affiliations by newlines' %}"
-                                    data-model="creator.affiliations">
-                                </formgroup>
+                            <div class="col-md-4">
                             </div>
-                            <div class="col-md-3">
+                            <div class="col-md-4">
                                 <button type="button" class="btn btn-danger form-inline-button"
                                     ng-click="service.removePerson('creators', $index)">
 
                                     {% trans 'Remove creator' %}
                                 </button>
                             </div>
                         </div>
```

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_schemas_description.html` & `django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_form_schemas_description.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_tables.html` & `django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_form_tables.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_tables_attribution.html` & `django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_form_tables_attribution.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_tables_contributors.html` & `django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_form_schemas_contributors.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,55 @@
 {% load i18n %}
 
-    <div class="modal" id="tables-contributors-form-modal" tabindex="-1">
+    <div class="modal" id="schemas-contributors-form-modal" tabindex="-1">
         <div class="modal-dialog modal-lg">
             <div class="modal-content">
                 <div class="modal-header">
                     <button type="button" class="close" data-dismiss="modal" tabindex="-1">
                         <span aria-hidden="true">&times;</span>
                     </button>
                     <h4 class="modal-title">
-                        {% trans 'Update table contributors' %}
+                        {% trans 'Update schema contributors' %}
                     </h4>
                 </div>
 
                 <div class="modal-body">
                     <div class="daiquiri-metadata-modal-person"
                         ng-repeat="contributor in service.values.contributors">
 
                         <div class="row">
                             <formgroup
-                                class="col-md-3"
+                                class="col-md-4"
                                 data-type="text"
                                 data-label="{% trans 'Name' %}"
                                 data-model="contributor.name">
                             </formgroup>
                             <formgroup
-                                class="col-md-3"
+                                class="col-md-4"
                                 data-type="text"
                                 data-label="{% trans 'First name' %}"
                                 data-model="contributor.first_name">
                             </formgroup>
                             <formgroup
-                                class="col-md-3"
+                                class="col-md-4"
                                 data-type="text"
                                 data-label="{% trans 'Last name' %}"
                                 data-model="contributor.last_name">
                             </formgroup>
+                        </div>
+                        <div class="row">
                             <formgroup
-                                class="col-md-3"
+                                class="col-md-4"
                                 data-type="text"
                                 data-label="{% trans 'ORCID' %}"
                                 data-model="contributor.orcid">
                             </formgroup>
-                        </div>
-                        <div class="row">
-                            <div class="col-md-9">
-                               <formgroup
-                                    data-type="textareasplit"
-                                    data-label="{% trans 'Affiliations' %}"
-                                    data-help="{% trans 'Seperate multiple affiliations by newlines' %}"
-                                    data-model="contributor.affiliations">
-                                </formgroup>
+                            <div class="col-md-4">
                             </div>
-                            <div class="col-md-3">
+                            <div class="col-md-4">
                                 <button type="button" class="btn btn-danger form-inline-button"
                                     ng-click="service.removePerson('contributors', $index)">
 
                                     {% trans 'Remove contributor' %}
                                 </button>
                             </div>
                         </div>
@@ -67,14 +61,14 @@
                 </div>
 
                 <div class="modal-footer">
                     <button type="button" class="btn btn-default" data-dismiss="modal">
                         {% trans 'Close' %}
                     </button>
                     <button type="button" class="btn btn-primary"
-                            ng-click="service.submitFormModal('tables')">
+                            ng-click="service.submitFormModal('schemas')">
                         {% trans 'Save' %}
                     </button>
                 </div>
             </div>
         </div>
     </div>
```

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_tables_creators.html` & `django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_form_tables_creators.html`

 * *Files 24% similar despite different names*

```diff
@@ -14,48 +14,42 @@
 
                 <div class="modal-body">
                     <div class="daiquiri-metadata-modal-person"
                         ng-repeat="creator in service.values.creators">
 
                         <div class="row">
                             <formgroup
-                                class="col-md-3"
+                                class="col-md-4"
                                 data-type="text"
                                 data-label="{% trans 'Name' %}"
                                 data-model="creator.name">
                             </formgroup>
                             <formgroup
-                                class="col-md-3"
+                                class="col-md-4"
                                 data-type="text"
                                 data-label="{% trans 'First name' %}"
                                 data-model="creator.first_name">
                             </formgroup>
                             <formgroup
-                                class="col-md-3"
+                                class="col-md-4"
                                 data-type="text"
                                 data-label="{% trans 'Last name' %}"
                                 data-model="creator.last_name">
                             </formgroup>
+                        </div>
+                        <div class="row">
                             <formgroup
-                                class="col-md-3"
+                                class="col-md-4"
                                 data-type="text"
                                 data-label="{% trans 'ORCID' %}"
                                 data-model="creator.orcid">
                             </formgroup>
-                        </div>
-                        <div class="row">
-                            <div class="col-md-9">
-                               <formgroup
-                                    data-type="textareasplit"
-                                    data-label="{% trans 'Affiliations' %}"
-                                    data-help="{% trans 'Seperate multiple affiliations by newlines' %}"
-                                    data-model="creator.affiliations">
-                                </formgroup>
+                            <div class="col-md-4">
                             </div>
-                            <div class="col-md-3">
+                            <div class="col-md-4">
                                 <button type="button" class="btn btn-danger form-inline-button"
                                     ng-click="service.removePerson('creators', $index)">
 
                                     {% trans 'Remove creator' %}
                                 </button>
                             </div>
                         </div>
```

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_modal_form_tables_description.html` & `django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_modal_form_tables_description.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/management_options.html` & `django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/management_options.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/schema.html` & `django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/schema.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/table.html` & `django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/table.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/templates/metadata/tags/license_panel.html` & `django-daiquiri-0.4.3/daiquiri/metadata/templates/metadata/tags/license_panel.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/templatetags/metadata_tags.py` & `django-daiquiri-0.4.3/daiquiri/metadata/templatetags/metadata_tags.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/tests/test_views.py` & `django-daiquiri-0.4.3/daiquiri/metadata/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/tests/test_viewset_column.py` & `django-daiquiri-0.4.3/daiquiri/metadata/tests/test_viewset_column.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/tests/test_viewset_function.py` & `django-daiquiri-0.4.3/daiquiri/metadata/tests/test_viewset_function.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/tests/test_viewset_schema.py` & `django-daiquiri-0.4.3/daiquiri/metadata/tests/test_viewset_schema.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/tests/test_viewset_table.py` & `django-daiquiri-0.4.3/daiquiri/metadata/tests/test_viewset_table.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/urls.py` & `django-daiquiri-0.4.3/daiquiri/metadata/urls.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/utils.py` & `django-daiquiri-0.4.3/daiquiri/metadata/utils.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/views.py` & `django-daiquiri-0.4.3/daiquiri/metadata/views.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/metadata/viewsets.py` & `django-daiquiri-0.4.3/daiquiri/metadata/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/oai/adapter.py` & `django-daiquiri-0.4.3/daiquiri/oai/adapter.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/oai/management/commands/rebuild_oai_schema.py` & `django-daiquiri-0.4.3/daiquiri/oai/management/commands/rebuild_oai_schema.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/oai/migrations/0001_initial.py` & `django-daiquiri-0.4.3/daiquiri/oai/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/oai/migrations/0002_resource_type.py` & `django-daiquiri-0.4.3/daiquiri/oai/migrations/0002_resource_type.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/oai/models.py` & `django-daiquiri-0.4.3/daiquiri/oai/models.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/oai/renderers.py` & `django-daiquiri-0.4.3/daiquiri/oai/renderers.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/oai/settings.py` & `django-daiquiri-0.4.3/daiquiri/oai/settings.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/oai/utils.py` & `django-daiquiri-0.4.3/daiquiri/oai/utils.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/oai/views.py` & `django-daiquiri-0.4.3/daiquiri/oai/views.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/admin.py` & `django-daiquiri-0.4.3/daiquiri/query/admin.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/apps.py` & `django-daiquiri-0.4.3/daiquiri/query/apps.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/filters.py` & `django-daiquiri-0.4.3/daiquiri/query/filters.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/handlers.py` & `django-daiquiri-0.4.3/daiquiri/query/handlers.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/management/commands/archive_query_jobs.py` & `django-daiquiri-0.4.3/daiquiri/query/management/commands/archive_query_jobs.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/management/commands/fix_query_jobs.py` & `django-daiquiri-0.4.3/daiquiri/query/management/commands/fix_query_jobs.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/management/commands/scrub_query_jobs.py` & `django-daiquiri-0.4.3/daiquiri/query/management/commands/scrub_query_jobs.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/management/commands/scrub_user_tables.py` & `django-daiquiri-0.4.3/daiquiri/query/management/commands/scrub_user_tables.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/migrations/0001_initial.py` & `django-daiquiri-0.4.3/daiquiri/query/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/migrations/0003_query_language_and_actual_query.py` & `django-daiquiri-0.4.3/daiquiri/query/migrations/0003_query_language_and_actual_query.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/migrations/0004_table_name.py` & `django-daiquiri-0.4.3/daiquiri/query/migrations/0004_table_name.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/migrations/0005_meta.py` & `django-daiquiri-0.4.3/daiquiri/query/migrations/0005_meta.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/migrations/0006_example.py` & `django-daiquiri-0.4.3/daiquiri/query/migrations/0006_example.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/migrations/0009_remove_choices.py` & `django-daiquiri-0.4.3/daiquiri/query/migrations/0009_remove_choices.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/migrations/0013_refactoring.py` & `django-daiquiri-0.4.3/daiquiri/query/migrations/0013_refactoring.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/migrations/0014_downloadjob.py` & `django-daiquiri-0.4.3/daiquiri/query/migrations/0014_downloadjob.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/migrations/0015_queryarchivejob.py` & `django-daiquiri-0.4.3/daiquiri/query/migrations/0015_queryarchivejob.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/migrations/0017_big_integer_fields.py` & `django-daiquiri-0.4.3/daiquiri/query/migrations/0017_big_integer_fields.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/migrations/0019_remove_sync_jobs.py` & `django-daiquiri-0.4.3/daiquiri/query/migrations/0019_remove_sync_jobs.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/migrations/0020_python3.py` & `django-daiquiri-0.4.3/daiquiri/query/migrations/0020_python3.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/migrations/0021_django2.py` & `django-daiquiri-0.4.3/daiquiri/query/migrations/0021_django2.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/migrations/0022_blank_fields.py` & `django-daiquiri-0.4.3/daiquiri/query/migrations/0022_blank_fields.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/migrations/0024_fix_jsonfield.py` & `django-daiquiri-0.4.3/daiquiri/query/migrations/0024_fix_jsonfield.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/migrations/0026_use_django_jsonfield.py` & `django-daiquiri-0.4.3/daiquiri/query/migrations/0026_use_django_jsonfield.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/migrations/0027_rename_job_to_query_job.py` & `django-daiquiri-0.4.3/daiquiri/query/migrations/0027_rename_job_to_query_job.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/models.py` & `django-daiquiri-0.4.3/daiquiri/query/models.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/process.py` & `django-daiquiri-0.4.3/daiquiri/query/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,16 +211,17 @@
 
 def process_display_columns(processor_display_columns):
     # process display_columns to expand *
     display_columns = []
     for processor_display_column, original_column in processor_display_columns:
         if processor_display_column == '*':
             schema_name, table_name, tmp = original_column
-            for column_name in DatabaseAdapter().fetch_column_names(schema_name, table_name):
-                display_columns.append((column_name, (schema_name, table_name, column_name)))
+            columns = Column.objects.filter(table__schema__name=schema_name).filter(table__name=table_name).order_by('order')
+            for column in columns:
+                display_columns.append((column.name, (schema_name, table_name, column.name)))
 
         else:
             display_columns.append((processor_display_column, original_column))
 
     # check for duplicate columns in display_columns
     seen = set()
     errors = []
```

### Comparing `django-daiquiri-0.4.2/daiquiri/query/serializers.py` & `django-daiquiri-0.4.3/daiquiri/query/serializers.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/settings.py` & `django-daiquiri-0.4.3/daiquiri/query/settings.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/static/query/css/query.scss` & `django-daiquiri-0.4.3/daiquiri/query/static/query/css/query.scss`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/static/query/js/apps/query.js` & `django-daiquiri-0.4.3/daiquiri/query/static/query/js/apps/query.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/static/query/js/downloads/archive.js` & `django-daiquiri-0.4.3/daiquiri/query/static/query/js/downloads/archive.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/static/query/js/dropdowns/simbad.js` & `django-daiquiri-0.4.3/daiquiri/query/static/query/js/dropdowns/simbad.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/static/query/js/dropdowns/vizier.js` & `django-daiquiri-0.4.3/daiquiri/query/static/query/js/dropdowns/vizier.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/static/query/js/forms/box.js` & `django-daiquiri-0.4.3/daiquiri/query/static/query/js/forms/box.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/static/query/js/forms/cone.js` & `django-daiquiri-0.4.3/daiquiri/query/static/query/js/forms/cone.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/static/query/js/forms/sql.js` & `django-daiquiri-0.4.3/daiquiri/query/static/query/js/forms/sql.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/static/query/js/forms/upload.js` & `django-daiquiri-0.4.3/daiquiri/query/static/query/js/forms/upload.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/static/query/js/services/download.js` & `django-daiquiri-0.4.3/daiquiri/query/static/query/js/services/download.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/static/query/js/services/examples.js` & `django-daiquiri-0.4.3/daiquiri/query/static/query/js/services/examples.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/static/query/js/services/jobs.js` & `django-daiquiri-0.4.3/daiquiri/query/static/query/js/services/jobs.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/static/query/js/services/plot.js` & `django-daiquiri-0.4.3/daiquiri/query/static/query/js/services/plot.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/static/query/js/services/query.js` & `django-daiquiri-0.4.3/daiquiri/query/static/query/js/services/query.js`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/tasks.py` & `django-daiquiri-0.4.3/daiquiri/query/tasks.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/examples.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/examples.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/examples_modal_delete.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/examples_modal_delete.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/examples_modal_form.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/examples_modal_form.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/jobs.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/jobs.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/jobs_modal_show_job.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/jobs_modal_show_job.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/query.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/query.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_download_archive.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/query_download_archive.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_download_table.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/query_download_table.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_dropdown_columns.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/query_dropdown_columns.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_dropdown_examples.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/query_dropdown_examples.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_dropdown_functions.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/query_dropdown_functions.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_dropdown_schemas.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/query_dropdown_schemas.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_dropdown_simbad.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/query_dropdown_simbad.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_dropdown_vizier.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/query_dropdown_vizier.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_form_box.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/query_form_box.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_form_cone.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/query_form_cone.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_form_sql.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/query_form_sql.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_form_upload.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/query_form_upload.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_modal_abort_job.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/query_modal_abort_job.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_modal_archive_job.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/query_modal_archive_job.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_modal_logout.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/query_modal_logout.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_modal_update_job.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/query_modal_update_job.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_overview.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/query_overview.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_plot.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/query_plot.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_plot_histogram.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/query_plot_histogram.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_plot_scatter.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/query_plot_scatter.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_plot_scatter_cmap.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/query_plot_scatter_cmap.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/templates/query/query_sidebar.html` & `django-daiquiri-0.4.3/daiquiri/query/templates/query/query_sidebar.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/tests/test_permissions.py` & `django-daiquiri-0.4.3/daiquiri/query/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/tests/test_views.py` & `django-daiquiri-0.4.3/daiquiri/query/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/tests/test_viewset_download.py` & `django-daiquiri-0.4.3/daiquiri/query/tests/test_viewset_download.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/tests/test_viewset_dropdown.py` & `django-daiquiri-0.4.3/daiquiri/query/tests/test_viewset_dropdown.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/tests/test_viewset_example.py` & `django-daiquiri-0.4.3/daiquiri/query/tests/test_viewset_example.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/tests/test_viewset_form.py` & `django-daiquiri-0.4.3/daiquiri/query/tests/test_viewset_form.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/tests/test_viewset_job.py` & `django-daiquiri-0.4.3/daiquiri/query/tests/test_viewset_job.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/tests/test_viewset_status.py` & `django-daiquiri-0.4.3/daiquiri/query/tests/test_viewset_status.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/urls.py` & `django-daiquiri-0.4.3/daiquiri/query/urls.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/utils.py` & `django-daiquiri-0.4.3/daiquiri/query/utils.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/validators.py` & `django-daiquiri-0.4.3/daiquiri/query/validators.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/views.py` & `django-daiquiri-0.4.3/daiquiri/query/views.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/query/viewsets.py` & `django-daiquiri-0.4.3/daiquiri/query/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/registry/serializers.py` & `django-daiquiri-0.4.3/daiquiri/registry/serializers.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/registry/templates/registry/root.html` & `django-daiquiri-0.4.3/daiquiri/registry/templates/registry/root.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/registry/urls.py` & `django-daiquiri-0.4.3/daiquiri/registry/urls.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/registry/views.py` & `django-daiquiri-0.4.3/daiquiri/registry/views.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/registry/vo.py` & `django-daiquiri-0.4.3/daiquiri/registry/vo.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/serve/tasks.py` & `django-daiquiri-0.4.3/daiquiri/serve/tasks.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/serve/templates/serve/table.html` & `django-daiquiri-0.4.3/daiquiri/serve/templates/serve/table.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/serve/tests/test_views.py` & `django-daiquiri-0.4.3/daiquiri/serve/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/serve/tests/test_viewsets.py` & `django-daiquiri-0.4.3/daiquiri/serve/tests/test_viewsets.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/serve/urls.py` & `django-daiquiri-0.4.3/daiquiri/serve/urls.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/serve/views.py` & `django-daiquiri-0.4.3/daiquiri/serve/views.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/serve/viewsets.py` & `django-daiquiri-0.4.3/daiquiri/serve/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/stats/migrations/0001_initial.py` & `django-daiquiri-0.4.3/daiquiri/stats/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/stats/migrations/0002_data_migration.py` & `django-daiquiri-0.4.3/daiquiri/stats/migrations/0002_data_migration.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/stats/migrations/0003_data_migration.py` & `django-daiquiri-0.4.3/daiquiri/stats/migrations/0003_data_migration.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/stats/migrations/0004_set_record_null.py` & `django-daiquiri-0.4.3/daiquiri/stats/migrations/0004_set_record_null.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/stats/models.py` & `django-daiquiri-0.4.3/daiquiri/stats/models.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/stats/templates/stats/management.html` & `django-daiquiri-0.4.3/daiquiri/stats/templates/stats/management.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/stats/views.py` & `django-daiquiri-0.4.3/daiquiri/stats/views.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/tap/constants.py` & `django-daiquiri-0.4.3/daiquiri/tap/constants.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/tap/management/commands/rebuild_tap_schema.py` & `django-daiquiri-0.4.3/daiquiri/tap/management/commands/rebuild_tap_schema.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/tap/management/commands/setup_tap_metadata.py` & `django-daiquiri-0.4.3/daiquiri/tap/management/commands/setup_tap_metadata.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/tap/migrations/0001_initial.py` & `django-daiquiri-0.4.3/daiquiri/tap/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/tap/migrations/0002_alter_ids.py` & `django-daiquiri-0.4.3/daiquiri/tap/migrations/0002_alter_ids.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/tap/models.py` & `django-daiquiri-0.4.3/daiquiri/tap/models.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/tap/serializers.py` & `django-daiquiri-0.4.3/daiquiri/tap/serializers.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/tap/templates/tap/examples.html` & `django-daiquiri-0.4.3/daiquiri/tap/templates/tap/examples.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/tap/templates/tap/root.html` & `django-daiquiri-0.4.3/daiquiri/tap/templates/tap/root.html`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/tap/tests/test_async.py` & `django-daiquiri-0.4.3/daiquiri/tap/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/tap/tests/test_sync.py` & `django-daiquiri-0.4.3/daiquiri/tap/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/tap/tests/test_views.py` & `django-daiquiri-0.4.3/daiquiri/tap/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/tap/urls.py` & `django-daiquiri-0.4.3/daiquiri/tap/urls.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/tap/utils.py` & `django-daiquiri-0.4.3/daiquiri/tap/utils.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/tap/views.py` & `django-daiquiri-0.4.3/daiquiri/tap/views.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/tap/vo.py` & `django-daiquiri-0.4.3/daiquiri/tap/vo.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/daiquiri/uws/urls.py` & `django-daiquiri-0.4.3/daiquiri/uws/urls.py`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/django_daiquiri.egg-info/PKG-INFO` & `django-daiquiri-0.4.3/django_daiquiri.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-daiquiri
-Version: 0.4.2
+Version: 0.4.3
 Summary: Daiquiri is a framework for the publication of scientific databases.
 Home-page: https://github.com/django-daiquiri/daiquiri
 Author: Jochen Klar
 Author-email: mail@jochenklar.de
 Maintainer: Jochen Klar
 Maintainer-email: mail@jochenklar.de
 License: Apache-2.0
```

### Comparing `django-daiquiri-0.4.2/django_daiquiri.egg-info/SOURCES.txt` & `django-daiquiri-0.4.3/django_daiquiri.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -412,14 +412,15 @@
 daiquiri/metadata/migrations/__init__.py
 daiquiri/metadata/serializers/__init__.py
 daiquiri/metadata/serializers/datacite.py
 daiquiri/metadata/serializers/dublincore.py
 daiquiri/metadata/serializers/export.py
 daiquiri/metadata/serializers/management.py
 daiquiri/metadata/serializers/user.py
+daiquiri/metadata/serializers/validators.py
 daiquiri/metadata/static/metadata/css/metadata.scss
 daiquiri/metadata/static/metadata/img/by.png
 daiquiri/metadata/static/metadata/img/by_nc.png
 daiquiri/metadata/static/metadata/img/by_nc_nd.png
 daiquiri/metadata/static/metadata/img/by_nc_sa.png
 daiquiri/metadata/static/metadata/img/by_nd.png
 daiquiri/metadata/static/metadata/img/by_sa.png
```

### Comparing `django-daiquiri-0.4.2/django_daiquiri.egg-info/requires.txt` & `django-daiquiri-0.4.3/django_daiquiri.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `django-daiquiri-0.4.2/setup.py` & `django-daiquiri-0.4.3/setup.py`

 * *Files identical despite different names*

