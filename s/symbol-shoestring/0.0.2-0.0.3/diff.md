# Comparing `tmp/symbol_shoestring-0.0.2.tar.gz` & `tmp/symbol-shoestring-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbol_shoestring-0.0.2.tar", max compression
+gzip compressed data, was "symbol-shoestring-0.0.3.tar", max compression
```

## Comparing `symbol_shoestring-0.0.2.tar` & `symbol-shoestring-0.0.3.tar`

### file list

```diff
@@ -1,79 +1,80 @@
--rw-r--r--   0        0        0     9931 2023-07-12 01:51:37.859111 symbol_shoestring-0.0.2/README.md
--rw-r--r--   0        0        0    25496 2023-07-17 14:34:37.741471 symbol_shoestring-0.0.2/lang/en/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    19551 2023-07-17 14:34:37.861482 symbol_shoestring-0.0.2/lang/ja/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    18739 2023-07-17 14:34:37.601460 symbol_shoestring-0.0.2/lang/messages.pot
--rw-r--r--   0        0        0      169 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/lang/po.header.txt
--rw-r--r--   0        0        0      582 2023-07-17 15:25:15.924739 symbol_shoestring-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/__init__.py
--rw-r--r--   0        0        0     1856 2023-07-17 15:22:51.737379 symbol_shoestring-0.0.2/shoestring/__main__.py
--rw-r--r--   0        0        0        0 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/commands/__init__.py
--rw-r--r--   0        0        0     1552 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/commands/announce_transaction.py
--rw-r--r--   0        0        0     2491 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/commands/health.py
--rw-r--r--   0        0        0     1262 2023-06-20 18:13:02.274119 symbol_shoestring-0.0.2/shoestring/commands/import_bootstrap.py
--rw-r--r--   0        0        0     1025 2023-07-12 01:51:37.859111 symbol_shoestring-0.0.2/shoestring/commands/init.py
--rw-r--r--   0        0        0     1692 2023-06-20 18:13:02.274119 symbol_shoestring-0.0.2/shoestring/commands/min_cosignatures_count.py
--rw-r--r--   0        0        0     1733 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/commands/pemtool.py
--rw-r--r--   0        0        0     1569 2023-07-04 16:02:45.782811 symbol_shoestring-0.0.2/shoestring/commands/renew_certificates.py
--rw-r--r--   0        0        0     5270 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/commands/renew_voting_keys.py
--rw-r--r--   0        0        0     3071 2023-06-20 18:13:02.274119 symbol_shoestring-0.0.2/shoestring/commands/reset_data.py
--rw-r--r--   0        0        0     5330 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/commands/setup.py
--rw-r--r--   0        0        0     3367 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/commands/signer.py
--rw-r--r--   0        0        0     2246 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/commands/upgrade.py
--rw-r--r--   0        0        0        0 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/healthagents/__init__.py
--rw-r--r--   0        0        0      594 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/healthagents/peer_api.py
--rw-r--r--   0        0        0     3586 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/healthagents/peer_certificate.py
--rw-r--r--   0        0        0      644 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/healthagents/rest_api.py
--rw-r--r--   0        0        0     1901 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/healthagents/rest_https_certificate.py
--rw-r--r--   0        0        0     1686 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/healthagents/voting_keys.py
--rw-r--r--   0        0        0     1573 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/healthagents/websockets.py
--rw-r--r--   0        0        0     5055 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/CertificateFactory.py
--rw-r--r--   0        0        0     3233 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/ConfigurationManager.py
--rw-r--r--   0        0        0     1656 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/FileDownloader.py
--rw-r--r--   0        0        0      360 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/FileTemplater.py
--rw-r--r--   0        0        0     1961 2023-07-04 16:02:45.782811 symbol_shoestring-0.0.2/shoestring/internal/HarvesterConfigurator.py
--rw-r--r--   0        0        0      830 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/HeightGrouping.py
--rw-r--r--   0        0        0     3089 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/LinkTransactionBuilder.py
--rw-r--r--   0        0        0      655 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/MultisigAnalyzer.py
--rw-r--r--   0        0        0     2789 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/NodeDownloader.py
--rw-r--r--   0        0        0      578 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/NodeFeatures.py
--rw-r--r--   0        0        0     1412 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/NodewatchClient.py
--rw-r--r--   0        0        0     1356 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/OpensslExecutor.py
--rw-r--r--   0        0        0     3050 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/PackageResolver.py
--rw-r--r--   0        0        0     2139 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/PeerDownloader.py
--rw-r--r--   0        0        0     2372 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/PemUtils.py
--rw-r--r--   0        0        0    12610 2023-07-17 14:33:58.342037 symbol_shoestring-0.0.2/shoestring/internal/Preparer.py
--rw-r--r--   0        0        0     3509 2023-06-20 18:13:02.274119 symbol_shoestring-0.0.2/shoestring/internal/ShoestringConfiguration.py
--rw-r--r--   0        0        0      371 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/TransactionSerializer.py
--rw-r--r--   0        0        0     3947 2023-06-20 18:13:02.274119 symbol_shoestring-0.0.2/shoestring/internal/VoterConfigurator.py
--rw-r--r--   0        0        0        0 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/shoestring/internal/__init__.py
--rw-r--r--   0        0        0     1004 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/Screen.py
--rw-r--r--   0        0        0     2094 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/Screens.py
--rw-r--r--   0        0        0     1781 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/ShoestringOperation.py
--rw-r--r--   0        0        0     4647 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/TabbedView.py
--rw-r--r--   0        0        0      843 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/TitleBar.py
--rw-r--r--   0        0        0     2708 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/ValidatingTextBox.py
--rw-r--r--   0        0        0        0 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/__init__.py
--rw-r--r--   0        0        0     3660 2023-07-17 15:22:51.737379 symbol_shoestring-0.0.2/shoestring/wizard/__main__.py
--rw-r--r--   0        0        0     1970 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/buttons.py
--rw-r--r--   0        0        0      484 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/keybindings.py
--rw-r--r--   0        0        0     1553 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/navigation.py
--rw-r--r--   0        0        0     1635 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/screen_loader.py
--rw-r--r--   0        0        0        0 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/screens/__init__.py
--rw-r--r--   0        0        0     1890 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/screens/certificates.py
--rw-r--r--   0        0        0      652 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/screens/end_screen.py
--rw-r--r--   0        0        0     6536 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/screens/harvesting.py
--rw-r--r--   0        0        0     1625 2023-07-13 18:14:24.410747 symbol_shoestring-0.0.2/shoestring/wizard/screens/modal.py
--rw-r--r--   0        0        0      799 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.2/shoestring/wizard/screens/network_type.py
--rw-r--r--   0        0        0     2981 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.2/shoestring/wizard/screens/node_settings.py
--rw-r--r--   0        0        0      757 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.2/shoestring/wizard/screens/node_type.py
--rw-r--r--   0        0        0     6862 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.2/shoestring/wizard/screens/obligatory.py
--rw-r--r--   0        0        0      827 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.2/shoestring/wizard/screens/root_check.py
--rw-r--r--   0        0        0      799 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.2/shoestring/wizard/screens/voting.py
--rw-r--r--   0        0        0     1835 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.2/shoestring/wizard/screens/welcome.py
--rw-r--r--   0        0        0     3810 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.2/shoestring/wizard/setup_file_generator.py
--rw-r--r--   0        0        0     1744 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.2/shoestring/wizard/shoestring_dispatcher.py
--rw-r--r--   0        0        0     1095 2023-07-13 18:14:24.414747 symbol_shoestring-0.0.2/shoestring/wizard/styles.py
--rw-r--r--   0        0        0     2830 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/templates/docker-compose-dual.yaml
--rw-r--r--   0        0        0      629 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/templates/docker-compose-peer.yaml
--rw-r--r--   0        0        0      299 2023-06-15 01:55:07.107303 symbol_shoestring-0.0.2/templates/nginx.conf.erb
--rw-r--r--   0        0        0    10861 1970-01-01 00:00:00.000000 symbol_shoestring-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     9931 2023-07-31 17:18:59.695940 symbol-shoestring-0.0.3/README.md
+-rw-r--r--   0        0        0    25392 2023-07-31 17:21:00.828046 symbol-shoestring-0.0.3/lang/en/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    18950 2023-07-31 17:21:01.248046 symbol-shoestring-0.0.3/lang/ja/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    18737 2023-07-31 17:21:00.436046 symbol-shoestring-0.0.3/lang/messages.pot
+-rw-r--r--   0        0        0      213 2023-07-31 17:18:59.695940 symbol-shoestring-0.0.3/lang/po.header.txt
+-rw-r--r--   0        0        0      772 2023-07-31 17:23:41.796198 symbol-shoestring-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-31 17:18:59.695940 symbol-shoestring-0.0.3/shoestring/__init__.py
+-rw-r--r--   0        0        0     1856 2023-07-31 17:18:59.695940 symbol-shoestring-0.0.3/shoestring/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-31 17:18:59.695940 symbol-shoestring-0.0.3/shoestring/commands/__init__.py
+-rw-r--r--   0        0        0     1552 2023-07-31 17:18:59.695940 symbol-shoestring-0.0.3/shoestring/commands/announce_transaction.py
+-rw-r--r--   0        0        0     2475 2023-07-31 17:18:59.695940 symbol-shoestring-0.0.3/shoestring/commands/health.py
+-rw-r--r--   0        0        0     1262 2023-07-31 17:18:59.695940 symbol-shoestring-0.0.3/shoestring/commands/import_bootstrap.py
+-rw-r--r--   0        0        0     1025 2023-07-31 17:18:59.695940 symbol-shoestring-0.0.3/shoestring/commands/init.py
+-rw-r--r--   0        0        0     1692 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/commands/min_cosignatures_count.py
+-rw-r--r--   0        0        0     1733 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/commands/pemtool.py
+-rw-r--r--   0        0        0     1569 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/commands/renew_certificates.py
+-rw-r--r--   0        0        0     5270 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/commands/renew_voting_keys.py
+-rw-r--r--   0        0        0     3071 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/commands/reset_data.py
+-rw-r--r--   0        0        0     5330 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/commands/setup.py
+-rw-r--r--   0        0        0     3332 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/commands/signer.py
+-rw-r--r--   0        0        0     2246 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/commands/upgrade.py
+-rw-r--r--   0        0        0        0 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/healthagents/__init__.py
+-rw-r--r--   0        0        0      594 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/healthagents/peer_api.py
+-rw-r--r--   0        0        0     3586 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/healthagents/peer_certificate.py
+-rw-r--r--   0        0        0      644 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/healthagents/rest_api.py
+-rw-r--r--   0        0        0     2985 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/healthagents/rest_https_certificate.py
+-rw-r--r--   0        0        0     1686 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/healthagents/voting_keys.py
+-rw-r--r--   0        0        0     1573 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/healthagents/websockets.py
+-rw-r--r--   0        0        0     5055 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/internal/CertificateFactory.py
+-rw-r--r--   0        0        0     3233 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/internal/ConfigurationManager.py
+-rw-r--r--   0        0        0     1656 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/internal/FileDownloader.py
+-rw-r--r--   0        0        0      360 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/internal/FileTemplater.py
+-rw-r--r--   0        0        0     1961 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/internal/HarvesterConfigurator.py
+-rw-r--r--   0        0        0      830 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/internal/HeightGrouping.py
+-rw-r--r--   0        0        0     3089 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/internal/LinkTransactionBuilder.py
+-rw-r--r--   0        0        0      655 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/internal/MultisigAnalyzer.py
+-rw-r--r--   0        0        0     2789 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/internal/NodeDownloader.py
+-rw-r--r--   0        0        0      578 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/internal/NodeFeatures.py
+-rw-r--r--   0        0        0     1412 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/internal/NodewatchClient.py
+-rw-r--r--   0        0        0     1381 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/internal/OpensslExecutor.py
+-rw-r--r--   0        0        0     3060 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/internal/PackageResolver.py
+-rw-r--r--   0        0        0     2139 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/internal/PeerDownloader.py
+-rw-r--r--   0        0        0     2372 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/internal/PemUtils.py
+-rw-r--r--   0        0        0    12610 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/internal/Preparer.py
+-rw-r--r--   0        0        0     3509 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/internal/ShoestringConfiguration.py
+-rw-r--r--   0        0        0      371 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/internal/TransactionSerializer.py
+-rw-r--r--   0        0        0     3947 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/internal/VoterConfigurator.py
+-rw-r--r--   0        0        0        0 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/internal/__init__.py
+-rw-r--r--   0        0        0     1004 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/wizard/Screen.py
+-rw-r--r--   0        0        0     2102 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/wizard/ScreenContainer.py
+-rw-r--r--   0        0        0     1781 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/wizard/ShoestringOperation.py
+-rw-r--r--   0        0        0     4774 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/wizard/TabbedView.py
+-rw-r--r--   0        0        0      843 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/wizard/TitleBar.py
+-rw-r--r--   0        0        0     2708 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/wizard/ValidatingTextBox.py
+-rw-r--r--   0        0        0        0 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/wizard/__init__.py
+-rw-r--r--   0        0        0     3671 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/wizard/__main__.py
+-rw-r--r--   0        0        0     1970 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/wizard/buttons.py
+-rw-r--r--   0        0        0      484 2023-07-31 17:18:59.699940 symbol-shoestring-0.0.3/shoestring/wizard/keybindings.py
+-rw-r--r--   0        0        0     1553 2023-07-31 17:18:59.707940 symbol-shoestring-0.0.3/shoestring/wizard/navigation.py
+-rw-r--r--   0        0        0     1635 2023-07-31 17:18:59.707940 symbol-shoestring-0.0.3/shoestring/wizard/screen_loader.py
+-rw-r--r--   0        0        0        0 2023-07-31 17:18:59.707940 symbol-shoestring-0.0.3/shoestring/wizard/screens/__init__.py
+-rw-r--r--   0        0        0     1890 2023-07-31 17:18:59.707940 symbol-shoestring-0.0.3/shoestring/wizard/screens/certificates.py
+-rw-r--r--   0        0        0      652 2023-07-31 17:18:59.707940 symbol-shoestring-0.0.3/shoestring/wizard/screens/end_screen.py
+-rw-r--r--   0        0        0     6498 2023-07-31 17:18:59.707940 symbol-shoestring-0.0.3/shoestring/wizard/screens/harvesting.py
+-rw-r--r--   0        0        0     1625 2023-07-31 17:18:59.707940 symbol-shoestring-0.0.3/shoestring/wizard/screens/modal.py
+-rw-r--r--   0        0        0      799 2023-07-31 17:18:59.707940 symbol-shoestring-0.0.3/shoestring/wizard/screens/network_type.py
+-rw-r--r--   0        0        0     2981 2023-07-31 17:18:59.707940 symbol-shoestring-0.0.3/shoestring/wizard/screens/node_settings.py
+-rw-r--r--   0        0        0      757 2023-07-31 17:18:59.707940 symbol-shoestring-0.0.3/shoestring/wizard/screens/node_type.py
+-rw-r--r--   0        0        0     6789 2023-07-31 17:18:59.707940 symbol-shoestring-0.0.3/shoestring/wizard/screens/obligatory.py
+-rw-r--r--   0        0        0      827 2023-07-31 17:18:59.707940 symbol-shoestring-0.0.3/shoestring/wizard/screens/root_check.py
+-rw-r--r--   0        0        0      799 2023-07-31 17:18:59.707940 symbol-shoestring-0.0.3/shoestring/wizard/screens/voting.py
+-rw-r--r--   0        0        0     1835 2023-07-31 17:18:59.707940 symbol-shoestring-0.0.3/shoestring/wizard/screens/welcome.py
+-rw-r--r--   0        0        0     3810 2023-07-31 17:18:59.707940 symbol-shoestring-0.0.3/shoestring/wizard/setup_file_generator.py
+-rw-r--r--   0        0        0     1744 2023-07-31 17:18:59.707940 symbol-shoestring-0.0.3/shoestring/wizard/shoestring_dispatcher.py
+-rw-r--r--   0        0        0     1095 2023-07-31 17:18:59.707940 symbol-shoestring-0.0.3/shoestring/wizard/styles.py
+-rw-r--r--   0        0        0     2830 2023-07-31 17:18:59.707940 symbol-shoestring-0.0.3/templates/docker-compose-dual.yaml
+-rw-r--r--   0        0        0      629 2023-07-31 17:18:59.707940 symbol-shoestring-0.0.3/templates/docker-compose-peer.yaml
+-rw-r--r--   0        0        0      299 2023-07-31 17:18:59.707940 symbol-shoestring-0.0.3/templates/nginx.conf.erb
+-rw-r--r--   0        0        0    11307 2023-07-31 17:23:48.202209 symbol-shoestring-0.0.3/setup.py
+-rw-r--r--   0        0        0    11035 2023-07-31 17:23:48.202879 symbol-shoestring-0.0.3/PKG-INFO
```

### Comparing `symbol_shoestring-0.0.2/README.md` & `symbol-shoestring-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/lang/en/LC_MESSAGES/messages.po` & `symbol-shoestring-0.0.3/lang/en/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Translations for Shoestring.
 # Copyright (C) 2023 Symbol Contributors
 # This file is distributed under the same license as the Shoestring project.
 msgid ""
 msgstr ""
