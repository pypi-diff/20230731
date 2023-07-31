# Comparing `tmp/vdk_jupyterlab_extension-0.1.947240835.tar.gz` & `tmp/vdk_jupyterlab_extension-0.1.950282415.tar.gz`

## Comparing `vdk_jupyterlab_extension-0.1.947240835.tar` & `vdk_jupyterlab_extension-0.1.950282415.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/.eslintignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/.eslintrc.js
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/.stylelintrc
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/babel.config.js
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/conftest.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/install.json
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/jest.config.js
--rw-r--r--   0        0        0   637378 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/package-lock.json
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/package.json
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/tsconfig.json
--rw-r--r--   0        0        0   425068 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/yarn.lock
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/jupyter-config/nb-config/vdk-jupyterlab-extension.json
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/jupyter-config/server-config/vdk-jupyterlab-extension.json
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/schema/plugin.json
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/commandsAndMenu.tsx
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/handler.ts
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/index.ts
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/initVDKConfigCell.ts
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/jobData.ts
--rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/serverRequests.ts
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/utils.ts
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/vdkTags.ts
--rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/__tests__/convert-job-to-notebook-component.spec.ts
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/__tests__/create-job-component.spec.ts
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/__tests__/deploy-job-component.spec.ts
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/__tests__/download-job-component.spec.ts
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/__tests__/handler.spec.ts
--rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/__tests__/resquests.spec.ts
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/__tests__/run-job-component.spec.tsx
--rw-r--r--   0        0        0     6907 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/__tests__/show-dialog.spec.tsx
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/__tests__/vdk-error-message.spec.ts
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/__tests__/vdk-jupyterlab-extension.spec.ts
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/__tests__/vdk-tags.spec.ts
--rw-r--r--   0        0        0    12078 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/components/ConvertJobToNotebook.tsx
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/components/CreateJob.tsx
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/components/DeployJob.tsx
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/components/DownloadJob.tsx
--rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/components/RunJob.tsx
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/components/VdkErrorMessage.ts
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/components/VdkTextInput.tsx
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/components/props.tsx
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/src/vdkOptions/vdk_options.ts
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/style/base.css
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/style/index.css
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/style/index.js
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/style/vdkDialogs.css
--rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/style/images/versatile-data-kit-logo.svg
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/testutils/jest-file-mock.js
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/testutils/jest-setup-files.js
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/ui-tests/README.md
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/ui-tests/package.json
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/ui-tests/playwright.config.js
--rw-r--r--   0        0        0     7410 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/ui-tests/tests/convert-job.spec.ts
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/ui-tests/tests/utils.ts
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/ui-tests/tests/vdk-jupyterlab-extension.spec.ts
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/ui-tests/tests/data/convert-test-job-dirty/10_drop_table.sql
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/ui-tests/tests/data/convert-test-job-dirty/20_create_table.sql
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/ui-tests/tests/data/convert-test-job-dirty/30_ingest_to_table.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/_version.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/convert_job.py
--rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/handlers.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/job_data.py
--rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/vdk_ui.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/jupyter_sample_job/README.md
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/jupyter_sample_job/config.ini
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/jupyter_sample_job/requirements.txt
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/package.json
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json
--rw-r--r--   0        0        0    21056 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/static/161.8695b9e5520bd63d9d87.js
--rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js
--rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/static/remoteEntry.f0c41c67a1da9120d996.js
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/tests/__init__.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/tests/test_convert_job_directory_processor.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/tests/test_directory_archiver.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/tests/test_handlers.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/vdk_options/__init__.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/vdk_options/vdk_options.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/LICENSE
--rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/README.md
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/pyproject.toml
--rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.947240835/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/.eslintignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/.eslintrc.js
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/.stylelintrc
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/babel.config.js
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/conftest.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/install.json
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/jest.config.js
+-rw-r--r--   0        0        0   637378 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/package-lock.json
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/package.json
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/tsconfig.json
+-rw-r--r--   0        0        0   425098 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/yarn.lock
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/jupyter-config/nb-config/vdk-jupyterlab-extension.json
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/jupyter-config/server-config/vdk-jupyterlab-extension.json
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/schema/plugin.json
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/commandsAndMenu.tsx
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/handler.ts
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/index.ts
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/initVDKConfigCell.ts
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/jobData.ts
+-rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/serverRequests.ts
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/utils.ts
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/vdkTags.ts
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/__tests__/convert-job-to-notebook-component.spec.ts
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/__tests__/create-job-component.spec.ts
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/__tests__/deploy-job-component.spec.ts
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/__tests__/download-job-component.spec.ts
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/__tests__/handler.spec.ts
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/__tests__/resquests.spec.ts
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/__tests__/run-job-component.spec.tsx
+-rw-r--r--   0        0        0     6907 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/__tests__/show-dialog.spec.tsx
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/__tests__/vdk-error-message.spec.ts
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/__tests__/vdk-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/__tests__/vdk-tags.spec.ts
+-rw-r--r--   0        0        0    12092 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/components/ConvertJobToNotebook.tsx
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/components/CreateJob.tsx
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/components/DeployJob.tsx
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/components/DownloadJob.tsx
+-rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/components/RunJob.tsx
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/components/VdkErrorMessage.ts
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/components/VdkTextInput.tsx
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/components/props.tsx
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/src/vdkOptions/vdk_options.ts
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/style/base.css
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/style/index.css
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/style/index.js
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/style/vdkDialogs.css
+-rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/style/images/versatile-data-kit-logo.svg
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/testutils/jest-file-mock.js
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/testutils/jest-setup-files.js
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/ui-tests/README.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/ui-tests/package.json
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/ui-tests/tests/convert-job.spec.ts
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/ui-tests/tests/utils.ts
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/ui-tests/tests/vdk-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/ui-tests/tests/data/convert-test-job-dirty/10_drop_table.sql
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/ui-tests/tests/data/convert-test-job-dirty/20_create_table.sql
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/ui-tests/tests/data/convert-test-job-dirty/30_ingest_to_table.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/_version.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/convert_job.py
+-rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/handlers.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/job_data.py
+-rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/vdk_ui.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/jupyter_sample_job/README.md
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/jupyter_sample_job/config.ini
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/jupyter_sample_job/requirements.txt
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/package.json
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json
+-rw-r--r--   0        0        0    21084 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/static/161.687b3e6d54b7501a02f7.js
+-rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js
+-rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/static/remoteEntry.74be29b03cb2d5a0e3ab.js
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/tests/__init__.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/tests/test_convert_job_directory_processor.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/tests/test_directory_archiver.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/tests/test_handlers.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/vdk_options/__init__.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/vdk_options/vdk_options.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/LICENSE
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/README.md
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/pyproject.toml
+-rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.950282415/PKG-INFO
```

### Comparing `vdk_jupyterlab_extension-0.1.947240835/.eslintrc.js` & `vdk_jupyterlab_extension-0.1.950282415/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/jest.config.js` & `vdk_jupyterlab_extension-0.1.950282415/jest.config.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/package-lock.json` & `vdk_jupyterlab_extension-0.1.950282415/package-lock.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/package.json` & `vdk_jupyterlab_extension-0.1.950282415/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.1.950282415'"}*