+"Content-Type: text/plain; charset=UTF-8\n"
 
 #: shoestring/commands/announce_transaction.py:31
 msgid "announce-transaction-announce-successful"
 msgstr "transaction was successfully sent to the network"
 
 #: shoestring/commands/announce_transaction.py:24
 msgid "announce-transaction-preparing-to-announce"
@@ -16,26 +17,26 @@
 
 #: shoestring/commands/announce_transaction.py:36
 msgid "argument-help-announce-transaction-transaction"
 msgstr "file containing serialized transaction to send"
 
 #: shoestring/commands/min_cosignatures_count.py:35
 #: shoestring/commands/renew_certificates.py:31
-#: shoestring/commands/setup.py:139 shoestring/commands/signer.py:95
+#: shoestring/commands/setup.py:139 shoestring/commands/signer.py:93
 msgid "argument-help-ca-key-path"
 msgstr "path to main private key PEM file"
 
 #: shoestring/commands/announce_transaction.py:35
 #: shoestring/commands/health.py:75 shoestring/commands/import_bootstrap.py:28
 #: shoestring/commands/init.py:29
 #: shoestring/commands/min_cosignatures_count.py:34
 #: shoestring/commands/renew_certificates.py:29
 #: shoestring/commands/renew_voting_keys.py:112
 #: shoestring/commands/reset_data.py:87 shoestring/commands/setup.py:131
-#: shoestring/commands/signer.py:94
+#: shoestring/commands/signer.py:92
 msgid "argument-help-config"
 msgstr "path to shoestring configuration file"
 
 #: shoestring/commands/health.py:76
 #: shoestring/commands/renew_certificates.py:30
 #: shoestring/commands/renew_voting_keys.py:113
 #: shoestring/commands/reset_data.py:88 shoestring/commands/setup.py:133
@@ -88,19 +89,19 @@
 "Network configuration package. Possible values: (name | file:///filename "
 "| http(s)://uri) (default: mainnet)"
 
 #: shoestring/commands/setup.py:138
 msgid "argument-help-setup-security"
 msgstr "security mode (default: default)"
 
-#: shoestring/commands/signer.py:97
+#: shoestring/commands/signer.py:95
 msgid "argument-help-signer-filename"
 msgstr "transaction binary payload"
 
-#: shoestring/commands/signer.py:96
+#: shoestring/commands/signer.py:94
 msgid "argument-help-signer-save"
 msgstr "save signed payload into same file as input"
 
 #: shoestring/internal/FileDownloader.py:40
 msgid "file-downloader-already-downloaded"
 msgstr "proper file already downloaded ({name})"
 
@@ -173,19 +174,19 @@
 msgid "health-rest-api-error"
 msgstr "cannot access REST API at {endpoint}"
 
 #: shoestring/healthagents/rest_api.py:20
 msgid "health-rest-api-success"
 msgstr "REST API accessible, height = {height}"
 
-#: shoestring/healthagents/rest_https_certificate.py:55
+#: shoestring/healthagents/rest_https_certificate.py:96
 msgid "health-rest-https-certificate-invalid"
 msgstr "HTTPS certificate looks invalid: {error_message}"
 
-#: shoestring/healthagents/rest_https_certificate.py:58
+#: shoestring/healthagents/rest_https_certificate.py:99
 msgid "health-rest-https-certificate-valid"
 msgstr "HTTPS certificate looks ok: valid from {start_date} to {end_date}"
 
 #: shoestring/commands/health.py:70
 msgid "health-running-health-agent"
 msgstr "running health agent for {module_name}"
 
@@ -233,67 +234,67 @@
 msgid "import-bootstrap-importing-harvester"
 msgstr "importing harvesting keys from bootstrap ({path})"
 
 #: shoestring/commands/import_bootstrap.py:19
 msgid "import-bootstrap-importing-voter"
 msgstr "importing voting keys from bootstrap ({path})"
 
-#: shoestring/__main__.py:19
+#: shoestring/__main__.py:20
 msgid "main-announce-transaction-help"
 msgstr "announces a transaction to the network"
 
-#: shoestring/__main__.py:20
+#: shoestring/__main__.py:21
 msgid "main-health-help"
 msgstr "does health check"
 
-#: shoestring/__main__.py:21
+#: shoestring/__main__.py:22
 msgid "main-import-bootstrap-help"
 msgstr "imports settings from a bootstap installation"
 
-#: shoestring/__main__.py:22
+#: shoestring/__main__.py:23
 msgid "main-init-help"
 msgstr "extracts a template shoestring configuration file from a package"
 
-#: shoestring/__main__.py:23
+#: shoestring/__main__.py:24
 msgid "main-min-cosignatures-count-help"
 msgstr "detects minimum cosignatures required for an account"
 
-#: shoestring/__main__.py:24
+#: shoestring/__main__.py:25
 msgid "main-pemtool-help"
 msgstr "generates PEM files"
 
-#: shoestring/__main__.py:25
+#: shoestring/__main__.py:26
 msgid "main-renew-certificates-help"
 msgstr "renews certificates"
 
-#: shoestring/__main__.py:26
+#: shoestring/__main__.py:27
 msgid "main-renew-voting-keys-help"
 msgstr "renews voting keys"
 
-#: shoestring/__main__.py:27
+#: shoestring/__main__.py:28
 msgid "main-reset-data-help"
 msgstr "resets data to allow a resync from scratch"
 
-#: shoestring/__main__.py:28
+#: shoestring/__main__.py:29
 msgid "main-setup-help"
 msgstr "sets up a node"
 
-#: shoestring/__main__.py:29
+#: shoestring/__main__.py:30
 msgid "main-signer-help"
 msgstr "signs a transaction"
 
-#: shoestring/__main__.py:17
+#: shoestring/__main__.py:18
 msgid "main-subcommands-help"
 msgstr "valid subcommands"
 
-#: shoestring/__main__.py:16
+#: shoestring/__main__.py:17
 msgid "main-title"
 msgstr "Shoestring Tool"
 
-#: shoestring/__main__.py:30
+#: shoestring/__main__.py:31
 msgid "main-upgrade-help"
 msgstr "upgrades a node to the latest client version"
 
 #: shoestring/commands/min_cosignatures_count.py:24
 msgid "min-cosignatures-count-cosignatures-detected"
 msgstr ""
 "detected at least {min_cosignatures_count} cosignatures are required for "
@@ -385,15 +386,15 @@
 msgid "upgrade-purging-directory"
 msgstr "purging DIRECTORY {directory}"
 
 #: shoestring/commands/upgrade.py:21
 msgid "upgrade-recreating-directory"
 msgstr "recreating DIRECTORY {directory}"
 
-#: shoestring/wizard/__main__.py:97 shoestring/wizard/buttons.py:29
+#: shoestring/wizard/__main__.py:99 shoestring/wizard/buttons.py:29
 msgid "wizard-button-finish"
 msgstr "Finish!"
 
 #: shoestring/wizard/buttons.py:53 shoestring/wizard/navigation.py:52
 msgid "wizard-button-next"
 msgstr "Next"
 
@@ -421,123 +422,123 @@
 msgid "wizard-certificates-peer-cert-label"
 msgstr "Cert Peer name"
 
 #: shoestring/wizard/screens/certificates.py:50
 msgid "wizard-certificates-title"
 msgstr "CA name + node cert name"
 
-#: shoestring/wizard/screens/obligatory.py:84
+#: shoestring/wizard/screens/obligatory.py:83
 msgid "wizard-dialog-message-generation-text"
 msgstr "Key generated and saved to file."
 
-#: shoestring/wizard/screens/obligatory.py:83
+#: shoestring/wizard/screens/obligatory.py:82
 msgid "wizard-dialog-message-generation-title"
 msgstr "Key generation"
 
-#: shoestring/wizard/screens/obligatory.py:101
+#: shoestring/wizard/screens/obligatory.py:99
 msgid "wizard-dialog-message-import-text"
 msgstr "Private key imported and saved to file."
 
-#: shoestring/wizard/screens/obligatory.py:100
+#: shoestring/wizard/screens/obligatory.py:98
 msgid "wizard-dialog-message-import-title"
 msgstr "Key import"
 
 #: shoestring/wizard/screens/end_screen.py:19
 msgid "wizard-end-title"
 msgstr "writing configuration"
 
-#: shoestring/wizard/screens/harvesting.py:109
+#: shoestring/wizard/screens/harvesting.py:108
 msgid "wizard-harvesting-active"
 msgstr "would you like to enable harvesting?"
 
-#: shoestring/wizard/screens/harvesting.py:113
+#: shoestring/wizard/screens/harvesting.py:112
 msgid "wizard-harvesting-auto-harvest"
 msgstr "would you like to auto harvest?"
 
-#: shoestring/wizard/screens/harvesting.py:148
+#: shoestring/wizard/screens/harvesting.py:147
 msgid "wizard-harvesting-beneficiary-address-error-text"
 msgstr "beneficiary address needs to be address (in proper network)"
 
-#: shoestring/wizard/screens/harvesting.py:146
+#: shoestring/wizard/screens/harvesting.py:145
 msgid "wizard-harvesting-beneficiary-address-label"
 msgstr "beneficiary address"
 
-#: shoestring/wizard/screens/harvesting.py:130
+#: shoestring/wizard/screens/harvesting.py:129
 msgid "wizard-harvesting-delegate"
 msgstr "enable delegated harvesters auto detection?"
 
-#: shoestring/wizard/screens/harvesting.py:117
+#: shoestring/wizard/screens/harvesting.py:116
 msgid "wizard-harvesting-generate-keys"
 msgstr "generate new random keys and transaction"
 
-#: shoestring/wizard/screens/harvesting.py:136
+#: shoestring/wizard/screens/harvesting.py:135
 msgid "wizard-harvesting-max-unlocked-accounts-error-text"
 msgstr "max unlocked accounts value must be a number"
 
-#: shoestring/wizard/screens/harvesting.py:134
+#: shoestring/wizard/screens/harvesting.py:133
 msgid "wizard-harvesting-max-unlocked-accounts-label"
 msgstr "max unlocked accounts"
 
-#: shoestring/wizard/screens/harvesting.py:142
+#: shoestring/wizard/screens/harvesting.py:141
 msgid "wizard-harvesting-min-fee-multiplier-error-text"
 msgstr "min fee multiplier value must be a number"
 
-#: shoestring/wizard/screens/harvesting.py:140
+#: shoestring/wizard/screens/harvesting.py:139
 msgid "wizard-harvesting-min-fee-multiplier-label"
 msgstr "min fee multiplier"
 
-#: shoestring/wizard/screens/harvesting.py:123
+#: shoestring/wizard/screens/harvesting.py:122
 msgid "wizard-harvesting-signing-key-error-text"
 msgstr "signing private key must be a valid hex private key string"
 
-#: shoestring/wizard/screens/harvesting.py:121
+#: shoestring/wizard/screens/harvesting.py:120
 msgid "wizard-harvesting-signing-key-label"
 msgstr "harvester signing key"
 
-#: shoestring/wizard/screens/harvesting.py:170
+#: shoestring/wizard/screens/harvesting.py:169
 msgid "wizard-harvesting-title"
 msgstr "Harvester settings"
 
-#: shoestring/wizard/screens/harvesting.py:80
+#: shoestring/wizard/screens/harvesting.py:79
 msgid "wizard-harvesting-token-active"
 msgstr "harvester role"
 
-#: shoestring/wizard/screens/harvesting.py:83
+#: shoestring/wizard/screens/harvesting.py:82
 msgid "wizard-harvesting-token-auto-harvest"
 msgstr "* auto harvest?"
 
-#: shoestring/wizard/screens/harvesting.py:88
+#: shoestring/wizard/screens/harvesting.py:87
 msgid "wizard-harvesting-token-beneficiary-address"
 msgstr "* beneficiary address"
 
-#: shoestring/wizard/screens/harvesting.py:85
+#: shoestring/wizard/screens/harvesting.py:84
 msgid "wizard-harvesting-token-delegate"
 msgstr "* auto detect delegates?"
 
-#: shoestring/wizard/screens/harvesting.py:84
+#: shoestring/wizard/screens/harvesting.py:83
 msgid "wizard-harvesting-token-generate-keys"
 msgstr "* generate keys?"
 
-#: shoestring/wizard/screens/harvesting.py:86
+#: shoestring/wizard/screens/harvesting.py:85
 msgid "wizard-harvesting-token-max-unlocked-accounts"
 msgstr "* max unlocked accounts"
 
-#: shoestring/wizard/screens/harvesting.py:87
+#: shoestring/wizard/screens/harvesting.py:86
 msgid "wizard-harvesting-token-min-fee-multiplier"
 msgstr "* min fee multiplier"
 
-#: shoestring/wizard/screens/harvesting.py:127
+#: shoestring/wizard/screens/harvesting.py:126
 msgid "wizard-harvesting-vrf-key-error-text"
 msgstr "vrf private key must be a valid hex private key string"
 