```diff
@@ -147,9 +147,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.947240835"
+    "version": "0.1.950282415"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.947240835/tsconfig.json` & `vdk_jupyterlab_extension-0.1.950282415/tsconfig.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/yarn.lock` & `vdk_jupyterlab_extension-0.1.950282415/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2077,18 +2077,18 @@
     typestyle "^2.0.4"
 
 "@lumino/algorithm@^1.9.0", "@lumino/algorithm@^1.9.1", "@lumino/algorithm@^1.9.2":
   version "1.9.2"
   resolved "https://registry.yarnpkg.com/@lumino/algorithm/-/algorithm-1.9.2.tgz#b95e6419aed58ff6b863a51bfb4add0f795141d3"
   integrity sha512-Z06lp/yuhz8CtIir3PNTGnuk7909eXt4ukJsCzChsGuot2l5Fbs96RJ/FOHgwCedaX74CtxPjXHXoszFbUA+4A==
 
-"@lumino/algorithm@^2.0.0":
-  version "2.0.0"
-  resolved "https://registry.yarnpkg.com/@lumino/algorithm/-/algorithm-2.0.0.tgz#f36e4b6bf6d2b9bde66dc3162afc9a0d2ef47530"
-  integrity sha512-SwM/8U1zlMWMJj00wTCThdTUit9zap2Xghuo4uUxvZ+mfog5b1UIk2j1dP8TPpzEXHCDPEb85s2/ERo1tee3Dw==
+"@lumino/algorithm@^2.0.1":
+  version "2.0.1"
+  resolved "https://registry.yarnpkg.com/@lumino/algorithm/-/algorithm-2.0.1.tgz#1045f4629f96076b431fc1a8c0005e13d8b95a56"
+  integrity sha512-iA+uuvA7DeNFB0/cQpIWNgO1c6z4pOSigifjstLy+rxf1U5ZzxIq+xudnEuTbWgKSTviG02j4cKwCyx1PO6rzA==
 
 "@lumino/application@^1.31.4":
   version "1.31.4"
   resolved "https://registry.yarnpkg.com/@lumino/application/-/application-1.31.4.tgz#b804fcc46fb77deb41aee94c48bea990f735d6b9"
   integrity sha512-dOSsDJ1tXOxC3fnSHvtDQK5RcICLEVPtO19HeCGwurb5W2ZZ55SZT2b5jZu6V/v8lGdtkNbr1RJltRpJRSRb/A==
   dependencies:
     "@lumino/commands" "^1.21.1"
@@ -2116,33 +2116,33 @@
     "@lumino/virtualdom" "^1.14.3"
 
 "@lumino/coreutils@^1.11.0", "@lumino/coreutils@^1.12.0", "@lumino/coreutils@^1.12.1":
   version "1.12.1"
   resolved "https://registry.yarnpkg.com/@lumino/coreutils/-/coreutils-1.12.1.tgz#79860c9937483ddf6cda87f6c2b9da8eb1a5d768"
   integrity sha512-JLu3nTHzJk9N8ohZ85u75YxemMrmDzJdNgZztfP7F7T7mxND3YVNCkJG35a6aJ7edu1sIgCjBxOvV+hv27iYvQ==
 
-"@lumino/coreutils@^1.11.0 || ^2.0.0-alpha.6", "@lumino/coreutils@^2.1.1":
-  version "2.1.1"
-  resolved "https://registry.yarnpkg.com/@lumino/coreutils/-/coreutils-2.1.1.tgz#e867a501f3564987a757005c81aa4b0d4ea5ff4c"
-  integrity sha512-OmEzvphZC/EVpFfwBkmcuzNwKXvkij6gJo1mbf4/tZMC1/8NO3aVnjK1FsgC0TlaGwMD1BLIFgGay2mC/I/cyQ==
+"@lumino/coreutils@^1.11.0 || ^2.0.0-alpha.6", "@lumino/coreutils@^2.1.1", "@lumino/coreutils@^2.1.2":
+  version "2.1.2"
+  resolved "https://registry.yarnpkg.com/@lumino/coreutils/-/coreutils-2.1.2.tgz#354e658353e99969329c9ee33b0692ecd97abe1f"
+  integrity sha512-vyz7WzchTO4HQ8iVAxvSUmb5o/8t3cz1vBo8V4ZIaPGada0Jx0xe3tKQ8bXp4pjHc+AEhMnkCnlUyVYMWbnj4A==
 
 "@lumino/disposable@^1.10.0", "@lumino/disposable@^1.10.1", "@lumino/disposable@^1.10.4":
   version "1.10.4"
   resolved "https://registry.yarnpkg.com/@lumino/disposable/-/disposable-1.10.4.tgz#73b452044fecf988d7fa73fac9451b1a7f987323"
   integrity sha512-4ZxyYcyzUS+ZeB2KAH9oAH3w0DUUceiVr+FIZHZ2TAYGWZI/85WlqJtfm0xjwEpCwLLW1TDqJrISuZu3iMmVMA==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
     "@lumino/signaling" "^1.11.1"
 
 "@lumino/disposable@^1.10.0 || ^2.0.0-alpha.6":
-  version "2.1.1"
-  resolved "https://registry.yarnpkg.com/@lumino/disposable/-/disposable-2.1.1.tgz#9c6dace68320538532ebd4fb91b159c532baf62e"
-  integrity sha512-zGl5hDDgDgPlrCN8b37gmNRjmYrTXnVq4WaseRtEgjj/en+gHLQW7sgTzkLgPj5rFaVETPkyrDTQ5uZVewFOAw==
+  version "2.1.2"
+  resolved "https://registry.yarnpkg.com/@lumino/disposable/-/disposable-2.1.2.tgz#a4df34a50d23e577051eee27c000fc9ad37f35bb"
+  integrity sha512-0qmB6zPt9+uj4SVMTfISn0wUOjYHahtKotwxDD5flfcscj2gsXaFCXO4Oqot1zcsZbg8uJmTUhEzAvFW0QhFNA==
   dependencies:
-    "@lumino/signaling" "^2.1.1"
+    "@lumino/signaling" "^2.1.2"
 
 "@lumino/domutils@^1.8.0", "@lumino/domutils@^1.8.1", "@lumino/domutils@^1.8.2":
   version "1.8.2"
   resolved "https://registry.yarnpkg.com/@lumino/domutils/-/domutils-1.8.2.tgz#d15cdbae12bea52852bbc13c4629360f9f05b7f5"
   integrity sha512-QIpMfkPJrs4GrWBuJf2Sn1fpyVPmvqUUAeD8xAQo8+4V5JAT0vUDLxZ9HijefMgNCi3+Bs8Z3lQwRCrz+cFP1A==
 
 "@lumino/dragdrop@^1.13.0", "@lumino/dragdrop@^1.14.0", "@lumino/dragdrop@^1.14.5":
@@ -2184,21 +2184,21 @@
   version "1.11.1"
   resolved "https://registry.yarnpkg.com/@lumino/signaling/-/signaling-1.11.1.tgz#438f447a1b644fd286549804f9851b5aec9679a2"
   integrity sha512-YCUmgw08VoyMN5KxzqPO3KMx+cwdPv28tAN06C0K7Q/dQf+oufb1XocuhZb5selTrTmmuXeizaYxgLIQGdS1fA==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
     "@lumino/properties" "^1.8.2"
 
-"@lumino/signaling@^1.10.0 || ^2.0.0-alpha.6", "@lumino/signaling@^2.1.1":
-  version "2.1.1"
-  resolved "https://registry.yarnpkg.com/@lumino/signaling/-/signaling-2.1.1.tgz#aae22e4cfb8f99baaa54cefaf1555be2c4148f0f"
-  integrity sha512-EUPJlC/kis5DEPA4UxsJRPidGk4qcgS+rfQlYfGfA4Z6vR8nzcwU9WE0UIWdqo6GN7cLWR8lGLzZzyIGY3+qiA==
+"@lumino/signaling@^1.10.0 || ^2.0.0-alpha.6", "@lumino/signaling@^2.1.2":
+  version "2.1.2"
+  resolved "https://registry.yarnpkg.com/@lumino/signaling/-/signaling-2.1.2.tgz#b5f127463165884174f1446e8364794af831a852"
+  integrity sha512-KtwKxx+xXkLOX/BdSqtvnsqBTPKDIENFBKeYkMTxstQc3fHRmyTzmaVoeZES+pr1EUy3e8vM4pQFVQpb8VsDdA==
   dependencies:
-    "@lumino/algorithm" "^2.0.0"
-    "@lumino/coreutils" "^2.1.1"
+    "@lumino/algorithm" "^2.0.1"
+    "@lumino/coreutils" "^2.1.2"
 
 "@lumino/virtualdom@^1.14.0", "@lumino/virtualdom@^1.14.1", "@lumino/virtualdom@^1.14.3":
   version "1.14.3"
   resolved "https://registry.yarnpkg.com/@lumino/virtualdom/-/virtualdom-1.14.3.tgz#e490c36ff506d877cf45771d6968e3e26a8919fd"
   integrity sha512-5joUC1yuxeXbpfbSBm/OR8Mu9HoTo6PDX0RKqzlJ9o97iml7zayFN/ynzcxScKGQAo9iaXOY8uVIvGUT8FnsGw==
   dependencies:
     "@lumino/algorithm" "^1.9.2"
@@ -3188,21 +3188,21 @@
 
 browser-process-hrtime@^1.0.0:
   version "1.0.0"
   resolved "https://registry.yarnpkg.com/browser-process-hrtime/-/browser-process-hrtime-1.0.0.tgz#3c9b4b7d782c8121e56f10106d84c0d0ffc94626"
   integrity sha512-9o5UecI3GhkpM6DrXr69PblIuWxPKk9Y0jHBRhdocZ2y7YECBFCsHm79Pr3OyR2AvjhDkabFJaDJMYRazHgsow==
 
 browserslist@^4.1.0, browserslist@^4.14.5, browserslist@^4.21.9:
-  version "4.21.9"
-  resolved "https://registry.yarnpkg.com/browserslist/-/browserslist-4.21.9.tgz#e11bdd3c313d7e2a9e87e8b4b0c7872b13897635"
-  integrity sha512-M0MFoZzbUrRU4KNfCrDLnvyE7gub+peetoTid3TBIqtunaDJyXlwhakT+/VkvSXcfIzFfK/nkCs4nmyTmxdNSg==
-  dependencies:
-    caniuse-lite "^1.0.30001503"
-    electron-to-chromium "^1.4.431"
-    node-releases "^2.0.12"
+  version "4.21.10"
+  resolved "https://registry.yarnpkg.com/browserslist/-/browserslist-4.21.10.tgz#dbbac576628c13d3b2231332cb2ec5a46e015bb0"
+  integrity sha512-bipEBdZfVH5/pwrvqc+Ub0kUPVfGUhlKxbvfD+z1BDnPEO/X98ruXGA1WP5ASpAFKan7Qr6j736IacbZQuAlKQ==
+  dependencies:
+    caniuse-lite "^1.0.30001517"
+    electron-to-chromium "^1.4.477"
+    node-releases "^2.0.13"
     update-browserslist-db "^1.0.11"
 
 bs-logger@0.x:
   version "0.2.6"
   resolved "https://registry.yarnpkg.com/bs-logger/-/bs-logger-0.2.6.tgz#eb7d365307a72cf974cc6cda76b68354ad336bd8"
   integrity sha512-pd8DCoxmbgc7hyPKOvxtqNcjYoOsABPQdcCUjGp3d42VR2CX1ORhk2A87oqqu5R1kk+76nsxZupkmyd+MVtCog==
   dependencies:
@@ -3303,15 +3303,15 @@
   integrity sha512-L28STB170nwWS63UjtlEOE3dldQApaJXZkOI1uMFfzf3rRuPegHaHesyee+YxQ+W6SvRDQV6UrdOdRiR153wJg==
 
 camelcase@^6.0.0, camelcase@^6.2.0:
   version "6.3.0"
   resolved "https://registry.yarnpkg.com/camelcase/-/camelcase-6.3.0.tgz#5685b95eb209ac9c0c177467778c9c84df58ba9a"
   integrity sha512-Gmy6FhYlCY7uOElZUSbxo2UCDH8owEk996gkbrpsgGtrJLM3J7jGxl9Ic7Qwwj4ivOE5AWZWRMecDdF7hqGjFA==
 
-caniuse-lite@^1.0.30001503:
+caniuse-lite@^1.0.30001517:
   version "1.0.30001517"
   resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001517.tgz#90fabae294215c3495807eb24fc809e11dc2f0a8"
   integrity sha512-Vdhm5S11DaFVLlyiKu4hiUTkpZu+y1KA/rZZqVQfOD5YdDT/eQKlkt7NaE0WGOFgX32diqt9MiP9CAiFeRklaA==
 
 capture-exit@^2.0.0:
   version "2.0.0"
   resolved "https://registry.yarnpkg.com/capture-exit/-/capture-exit-2.0.0.tgz#fb953bfaebeb781f62898239dabb426d08a509a4"
@@ -3567,17 +3567,17 @@
 
 copy-descriptor@^0.1.0:
   version "0.1.1"
   resolved "https://registry.yarnpkg.com/copy-descriptor/-/copy-descriptor-0.1.1.tgz#676f6eb3c39997c2ee1ac3a924fd6124748f578d"
   integrity sha512-XgZ0pFcakEUlbwQEVNg3+QAis1FyTL3Qel9FYy8pSkQqoG3PNoT0bOCQtOXcOkur21r2Eq2kI+IE+gsmAEVlYw==
 
 core-js-pure@^3.6.5:
-  version "3.31.1"
-  resolved "https://registry.yarnpkg.com/core-js-pure/-/core-js-pure-3.31.1.tgz#73d154958881873bc19381df80bddb20c8d0cdb5"
-  integrity sha512-w+C62kvWti0EPs4KPMCMVv9DriHSXfQOCQ94bGGBiEW5rrbtt/Rz8n5Krhfw9cpFyzXBjf3DB3QnPdEzGDY4Fw==
+  version "3.32.0"
+  resolved "https://registry.yarnpkg.com/core-js-pure/-/core-js-pure-3.32.0.tgz#5d79f85da7a4373e9a06494ccbef995a4c639f8b"
+  integrity sha512-qsev1H+dTNYpDUEURRuOXMvpdtAnNEvQWS/FMJ2Vb5AY8ZP4rAPQldkE27joykZPJTe0+IVgHZYh1P5Xu1/i1g==
 
 cosmiconfig@^7.0.1:
   version "7.1.0"
   resolved "https://registry.yarnpkg.com/cosmiconfig/-/cosmiconfig-7.1.0.tgz#1443b9afa596b670082ea46cbd8f6a62b84635f6"
   integrity sha512-AdmX6xUzdNASswsFtmwSt7Vj8po9IuqXm0UXz7QKPuEUmPB4XyjGfaAr2PSuELMwkRMVH1EpIkX5bTZGRB3eCA==
   dependencies:
     "@types/parse-json" "^4.0.0"
@@ -3895,18 +3895,18 @@
   integrity sha512-aO50/qPC7X2ChjRFniRiscxBLT/K01bALqfcDaf8Ih5OqQ1N4iT/Abx9Ofu3/ms446vHTm46FACIuJUmgUQcDQ==
   dependencies:
     chalk "^2.3.0"
     find-root "^1.0.0"
     lodash "^4.17.4"
     semver "^5.4.1"
 
-electron-to-chromium@^1.4.431:
-  version "1.4.473"
-  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.473.tgz#4853de13a335c70fe1f9df8d4029be54068767d1"
-  integrity sha512-aVfC8+440vGfl06l8HKKn8/PD5jRfSnLkTTD65EFvU46igbpQRri1gxSzW9/+TeUlwYzrXk1sw867T96zlyECA==
+electron-to-chromium@^1.4.477:
+  version "1.4.477"
+  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.477.tgz#05669aa6f161ee9076a6805457e9bd9fe6d0dfd1"
+  integrity sha512-shUVy6Eawp33dFBFIoYbIwLHrX0IZ857AlH9ug2o4rvbWmpaCUdBpQ5Zw39HRrfzAFm4APJE9V+E2A/WB0YqJw==
 
 emittery@^0.7.1:
   version "0.7.2"
   resolved "https://registry.yarnpkg.com/emittery/-/emittery-0.7.2.tgz#25595908e13af0f5674ab419396e2fb394cdfa82"
   integrity sha512-A8OG5SR/ij3SsJdWDJdkkSYUjQdCUx6APQXem0SaEePBSRg4eymGYwBkKo1Y6DU+af/Jn2dBQqDBvjnr9Vi8nQ==
 
 emittery@^0.8.1:
@@ -3951,17 +3951,17 @@
   resolved "https://registry.yarnpkg.com/enhanced-resolve/-/enhanced-resolve-5.15.0.tgz#1af946c7d93603eb88e9896cee4904dc012e9c35"
   integrity sha512-LXYT42KJ7lpIKECr2mAXIaMldcNCh/7E0KBKOu4KSfkHmP+mZmSs+8V5gBAqisWBy0OO4W5Oyys0GO1Y8KtdKg==
   dependencies:
     graceful-fs "^4.2.4"
     tapable "^2.2.0"
 
 enquirer@^2.3.5:
-  version "2.4.0"
-  resolved "https://registry.yarnpkg.com/enquirer/-/enquirer-2.4.0.tgz#4f36f6c644137cc4fd2891da407ede2b1fea904a"
-  integrity sha512-ehu97t6FTYK2I3ZYtnp0BZ9vt0mvEL/cnHBds7Ct6jo9VX1VIkiFhOvVRWh6eblQqd7KOoICIQV+syZ3neXO/Q==
+  version "2.4.1"
+  resolved "https://registry.yarnpkg.com/enquirer/-/enquirer-2.4.1.tgz#93334b3fbd74fc7097b224ab4a8fb7e40bf4ae56"
+  integrity sha512-rRqJg/6gd538VHvR3PSrdRBb/1Vy2YfzHqzvbhGIQpDRKIa4FgV/54b5Q1xYSxOOwKvjXweS26E0Q+nAMwp2pQ==
   dependencies:
     ansi-colors "^4.1.1"
     strip-ansi "^6.0.1"
 
 entities@^2.0.0:
   version "2.2.0"
   resolved "https://registry.yarnpkg.com/entities/-/entities-2.2.0.tgz#098dc90ebb83d8dffa089d55256b351d34c4da55"
@@ -6993,15 +6993,15 @@
     growly "^1.3.0"
     is-wsl "^2.2.0"
     semver "^7.3.2"
     shellwords "^0.1.1"
     uuid "^8.3.0"
     which "^2.0.2"
 
-node-releases@^2.0.12:
+node-releases@^2.0.13:
   version "2.0.13"
   resolved "https://registry.yarnpkg.com/node-releases/-/node-releases-2.0.13.tgz#d5ed1627c23e3461e819b02e57b75e4899b1c81d"
   integrity sha512-uYr7J37ae/ORWdZeQ1xxMJe3NtdmqMC/JZK+geofDrkLUApKRHPd18/TxtBOJ4A0/+uUIliorNrfYV6s1b02eQ==
 
 normalize-package-data@^2.3.2, normalize-package-data@^2.5.0:
   version "2.5.0"
   resolved "https://registry.yarnpkg.com/normalize-package-data/-/normalize-package-data-2.5.0.tgz#e66db1838b200c1dfc233225d12cb36520e234a8"
```