-#: shoestring/wizard/screens/harvesting.py:125
+#: shoestring/wizard/screens/harvesting.py:124
 msgid "wizard-harvesting-vrf-key-label"
 msgstr "harvester vrf key"
 
-#: shoestring/wizard/__main__.py:103
+#: shoestring/wizard/__main__.py:104
 msgid "wizard-main-done"
 msgstr "Done 👋"
 
 #: shoestring/wizard/TitleBar.py:26
 msgid "wizard-main-initial-title"
 msgstr "<b>Welcome, pick operation</b>"
 
@@ -619,79 +620,79 @@
 msgid "wizard-node-type-title"
 msgstr "Choose node type"
 
 #: shoestring/wizard/screens/node_type.py:16
 msgid "wizard-node-type-token"
 msgstr "node type"
 
-#: shoestring/wizard/screens/obligatory.py:122
-#: shoestring/wizard/screens/obligatory.py:130
+#: shoestring/wizard/screens/obligatory.py:120
+#: shoestring/wizard/screens/obligatory.py:128
 msgid "wizard-obligatory-ca-pem-path-error-text"
 msgstr "ca pem file path must be a valid file"
 
-#: shoestring/wizard/screens/obligatory.py:123
-#: shoestring/wizard/screens/obligatory.py:124
+#: shoestring/wizard/screens/obligatory.py:121
+#: shoestring/wizard/screens/obligatory.py:122
 msgid "wizard-obligatory-ca-pem-path-error-text-not-exist"
 msgstr ""
 "ca pem path needs to point to non-existing file in existing directory and"
 " must have .pem extension"
 
-#: shoestring/wizard/screens/obligatory.py:128
+#: shoestring/wizard/screens/obligatory.py:126
 msgid "wizard-obligatory-ca-pem-path-label"
 msgstr "CA PEM file path (main account)"
 
-#: shoestring/wizard/screens/obligatory.py:109
+#: shoestring/wizard/screens/obligatory.py:107
 msgid "wizard-obligatory-destination-directory-error-text"
 msgstr "destination directory must be a valid directory"
 
-#: shoestring/wizard/screens/obligatory.py:107
+#: shoestring/wizard/screens/obligatory.py:105
 msgid "wizard-obligatory-destination-directory-label"
 msgstr "Configuration destination directory"
 
-#: shoestring/wizard/screens/obligatory.py:142
+#: shoestring/wizard/screens/obligatory.py:140
 msgid "wizard-obligatory-generate-button"
 msgstr "Generate!"
 
-#: shoestring/wizard/screens/obligatory.py:141
+#: shoestring/wizard/screens/obligatory.py:139
 msgid "wizard-obligatory-import-button"
 msgstr "Import!"
 
-#: shoestring/wizard/screens/obligatory.py:113
+#: shoestring/wizard/screens/obligatory.py:111
 msgid "wizard-obligatory-priv-ca"
 msgstr "CA PEM file"
 
-#: shoestring/wizard/screens/obligatory.py:115
+#: shoestring/wizard/screens/obligatory.py:113
 msgid "wizard-obligatory-priv-generate-new"
 msgstr "Generate random private key"
 
-#: shoestring/wizard/screens/obligatory.py:114
+#: shoestring/wizard/screens/obligatory.py:112
 msgid "wizard-obligatory-priv-import-hex"
 msgstr "Import main private key in hex"
 
-#: shoestring/wizard/screens/obligatory.py:146
+#: shoestring/wizard/screens/obligatory.py:144
 msgid "wizard-obligatory-private-key-ca-pem-path-description"
 msgstr "Specify input location of private key PEM file above."
 
-#: shoestring/wizard/screens/obligatory.py:157
+#: shoestring/wizard/screens/obligatory.py:155
 msgid "wizard-obligatory-private-key-generate-description"
 msgstr "Specify output location of private key PEM file above."
 
-#: shoestring/wizard/screens/obligatory.py:149
+#: shoestring/wizard/screens/obligatory.py:147
 msgid "wizard-obligatory-private-key-hex-description"
 msgstr "Specify output location of private key PEM file above."
 
-#: shoestring/wizard/screens/obligatory.py:136
+#: shoestring/wizard/screens/obligatory.py:134
 msgid "wizard-obligatory-private-key-hex-error-text"
 msgstr "must be private key in hex format"
 
-#: shoestring/wizard/screens/obligatory.py:134
+#: shoestring/wizard/screens/obligatory.py:132
 msgid "wizard-obligatory-private-key-hex-label"
 msgstr "Enter private key"
 
-#: shoestring/wizard/screens/obligatory.py:177
+#: shoestring/wizard/screens/obligatory.py:175
 msgid "wizard-obligatory-title"
 msgstr "Obligatory settings"
 
 #: shoestring/wizard/screens/obligatory.py:41
 msgid "wizard-obligatory-token-ca-pem-path"
 msgstr "ca pem path"
 
@@ -782,16 +783,7 @@
 msgid "wizard-welcome-title"
 msgstr "Welcome"
 
 #: shoestring/wizard/screens/welcome.py:36
 msgid "wizard-welcome-upgrade"
 msgstr "upgrade"
 
-#~ msgid "CA PEM file"
-#~ msgstr ""
-
-#~ msgid "Generate random private key"
-#~ msgstr ""
-
-#~ msgid "Import main private key in hex"
-#~ msgstr ""
-
```

### Comparing `symbol_shoestring-0.0.2/lang/ja/LC_MESSAGES/messages.po` & `symbol-shoestring-0.0.3/lang/ja/LC_MESSAGES/messages.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Translations for Shoestring.
 # Copyright (C) 2023 Symbol Contributors
 # This file is distributed under the same license as the Shoestring project.
 msgid ""
 msgstr ""
+"Content-Type: text/plain; charset=UTF-8\n"
 
 #: shoestring/commands/announce_transaction.py:31
 msgid "announce-transaction-announce-successful"
 msgstr ""
 
 #: shoestring/commands/announce_transaction.py:24
 msgid "announce-transaction-preparing-to-announce"
@@ -14,26 +15,26 @@
 
 #: shoestring/commands/announce_transaction.py:36
 msgid "argument-help-announce-transaction-transaction"
 msgstr ""
 
 #: shoestring/commands/min_cosignatures_count.py:35
 #: shoestring/commands/renew_certificates.py:31
-#: shoestring/commands/setup.py:139 shoestring/commands/signer.py:95
+#: shoestring/commands/setup.py:139 shoestring/commands/signer.py:93
 msgid "argument-help-ca-key-path"
 msgstr ""
 
 #: shoestring/commands/announce_transaction.py:35
 #: shoestring/commands/health.py:75 shoestring/commands/import_bootstrap.py:28
 #: shoestring/commands/init.py:29
 #: shoestring/commands/min_cosignatures_count.py:34
 #: shoestring/commands/renew_certificates.py:29
 #: shoestring/commands/renew_voting_keys.py:112
 #: shoestring/commands/reset_data.py:87 shoestring/commands/setup.py:131
-#: shoestring/commands/signer.py:94
+#: shoestring/commands/signer.py:92
 msgid "argument-help-config"
 msgstr ""
 
 #: shoestring/commands/health.py:76
 #: shoestring/commands/renew_certificates.py:30
 #: shoestring/commands/renew_voting_keys.py:113
 #: shoestring/commands/reset_data.py:88 shoestring/commands/setup.py:133
@@ -84,19 +85,19 @@
 msgid "argument-help-setup-package"
 msgstr ""
 
 #: shoestring/commands/setup.py:138
 msgid "argument-help-setup-security"
 msgstr ""
 
-#: shoestring/commands/signer.py:97
+#: shoestring/commands/signer.py:95
 msgid "argument-help-signer-filename"
 msgstr ""
 
-#: shoestring/commands/signer.py:96
+#: shoestring/commands/signer.py:94
 msgid "argument-help-signer-save"
 msgstr ""
 
 #: shoestring/internal/FileDownloader.py:40
 msgid "file-downloader-already-downloaded"
 msgstr ""
 
@@ -169,19 +170,19 @@
 msgid "health-rest-api-error"
 msgstr ""
 
 #: shoestring/healthagents/rest_api.py:20
 msgid "health-rest-api-success"
 msgstr ""
 
-#: shoestring/healthagents/rest_https_certificate.py:55
+#: shoestring/healthagents/rest_https_certificate.py:96
 msgid "health-rest-https-certificate-invalid"
 msgstr ""
 
-#: shoestring/healthagents/rest_https_certificate.py:58
+#: shoestring/healthagents/rest_https_certificate.py:99
 msgid "health-rest-https-certificate-valid"
 msgstr ""
 
 #: shoestring/commands/health.py:70
 msgid "health-running-health-agent"
 msgstr ""
 
@@ -225,67 +226,67 @@
 msgid "import-bootstrap-importing-harvester"
 msgstr ""
 
 #: shoestring/commands/import_bootstrap.py:19
 msgid "import-bootstrap-importing-voter"
 msgstr ""
 
-#: shoestring/__main__.py:19
+#: shoestring/__main__.py:20
 msgid "main-announce-transaction-help"
 msgstr ""
 
-#: shoestring/__main__.py:20
+#: shoestring/__main__.py:21
 msgid "main-health-help"
 msgstr ""
 
-#: shoestring/__main__.py:21
+#: shoestring/__main__.py:22
 msgid "main-import-bootstrap-help"
 msgstr ""
 
-#: shoestring/__main__.py:22
+#: shoestring/__main__.py:23
 msgid "main-init-help"
 msgstr ""
 
-#: shoestring/__main__.py:23
+#: shoestring/__main__.py:24
 msgid "main-min-cosignatures-count-help"
 msgstr ""
 
-#: shoestring/__main__.py:24
+#: shoestring/__main__.py:25
 msgid "main-pemtool-help"
 msgstr ""
 
-#: shoestring/__main__.py:25
+#: shoestring/__main__.py:26
 msgid "main-renew-certificates-help"
 msgstr ""
 
-#: shoestring/__main__.py:26
+#: shoestring/__main__.py:27
 msgid "main-renew-voting-keys-help"
 msgstr ""
 