### Comparing `vdk_jupyterlab_extension-0.1.947240835/schema/plugin.json` & `vdk_jupyterlab_extension-0.1.950282415/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/commandsAndMenu.tsx` & `vdk_jupyterlab_extension-0.1.950282415/src/commandsAndMenu.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/handler.ts` & `vdk_jupyterlab_extension-0.1.950282415/src/handler.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/index.ts` & `vdk_jupyterlab_extension-0.1.950282415/src/index.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/initVDKConfigCell.ts` & `vdk_jupyterlab_extension-0.1.950282415/src/initVDKConfigCell.ts`

 * *Files 7% similar despite different names*

```diff
@@ -13,26 +13,26 @@
   if (notebookPanel) {
     const initCell =
       notebookPanel.content.model?.contentFactory?.createCodeCell({
         cell: {
           cell_type: 'code',
           source: [
             `"""\n`,
-            `vdk_ipython extension introduces a magic command for Jupyter.\n`,
+            `vdk.plugin.ipython extension introduces a magic command for Jupyter.\n`,
             `The command enables the user to load VDK for the current notebook.\n`,
             `VDK provides the job_input API, which has methods for:\n`,
             `    * executing queries to an OLAP database;\n`,
             `    * ingesting data into a database;\n`,
             `    * processing data into a database.\n`,
             `See the IJobInput documentation for more details.\n`,
             `https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-core/src/vdk/api/job_input.py\n`,
             `Please refrain from tagging this cell with VDK as it is not an actual part of the data job\n`,
             `and is only used for development purposes.\n`,
             `"""\n`,
-            `%reload_ext vdk_ipython\n`,
+            `%reload_ext vdk.plugin.ipython\n`,
             `%reload_VDK\n`,
             `job_input = VDK.get_initialized_job_input()`
           ],
           metadata: {}
         }
       });
     const cells = notebookTracker.currentWidget?.content.model?.cells;
```

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/jobData.ts` & `vdk_jupyterlab_extension-0.1.950282415/src/jobData.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/serverRequests.ts` & `vdk_jupyterlab_extension-0.1.950282415/src/serverRequests.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/vdkTags.ts` & `vdk_jupyterlab_extension-0.1.950282415/src/vdkTags.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/__tests__/convert-job-to-notebook-component.spec.ts` & `vdk_jupyterlab_extension-0.1.950282415/src/__tests__/convert-job-to-notebook-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/__tests__/create-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.950282415/src/__tests__/create-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/__tests__/deploy-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.950282415/src/__tests__/deploy-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/__tests__/download-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.950282415/src/__tests__/download-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/__tests__/handler.spec.ts` & `vdk_jupyterlab_extension-0.1.950282415/src/__tests__/handler.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/__tests__/resquests.spec.ts` & `vdk_jupyterlab_extension-0.1.950282415/src/__tests__/resquests.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/__tests__/run-job-component.spec.tsx` & `vdk_jupyterlab_extension-0.1.950282415/src/__tests__/run-job-component.spec.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/__tests__/show-dialog.spec.tsx` & `vdk_jupyterlab_extension-0.1.950282415/src/__tests__/show-dialog.spec.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/__tests__/vdk-error-message.spec.ts` & `vdk_jupyterlab_extension-0.1.950282415/src/__tests__/vdk-error-message.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/__tests__/vdk-tags.spec.ts` & `vdk_jupyterlab_extension-0.1.950282415/src/__tests__/vdk-tags.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/components/ConvertJobToNotebook.tsx` & `vdk_jupyterlab_extension-0.1.950282415/src/components/ConvertJobToNotebook.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -250,26 +250,26 @@
           "* *Before running the job, it is recommended to review the cells\n",
           "    to ensure a clear understanding of the data job run.  \n",
           "    This will help to ensure the desired outcome.* "
         ]);
 
         addCodeCell([
           `"""\n`,
-          `vdk_ipython extension introduces a magic command for Jupyter.\n`,
+          `vdk.plugin.ipython extension introduces a magic command for Jupyter.\n`,
           `The command enables the user to load VDK for the current notebook.\n`,
           `VDK provides the job_input API, which has methods for:\n`,
           `    * executing queries to an OLAP database;\n`,
           `    * ingesting data into a database;\n`,
           `    * processing data into a database.\n`,
           `See the IJobInput documentation for more details.\n`,
           `https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-core/src/vdk/api/job_input.py\n`,
           `Please refrain from tagging this cell with VDK as it is not an actual part of the data job\n`,
           `and is only used for development purposes.\n`,
           `"""\n`,
-          `%reload_ext vdk_ipython\n`,
+          `%reload_ext vdk.plugin.ipython\n`,
           `%reload_VDK\n`,
           `job_input = VDK.get_initialized_job_input()`
         ], {})
 
         // add code that came from the previous version of the job and the names of the files where they came from
         for (const cellProps of notebookContent) {
           if (cellProps.type === 'markdown') {
```

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/components/CreateJob.tsx` & `vdk_jupyterlab_extension-0.1.950282415/src/components/CreateJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/components/DeployJob.tsx` & `vdk_jupyterlab_extension-0.1.950282415/src/components/DeployJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/components/DownloadJob.tsx` & `vdk_jupyterlab_extension-0.1.950282415/src/components/DownloadJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/components/RunJob.tsx` & `vdk_jupyterlab_extension-0.1.950282415/src/components/RunJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/components/VdkErrorMessage.ts` & `vdk_jupyterlab_extension-0.1.950282415/src/components/VdkErrorMessage.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/src/components/VdkTextInput.tsx` & `vdk_jupyterlab_extension-0.1.950282415/src/components/VdkTextInput.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/style/base.css` & `vdk_jupyterlab_extension-0.1.950282415/style/base.css`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/style/vdkDialogs.css` & `vdk_jupyterlab_extension-0.1.950282415/style/vdkDialogs.css`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/style/images/versatile-data-kit-logo.svg` & `vdk_jupyterlab_extension-0.1.950282415/style/images/versatile-data-kit-logo.svg`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/ui-tests/README.md` & `vdk_jupyterlab_extension-0.1.950282415/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/ui-tests/jupyter_server_test_config.py` & `vdk_jupyterlab_extension-0.1.950282415/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/ui-tests/tests/convert-job.spec.ts` & `vdk_jupyterlab_extension-0.1.950282415/ui-tests/tests/convert-job.spec.ts`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
       .locator('pre')
       .filter({ hasText: '#### Execution Order and Identifying Cells' });
     await page.locator('pre').filter({ hasText: '#### Tips:' });
 
     // go through ipython configuration
     await page
       .locator('pre')
-      .filter({ hasText: '%reload_ext vdk_ipython' })
+      .filter({ hasText: '%reload_ext vdk.plugin.ipython' })
       .click();
     await page.locator('pre').filter({ hasText: '%reload_VDK' }).click();
     await page
       .locator('pre')
       .filter({ hasText: 'job_input = VDK.get_initialized_job_input()' })
       .click();
```

### Comparing `vdk_jupyterlab_extension-0.1.947240835/ui-tests/tests/vdk-jupyterlab-extension.spec.ts` & `vdk_jupyterlab_extension-0.1.950282415/ui-tests/tests/vdk-jupyterlab-extension.spec.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 /*
  * Copyright 2021-2023 VMware, Inc.
  * SPDX-License-Identifier: Apache-2.0
  */
 
 import { expect, test } from '@jupyterlab/galata';
-import { assert } from 'console';
 
 /**
  * Don't load JupyterLab webpage before running the tests.
  * This is required to ensure we capture all log messages.
  */
 test.use({ autoGoto: false });
```

### Comparing `vdk_jupyterlab_extension-0.1.947240835/ui-tests/tests/data/convert-test-job-dirty/30_ingest_to_table.py` & `vdk_jupyterlab_extension-0.1.950282415/ui-tests/tests/data/convert-test-job-dirty/30_ingest_to_table.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/__init__.py` & `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/convert_job.py` & `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/convert_job.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/handlers.py` & `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/handlers.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/job_data.py` & `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/job_data.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/vdk_ui.py` & `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/vdk_ui.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb` & `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992283950617284%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(1, 'vdk.plugin.ipython extension introduces a magic command "*

 * *            "for Jupyter.\\n'), (13, '%reload_ext vdk.plugin.ipython\\n')], delete: [13, 1]}}}"}*

```diff
@@ -6,27 +6,27 @@
             "id": "16a6ea87-7142-44dd-94b6-e95fe2d57d06",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "\"\"\"\n",
-                "vdk_ipython extension introduces a magic command for Jupyter.\n",
+                "vdk.plugin.ipython extension introduces a magic command for Jupyter.\n",
                 "The command enables the user to load VDK for the current notebook.\n",
                 "VDK provides the job_input API, which has methods for:\n",
                 "    * executing queries to an OLAP database;\n",
                 "    * ingesting data into a database;\n",
                 "    * processing data into a database.\n",
                 "See the IJobInput documentation for more details.\n",
                 "https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-core/src/vdk/api/job_input.py\n",
                 "\n",
                 "Please refrain from tagging this cell with VDK as it is not an actual part of the data job\n",
                 "and is only used for development purposes.\n",
                 "\"\"\"\n",
-                "%reload_ext vdk_ipython\n",
+                "%reload_ext vdk.plugin.ipython\n",
                 "%reload_VDK\n",
                 "job_input = VDK.get_initialized_job_input()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/jupyter_sample_job/README.md` & `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/jupyter_sample_job/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/jupyter_sample_job/config.ini` & `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/jupyter_sample_job/config.ini`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/package.json` & `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9768939393939394%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.74be29b03cb2d5a0e3ab.js'}}",*

 * * "'version'": "'0.1.950282415'"}*

```diff
@@ -79,15 +79,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.f0c41c67a1da9120d996.js",
+            "load": "static/remoteEntry.74be29b03cb2d5a0e3ab.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "vdk_jupyterlab_extension"
                 },
@@ -152,9 +152,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.947240835"
+    "version": "0.1.950282415"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig` & `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.1.950282415'"}*

```diff
@@ -147,9 +147,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.947240835"
+    "version": "0.1.950282415"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json` & `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/static/161.8695b9e5520bd63d9d87.js` & `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/static/161.687b3e6d54b7501a02f7.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -587,15 +587,15 @@
                             "jp-vdk:menu-convert-job-to-notebook" !== V ? function(e) {
                                 var t, o, n, a;
                                 const l = e.currentWidget;
                                 if (l) {
                                     const r = null === (o = null === (t = l.content.model) || void 0 === t ? void 0 : t.contentFactory) || void 0 === o ? void 0 : o.createCodeCell({
                                             cell: {
                                                 cell_type: "code",
-                                                source: ['"""\n', "vdk_ipython extension introduces a magic command for Jupyter.\n", "The command enables the user to load VDK for the current notebook.\n", "VDK provides the job_input API, which has methods for:\n", "    * executing queries to an OLAP database;\n", "    * ingesting data into a database;\n", "    * processing data into a database.\n", "See the IJobInput documentation for more details.\n", "https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-core/src/vdk/api/job_input.py\n", "Please refrain from tagging this cell with VDK as it is not an actual part of the data job\n", "and is only used for development purposes.\n", '"""\n', "%reload_ext vdk_ipython\n", "%reload_VDK\n", "job_input = VDK.get_initialized_job_input()"],
+                                                source: ['"""\n', "vdk.plugin.ipython extension introduces a magic command for Jupyter.\n", "The command enables the user to load VDK for the current notebook.\n", "VDK provides the job_input API, which has methods for:\n", "    * executing queries to an OLAP database;\n", "    * ingesting data into a database;\n", "    * processing data into a database.\n", "See the IJobInput documentation for more details.\n", "https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-core/src/vdk/api/job_input.py\n", "Please refrain from tagging this cell with VDK as it is not an actual part of the data job\n", "and is only used for development purposes.\n", '"""\n', "%reload_ext vdk.plugin.ipython\n", "%reload_VDK\n", "job_input = VDK.get_initialized_job_input()"],
                                                 metadata: {}
                                             }
                                         }),
                                         s = null === (a = null === (n = e.currentWidget) || void 0 === n ? void 0 : n.content.model) || void 0 === a ? void 0 : a.cells,
                                         i = null == s ? void 0 : s.get(0).value.text;
                                     s && r && s.length <= 1 && "" == i && (s.insert(0, r), s.remove(1))
                                 }
@@ -625,15 +625,15 @@
                                                         cell_type: "code",
                                                         source: e,
                                                         metadata: t
                                                     }
                                                 });
                                                 r && l.push(r)
                                             };