-#: shoestring/__main__.py:27
+#: shoestring/__main__.py:28
 msgid "main-reset-data-help"
 msgstr ""
 
-#: shoestring/__main__.py:28
+#: shoestring/__main__.py:29
 msgid "main-setup-help"
 msgstr ""
 
-#: shoestring/__main__.py:29
+#: shoestring/__main__.py:30
 msgid "main-signer-help"
 msgstr ""
 
-#: shoestring/__main__.py:17
+#: shoestring/__main__.py:18
 msgid "main-subcommands-help"
 msgstr ""
 
-#: shoestring/__main__.py:16
+#: shoestring/__main__.py:17
 msgid "main-title"
 msgstr ""
 
-#: shoestring/__main__.py:30
+#: shoestring/__main__.py:31
 msgid "main-upgrade-help"
 msgstr ""
 
 #: shoestring/commands/min_cosignatures_count.py:24
 msgid "min-cosignatures-count-cosignatures-detected"
 msgstr ""
 
@@ -373,15 +374,15 @@
 msgid "upgrade-purging-directory"
 msgstr ""
 
 #: shoestring/commands/upgrade.py:21
 msgid "upgrade-recreating-directory"
 msgstr ""
 
-#: shoestring/wizard/__main__.py:97 shoestring/wizard/buttons.py:29
+#: shoestring/wizard/__main__.py:99 shoestring/wizard/buttons.py:29
 msgid "wizard-button-finish"
 msgstr ""
 
 #: shoestring/wizard/buttons.py:53 shoestring/wizard/navigation.py:52
 msgid "wizard-button-next"
 msgstr ""
 
@@ -409,123 +410,123 @@
 msgid "wizard-certificates-peer-cert-label"
 msgstr ""
 
 #: shoestring/wizard/screens/certificates.py:50
 msgid "wizard-certificates-title"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:84
+#: shoestring/wizard/screens/obligatory.py:83
 msgid "wizard-dialog-message-generation-text"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:83
+#: shoestring/wizard/screens/obligatory.py:82
 msgid "wizard-dialog-message-generation-title"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:101
+#: shoestring/wizard/screens/obligatory.py:99
 msgid "wizard-dialog-message-import-text"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:100
+#: shoestring/wizard/screens/obligatory.py:98
 msgid "wizard-dialog-message-import-title"
 msgstr ""
 
 #: shoestring/wizard/screens/end_screen.py:19
 msgid "wizard-end-title"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:109
+#: shoestring/wizard/screens/harvesting.py:108
 msgid "wizard-harvesting-active"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:113
+#: shoestring/wizard/screens/harvesting.py:112
 msgid "wizard-harvesting-auto-harvest"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:148
+#: shoestring/wizard/screens/harvesting.py:147
 msgid "wizard-harvesting-beneficiary-address-error-text"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:146
+#: shoestring/wizard/screens/harvesting.py:145
 msgid "wizard-harvesting-beneficiary-address-label"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:130
+#: shoestring/wizard/screens/harvesting.py:129
 msgid "wizard-harvesting-delegate"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:117
+#: shoestring/wizard/screens/harvesting.py:116
 msgid "wizard-harvesting-generate-keys"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:136
+#: shoestring/wizard/screens/harvesting.py:135
 msgid "wizard-harvesting-max-unlocked-accounts-error-text"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:134
+#: shoestring/wizard/screens/harvesting.py:133
 msgid "wizard-harvesting-max-unlocked-accounts-label"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:142
+#: shoestring/wizard/screens/harvesting.py:141
 msgid "wizard-harvesting-min-fee-multiplier-error-text"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:140
+#: shoestring/wizard/screens/harvesting.py:139
 msgid "wizard-harvesting-min-fee-multiplier-label"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:123
+#: shoestring/wizard/screens/harvesting.py:122
 msgid "wizard-harvesting-signing-key-error-text"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:121
+#: shoestring/wizard/screens/harvesting.py:120
 msgid "wizard-harvesting-signing-key-label"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:170
+#: shoestring/wizard/screens/harvesting.py:169
 msgid "wizard-harvesting-title"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:80
+#: shoestring/wizard/screens/harvesting.py:79
 msgid "wizard-harvesting-token-active"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:83
+#: shoestring/wizard/screens/harvesting.py:82
 msgid "wizard-harvesting-token-auto-harvest"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:88
+#: shoestring/wizard/screens/harvesting.py:87
 msgid "wizard-harvesting-token-beneficiary-address"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:85
+#: shoestring/wizard/screens/harvesting.py:84
 msgid "wizard-harvesting-token-delegate"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:84
+#: shoestring/wizard/screens/harvesting.py:83
 msgid "wizard-harvesting-token-generate-keys"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:86
+#: shoestring/wizard/screens/harvesting.py:85
 msgid "wizard-harvesting-token-max-unlocked-accounts"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:87
+#: shoestring/wizard/screens/harvesting.py:86
 msgid "wizard-harvesting-token-min-fee-multiplier"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:127
+#: shoestring/wizard/screens/harvesting.py:126
 msgid "wizard-harvesting-vrf-key-error-text"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:125
+#: shoestring/wizard/screens/harvesting.py:124
 msgid "wizard-harvesting-vrf-key-label"
 msgstr ""
 
-#: shoestring/wizard/__main__.py:103
+#: shoestring/wizard/__main__.py:104
 msgid "wizard-main-done"
 msgstr ""
 
 #: shoestring/wizard/TitleBar.py:26
 msgid "wizard-main-initial-title"
 msgstr ""
 
@@ -605,77 +606,77 @@
 msgid "wizard-node-type-title"
 msgstr ""
 
 #: shoestring/wizard/screens/node_type.py:16
 msgid "wizard-node-type-token"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:122
-#: shoestring/wizard/screens/obligatory.py:130
+#: shoestring/wizard/screens/obligatory.py:120
+#: shoestring/wizard/screens/obligatory.py:128
 msgid "wizard-obligatory-ca-pem-path-error-text"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:123
-#: shoestring/wizard/screens/obligatory.py:124
+#: shoestring/wizard/screens/obligatory.py:121
+#: shoestring/wizard/screens/obligatory.py:122
 msgid "wizard-obligatory-ca-pem-path-error-text-not-exist"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:128
+#: shoestring/wizard/screens/obligatory.py:126
 msgid "wizard-obligatory-ca-pem-path-label"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:109
+#: shoestring/wizard/screens/obligatory.py:107
 msgid "wizard-obligatory-destination-directory-error-text"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:107
+#: shoestring/wizard/screens/obligatory.py:105
 msgid "wizard-obligatory-destination-directory-label"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:142
+#: shoestring/wizard/screens/obligatory.py:140
 msgid "wizard-obligatory-generate-button"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:141
+#: shoestring/wizard/screens/obligatory.py:139
 msgid "wizard-obligatory-import-button"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:113
+#: shoestring/wizard/screens/obligatory.py:111
 msgid "wizard-obligatory-priv-ca"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:115
+#: shoestring/wizard/screens/obligatory.py:113
 msgid "wizard-obligatory-priv-generate-new"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:114
+#: shoestring/wizard/screens/obligatory.py:112
 msgid "wizard-obligatory-priv-import-hex"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:146
+#: shoestring/wizard/screens/obligatory.py:144
 msgid "wizard-obligatory-private-key-ca-pem-path-description"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:157
+#: shoestring/wizard/screens/obligatory.py:155
 msgid "wizard-obligatory-private-key-generate-description"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:149
+#: shoestring/wizard/screens/obligatory.py:147
 msgid "wizard-obligatory-private-key-hex-description"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:136
+#: shoestring/wizard/screens/obligatory.py:134
 msgid "wizard-obligatory-private-key-hex-error-text"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:134
+#: shoestring/wizard/screens/obligatory.py:132
 msgid "wizard-obligatory-private-key-hex-label"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:177
+#: shoestring/wizard/screens/obligatory.py:175
 msgid "wizard-obligatory-title"
 msgstr ""
 
 #: shoestring/wizard/screens/obligatory.py:41
 msgid "wizard-obligatory-token-ca-pem-path"
 msgstr ""
 
@@ -763,46 +764,7 @@
 msgid "wizard-welcome-title"
 msgstr ""
 
 #: shoestring/wizard/screens/welcome.py:36
 msgid "wizard-welcome-upgrade"
 msgstr ""
 