-                                        e(["# " + i.get(n.NAME)]), e(["### Please go through this guide before continuing with the data job run and development."]), e(["#### Introduction and Preparations\n", "*  *This is a notebook transformed from a directory style data job located in " + i.get(n.PATH) + ".*\n", "*  *If you are not familiar with notebook data jobs make sure to check the **Getting Started**(TODO: add link) page.*\n", "*  *You can find the **original job** at " + i.get(n.PATH).split(/[/\\]/).slice(0, -1).join("/") + ".*"]), e(["#### Execution Order and Identifying Cells\n", "*  *The below cells are automatically generated corresponding to a step(.sql or .py file with VDK run function) \n", "    in your original job.* \n", "*  *You will notice that some cells are coloured and include the VDK logo and a numbering. \n", '    These are the "vdk" tagged cells.\n', "    Only these cells are executed during VDK run and all the others are ignored(for example the current cell).*\n", "*  *Code cells in the notebook will be executed according to the numbering when running the notebook data job with VDK.\n", "    This means that the steps in the job are organized from the top to the bottom, starting with the first step.*\n", '*  *When you see a title saying **"Step generated from: sample.py"** before some blocks of code, \n', '    it means that the code below that title was created from the "sample.py" file.*\n', '*  *Similarly, if you come across code cells that have the format **"job_input.execute_query(query_string)"** ,\n', '    it means that those cells contain code generated from ".sql" files.*\n', '*  *On the other hand, code cells originating from ".py" files remain unchanged.\n', '    However, an additional cell is included that calls the "run" function using the command **"run(job_input)"** . \n', '    This cell executes the "run" function from the code generated from the ".py" file.*\n', '*  *You can delete the cells that are not tagged with "vdk" \n', "    as they are not essential to the data job's execution.\n", "    However, removing tagged cells will result in a different data job run.* "]), e(["#### Tips: \n", "* *Before running the job, it is recommended to review the cells\n", "    to ensure a clear understanding of the data job run.  \n", "    This will help to ensure the desired outcome.* "]), t(['"""\n', "vdk_ipython extension introduces a magic command for Jupyter.\n", "The command enables the user to load VDK for the current notebook.\n", "VDK provides the job_input API, which has methods for:\n", "    * executing queries to an OLAP database;\n", "    * ingesting data into a database;\n", "    * processing data into a database.\n", "See the IJobInput documentation for more details.\n", "https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-core/src/vdk/api/job_input.py\n", "Please refrain from tagging this cell with VDK as it is not an actual part of the data job\n", "and is only used for development purposes.\n", '"""\n', "%reload_ext vdk_ipython\n", "%reload_VDK\n", "job_input = VDK.get_initialized_job_input()"], {});
+                                        e(["# " + i.get(n.NAME)]), e(["### Please go through this guide before continuing with the data job run and development."]), e(["#### Introduction and Preparations\n", "*  *This is a notebook transformed from a directory style data job located in " + i.get(n.PATH) + ".*\n", "*  *If you are not familiar with notebook data jobs make sure to check the **Getting Started**(TODO: add link) page.*\n", "*  *You can find the **original job** at " + i.get(n.PATH).split(/[/\\]/).slice(0, -1).join("/") + ".*"]), e(["#### Execution Order and Identifying Cells\n", "*  *The below cells are automatically generated corresponding to a step(.sql or .py file with VDK run function) \n", "    in your original job.* \n", "*  *You will notice that some cells are coloured and include the VDK logo and a numbering. \n", '    These are the "vdk" tagged cells.\n', "    Only these cells are executed during VDK run and all the others are ignored(for example the current cell).*\n", "*  *Code cells in the notebook will be executed according to the numbering when running the notebook data job with VDK.\n", "    This means that the steps in the job are organized from the top to the bottom, starting with the first step.*\n", '*  *When you see a title saying **"Step generated from: sample.py"** before some blocks of code, \n', '    it means that the code below that title was created from the "sample.py" file.*\n', '*  *Similarly, if you come across code cells that have the format **"job_input.execute_query(query_string)"** ,\n', '    it means that those cells contain code generated from ".sql" files.*\n', '*  *On the other hand, code cells originating from ".py" files remain unchanged.\n', '    However, an additional cell is included that calls the "run" function using the command **"run(job_input)"** . \n', '    This cell executes the "run" function from the code generated from the ".py" file.*\n', '*  *You can delete the cells that are not tagged with "vdk" \n', "    as they are not essential to the data job's execution.\n", "    However, removing tagged cells will result in a different data job run.* "]), e(["#### Tips: \n", "* *Before running the job, it is recommended to review the cells\n", "    to ensure a clear understanding of the data job run.  \n", "    This will help to ensure the desired outcome.* "]), t(['"""\n', "vdk.plugin.ipython extension introduces a magic command for Jupyter.\n", "The command enables the user to load VDK for the current notebook.\n", "VDK provides the job_input API, which has methods for:\n", "    * executing queries to an OLAP database;\n", "    * ingesting data into a database;\n", "    * processing data into a database.\n", "See the IJobInput documentation for more details.\n", "https://github.com/vmware/versatile-data-kit/blob/main/projects/vdk-core/src/vdk/api/job_input.py\n", "Please refrain from tagging this cell with VDK as it is not an actual part of the data job\n", "and is only used for development purposes.\n", '"""\n', "%reload_ext vdk.plugin.ipython\n", "%reload_VDK\n", "job_input = VDK.get_initialized_job_input()"], {});
                                         for (const o of B) "markdown" === o.type ? e([o.source]) : "code" === o.type && t([o.source], {
                                             tags: ["vdk"]
                                         });
                                         B = []
                                     }
                                 }
                             })(a)