-#~ msgid "wizard-network-type-mainnet"
-#~ msgstr ""
-
-#~ msgid "wizard-network-type-testnet"
-#~ msgstr ""
-
-#~ msgid "wizard-node-harvester-title"
-#~ msgstr ""
-
-#~ msgid "wizard-node-https-title"
-#~ msgstr ""
-
-#~ msgid "wizard-node-type-dual"
-#~ msgstr ""
-
-#~ msgid "wizard-node-type-peer"
-#~ msgstr ""
-
-#~ msgid "wizard-node-voter-title"
-#~ msgstr ""
-
-#~ msgid "wizard-peer-cert-names-title"
-#~ msgstr ""
-
-#~ msgid "wizard-welcome-steps"
-#~ msgstr ""
-
-#~ msgid "wizard-welcome-title"
-#~ msgstr ""
-
-#~ msgid "CA PEM file"
-#~ msgstr ""
-
-#~ msgid "Generate random private key"
-#~ msgstr ""
-
-#~ msgid "Import main private key in hex"
-#~ msgstr ""
-
```

### Comparing `symbol_shoestring-0.0.2/lang/messages.pot` & `symbol-shoestring-0.0.3/lang/messages.pot`

 * *Files 1% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 
 #: shoestring/commands/announce_transaction.py:36
 msgid "argument-help-announce-transaction-transaction"
 msgstr ""
 
 #: shoestring/commands/min_cosignatures_count.py:35
 #: shoestring/commands/renew_certificates.py:31
-#: shoestring/commands/setup.py:139 shoestring/commands/signer.py:95
+#: shoestring/commands/setup.py:139 shoestring/commands/signer.py:93
 msgid "argument-help-ca-key-path"
 msgstr ""
 
 #: shoestring/commands/announce_transaction.py:35
 #: shoestring/commands/health.py:75 shoestring/commands/import_bootstrap.py:28
 #: shoestring/commands/init.py:29
 #: shoestring/commands/min_cosignatures_count.py:34
 #: shoestring/commands/renew_certificates.py:29
 #: shoestring/commands/renew_voting_keys.py:112
 #: shoestring/commands/reset_data.py:87 shoestring/commands/setup.py:131
-#: shoestring/commands/signer.py:94
+#: shoestring/commands/signer.py:92
 msgid "argument-help-config"
 msgstr ""
 
 #: shoestring/commands/health.py:76
 #: shoestring/commands/renew_certificates.py:30
 #: shoestring/commands/renew_voting_keys.py:113
 #: shoestring/commands/reset_data.py:88 shoestring/commands/setup.py:133
@@ -78,19 +78,19 @@
 msgid "argument-help-setup-package"
 msgstr ""
 
 #: shoestring/commands/setup.py:138
 msgid "argument-help-setup-security"
 msgstr ""
 
-#: shoestring/commands/signer.py:97
+#: shoestring/commands/signer.py:95
 msgid "argument-help-signer-filename"
 msgstr ""
 
-#: shoestring/commands/signer.py:96
+#: shoestring/commands/signer.py:94
 msgid "argument-help-signer-save"
 msgstr ""
 
 #: shoestring/internal/FileDownloader.py:40
 msgid "file-downloader-already-downloaded"
 msgstr ""
 
@@ -163,19 +163,19 @@
 msgid "health-rest-api-error"
 msgstr ""
 
 #: shoestring/healthagents/rest_api.py:20
 msgid "health-rest-api-success"
 msgstr ""
 
-#: shoestring/healthagents/rest_https_certificate.py:55
+#: shoestring/healthagents/rest_https_certificate.py:96
 msgid "health-rest-https-certificate-invalid"
 msgstr ""
 
-#: shoestring/healthagents/rest_https_certificate.py:58
+#: shoestring/healthagents/rest_https_certificate.py:99
 msgid "health-rest-https-certificate-valid"
 msgstr ""
 
 #: shoestring/commands/health.py:70
 msgid "health-running-health-agent"
 msgstr ""
 
@@ -219,67 +219,67 @@
 msgid "import-bootstrap-importing-harvester"
 msgstr ""
 
 #: shoestring/commands/import_bootstrap.py:19
 msgid "import-bootstrap-importing-voter"
 msgstr ""
 
-#: shoestring/__main__.py:19
+#: shoestring/__main__.py:20
 msgid "main-announce-transaction-help"
 msgstr ""
 
-#: shoestring/__main__.py:20
+#: shoestring/__main__.py:21
 msgid "main-health-help"
 msgstr ""
 
-#: shoestring/__main__.py:21
+#: shoestring/__main__.py:22
 msgid "main-import-bootstrap-help"
 msgstr ""
 
-#: shoestring/__main__.py:22
+#: shoestring/__main__.py:23
 msgid "main-init-help"
 msgstr ""
 
-#: shoestring/__main__.py:23
+#: shoestring/__main__.py:24
 msgid "main-min-cosignatures-count-help"
 msgstr ""
 
-#: shoestring/__main__.py:24
+#: shoestring/__main__.py:25
 msgid "main-pemtool-help"
 msgstr ""
 
-#: shoestring/__main__.py:25
+#: shoestring/__main__.py:26
 msgid "main-renew-certificates-help"
 msgstr ""
 
-#: shoestring/__main__.py:26
+#: shoestring/__main__.py:27
 msgid "main-renew-voting-keys-help"
 msgstr ""
 
-#: shoestring/__main__.py:27
+#: shoestring/__main__.py:28
 msgid "main-reset-data-help"
 msgstr ""
 
-#: shoestring/__main__.py:28
+#: shoestring/__main__.py:29
 msgid "main-setup-help"
 msgstr ""
 
-#: shoestring/__main__.py:29
+#: shoestring/__main__.py:30
 msgid "main-signer-help"
 msgstr ""
 
-#: shoestring/__main__.py:17
+#: shoestring/__main__.py:18
 msgid "main-subcommands-help"
 msgstr ""
 
-#: shoestring/__main__.py:16
+#: shoestring/__main__.py:17
 msgid "main-title"
 msgstr ""
 
-#: shoestring/__main__.py:30
+#: shoestring/__main__.py:31
 msgid "main-upgrade-help"
 msgstr ""
 
 #: shoestring/commands/min_cosignatures_count.py:24
 msgid "min-cosignatures-count-cosignatures-detected"
 msgstr ""
 
@@ -367,15 +367,15 @@
 msgid "upgrade-purging-directory"
 msgstr ""
 
 #: shoestring/commands/upgrade.py:21
 msgid "upgrade-recreating-directory"
 msgstr ""
 
-#: shoestring/wizard/__main__.py:97 shoestring/wizard/buttons.py:29
+#: shoestring/wizard/__main__.py:99 shoestring/wizard/buttons.py:29
 msgid "wizard-button-finish"
 msgstr ""
 
 #: shoestring/wizard/buttons.py:53 shoestring/wizard/navigation.py:52
 msgid "wizard-button-next"
 msgstr ""
 
@@ -403,123 +403,123 @@
 msgid "wizard-certificates-peer-cert-label"
 msgstr ""
 
 #: shoestring/wizard/screens/certificates.py:50
 msgid "wizard-certificates-title"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:84
+#: shoestring/wizard/screens/obligatory.py:83
 msgid "wizard-dialog-message-generation-text"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:83
+#: shoestring/wizard/screens/obligatory.py:82
 msgid "wizard-dialog-message-generation-title"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:101
+#: shoestring/wizard/screens/obligatory.py:99
 msgid "wizard-dialog-message-import-text"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:100
+#: shoestring/wizard/screens/obligatory.py:98
 msgid "wizard-dialog-message-import-title"
 msgstr ""
 
 #: shoestring/wizard/screens/end_screen.py:19
 msgid "wizard-end-title"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:109
+#: shoestring/wizard/screens/harvesting.py:108
 msgid "wizard-harvesting-active"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:113
+#: shoestring/wizard/screens/harvesting.py:112
 msgid "wizard-harvesting-auto-harvest"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:148
+#: shoestring/wizard/screens/harvesting.py:147
 msgid "wizard-harvesting-beneficiary-address-error-text"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:146
+#: shoestring/wizard/screens/harvesting.py:145
 msgid "wizard-harvesting-beneficiary-address-label"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:130
+#: shoestring/wizard/screens/harvesting.py:129
 msgid "wizard-harvesting-delegate"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:117
+#: shoestring/wizard/screens/harvesting.py:116
 msgid "wizard-harvesting-generate-keys"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:136
+#: shoestring/wizard/screens/harvesting.py:135
 msgid "wizard-harvesting-max-unlocked-accounts-error-text"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:134
+#: shoestring/wizard/screens/harvesting.py:133
 msgid "wizard-harvesting-max-unlocked-accounts-label"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:142
+#: shoestring/wizard/screens/harvesting.py:141
 msgid "wizard-harvesting-min-fee-multiplier-error-text"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:140
+#: shoestring/wizard/screens/harvesting.py:139
 msgid "wizard-harvesting-min-fee-multiplier-label"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:123
+#: shoestring/wizard/screens/harvesting.py:122
 msgid "wizard-harvesting-signing-key-error-text"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:121
+#: shoestring/wizard/screens/harvesting.py:120
 msgid "wizard-harvesting-signing-key-label"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:170
+#: shoestring/wizard/screens/harvesting.py:169
 msgid "wizard-harvesting-title"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:80
+#: shoestring/wizard/screens/harvesting.py:79
 msgid "wizard-harvesting-token-active"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:83
+#: shoestring/wizard/screens/harvesting.py:82
 msgid "wizard-harvesting-token-auto-harvest"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:88
+#: shoestring/wizard/screens/harvesting.py:87
 msgid "wizard-harvesting-token-beneficiary-address"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:85
+#: shoestring/wizard/screens/harvesting.py:84
 msgid "wizard-harvesting-token-delegate"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:84
+#: shoestring/wizard/screens/harvesting.py:83
 msgid "wizard-harvesting-token-generate-keys"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:86
+#: shoestring/wizard/screens/harvesting.py:85
 msgid "wizard-harvesting-token-max-unlocked-accounts"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:87
+#: shoestring/wizard/screens/harvesting.py:86
 msgid "wizard-harvesting-token-min-fee-multiplier"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:127
+#: shoestring/wizard/screens/harvesting.py:126
 msgid "wizard-harvesting-vrf-key-error-text"
 msgstr ""
 
-#: shoestring/wizard/screens/harvesting.py:125
+#: shoestring/wizard/screens/harvesting.py:124
 msgid "wizard-harvesting-vrf-key-label"
 msgstr ""
 
-#: shoestring/wizard/__main__.py:103
+#: shoestring/wizard/__main__.py:104
 msgid "wizard-main-done"
 msgstr ""
 
 #: shoestring/wizard/TitleBar.py:26
 msgid "wizard-main-initial-title"
 msgstr ""
 
@@ -599,77 +599,77 @@
 msgid "wizard-node-type-title"
 msgstr ""
 
 #: shoestring/wizard/screens/node_type.py:16
 msgid "wizard-node-type-token"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:122
-#: shoestring/wizard/screens/obligatory.py:130
+#: shoestring/wizard/screens/obligatory.py:120
+#: shoestring/wizard/screens/obligatory.py:128
 msgid "wizard-obligatory-ca-pem-path-error-text"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:123
-#: shoestring/wizard/screens/obligatory.py:124
+#: shoestring/wizard/screens/obligatory.py:121
+#: shoestring/wizard/screens/obligatory.py:122
 msgid "wizard-obligatory-ca-pem-path-error-text-not-exist"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:128
+#: shoestring/wizard/screens/obligatory.py:126
 msgid "wizard-obligatory-ca-pem-path-label"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:109
+#: shoestring/wizard/screens/obligatory.py:107
 msgid "wizard-obligatory-destination-directory-error-text"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:107
+#: shoestring/wizard/screens/obligatory.py:105
 msgid "wizard-obligatory-destination-directory-label"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:142
+#: shoestring/wizard/screens/obligatory.py:140
 msgid "wizard-obligatory-generate-button"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:141
+#: shoestring/wizard/screens/obligatory.py:139
 msgid "wizard-obligatory-import-button"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:113
+#: shoestring/wizard/screens/obligatory.py:111
 msgid "wizard-obligatory-priv-ca"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:115
+#: shoestring/wizard/screens/obligatory.py:113
 msgid "wizard-obligatory-priv-generate-new"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:114
+#: shoestring/wizard/screens/obligatory.py:112
 msgid "wizard-obligatory-priv-import-hex"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:146
+#: shoestring/wizard/screens/obligatory.py:144
 msgid "wizard-obligatory-private-key-ca-pem-path-description"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:157
+#: shoestring/wizard/screens/obligatory.py:155
 msgid "wizard-obligatory-private-key-generate-description"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:149
+#: shoestring/wizard/screens/obligatory.py:147
 msgid "wizard-obligatory-private-key-hex-description"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:136
+#: shoestring/wizard/screens/obligatory.py:134
 msgid "wizard-obligatory-private-key-hex-error-text"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:134
+#: shoestring/wizard/screens/obligatory.py:132
 msgid "wizard-obligatory-private-key-hex-label"
 msgstr ""
 
-#: shoestring/wizard/screens/obligatory.py:177
+#: shoestring/wizard/screens/obligatory.py:175
 msgid "wizard-obligatory-title"
 msgstr ""
 
 #: shoestring/wizard/screens/obligatory.py:41
 msgid "wizard-obligatory-token-ca-pem-path"
 msgstr ""
```

### Comparing `symbol_shoestring-0.0.2/shoestring/__main__.py` & `symbol-shoestring-0.0.3/shoestring/__main__.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/commands/announce_transaction.py` & `symbol-shoestring-0.0.3/shoestring/commands/announce_transaction.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/commands/health.py` & `symbol-shoestring-0.0.3/shoestring/commands/health.py`

 * *Files 11% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 		if self.config.node.api_https:
 			return self.config_manager.lookup('config-node.properties', [('localnode', 'host')])[0]
 
 		return 'localhost'
 
 	def _load_rest_port(self):
 		if self.config.node.api_https:
-			return 3001  # TODO: should we read this from somewhere?
+			return 3001  # assume default HTTPS port
 
 		with open(self.directories.userconfig / 'rest.json', 'rt', encoding='utf8') as infile:
 			rest_json = json.loads(infile.read())
 			return int(rest_json['port'])
 
 
 async def run_main(args):
```

### Comparing `symbol_shoestring-0.0.2/shoestring/commands/import_bootstrap.py` & `symbol-shoestring-0.0.3/shoestring/commands/import_bootstrap.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/commands/init.py` & `symbol-shoestring-0.0.3/shoestring/commands/init.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/commands/min_cosignatures_count.py` & `symbol-shoestring-0.0.3/shoestring/commands/min_cosignatures_count.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/commands/pemtool.py` & `symbol-shoestring-0.0.3/shoestring/commands/pemtool.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/commands/renew_certificates.py` & `symbol-shoestring-0.0.3/shoestring/commands/renew_certificates.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/commands/renew_voting_keys.py` & `symbol-shoestring-0.0.3/shoestring/commands/renew_voting_keys.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/commands/reset_data.py` & `symbol-shoestring-0.0.3/shoestring/commands/reset_data.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/commands/setup.py` & `symbol-shoestring-0.0.3/shoestring/commands/setup.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/commands/signer.py` & `symbol-shoestring-0.0.3/shoestring/commands/signer.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,14 @@
 	key_pair = KeyPair(read_private_key_from_private_key_pem_file(args.ca_key_path, config.node.ca_password))
 
 	if _is_aggregate(transaction):  # change the aggregate signer to be a valid cosigner
 		transaction.signer_public_key = sc.PublicKey(key_pair.public_key.bytes)
 
 	_print_transaction(transaction)
 
-	# todo: query if it's ok to sign
-
 	transaction_hash = _sign_transaction(facade, key_pair, transaction)
 
 	if args.save:
 		write_transaction_to_file(transaction, Path(args.filename))
 
 	if sc.TransactionType.AGGREGATE_BONDED != transaction.type_:
 		return
```

### Comparing `symbol_shoestring-0.0.2/shoestring/commands/upgrade.py` & `symbol-shoestring-0.0.3/shoestring/commands/upgrade.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/healthagents/peer_api.py` & `symbol-shoestring-0.0.3/shoestring/healthagents/peer_api.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/healthagents/peer_certificate.py` & `symbol-shoestring-0.0.3/shoestring/healthagents/peer_certificate.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/healthagents/rest_api.py` & `symbol-shoestring-0.0.3/shoestring/healthagents/rest_api.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/healthagents/voting_keys.py` & `symbol-shoestring-0.0.3/shoestring/healthagents/voting_keys.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/healthagents/websockets.py` & `symbol-shoestring-0.0.3/shoestring/healthagents/websockets.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/internal/CertificateFactory.py` & `symbol-shoestring-0.0.3/shoestring/internal/CertificateFactory.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/internal/ConfigurationManager.py` & `symbol-shoestring-0.0.3/shoestring/internal/ConfigurationManager.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/internal/FileDownloader.py` & `symbol-shoestring-0.0.3/shoestring/internal/FileDownloader.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/internal/HarvesterConfigurator.py` & `symbol-shoestring-0.0.3/shoestring/internal/HarvesterConfigurator.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/internal/HeightGrouping.py` & `symbol-shoestring-0.0.3/shoestring/internal/HeightGrouping.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/internal/LinkTransactionBuilder.py` & `symbol-shoestring-0.0.3/shoestring/internal/LinkTransactionBuilder.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/internal/MultisigAnalyzer.py` & `symbol-shoestring-0.0.3/shoestring/internal/MultisigAnalyzer.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/internal/NodeDownloader.py` & `symbol-shoestring-0.0.3/shoestring/internal/NodeDownloader.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/internal/NodeFeatures.py` & `symbol-shoestring-0.0.3/shoestring/internal/NodeFeatures.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/internal/NodewatchClient.py` & `symbol-shoestring-0.0.3/shoestring/internal/NodewatchClient.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/internal/OpensslExecutor.py` & `symbol-shoestring-0.0.3/shoestring/internal/OpensslExecutor.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,10 +33,10 @@
 
 				if show_output:
 					sys.stdout.write(line)
 					sys.stdout.flush()
 
 			if 0 != process.returncode:
 				formatted_command_line = ' '.join(command_line)
-				raise RuntimeError(f'{formatted_command_line} exited with {process.returncode}')
+				raise RuntimeError(f'{formatted_command_line} exited with {process.returncode}, stdout:\n{stdout_lines}')
 
 		return all_lines
```

### Comparing `symbol_shoestring-0.0.2/shoestring/internal/PackageResolver.py` & `symbol-shoestring-0.0.3/shoestring/internal/PackageResolver.py`

 * *Files 7% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 			continue
 
 		seed_directory = subdir / 'seed'
 		if not seed_directory.is_dir():
 			continue
 
 		for file in subdir.glob('*'):
-			shutil.move(file, destination_directory)
+			shutil.move(str(file), str(destination_directory))
 
 		subdir.rmdir()
 
 		break
 	else:
 		raise RuntimeError('could not find package candidate directory')
```

### Comparing `symbol_shoestring-0.0.2/shoestring/internal/PeerDownloader.py` & `symbol-shoestring-0.0.3/shoestring/internal/PeerDownloader.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/internal/PemUtils.py` & `symbol-shoestring-0.0.3/shoestring/internal/PemUtils.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/internal/Preparer.py` & `symbol-shoestring-0.0.3/shoestring/internal/Preparer.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/internal/ShoestringConfiguration.py` & `symbol-shoestring-0.0.3/shoestring/internal/ShoestringConfiguration.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/internal/VoterConfigurator.py` & `symbol-shoestring-0.0.3/shoestring/internal/VoterConfigurator.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/Screen.py` & `symbol-shoestring-0.0.3/shoestring/wizard/Screen.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/Screens.py` & `symbol-shoestring-0.0.3/shoestring/wizard/ScreenContainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-class Screens:
+class ScreenContainer:
 	"""Container of screens."""
 
 	def __init__(self, navbar):
 		"""Creates a screen container."""
 
 		self.navbar = navbar  # added so that screens can access and modify it directly
 		self.ordered = []