```

### Comparing `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js` & `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/static/remoteEntry.f0c41c67a1da9120d996.js` & `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/static/remoteEntry.74be29b03cb2d5a0e3ab.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -43,18 +43,18 @@
         }), r
     }, y.d = (e, r) => {
         for (var t in r) y.o(r, t) && !y.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, y.f = {}, y.e = e => Promise.all(Object.keys(y.f).reduce(((r, t) => (y.f[t](e, r), r)), [])), y.u = e => e + "." + {
-        161: "8695b9e5520bd63d9d87",
+        161: "687b3e6d54b7501a02f7",
         747: "e678254df7945f8ed34d"
     } [e] + ".js?v=" + {
-        161: "8695b9e5520bd63d9d87",
+        161: "687b3e6d54b7501a02f7",
         747: "e678254df7945f8ed34d"
     } [e], y.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => y.e(161).then((() => () => y(161))),
                         from: i,
                         eager: !1
                     })
-                })("vdk-jupyterlab-extension", "0.1.947240835"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("vdk-jupyterlab-extension", "0.1.950282415"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         y.g.importScripts && (e = y.g.location + "");
         var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json` & `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/tests/test_convert_job_directory_processor.py` & `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/tests/test_convert_job_directory_processor.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/vdk_jupyterlab_extension/tests/test_directory_archiver.py` & `vdk_jupyterlab_extension-0.1.950282415/vdk_jupyterlab_extension/tests/test_directory_archiver.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/.gitignore` & `vdk_jupyterlab_extension-0.1.950282415/.gitignore`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/README.md` & `vdk_jupyterlab_extension-0.1.950282415/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/pyproject.toml` & `vdk_jupyterlab_extension-0.1.950282415/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.947240835/PKG-INFO` & `vdk_jupyterlab_extension-0.1.950282415/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-jupyterlab-extension
-Version: 0.1.947240835
+Version: 0.1.950282415
 Summary: A Jupyterlab extension for using VDK
 Project-URL: Homepage, https://github.com/vmware/versatile-data-kit
 Project-URL: Bug Tracker, https://github.com/vmware/versatile-data-kit/issues
 Project-URL: Repository, https://github.com/vmware/versatile-data-kit
 Author-email: Versatile Data Kit Development Team <versatile-data-kit@vmware.com>
 License: See https://github.com/vmware/versatile-data-kit/blob/main/LICENSE
 License-File: LICENSE
```