```

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/ShoestringOperation.py` & `symbol-shoestring-0.0.3/shoestring/wizard/ShoestringOperation.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/TabbedView.py` & `symbol-shoestring-0.0.3/shoestring/wizard/TabbedView.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,59 +41,65 @@
 		kb = self.control.key_bindings  # pylint: disable=invalid-name
 		_up = kb.get_bindings_for_keys((Keys.Up, ))[-1]
 		_down = kb.get_bindings_for_keys((Keys.Down, ))[-1]
 		kb.add('left',)(_up.handler)
 		kb.add('right',)(_down.handler)
 
 	def _get_text_fragments(self):
-		# TODO: this mouse handler is likely wrong I (gimre) cannot verify/test it
-		def mouse_handler(mouse_event):
-			"""
-			Set `_selected_index` and `current_value` according to the y
-			position of the mouse click event.
-			"""
-			if mouse_event.event_type == MouseEventType.MOUSE_UP:
-				# self._selected_index = mouse_event.position.y
-				# self._handle_enter()
-				pass
+		def create_mouse_handler(selected_index):
+			def mouse_handler(mouse_event):
+				"""
+				Set `_selected_index` and `current_value` according to the y
+				position of the mouse click event.
+				"""
+				if mouse_event.event_type == MouseEventType.MOUSE_UP:
+					self._selected_index = selected_index
+					self._handle_enter()
+
+			return mouse_handler
+
+		def fragments_to_items(selected_index, fragments):
+			return map(lambda item: (*item, create_mouse_handler(selected_index)), fragments)
 
 		result = []
 		for i, value in enumerate(self.values):
+			fragments = []
 			checked = value[0] == self.current_value
 			selected = i == self._selected_index
 
 			style = self.default_style
 			if checked:
 				style += ' ' + self.checked_style
 			if selected:
 				style += ' ' + self.selected_style
 
 			# note: the else condition relies on the fact, that values are 0-based indexes
 			if checked:
-				result.append(('', Border.VERTICAL))
+				fragments.append(('', Border.VERTICAL))
 			elif i - 1 != self.current_value:
-				result.append(('', ' '))
+				fragments.append(('', ' '))
 
 			if checked:
-				result.append((style, ' *'))
+				fragments.append((style, ' *'))
 			else:
-				result.append((style, '  '))
+				fragments.append((style, '  '))
 
 			if selected:
-				result.append(('[SetCursorPosition]', ''))
+				fragments.append(('[SetCursorPosition]', ''))
 
-			result.append((style, ' '))
-			result.extend(to_formatted_text(value[1], style=style))
-			result.append((style, ' '))
+			fragments.append((style, ' '))
+			fragments.extend(to_formatted_text(value[1], style=style))
+			fragments.append((style, ' '))
 
 			if checked:
-				result.append(('', Border.VERTICAL))
+				fragments.append(('', Border.VERTICAL))
+
+			result.extend(fragments_to_items(i, fragments))
 
-		# Add mouse handler to all fragments.
-		return list(map(lambda item: (*item, mouse_handler), result))
+		return result
 
 
 def _create_condition(controller, index):
 	return Condition(lambda: controller.current_value == index)
 
 
 class Tabs(HSplit):
```

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/TitleBar.py` & `symbol-shoestring-0.0.3/shoestring/wizard/TitleBar.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/ValidatingTextBox.py` & `symbol-shoestring-0.0.3/shoestring/wizard/ValidatingTextBox.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/__main__.py` & `symbol-shoestring-0.0.3/shoestring/wizard/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from shoestring.__main__ import main as shoestring_main
 from shoestring.wizard.screens.modal import create as create_message_box_float
 from shoestring.wizard.screens.modal import show as show_message_box
 
 from . import keybindings, navigation, styles
 from .buttons import create_next_clicked_handler, create_operation_button_handler, create_prev_clicked_handler
 from .screen_loader import load_screens
-from .Screens import Screens
+from .ScreenContainer import ScreenContainer
 from .shoestring_dispatcher import dispatch_shoestring_command
 from .TitleBar import TitleBar
 
 
 async def main():  # pylint: disable=too-many-locals
 	lang_directory = Path(__file__).resolve().parent.parent.parent / 'lang'
 	lang = gettext.translation('messages', localedir=lang_directory, languages=(os.environ.get('LC_MESSAGES', 'en'), 'en'))
@@ -33,15 +33,15 @@
 
 	message_box_float = create_message_box_float()
 
 	key_bindings = keybindings.initialize(lambda: message_box_float.visible)
 	app_styles = styles.initialize()
 	navbar = navigation.initialize()
 
-	screens = Screens(navbar)
+	screens = ScreenContainer(navbar)
 	load_screens(screens)
 	screens.message_box = partial(show_message_box, message_box_float)
 
 	main_container = screens.current
 	root_container = HSplit([
 		# note: we can use this titlebar to show where are we in the wizard
 		Label(style='class:titlebar', text=HTML('')),
@@ -71,15 +71,15 @@
 	root_with_dialog_box = FloatContainer(
 		content=root_container,
 		floats=[message_box_float],
 		modal=True
 	)
 	layout = Layout(root_with_dialog_box, focused_element=navbar.next)
 
-	app = Application(layout, key_bindings=key_bindings, style=app_styles, full_screen=True)
+	app = Application(layout, key_bindings=key_bindings, style=app_styles, full_screen=True, mouse_support=True)
 
 	layout.focus(root_container.children[2])
 
 	# set navigation bar button handlers
 
 	def activate_screen(screen):
 		root_container.children[2] = screen
@@ -95,15 +95,14 @@
 
 	result = await app.run_async()
 
 	# second condition is temporarily added, to break processing when ctrl-q or ctrl-c is pressed
 	if result or navbar.next.text != _('wizard-button-finish'):
 		return
 
-	# TODO: temporary here, move up
 	await dispatch_shoestring_command(screens, shoestring_main)
 
 	log.info(_('wizard-main-done'))
 
 
 if '__main__' == __name__:
 	asyncio.run(main())
```

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/buttons.py` & `symbol-shoestring-0.0.3/shoestring/wizard/buttons.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/navigation.py` & `symbol-shoestring-0.0.3/shoestring/wizard/navigation.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/screen_loader.py` & `symbol-shoestring-0.0.3/shoestring/wizard/screen_loader.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/screens/certificates.py` & `symbol-shoestring-0.0.3/shoestring/wizard/screens/certificates.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/screens/end_screen.py` & `symbol-shoestring-0.0.3/shoestring/wizard/screens/end_screen.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/screens/harvesting.py` & `symbol-shoestring-0.0.3/shoestring/wizard/screens/harvesting.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from shoestring.wizard.Screen import ScreenDialog
 from shoestring.wizard.styles import to_enabled_string
 from shoestring.wizard.ValidatingTextBox import ValidatingTextBox, is_hex_private_key_string, is_integer
 
 
 def facade(screens):
-	# TODO: not sure if this makes sense
 	network = 'mainnet' if 'mainnet' == screens.get('network-type').current_value else 'testnet'
 	return SymbolFacade(network)
 
 
 class HarvestingSettings:
 	# pylint: disable=too-many-instance-attributes
```

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/screens/modal.py` & `symbol-shoestring-0.0.3/shoestring/wizard/screens/modal.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/screens/network_type.py` & `symbol-shoestring-0.0.3/shoestring/wizard/screens/network_type.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/screens/node_settings.py` & `symbol-shoestring-0.0.3/shoestring/wizard/screens/node_settings.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/screens/node_type.py` & `symbol-shoestring-0.0.3/shoestring/wizard/screens/node_type.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/screens/obligatory.py` & `symbol-shoestring-0.0.3/shoestring/wizard/screens/obligatory.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,15 +68,14 @@
 	return ca_pem_path.input.buffer.validate()
 
 
 def generate_handler(screens, ca_pem_path, on_close_callback):
 	if not ca_pem_path.is_valid:
 		return
 
-	# TODO (optionally): password
 	filepath = Path(ca_pem_path.input.text)
 	storage = PrivateKeyStorage(filepath.parent.absolute())
 
 	if filepath.suffix == '.pem':
 		storage.save(filepath.stem, PrivateKey.random())
 
 	screens.message_box(
@@ -88,15 +87,14 @@
 def import_handler(screens, ca_pem_path, on_close_callback, private_key_hex):
 	if not ca_pem_path.is_valid or not private_key_hex.is_valid:
 		return
 
 	filepath = Path(ca_pem_path.input.text)
 	storage = PrivateKeyStorage(filepath.parent.absolute())
 
-	# TODO (optionally): password
 	if filepath.suffix == '.pem':
 		storage.save(filepath.stem, PrivateKey(private_key_hex.input.text))
 
 	screens.message_box(
 		title=_('wizard-dialog-message-import-title'),
 		text=_('wizard-dialog-message-import-text'),
 		on_close_callback=on_close_callback)
@@ -185,15 +183,15 @@
 					VSplit([
 						HSplit([ca_pem_path.label], width=40),
 						HSplit([ca_pem_path.input])
 					]),
 					filter=show_private_key_tabs
 				),
 				ConditionalContainer(main_private_key_tabs, filter=show_private_key_tabs)
-			], width=200),
+			]),
 			padding=1
 		),
 
 		accessor=ObligatorySettings(destination_directory, ca_pem_path),
 		is_valid=lambda: destination_directory.is_valid and (
 			not dialog.accessor.is_main_private_key_required or (
 				revalidate_ca_pem_path(ca_pem_path) and main_private_key_tabs.is_valid
```

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/screens/root_check.py` & `symbol-shoestring-0.0.3/shoestring/wizard/screens/root_check.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/screens/voting.py` & `symbol-shoestring-0.0.3/shoestring/wizard/screens/voting.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/screens/welcome.py` & `symbol-shoestring-0.0.3/shoestring/wizard/screens/welcome.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/setup_file_generator.py` & `symbol-shoestring-0.0.3/shoestring/wizard/setup_file_generator.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/shoestring_dispatcher.py` & `symbol-shoestring-0.0.3/shoestring/wizard/shoestring_dispatcher.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/shoestring/wizard/styles.py` & `symbol-shoestring-0.0.3/shoestring/wizard/styles.py`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/templates/docker-compose-dual.yaml` & `symbol-shoestring-0.0.3/templates/docker-compose-dual.yaml`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/templates/docker-compose-peer.yaml` & `symbol-shoestring-0.0.3/templates/docker-compose-peer.yaml`

 * *Files identical despite different names*

### Comparing `symbol_shoestring-0.0.2/PKG-INFO` & `symbol-shoestring-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 Metadata-Version: 2.1
 Name: symbol-shoestring
-Version: 0.0.2
+Version: 0.0.3
 Summary: Symbol Shoestring Deployment Tool
 Home-page: https://github.com/symbol/product/tree/main/tools/shoestring
 License: MIT
 Keywords: symbol,shoestring,deployment,node
 Author: Symbol Contributors
 Author-email: contributors@symbol.dev
 Maintainer: Symbol Contributors
 Maintainer-email: contributors@symbol.dev
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
+Requires-Dist: Jinja2 (==3.1.2)
+Requires-Dist: PyYAML (==6.0.1)
+Requires-Dist: aiohttp (==3.8.5)
+Requires-Dist: prompt-toolkit (==3.0.39)
+Requires-Dist: requests (==2.31.0)
+Requires-Dist: symbol-lightapi (==0.0.4)
+Requires-Dist: symbol-sdk-python (==3.0.11)
+Requires-Dist: websockets (==11.0.3)
+Requires-Dist: zenlog (==1.1)
 Project-URL: Repository, https://github.com/symbol/product/tree/main/tools/shoestring
 Description-Content-Type: text/markdown
 
 # shoestring
 
 # CLI Commands
```

