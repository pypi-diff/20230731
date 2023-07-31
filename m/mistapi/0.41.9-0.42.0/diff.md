# Comparing `tmp/mistapi-0.41.9.tar.gz` & `tmp/mistapi-0.42.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistapi-0.41.9.tar", last modified: Fri Jun 23 09:02:13 2023, max compression
+gzip compressed data, was "mistapi-0.42.0.tar", last modified: Mon Jul 31 13:11:03 2023, max compression
```

## Comparing `mistapi-0.41.9.tar` & `mistapi-0.42.0.tar`

### file list

```diff
@@ -1,237 +1,237 @@
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-23 09:02:13.130292 mistapi-0.41.9/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-01-13 07:55:51.000000 mistapi-0.41.9/LICENSE
--rw-r--r--   0 tmunzer    (502) staff       (20)    11281 2023-06-23 09:02:13.130521 mistapi-0.41.9/PKG-INFO
--rw-r--r--   0 tmunzer    (502) staff       (20)    10505 2023-06-13 20:27:38.000000 mistapi-0.41.9/README.md
--rw-r--r--   0 tmunzer    (502) staff       (20)      976 2023-06-23 09:02:07.000000 mistapi-0.41.9/pyproject.toml
--rw-r--r--   0 tmunzer    (502) staff       (20)      125 2023-06-23 09:02:13.130899 mistapi-0.41.9/setup.cfg
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-23 09:02:13.022473 mistapi-0.41.9/src/
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-23 09:02:13.035900 mistapi-0.41.9/src/mistapi/
--rw-r--r--   0 tmunzer    (502) staff       (20)    11088 2023-06-20 17:18:42.000000 mistapi-0.41.9/src/mistapi/__api_request.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2960 2023-06-20 17:15:44.000000 mistapi-0.41.9/src/mistapi/__api_response.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    23529 2023-06-23 09:01:34.000000 mistapi-0.41.9/src/mistapi/__api_session.py
--rw-r--r--   0 tmunzer    (502) staff       (20)      635 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2245 2023-06-20 17:16:22.000000 mistapi-0.41.9/src/mistapi/__logger.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-23 09:02:13.039084 mistapi-0.41.9/src/mistapi/__models/
--rw-r--r--   0 tmunzer    (502) staff       (20)        0 2023-02-21 08:35:01.000000 mistapi-0.41.9/src/mistapi/__models/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1530 2023-05-30 09:43:55.000000 mistapi-0.41.9/src/mistapi/__models/privilege.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2071 2023-06-20 17:17:24.000000 mistapi-0.41.9/src/mistapi/__pagination.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-23 09:02:13.039426 mistapi-0.41.9/src/mistapi/api/
--rw-r--r--   0 tmunzer    (502) staff       (20)      446 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-23 09:02:13.039751 mistapi-0.41.9/src/mistapi/api/v1/
--rw-r--r--   0 tmunzer    (502) staff       (20)      869 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-23 09:02:13.045880 mistapi-0.41.9/src/mistapi/api/v1/const/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1235 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/const/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1759 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/const/alarm_defs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2047 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/const/ap_channels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1760 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/const/ap_led_status.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/const/applications.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1786 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/const/call_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/const/client_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1737 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/const/countries.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1417 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/const/default_gateway_config.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/const/device_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/const/device_models.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1759 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/const/insight_metrics.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1742 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/const/languages.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/const/license_types.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/const/mxedge_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/const/mxedge_models.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1837 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/const/other_device_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/const/traffic_types.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-23 09:02:13.046203 mistapi-0.41.9/src/mistapi/api/v1/installer/
--rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/installer/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-23 09:02:13.048890 mistapi-0.41.9/src/mistapi/api/v1/installer/orgs/
--rw-r--r--   0 tmunzer    (502) staff       (20)      798 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/installer/orgs/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1988 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/installer/orgs/alarmtemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1988 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/installer/orgs/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7257 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/installer/orgs/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1992 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/installer/orgs/rftemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1967 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/installer/orgs/secpolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1960 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/installer/orgs/sitegroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7693 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/installer/orgs/sites.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-23 09:02:13.049538 mistapi-0.41.9/src/mistapi/api/v1/installer/sites/
--rw-r--r--   0 tmunzer    (502) staff       (20)      471 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/installer/sites/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1178 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/installer/sites/optimize.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-23 09:02:13.050198 mistapi-0.41.9/src/mistapi/api/v1/invite/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/invite/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1109 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/invite/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-23 09:02:13.052038 mistapi-0.41.9/src/mistapi/api/v1/login/
--rw-r--r--   0 tmunzer    (502) staff       (20)      584 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/login/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1154 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/login/login.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1163 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/login/lookup.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2656 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/login/oauth.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1173 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/login/two_factor.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-23 09:02:13.052739 mistapi-0.41.9/src/mistapi/api/v1/logout/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/logout/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)      999 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/logout/logout.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-23 09:02:13.053819 mistapi-0.41.9/src/mistapi/api/v1/mobile/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/mobile/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1270 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/mobile/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-23 09:02:13.060595 mistapi-0.41.9/src/mistapi/api/v1/msps/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1104 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/msps/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3925 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/msps/admins.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1263 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/msps/claim.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1746 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/msps/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1210 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/msps/inventory.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2693 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/msps/invites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2653 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/msps/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1851 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/msps/logo.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4542 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/msps/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3032 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/msps/msps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/msps/orggroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5309 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/msps/orgs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1674 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/msps/search.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4048 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/msps/ssoroles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6037 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/msps/ssos.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3709 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/msps/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1518 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/msps/suggestion.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3269 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/msps/tickets.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-23 09:02:13.096032 mistapi-0.41.9/src/mistapi/api/v1/orgs/
--rw-r--r--   0 tmunzer    (502) staff       (20)     3208 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3288 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/admins.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6526 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/alarms.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7670 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/alarmtemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/apitokens.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4781 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/aptemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4813 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/assetfilters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6148 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/assets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2337 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/call.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1729 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/cert.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1263 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/claim.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    11558 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1249 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/clone.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1869 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/crl.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7161 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    20361 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4863 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/evpn_topologies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4921 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/gatewaytemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6601 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/guests.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2959 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5098 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/inventory.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2693 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/invites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7004 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/jsi.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2536 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5309 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1910 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/maps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4805 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/mxclusters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    15544 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/mxedges.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/mxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4697 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/nacrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4669 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/nactags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4697 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/networks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4923 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/networktemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1417 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/ocdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3026 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/orgs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8805 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/otherdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1933 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/pma.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4753 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/pskportals.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8448 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/psks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4781 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/rftemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1324 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/sdkclients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6964 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/sdkinvites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4770 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/sdktemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4772 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/secpolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4876 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/servicepolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4697 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/services.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    16846 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/setting.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4753 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/sitegroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8845 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/sites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4839 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/sitetemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4697 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/ssoroles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8322 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/ssos.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4823 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/ssr.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    32619 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1767 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5508 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/templates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7068 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/tickets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1764 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/troubleshoot.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4592 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/vpns.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1374 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/wan_client.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4868 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/wan_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4697 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/webhooks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3602 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/wired_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7620 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/wlans.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5297 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/wxrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5953 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/wxtags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/orgs/wxtunnels.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-23 09:02:13.097139 mistapi-0.41.9/src/mistapi/api/v1/recover/
--rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/recover/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1176 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/recover/recover.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1120 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/recover/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-23 09:02:13.098107 mistapi-0.41.9/src/mistapi/api/v1/register/
--rw-r--r--   0 tmunzer    (502) staff       (20)      508 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/register/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1179 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/register/register.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1113 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/register/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-23 09:02:13.101497 mistapi-0.41.9/src/mistapi/api/v1/self/
--rw-r--r--   0 tmunzer    (502) staff       (20)      707 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/self/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2974 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/self/apitokens.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2654 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/self/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2033 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/self/oauth.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2157 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/self/self.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1773 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/self/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1884 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/self/two_factor.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1784 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/self/update.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-23 09:02:13.128317 mistapi-0.41.9/src/mistapi/api/v1/sites/
--rw-r--r--   0 tmunzer    (502) staff       (20)     2588 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8779 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/alarms.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2660 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/anomaly.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1881 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/apps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4848 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/assetfilters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6197 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/assets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4710 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/beacons.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2349 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/call.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    17510 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2418 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/count.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2356 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    59188 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5139 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4114 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/evpn_topologies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7121 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/guests.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     9228 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1167 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8644 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/location.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    15814 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/maps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5353 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/mxedges.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1189 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/mxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2314 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/networks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5879 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/otherdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5899 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/pcaps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7696 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/psks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5817 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/rfdiags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5813 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/rogues.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3862 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/rrm.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4762 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/rssizones.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2363 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/servicepolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2314 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/services.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6134 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/setting.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2437 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/sites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3886 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/skyatp.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    20773 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/sle.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1983 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/ssr.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    62170 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1727 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1928 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/synthetic_test.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4684 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/uisettings.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4734 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/vbeacons.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2308 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/visits.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2286 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/vpns.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1380 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/wan_client.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4886 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/wan_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5356 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/webhooks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3890 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/wired_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6960 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/wlans.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5340 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/wxrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6002 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/wxtags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4762 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/wxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4650 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/sites/zones.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-23 09:02:13.130062 mistapi-0.41.9/src/mistapi/api/v1/utils/
--rw-r--r--   0 tmunzer    (502) staff       (20)      511 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/utils/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1087 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/utils/test_telstra.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1202 2023-06-23 09:02:07.000000 mistapi-0.41.9/src/mistapi/api/v1/utils/test_twilio.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    11956 2023-06-23 07:23:05.000000 mistapi-0.41.9/src/mistapi/cli.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-06-23 09:02:13.038339 mistapi-0.41.9/src/mistapi.egg-info/
--rw-r--r--   0 tmunzer    (502) staff       (20)    11281 2023-06-23 09:02:12.000000 mistapi-0.41.9/src/mistapi.egg-info/PKG-INFO
--rw-r--r--   0 tmunzer    (502) staff       (20)     7781 2023-06-23 09:02:13.000000 mistapi-0.41.9/src/mistapi.egg-info/SOURCES.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)        1 2023-06-23 09:02:12.000000 mistapi-0.41.9/src/mistapi.egg-info/dependency_links.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)       66 2023-06-23 09:02:12.000000 mistapi-0.41.9/src/mistapi.egg-info/requires.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)        8 2023-06-23 09:02:12.000000 mistapi-0.41.9/src/mistapi.egg-info/top_level.txt
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-07-31 13:11:03.454388 mistapi-0.42.0/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-01-13 07:55:51.000000 mistapi-0.42.0/LICENSE
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11281 2023-07-31 13:11:03.454550 mistapi-0.42.0/PKG-INFO
+-rw-r--r--   0 tmunzer    (502) staff       (20)    10505 2023-06-13 20:27:38.000000 mistapi-0.42.0/README.md
+-rw-r--r--   0 tmunzer    (502) staff       (20)      976 2023-07-31 13:10:35.000000 mistapi-0.42.0/pyproject.toml
+-rw-r--r--   0 tmunzer    (502) staff       (20)      125 2023-07-31 13:11:03.455278 mistapi-0.42.0/setup.cfg
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-07-31 13:11:03.338897 mistapi-0.42.0/src/
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-07-31 13:11:03.347591 mistapi-0.42.0/src/mistapi/
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11088 2023-06-20 17:18:42.000000 mistapi-0.42.0/src/mistapi/__api_request.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2960 2023-06-20 17:15:44.000000 mistapi-0.42.0/src/mistapi/__api_response.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    24895 2023-07-31 13:09:25.000000 mistapi-0.42.0/src/mistapi/__api_session.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)      635 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2245 2023-06-20 17:16:22.000000 mistapi-0.42.0/src/mistapi/__logger.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-07-31 13:11:03.349581 mistapi-0.42.0/src/mistapi/__models/
+-rw-r--r--   0 tmunzer    (502) staff       (20)        0 2023-02-21 08:35:01.000000 mistapi-0.42.0/src/mistapi/__models/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1530 2023-05-30 09:43:55.000000 mistapi-0.42.0/src/mistapi/__models/privilege.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2071 2023-06-20 17:17:24.000000 mistapi-0.42.0/src/mistapi/__pagination.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-07-31 13:11:03.349998 mistapi-0.42.0/src/mistapi/api/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      446 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-07-31 13:11:03.350274 mistapi-0.42.0/src/mistapi/api/v1/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      869 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-07-31 13:11:03.356695 mistapi-0.42.0/src/mistapi/api/v1/const/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1189 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/const/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1759 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/const/alarm_defs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2047 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/const/ap_channels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1760 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/const/ap_led_status.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/const/applications.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/const/client_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1737 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/const/countries.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1412 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/const/default_gateway_config.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/const/device_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/const/device_models.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1759 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/const/insight_metrics.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1742 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/const/languages.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/const/license_types.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/const/mxedge_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/const/mxedge_models.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1837 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/const/other_device_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/const/traffic_types.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-07-31 13:11:03.357068 mistapi-0.42.0/src/mistapi/api/v1/installer/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/installer/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-07-31 13:11:03.359798 mistapi-0.42.0/src/mistapi/api/v1/installer/orgs/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      798 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/installer/orgs/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1988 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/installer/orgs/alarmtemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1988 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/installer/orgs/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7099 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/installer/orgs/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1992 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/installer/orgs/rftemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1967 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/installer/orgs/secpolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1960 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/installer/orgs/sitegroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7279 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/installer/orgs/sites.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-07-31 13:11:03.360544 mistapi-0.42.0/src/mistapi/api/v1/installer/sites/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      471 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/installer/sites/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1178 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/installer/sites/optimize.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-07-31 13:11:03.361324 mistapi-0.42.0/src/mistapi/api/v1/invite/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/invite/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1109 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/invite/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-07-31 13:11:03.362822 mistapi-0.42.0/src/mistapi/api/v1/login/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      584 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/login/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1154 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/login/login.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1163 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/login/lookup.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2656 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/login/oauth.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1173 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/login/two_factor.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-07-31 13:11:03.363469 mistapi-0.42.0/src/mistapi/api/v1/logout/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/logout/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)      999 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/logout/logout.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-07-31 13:11:03.364085 mistapi-0.42.0/src/mistapi/api/v1/mobile/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/mobile/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1270 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/mobile/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-07-31 13:11:03.370355 mistapi-0.42.0/src/mistapi/api/v1/msps/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1104 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/msps/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3925 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/msps/admins.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1263 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/msps/claim.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1746 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/msps/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1210 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/msps/inventory.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2693 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/msps/invites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2653 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/msps/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1851 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/msps/logo.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4542 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/msps/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3032 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/msps/msps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/msps/orggroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5309 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/msps/orgs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1674 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/msps/search.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4048 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/msps/ssoroles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7398 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/msps/ssos.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3709 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/msps/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1518 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/msps/suggestion.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3269 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/msps/tickets.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-07-31 13:11:03.416091 mistapi-0.42.0/src/mistapi/api/v1/orgs/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3253 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3288 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/admins.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6526 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/alarms.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7670 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/alarmtemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/apitokens.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4781 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/aptemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4813 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/assetfilters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6148 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/assets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2337 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/call.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1729 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/cert.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1263 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/claim.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11558 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1249 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/clone.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1869 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/crl.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7161 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    18956 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4863 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/evpn_topologies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4921 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/gatewaytemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6601 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/guests.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4781 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/idpprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2959 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5098 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/inventory.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2693 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/invites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7004 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/jsi.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2536 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5309 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1187 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/maps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4805 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/mxclusters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    17111 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/mxedges.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/mxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4697 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/nacrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4669 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/nactags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4697 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/networks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4923 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/networktemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1417 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/ocdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3018 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/orgs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8805 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/otherdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1933 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/pma.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    10111 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/pskportals.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8448 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/psks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4781 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/rftemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1324 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/sdkclients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6964 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/sdkinvites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4770 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/sdktemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4772 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/secpolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4876 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/servicepolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4697 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/services.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    16846 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/setting.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4753 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/sitegroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8632 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/sites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4839 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/sitetemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4697 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/ssoroles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8322 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/ssos.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5758 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/ssr.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    32619 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1767 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5508 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/templates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7068 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/tickets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1764 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/troubleshoot.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4592 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/vpns.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1374 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/wan_client.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4868 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/wan_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6797 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/webhooks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3602 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/wired_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6798 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/wlans.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5297 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/wxrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5953 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/wxtags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/orgs/wxtunnels.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-07-31 13:11:03.417010 mistapi-0.42.0/src/mistapi/api/v1/recover/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      505 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/recover/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1176 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/recover/recover.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1120 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/recover/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-07-31 13:11:03.417902 mistapi-0.42.0/src/mistapi/api/v1/register/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      508 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/register/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1179 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/register/register.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1113 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/register/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-07-31 13:11:03.420522 mistapi-0.42.0/src/mistapi/api/v1/self/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      707 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/self/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4317 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/self/apitokens.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2654 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/self/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2033 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/self/oauth.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2157 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/self/self.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1773 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/self/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1884 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/self/two_factor.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1784 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/self/update.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-07-31 13:11:03.453123 mistapi-0.42.0/src/mistapi/api/v1/sites/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2588 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8779 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/alarms.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2660 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/anomaly.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1881 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/apps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4848 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/assetfilters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6197 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/assets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4710 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/beacons.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2349 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/call.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    17510 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2418 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/count.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2356 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    60656 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5139 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4114 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/evpn_topologies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7121 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/guests.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     9228 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1167 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8644 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/location.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    15093 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/maps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5353 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/mxedges.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1189 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/mxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2314 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/networks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5879 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/otherdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5899 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/pcaps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7696 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/psks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5817 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/rfdiags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5809 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/rogues.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3862 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/rrm.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4762 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/rssizones.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2363 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/servicepolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2314 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/services.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6134 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/setting.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2437 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/sites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3886 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/skyatp.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    20772 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/sle.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1983 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/ssr.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    62756 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1751 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1928 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/synthetic_test.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5455 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/uisettings.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4734 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/vbeacons.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2308 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/visits.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2286 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/vpns.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1380 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/wan_client.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4886 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/wan_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6780 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/webhooks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3867 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/wired_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7902 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/wlans.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5340 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/wxrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6002 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/wxtags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4762 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/wxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4650 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/sites/zones.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-07-31 13:11:03.454157 mistapi-0.42.0/src/mistapi/api/v1/utils/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      511 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/utils/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1205 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/utils/test_telstra.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1202 2023-07-31 13:10:35.000000 mistapi-0.42.0/src/mistapi/api/v1/utils/test_twilio.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    12053 2023-07-10 08:34:04.000000 mistapi-0.42.0/src/mistapi/cli.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2023-07-31 13:11:03.349044 mistapi-0.42.0/src/mistapi.egg-info/
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11281 2023-07-31 13:11:03.000000 mistapi-0.42.0/src/mistapi.egg-info/PKG-INFO
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7780 2023-07-31 13:11:03.000000 mistapi-0.42.0/src/mistapi.egg-info/SOURCES.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)        1 2023-07-31 13:11:03.000000 mistapi-0.42.0/src/mistapi.egg-info/dependency_links.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)       66 2023-07-31 13:11:03.000000 mistapi-0.42.0/src/mistapi.egg-info/requires.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)        8 2023-07-31 13:11:03.000000 mistapi-0.42.0/src/mistapi.egg-info/top_level.txt
```

### Comparing `mistapi-0.41.9/LICENSE` & `mistapi-0.42.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/PKG-INFO` & `mistapi-0.42.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistapi
-Version: 0.41.9
+Version: 0.42.0
 Summary: Python package to simplify the Mist System APIs usage
 Author-email: Thomas Munzer <tmunzer@juniper.net>
 License: MIT
 Project-URL: Source, https://github.com/tmunzer/mistapi_python
 Project-URL: Bug Tracker, https://github.com/tmunzer/mistapi_python/issues
 Keywords: Mist,Juniper,API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mistapi-0.41.9/README.md` & `mistapi-0.42.0/README.md`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/pyproject.toml` & `mistapi-0.42.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mistapi"
-version = "0.41.9"
+version = "0.42.0"
 authors = [{name="Thomas Munzer", email="tmunzer@juniper.net"}]
 description = "Python package to simplify the Mist System APIs usage"
 keywords = ["Mist", "Juniper", "API"]
 license = {text =  "MIT"}
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mistapi-0.41.9/src/mistapi/__api_request.py` & `mistapi-0.42.0/src/mistapi/__api_request.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/__api_response.py` & `mistapi-0.42.0/src/mistapi/__api_response.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/__api_session.py` & `mistapi-0.42.0/src/mistapi/__api_session.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,20 +8,20 @@
     This package is licensed under the MIT License.
 
 --------------------------------------------------------------------------------
 This module provide the APISession class, which is used to manage authentication
 and HTTP session (if login/password is used) with Mist Cloud.
 """
 
+from pathlib import Path
+from getpass import getpass
 import os
 import sys
 import requests
 from dotenv import load_dotenv
-from pathlib import Path
-from getpass import getpass
 
 from mistapi.__logger import logger, console
 from mistapi.__api_request import APIRequest
 from mistapi.__api_response import APIResponse
 from mistapi.__models.privilege import Privileges
 
 
@@ -46,53 +46,72 @@
         email: str = None,
         password: str = None,
         apitoken: str = None,
         host: str = None,
         env_file: str = None,
         console_log_level: str = 20,
         logging_log_level: int = 10,
+        show_cli_notif: bool = True,
     ):
         """
         PARAMS
         -----------
         email : str
             used if login/password is used. Can be defined later
         password : str
             used if login/password is used. Can be defined later
         apitoken : str
             used if API Token is used. Can de defined later
         host : str
             Mist Cloud to reach (e.g. "api.mist.com"). Can de defined later
         env_file : str
             path to the env file to load. See README.md for allowed variables
-        console_log_level : int
-            param int logging_log_level
+        console_log_level : int, default: 20
+            Log level for the console output. Values are:
+                50 -> CRITICAL
+                40 -> ERROR
+                30 -> WARNING
+                20 -> INFO
+                10 -> DEBUG
+                0  -> DISABLED
+        logging_log_level : int, default: 10
+            Log level for the log file output. Values are:
+                Values:
+                50 -> CRITICAL
+                40 -> ERROR
+                30 -> WARNING
+                20 -> INFO
+                10 -> DEBUG
+                0  -> DISABLED
+        show_cli_notif : bool, default True
+            show/hide package decorative text on the console output
         """
         self._cloud_uri = None
         self.email = None
         self._password = None
         self._apitoken = None
         self._csrftoken = None
         self._authenticated = False
         self._session = requests.session()
         self._console_log_level = console_log_level
         self._logging_log_level = logging_log_level
+        self._show_cli_notif = show_cli_notif
 
         console._set_log_level(console_log_level, logging_log_level)
 
         self._load_env(env_file)
 
         if host:
-            self._cloud_uri = host
+            self.set_cloud(host)
         if email:
-            self.email = email
+            self.set_email(email)
         if password:
-            self._password = password
+            self.set_password(password)
         if apitoken:
-            self._apitoken = apitoken
+            self.set_api_token(apitoken)
         self.first_name = ""
         self.last_name = ""
         self.via_sso = False
         self.tags = []
 
         self.privileges = Privileges([])
         self.session_expiry = ""
@@ -137,18 +156,18 @@
                     os.path.expanduser("~"), env_file.replace("~/", "")
                 )
             env_file = os.path.abspath(env_file)
             console.debug(f"Loading settings from {env_file}")
             logger.debug(f"apisession:_load_env: loading settings from {env_file}")
             dotenv_path = Path(env_file)
             load_dotenv(dotenv_path=dotenv_path, override=True)
-        else:
-            console.debug("Loading settings from env file")
-            logger.debug(f"apisession:_load_env: loading settings from env file")
-            load_dotenv()
+        # else:
+        #     console.debug("Loading settings from env file")
+        #     logger.debug(f"apisession:_load_env: loading settings from env file")
+        #     load_dotenv()
 
         if os.getenv("MIST_HOST"):
             self.set_cloud(os.getenv("MIST_HOST"))
         if os.getenv("MIST_APITOKEN"):
             self.set_api_token(os.getenv("MIST_APITOKEN"))
         if os.getenv("MIST_USER"):
             self.set_email(os.getenv("MIST_USER"))
@@ -175,15 +194,17 @@
         if cloud_uri == "api.mistsys.com":
             self._cloud_uri = cloud_uri
         else:
             for cloud in clouds:
                 if cloud["host"] == cloud_uri:
                     self._cloud_uri = cloud_uri
         if self._cloud_uri:
-            logger.debug(f"apisession:set_cloud: Mist Cloud configured to {self._cloud_uri}")
+            logger.debug(
+                f"apisession:set_cloud: Mist Cloud configured to {self._cloud_uri}"
+            )
             console.debug(f"Mist Cloud configured to {self._cloud_uri}")
         else:
             logger.error(f"apisession:set_cloud: {cloud_uri} is not valid")
             console.error(f"{cloud_uri} is not valid")
 
     def get_cloud(self):
         """
@@ -193,39 +214,45 @@
         return self._cloud_uri
 
     def select_cloud(self) -> None:
         """
         Display a menu to select the Mist Cloud
         """
         logger.debug(f"apisession:select_cloud")
+        if self._show_cli_notif:
+            print()
+            print(" Mist Cloud Selection ".center(80, "-"))
+            print()
+
         resp = "x"
         i = 0
-        print()
-        print(" Mist Cloud Selection ".center(80, "-"))
-        print()
         for cloud in clouds:
             print(f"{i}) {cloud['short']} (host: {cloud['host']})")
             i += 1
 
         print()
-        resp = input(f"Select a Cloud (0 to {i}, or q to exit): ")
+        resp = input(f"Select a Cloud (0 to {i-1}, or q to exit): ")
         logger.info(f"apisession:select_cloud: input is {resp}")
         if resp == "q":
             sys.exit(0)
         elif resp == "i":
             self._cloud_uri = "api.mistsys.com"
         else:
             try:
                 resp_num = int(resp)
-                if resp_num >= 0 and resp_num <= i:
-                    logger.info(f"apisession:select_cloud: Mist Cloud is {clouds[resp_num]['host']}")
+                if resp_num >= 0 and resp_num < i:
+                    logger.info(
+                        f"apisession:select_cloud: Mist Cloud is {clouds[resp_num]['host']}"
+                    )
                     self.set_cloud(clouds[resp_num]["host"])
                 else:
                     print(f"Please enter a number between 0 and {i}.")
-                    logger.error(f"apisession:select_cloud: {resp} is not a valid input")
+                    logger.error(
+                        f"apisession:select_cloud: {resp} is not a valid input"
+                    )
                     self.select_cloud()
             except:
                 print("\r\nPlease enter a number.")
                 logger.error(f"apisession:select_cloud: {resp} is not a valid input")
                 self.select_cloud()
 
     ####################################
@@ -281,17 +308,18 @@
 
     def _process_login(self) -> None:
         """
         Function to authenticate a user with login/password.
         Will create and store a session used by other requests.
         """
         logger.debug(f"apisession:_process_login")
-        print()
-        print(" Login/Pwd authentication ".center(80, "-"))
-        print()
+        if self._show_cli_notif:
+            print()
+            print(" Login/Pwd authentication ".center(80, "-"))
+            print()
 
         self._session = requests.session()
         if not self.email:
             self.set_email()
         if not self._password:
             self.set_password()
 
@@ -355,80 +383,96 @@
             resp = self.mist_post(uri)
             if resp.status_code == 200:
                 logger.info(f"apisession:logout: Mist Session closed and cleaned up")
                 console.info("Logged out")
                 self._set_authenticated(False)
             else:
                 try:
-                    console.error(resp.json()["detail"])
+                    console.error(resp.data["detail"])
                 except:
-                    console.error(resp.text)
+                    console.error(resp.raw_data)
 
     def _set_authenticated(self, authentication_status: bool) -> None:
         """
         Set the authentication status.
         If True and Login/password is used, extract the HTTP session and
         CSRF Token from the cookies and store them in memory to be used
         during the future API requests.
         If False, clear the CSRF Token and delete the HTTP session.
 
         PARAMS
         -----------
         authentication_status : bool
         """
         logger.debug(f"apisession:_set_authenticated")
-        logger.debug(f"apisession:_set_authenticated: authentication_status is {authentication_status}")
+        logger.debug(
+            f"apisession:_set_authenticated: authentication_status is {authentication_status}"
+        )
         if authentication_status == True:
             self._authenticated = True
-            logger.info(f"apisession:_set_authenticated: session is now \"Authenticated\"")
+            logger.info(
+                f'apisession:_set_authenticated: session is now "Authenticated"'
+            )
             if not self._apitoken:
                 logger.info(f"apisession:_set_authenticated: processing HTTP cookies")
                 try:
                     cookies_ext = next(
                         item["cookies_ext"]
                         for item in clouds
                         if item["host"] == self._cloud_uri
                     )
-                    logger.info(f"apisession:_set_authenticated: HTTP session cookies extracted")
+                    logger.info(
+                        f"apisession:_set_authenticated: HTTP session cookies extracted"
+                    )
                 except:
                     cookies_ext = ""
-                    logger.error(f"apisession:_set_authenticated: unable to extract HTTP session cookies")
-                    logger.error("apirequest:mist_post_file: Exception occurred", exc_info=True)
+                    logger.error(
+                        f"apisession:_set_authenticated: unable to extract HTTP session cookies"
+                    )
+                    logger.error(
+                        "apirequest:mist_post_file: Exception occurred", exc_info=True
+                    )
                 self._csrftoken = self._session.cookies["csrftoken" + cookies_ext]
                 self._session.headers.update({"X-CSRFToken": self._csrftoken})
                 logger.info(f"apisession:_set_authenticated: CSRF Token stored")
         elif authentication_status == False:
             self._authenticated = False
-            logger.info(f"apisession:_set_authenticated: session is now \"Unauthenticated\"")
+            logger.info(
+                f'apisession:_set_authenticated: session is now "Unauthenticated"'
+            )
             self._csrftoken = ""
             del self._session
             logger.info(
                 f"apisession:_set_authenticated: CSRFT Token is cleaned up and HTTP Session deleted"
             )
 
     def get_authentication_status(self) -> bool:
         """
         RETURN
         -----------
         bool
             Return the authentication status.
         """
-        logger.debug(f"apisession:get_authentication_status: return {self._authenticated}")
+        logger.debug(
+            f"apisession:get_authentication_status: return {self._authenticated}"
+        )
         return self._authenticated
 
     def get_api_token(self) -> APIResponse:
         """
         Retrieve and display the User/Org API Tokens
 
         RETURN
         -----------
         mistapi.APIResponse
             api response for the GET /api/v1/self request
         """
-        logger.info(f'apisession:get_api_token: Sending GET request to "/api/v1/self/apitokens"')
+        logger.info(
+            f'apisession:get_api_token: Sending GET request to "/api/v1/self/apitokens"'
+        )
         resp = self.mist_get("/api/v1/self/apitokens")
         return resp
 
     def create_api_token(self, token_name: str = None) -> APIResponse:
         """
         Create a new API Token with the current account (user/org)
 
@@ -493,15 +537,17 @@
         body = {
             "email": self.email,
             "password": self._password,
             "two_factor": two_factor,
         }
         resp = self._session.post(self._url(uri), json=body)
         if resp.status_code == 200:
-            logger.info(f"apisession:: _two_factor_authentication2FA authentication successed")
+            logger.info(
+                f"apisession:: _two_factor_authentication2FA authentication successed"
+            )
             console.info("2FA authentication successed")
             self._set_authenticated(True)
             return True
         else:
             logger.error(
                 f"apisession:_two_factor_authentication: 2FA authentication failed with error code: {resp.status_code}"
             )
@@ -539,27 +585,27 @@
                     if key == "privileges":
                         self.privileges = Privileges(resp.data["privileges"])
                     if key == "tags":
                         for tag in resp.data["tags"]:
                             self.tags.append(tag)
                     else:
                         setattr(self, key, val)
-                print()
-                print(" Authenticated ".center(80, "-"))
-                print(f"\r\nWelcome {self.first_name} {self.last_name}!\r\n")
+                if self._show_cli_notif:
+                    print()
+                    print(" Authenticated ".center(80, "-"))
+                    print(f"\r\nWelcome {self.first_name} {self.last_name}!\r\n")
                 logger.info(
                     f"apisession:_getself: account used: {self.first_name} {self.last_name}"
                 )
                 return True
         else:
             logger.error(f"apisession:_getself: authentication not valid...")
             console.error("Authentication not valid...\r\n")
             resp = input(
                 f"Do you want to try with new credentials for {self._cloud_uri} (y/N)? "
-                % ()
             )
             if resp.lower() == "y":
                 self._process_login()
                 return self._getself()
             else:
                 sys.exit(0)
 
@@ -568,15 +614,17 @@
 
     def get_privilege_by_org_id(self, org_id: str):
         logger.debug(f"apisession:get_privilege_by_org_id")
         org_priv = next(
             (priv for priv in self.privileges if priv.get("org_id") == org_id), None
         )
         if org_priv:
-            logger.info(f"apisession:get_privilege_by_org_id: org {org_id} privileges found in user info")
+            logger.info(
+                f"apisession:get_privilege_by_org_id: org {org_id} privileges found in user info"
+            )
             logger.debug(f"apisession:get_privilege_by_org_id: {org_priv}")
             return org_priv
         else:
             logger.warn(
                 f"apisession:get_privilege_by_org_id: unable of find org {org_id} privileges in user data"
             )
             logger.info(
@@ -592,34 +640,38 @@
                     )
                     msp_id = resp.data.get("msp_id")
                 else:
                     logger.warn(
                         "apisession:get_privilege_by_org_id: not able to find msp_id information in the org info"
                     )
             except:
-                logger.error("apisession:get_privilege_by_org_id: error when retrieving org info")
-                logger.error("apirequest:mist_post_file: Exception occurred", exc_info=True)
+                logger.error(
+                    "apisession:get_privilege_by_org_id: error when retrieving org info"
+                )
+                logger.error(
+                    "apirequest:mist_post_file: Exception occurred", exc_info=True
+                )
             if msp_id:
                 msp_priv = next(
                     (
                         priv
                         for priv in self.privileges
                         if priv.get("scope") == "msp" and priv.get("msp_id") == msp_id
                     ),
                     None,
                 )
                 if not msp_priv:
-                    logger.warn(
+                    logger.warning(
                         f"apisession:get_privilege_by_org_id: unable of find msp {msp_id} privileges in user data"
                     )
                     return None
                 else:
                     return {
                         "scope": "org",
                         "org_id": org_id,
                         "name": resp.data.get("name"),
                         "role": msp_priv["role"],
                         "msp_id": msp_id,
                         "msp_name": msp_priv["name"],
                         "orggroup_ids": resp.data.get("orggroup_ids"),
-                        "msp_logo_url": resp.data.get("logo_url")
+                        "msp_logo_url": resp.data.get("logo_url"),
                     }
```

### Comparing `mistapi-0.41.9/src/mistapi/__init__.py` & `mistapi-0.42.0/src/mistapi/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 '''
 
 from mistapi.__api_session import APISession
 from mistapi import api
 from mistapi import cli
 from mistapi.__pagination import get_next, get_all
 
-__version__ = "0.41.9"
+__version__ = "0.42.0"
 __author__ = "Thomas Munzer <tmunzer@juniper.net>"
```

### Comparing `mistapi-0.41.9/src/mistapi/__logger.py` & `mistapi-0.42.0/src/mistapi/__logger.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/__models/privilege.py` & `mistapi-0.42.0/src/mistapi/__models/privilege.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/__pagination.py` & `mistapi-0.42.0/src/mistapi/__pagination.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/__init__.py` & `mistapi-0.42.0/src/mistapi/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/const/__init__.py` & `mistapi-0.42.0/src/mistapi/api/v1/const/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi.api.v1.const import alarm_defs
 from mistapi.api.v1.const import ap_channels
 from mistapi.api.v1.const import ap_led_status
 from mistapi.api.v1.const import applications
-from mistapi.api.v1.const import call_events
 from mistapi.api.v1.const import client_events
 from mistapi.api.v1.const import countries
 from mistapi.api.v1.const import default_gateway_config
 from mistapi.api.v1.const import device_events
 from mistapi.api.v1.const import device_models
 from mistapi.api.v1.const import insight_metrics
 from mistapi.api.v1.const import languages
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/const/alarm_defs.py` & `mistapi-0.42.0/src/mistapi/api/v1/const/alarm_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listAlarmDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listAlarmDefinitions")  
 def getAlarmDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listAlarmDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/const/ap_channels.py` & `mistapi-0.42.0/src/mistapi/api/v1/const/ap_channels.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listApChannels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listApChannels")  
 def getApChannels(mist_session:_APISession, country_code:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApChannels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/const/ap_led_status.py` & `mistapi-0.42.0/src/mistapi/api/v1/const/ap_led_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listApLedDefinition")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listApLedDefinition")  
 def getApLedDefinition(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApLedDefinition
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/const/applications.py` & `mistapi-0.42.0/src/mistapi/api/v1/const/applications.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listApplications")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listApplications")  
 def getApplications(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApplications
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/const/call_events.py` & `mistapi-0.42.0/src/mistapi/api/v1/const/device_events.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,46 +10,46 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listCallEventsDefinitions")  
-def getCallEventsDefinitions(mist_session:_APISession) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listDeviceEventsDefinitions")  
+def getDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listCallEventsDefinitions
+    API doc: https://doc.mist-lab.fr/#operation/listDeviceEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/const/call_events"
+    uri = f"/api/v1/const/device_events"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listCallEventsDefinitions(mist_session:_APISession) -> _APIResponse:
+def listDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listCallEventsDefinitions
+    API doc: https://doc.mist-lab.fr/#operation/listDeviceEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/const/call_events"
+    uri = f"/api/v1/const/device_events"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/const/client_events.py` & `mistapi-0.42.0/src/mistapi/api/v1/const/client_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listClientEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listClientEventsDefinitions")  
 def getClientEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listClientEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/const/countries.py` & `mistapi-0.42.0/src/mistapi/api/v1/const/countries.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listCountryCodes")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listCountryCodes")  
 def getCountryCodes(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listCountryCodes
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/const/default_gateway_config.py` & `mistapi-0.42.0/src/mistapi/api/v1/const/default_gateway_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getGatawayDefaultConfig(mist_session:_APISession, model:str=None, ha:str=None) -> _APIResponse:
+def getGatawayDefaultConfig(mist_session:_APISession, model:str, ha:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/getGatawayDefaultConfig
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/const/device_events.py` & `mistapi-0.42.0/src/mistapi/api/v1/const/other_device_events.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,46 +10,46 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listDeviceEventsDefinitions")  
-def getDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOtherDeviceEventsDefinitions")  
+def getOtherDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listDeviceEventsDefinitions
+    API doc: https://doc.mist-lab.fr/#operation/listOtherDeviceEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/const/device_events"
+    uri = f"/api/v1/const/other_device_events"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
+def listOtherDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listDeviceEventsDefinitions
+    API doc: https://doc.mist-lab.fr/#operation/listOtherDeviceEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/const/device_events"
+    uri = f"/api/v1/const/other_device_events"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/const/device_models.py` & `mistapi-0.42.0/src/mistapi/api/v1/const/device_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listDeviceModels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listDeviceModels")  
 def getDeviceModels(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listDeviceModels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/const/insight_metrics.py` & `mistapi-0.42.0/src/mistapi/api/v1/const/insight_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listInsightMetrics")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listInsightMetrics")  
 def getInsightMetrics(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInsightMetrics
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/const/languages.py` & `mistapi-0.42.0/src/mistapi/api/v1/const/languages.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteLanguages")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteLanguages")  
 def getSiteLanguages(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteLanguages
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/const/license_types.py` & `mistapi-0.42.0/src/mistapi/api/v1/const/license_types.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/const/mxedge_events.py` & `mistapi-0.42.0/src/mistapi/api/v1/const/mxedge_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listMxEdgeEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listMxEdgeEventsDefinitions")  
 def getMxEdgeEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMxEdgeEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/const/mxedge_models.py` & `mistapi-0.42.0/src/mistapi/api/v1/const/mxedge_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listMxEdgeModels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listMxEdgeModels")  
 def getMxEdgeModels(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMxEdgeModels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/const/other_device_events.py` & `mistapi-0.42.0/src/mistapi/api/v1/self/two_factor.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,46 +10,54 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOtherDeviceEventsDefinitions")  
-def getOtherDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
+def generateQrCodeForVerification(mist_session:_APISession, by:str="qrcode") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOtherDeviceEventsDefinitions
+    API doc: https://doc.mist-lab.fr/#operation/generateQrCodeForVerification
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
+    QUERY PARAMS
+    ------------
+    by : str{'qrcode'}, default: qrcode        
+    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/const/other_device_events"
-    query_params={}
+    uri = f"/api/v1/self/two_factor/token"
+    query_params={}
+    if by: query_params["by"]=by
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listOtherDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
+def verifyTwoFactor(mist_session:_APISession, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOtherDeviceEventsDefinitions
+    API doc: https://doc.mist-lab.fr/#operation/verifyTwoFactor
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/const/other_device_events"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/self/two_factor/verify"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/const/traffic_types.py` & `mistapi-0.42.0/src/mistapi/api/v1/const/traffic_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listTrafficTypes")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listTrafficTypes")  
 def getTrafficTypes(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listTrafficTypes
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/installer/orgs/__init__.py` & `mistapi-0.42.0/src/mistapi/api/v1/installer/orgs/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/installer/orgs/alarmtemplates.py` & `mistapi-0.42.0/src/mistapi/api/v1/installer/orgs/alarmtemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listInstallerAlarmTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listInstallerAlarmTemplates")  
 def getInstallerAlarmTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerAlarmTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/installer/orgs/deviceprofiles.py` & `mistapi-0.42.0/src/mistapi/api/v1/installer/orgs/deviceprofiles.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listInstallerDeviceProfiles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listInstallerDeviceProfiles")  
 def getInstallerDeviceProfiles(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerDeviceProfiles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/installer/orgs/devices.py` & `mistapi-0.42.0/src/mistapi/api/v1/installer/orgs/devices.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listInstallerListOfRenctlyClaimedDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listInstallerListOfRenctlyClaimedDevices")  
 def getInstallerListOfRenctlyClaimedDevices(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerListOfRenctlyClaimedDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -136,40 +136,35 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/installer/orgs/{org_id}/devices/{device_mac}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def startInstallerLocateDevice(mist_session:_APISession, org_id:str, device_mac:str, body:object) -> _APIResponse:
+def startInstallerLocateDevice(mist_session:_APISession, org_id:str, device_mac:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/startInstallerLocateDevice
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
     device_mac : str        
     
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
-    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/installer/orgs/{org_id}/devices/{device_mac}/locate"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    resp = mist_session.mist_post(uri=uri)
     return resp
     
 def stopInstallerLocateDevice(mist_session:_APISession, org_id:str, device_mac:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/stopInstallerLocateDevice
     
     PARAMS
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/installer/orgs/rftemplates.py` & `mistapi-0.42.0/src/mistapi/api/v1/installer/orgs/rftemplates.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listInstallerRfTemplatesNames")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listInstallerRfTemplatesNames")  
 def getInstallerRfTemplatesNames(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerRfTemplatesNames
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/installer/orgs/secpolicies.py` & `mistapi-0.42.0/src/mistapi/api/v1/installer/orgs/secpolicies.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listInstallerSecPolicies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listInstallerSecPolicies")  
 def getInstallerSecPolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerSecPolicies
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/installer/orgs/sitegroups.py` & `mistapi-0.42.0/src/mistapi/api/v1/installer/orgs/sitegroups.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listInstallerSiteGroups")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listInstallerSiteGroups")  
 def getInstallerSiteGroups(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerSiteGroups
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/installer/orgs/sites.py` & `mistapi-0.42.0/src/mistapi/api/v1/installer/orgs/sites.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listInstallerSites")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listInstallerSites")  
 def getInstallerSites(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerSites
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -85,15 +85,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/installer/orgs/{org_id}/sites/{site_name}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listInstallerMaps")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listInstallerMaps")  
 def getInstallerMaps(mist_session:_APISession, org_id:str, site_name:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerMaps
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -134,49 +134,34 @@
         response from the API call
     """
     uri = f"/api/v1/installer/orgs/{org_id}/sites/{site_name}/maps"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def importInstallerMapFile(mist_session:_APISession, org_id:str, site_name:str, csv:str=None, file:str=None, json:dict=None) -> _APIResponse:
+def importInstallerMapFile(mist_session:_APISession, org_id:str, site_name:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/importInstallerMap
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
     site_name : str        
     
-    BODY PARAMS
-    -----------
-    csv : str
-        path to the file to upload. 
-    file : str
-        path to the file to upload. 
-    json : dict
-        import_all_floorplans : bool
-        import_height : bool
-        import_orientation : bool
-        vendor_name : {'ibwave', 'ekahau'}
-    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     multipart_form_data = {
-        "csv":csv,
-        "file":file,
-        "json":json,
     }
     uri = f"/api/v1/installer/orgs/{org_id}/sites/{site_name}/maps/import"
     resp = mist_session.mist_post_file(uri=uri, multipart_form_data=multipart_form_data)
     return resp
 
 def deleteInstallerMap(mist_session:_APISession, org_id:str, site_name:str, map_id:str) -> _APIResponse:
     """
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/installer/sites/optimize.py` & `mistapi-0.42.0/src/mistapi/api/v1/installer/sites/optimize.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/invite/verify.py` & `mistapi-0.42.0/src/mistapi/api/v1/invite/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/login/__init__.py` & `mistapi-0.42.0/src/mistapi/api/v1/login/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/login/login.py` & `mistapi-0.42.0/src/mistapi/api/v1/login/login.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/login/lookup.py` & `mistapi-0.42.0/src/mistapi/api/v1/login/lookup.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/login/oauth.py` & `mistapi-0.42.0/src/mistapi/api/v1/login/oauth.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/login/two_factor.py` & `mistapi-0.42.0/src/mistapi/api/v1/login/two_factor.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/logout/logout.py` & `mistapi-0.42.0/src/mistapi/api/v1/logout/logout.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/mobile/verify.py` & `mistapi-0.42.0/src/mistapi/api/v1/mobile/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/msps/__init__.py` & `mistapi-0.42.0/src/mistapi/api/v1/msps/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/msps/admins.py` & `mistapi-0.42.0/src/mistapi/api/v1/msps/admins.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listMspAdmins")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listMspAdmins")  
 def getMspAdmins(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspAdmins
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/msps/claim.py` & `mistapi-0.42.0/src/mistapi/api/v1/msps/claim.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/msps/insights.py` & `mistapi-0.42.0/src/mistapi/api/v1/msps/insights.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/msps/inventory.py` & `mistapi-0.42.0/src/mistapi/api/v1/msps/inventory.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/msps/invites.py` & `mistapi-0.42.0/src/mistapi/api/v1/msps/invites.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/msps/licenses.py` & `mistapi-0.42.0/src/mistapi/api/v1/msps/licenses.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listMspLicenses")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listMspLicenses")  
 def getMspLicenses(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspLicenses
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/msps/logo.py` & `mistapi-0.42.0/src/mistapi/api/v1/msps/logo.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/msps/logs.py` & `mistapi-0.42.0/src/mistapi/api/v1/msps/logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listMspLogs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listMspLogs")  
 def getMspLogs(mist_session:_APISession, msp_id:str, site_id:str=None, admin_name:str=None, message:str=None, sort:str=None, start:int=None, end:int=None, limit:int=100, page:int=1, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspLogs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/msps/msps.py` & `mistapi-0.42.0/src/mistapi/api/v1/msps/msps.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/msps/orggroups.py` & `mistapi-0.42.0/src/mistapi/api/v1/msps/orggroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listMspOrgGroups")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listMspOrgGroups")  
 def getMspOrgGroups(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgGroups
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/msps/orgs.py` & `mistapi-0.42.0/src/mistapi/api/v1/msps/orgs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listMspOrgs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listMspOrgs")  
 def getMspOrgs(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/msps/search.py` & `mistapi-0.42.0/src/mistapi/api/v1/msps/search.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/msps/ssoroles.py` & `mistapi-0.42.0/src/mistapi/api/v1/msps/ssoroles.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listMspSsoRoles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listMspSsoRoles")  
 def getMspSsoRoles(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspSsoRoles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/msps/ssos.py` & `mistapi-0.42.0/src/mistapi/api/v1/msps/ssos.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,41 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getMspSso(mist_session:_APISession, msp_id:str) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listMspSsos")  
+def getMspSsos(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getMspSso
+    API doc: https://doc.mist-lab.fr/#operation/listMspSsos
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    msp_id : str        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/msps/{msp_id}/ssos"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def listMspSsos(mist_session:_APISession, msp_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/listMspSsos
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -60,14 +84,38 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/ssos"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
+def getMspSso(mist_session:_APISession, msp_id:str, sso_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/getMspSso
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    msp_id : str
+    sso_id : str        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/msps/{msp_id}/ssos/{sso_id}"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
 def deleteMspSso(mist_session:_APISession, msp_id:str, sso_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/deleteMspSso
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -112,15 +160,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/ssos/{sso_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listMspSsoLatestFailures")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listMspSsoLatestFailures")  
 def getMspSsoLatestFailures(mist_session:_APISession, msp_id:str, sso_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspSsoLatestFailures
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/msps/stats.py` & `mistapi-0.42.0/src/mistapi/api/v1/msps/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listMspOrgLicenses")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listMspOrgLicenses")  
 def getMspOrgLicenses(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgLicenses
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -57,15 +57,15 @@
         response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/stats/licenses"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listMspOrgStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listMspOrgStats")  
 def getMspOrgStats(mist_session:_APISession, msp_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/msps/suggestion.py` & `mistapi-0.42.0/src/mistapi/api/v1/msps/suggestion.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/msps/tickets.py` & `mistapi-0.42.0/src/mistapi/api/v1/msps/tickets.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listMspTickets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listMspTickets")  
 def getMspTickets(mist_session:_APISession, msp_id:str, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspTickets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/__init__.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from mistapi.api.v1.orgs import clone
 from mistapi.api.v1.orgs import crl
 from mistapi.api.v1.orgs import deviceprofiles
 from mistapi.api.v1.orgs import devices
 from mistapi.api.v1.orgs import evpn_topologies
 from mistapi.api.v1.orgs import gatewaytemplates
 from mistapi.api.v1.orgs import guests
+from mistapi.api.v1.orgs import idpprofiles
 from mistapi.api.v1.orgs import insights
 from mistapi.api.v1.orgs import inventory
 from mistapi.api.v1.orgs import invites
 from mistapi.api.v1.orgs import jsi
 from mistapi.api.v1.orgs import licenses
 from mistapi.api.v1.orgs import logs
 from mistapi.api.v1.orgs import maps
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/admins.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/admins.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgAdmins")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgAdmins")  
 def getOrgAdmins(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAdmins
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/alarms.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/alarms.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/alarmtemplates.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/alarmtemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgAlarmTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgAlarmTemplates")  
 def getOrgAlarmTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAlarmTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -84,15 +84,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/alarmtemplates"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgSuppressedAlarms")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgSuppressedAlarms")  
 def getOrgSuppressedAlarms(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSuppressedAlarms
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/apitokens.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/apitokens.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgApiTokens")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgApiTokens")  
 def getOrgApiTokens(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgApiTokens
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/aptemplates.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/aptemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgAptemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgAptemplates")  
 def getOrgAptemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAptemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/assetfilters.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/assetfilters.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgAssetFilters")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgAssetFilters")  
 def getOrgAssetFilters(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAssetFilters
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/assets.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgAssets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgAssets")  
 def getOrgAssets(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAssets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/call.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/call.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/cert.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/cert.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/claim.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/claim.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/clients.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/clone.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/clone.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/crl.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/crl.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/deviceprofiles.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/deviceprofiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgDeviceProfiles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgDeviceProfiles")  
 def getOrgDeviceProfiles(mist_session:_APISession, org_id:str, type:str="ap", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDeviceProfiles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/devices.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/devices.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgDevices")  
 def getOrgDevices(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -189,15 +189,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchOrgDevicesEvents(mist_session:_APISession, org_id:str, mac:str=None, model:str=None, text:str=None, timestamp:str=None, type:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def searchOrgDevicesEvents(mist_session:_APISession, org_id:str, mac:str=None, model:str=None, device_type:str="ap", text:str=None, timestamp:str=None, type:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/searchOrgDevicesEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -208,14 +208,16 @@
     
     QUERY PARAMS
     ------------
     mac : str
       device mac
     model : str
       device model
+    device_type : str{'ap', 'switch', 'gateway'}, default: ap
+      device type
     text : str
       event message
     timestamp : str
       event time
     type : str
       see [listDeviceEventsDefinitions](/#operation/listDeviceEventsDefinitions)
     limit : int, default: 100
@@ -228,14 +230,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/devices/events/search"
     query_params={}
     if mac: query_params["mac"]=mac
     if model: query_params["model"]=model
+    if device_type: query_params["device_type"]=device_type
     if text: query_params["text"]=text
     if timestamp: query_params["timestamp"]=timestamp
     if type: query_params["type"]=type
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
@@ -316,15 +319,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if limit: query_params["limit"]=limit
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgApsMacs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgApsMacs")  
 def getOrgApsMacs(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgApsMacs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -456,15 +459,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgMultiSitesDevicesUpgrades")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgMultiSitesDevicesUpgrades")  
 def getOrgMultiSitesDevicesUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMultiSitesDevicesUpgrades
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -553,64 +556,8 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/devices/upgrade/{upgrade_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
-    
-def clearOrgTunnel(mist_session:_APISession, org_id:str, device_id:str, body:object) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/clearOrgTunnel
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    org_id : str
-    device_id : str        
-    
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/orgs/{org_id}/devices/{device_id}/clear_tunnels"
-    resp = mist_session.mist_post(uri=uri, body=body)
-    return resp
-    
-def provisionOrgTunnel(mist_session:_APISession, org_id:str, device_id:str, body:object) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/provisionOrgTunnel
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    org_id : str
-    device_id : str        
-    
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/orgs/{org_id}/devices/{device_id}/provision_tunnels"
-    resp = mist_session.mist_post(uri=uri, body=body)
-    return resp
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/evpn_topologies.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/evpn_topologies.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgEvpnTopologies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgEvpnTopologies")  
 def getOrgEvpnTopologies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgEvpnTopologies
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/gatewaytemplates.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/gatewaytemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgGatewayTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgGatewayTemplates")  
 def getOrgGatewayTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgGatewayTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/guests.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/guests.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgGuestAuthorizations")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgGuestAuthorizations")  
 def getOrgGuestAuthorizations(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgGuestAuthorizations
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/insights.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/insights.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/inventory.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/inventory.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/invites.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/invites.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/jsi.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/jsi.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgJsiDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgJsiDevices")  
 def getOrgJsiDevices(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None, mac:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgJsiDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -157,15 +157,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/jsi/devices/{device_mac}/upgrade"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgJsiPastPurchases")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgJsiPastPurchases")  
 def getOrgJsiPastPurchases(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgJsiPastPurchases
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/licenses.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/licenses.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/logs.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgLogs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgLogs")  
 def getOrgLogs(mist_session:_APISession, org_id:str, site_id:str=None, admin_name:str=None, message:str=None, sort:str=None, start:int=None, end:int=None, limit:int=100, page:int=1, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgLogs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/maps.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/apps.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,49 +10,54 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def importOrgMapsFile(mist_session:_APISession, org_id:str, auto_deviceprofile_assignment:bool=None, csv:str=None, file:str=None, json:dict=None) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteApps")  
+def getSiteApps(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/importOrgMaps
+    API doc: https://doc.mist-lab.fr/#operation/listSiteApps
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
+    site_id : str        
     
-    BODY PARAMS
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/apps"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def listSiteApps(mist_session:_APISession, site_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/listSiteApps
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
     -----------
-    auto_deviceprofile_assignment : bool
-        whether to auto assign device to deviceprofile by name
-    csv : str
-        path to the file to upload. csv file for ap name mapping, optional
-    file : str
-        path to the file to upload. 
-    json : dict
-        import_all_floorplans : bool
-        import_height : bool, default: True
-        import_orientation : bool, default: True
-        site_id : str
-        vendor_name : {'ekahau', 'ibwave'}
+    site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    multipart_form_data = {
-        "auto_deviceprofile_assignment":auto_deviceprofile_assignment,
-        "csv":csv,
-        "file":file,
-        "json":json,
-    }
-    uri = f"/api/v1/orgs/{org_id}/maps/import"
-    resp = mist_session.mist_post_file(uri=uri, multipart_form_data=multipart_form_data)
+    uri = f"/api/v1/sites/{site_id}/apps"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
+
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/mxclusters.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/mxclusters.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgMxEdgeClusters")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgMxEdgeClusters")  
 def getOrgMxEdgeClusters(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgeClusters
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/mxedges.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/mxedges.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgMxEdges")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgMxEdges")  
 def getOrgMxEdges(mist_session:_APISession, org_id:str, for_sites:str="any", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdges
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -185,15 +185,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxedges/unassign"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgMxEdgeUpgrades")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgMxEdgeUpgrades")  
 def getOrgMxEdgeUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgeUpgrades
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -388,14 +388,68 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxedges/{mxedge_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
+def deleteOrgMxEdgeImage(mist_session:_APISession, org_id:str, mxedge_id:str, image_number:float) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrgMxEdgeImage
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    org_id : str
+    mxedge_id : str
+    image_number : float        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/orgs/{org_id}/mxedges/{mxedge_id}//image{image_number}"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    return resp
+    
+def addOrgMxEdgeImage(mist_session:_APISession, org_id:str, mxedge_id:str, image_number:float, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/addOrgMxEdgeImage
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    org_id : str
+    mxedge_id : str
+    image_number : float        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/orgs/{org_id}/mxedges/{mxedge_id}//image{image_number}"
+    resp = mist_session.mist_post(uri=uri, body=body)
+    return resp
+    
 def restartOrgMxEdge(mist_session:_APISession, org_id:str, mxedge_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/restartOrgMxEdge
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/mxtunnels.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/mxtunnels.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgMxTunnels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgMxTunnels")  
 def getOrgMxTunnels(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxTunnels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/nacrules.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/nacrules.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgNacRules")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgNacRules")  
 def getOrgNacRules(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNacRules
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/nactags.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/nactags.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgNacTags")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgNacTags")  
 def getOrgNacTags(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNacTags
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -108,17 +108,17 @@
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/nactags/{nactag_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def DeleteOrgNacTag(mist_session:_APISession, org_id:str, nactag_id:str) -> _APIResponse:
+def deleteOrgNacTag(mist_session:_APISession, org_id:str, nactag_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/DeleteOrgNacTag
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrgNacTag
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/networks.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgNetworks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgNetworks")  
 def getOrgNetworks(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNetworks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/networktemplates.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/networktemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgNetworkTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgNetworkTemplates")  
 def getOrgNetworkTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNetworkTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/ocdevices.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/ocdevices.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/orgs.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/orgs.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getOrgInfo(mist_session:_APISession, org_id:str) -> _APIResponse:
+def getOrg(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgInfo
+    API doc: https://doc.mist-lab.fr/#operation/getOrg
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/otherdevices.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/otherdevices.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgOtherDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgOtherDevices")  
 def getOrgOtherDevices(mist_session:_APISession, org_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgOtherDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/pma.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/pma.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgPmaDashboards")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgPmaDashboards")  
 def getOrgPmaDashboards(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPmaDashboards
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/pskportals.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/rftemplates.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgPskPortals")  
-def getOrgPskPortals(mist_session:_APISession, org_id:str) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgRfTemplates")  
+def getOrgRfTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgPskPortals
+    API doc: https://doc.mist-lab.fr/#operation/listOrgRfTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -29,22 +29,22 @@
     org_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/pskportals"
+    uri = f"/api/v1/orgs/{org_id}/rftemplates"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listOrgPskPortals(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgRfTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgPskPortals
+    API doc: https://doc.mist-lab.fr/#operation/listOrgRfTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -52,22 +52,22 @@
     org_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/pskportals"
+    uri = f"/api/v1/orgs/{org_id}/rftemplates"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createOrgPskPortal(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def createOrgRfTemplate(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createOrgPskPortal
+    API doc: https://doc.mist-lab.fr/#operation/createOrgRfTemplate
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -80,87 +80,87 @@
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/pskportals"
+    uri = f"/api/v1/orgs/{org_id}/rftemplates"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getOrgPskPortal(mist_session:_APISession, org_id:str, pskportal_id:str) -> _APIResponse:
+def getOrgRfTemplate(mist_session:_APISession, org_id:str, rftemplate_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgPskPortal
+    API doc: https://doc.mist-lab.fr/#operation/getOrgRfTemplate
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    pskportal_id : str        
+    rftemplate_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/pskportals/{pskportal_id}"
+    uri = f"/api/v1/orgs/{org_id}/rftemplates/{rftemplate_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteOrgPskPortal(mist_session:_APISession, org_id:str, pskportal_id:str) -> _APIResponse:
+def deleteOrgRfTemplate(mist_session:_APISession, org_id:str, rftemplate_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteOrgPskPortal
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrgRfTemplate
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    pskportal_id : str        
+    rftemplate_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/pskportals/{pskportal_id}"
+    uri = f"/api/v1/orgs/{org_id}/rftemplates/{rftemplate_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateOrgPskPortal(mist_session:_APISession, org_id:str, pskportal_id:str, body:object) -> _APIResponse:
+def updateOrgRfTemplate(mist_session:_APISession, org_id:str, rftemplate_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateOrgPskPortal
+    API doc: https://doc.mist-lab.fr/#operation/updateOrgRfTemplate
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    pskportal_id : str        
+    rftemplate_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/pskportals/{pskportal_id}"
+    uri = f"/api/v1/orgs/{org_id}/rftemplates/{rftemplate_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/psks.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/psks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgPsks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgPsks")  
 def getOrgPsks(mist_session:_APISession, org_id:str, name:str=None, ssid:str=None, role:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPsks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/rftemplates.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/sdktemplates.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgRfTemplates")  
-def getOrgRfTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSdkTemplates")  
+def getSdkTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgRfTemplates
+    API doc: https://doc.mist-lab.fr/#operation/listSdkTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -29,22 +29,22 @@
     org_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/rftemplates"
+    uri = f"/api/v1/orgs/{org_id}/sdktemplates"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listOrgRfTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listSdkTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgRfTemplates
+    API doc: https://doc.mist-lab.fr/#operation/listSdkTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -52,22 +52,22 @@
     org_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/rftemplates"
+    uri = f"/api/v1/orgs/{org_id}/sdktemplates"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createOrgRfTemplate(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def createSdkTemplate(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createOrgRfTemplate
+    API doc: https://doc.mist-lab.fr/#operation/createSdkTemplate
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -80,87 +80,87 @@
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/rftemplates"
+    uri = f"/api/v1/orgs/{org_id}/sdktemplates"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getOrgRfTemplate(mist_session:_APISession, org_id:str, rftemplate_id:str) -> _APIResponse:
+def getSdkTemplate(mist_session:_APISession, org_id:str, sdktemplate_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgRfTemplate
+    API doc: https://doc.mist-lab.fr/#operation/getSdkTemplate
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    rftemplate_id : str        
+    sdktemplate_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/rftemplates/{rftemplate_id}"
+    uri = f"/api/v1/orgs/{org_id}/sdktemplates/{sdktemplate_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteOrgRfTemplate(mist_session:_APISession, org_id:str, rftemplate_id:str) -> _APIResponse:
+def deleteSdkTemplate(mist_session:_APISession, org_id:str, sdktemplate_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteOrgRfTemplate
+    API doc: https://doc.mist-lab.fr/#operation/deleteSdkTemplate
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    rftemplate_id : str        
+    sdktemplate_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/rftemplates/{rftemplate_id}"
+    uri = f"/api/v1/orgs/{org_id}/sdktemplates/{sdktemplate_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateOrgRfTemplate(mist_session:_APISession, org_id:str, rftemplate_id:str, body:object) -> _APIResponse:
+def updateSdkTemplate(mist_session:_APISession, org_id:str, sdktemplate_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateOrgRfTemplate
+    API doc: https://doc.mist-lab.fr/#operation/updateSdkTemplate
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    rftemplate_id : str        
+    sdktemplate_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/rftemplates/{rftemplate_id}"
+    uri = f"/api/v1/orgs/{org_id}/sdktemplates/{sdktemplate_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/sdkclients.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/sdkclients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/sdkinvites.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/sdkinvites.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSdkInvites")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSdkInvites")  
 def getSdkInvites(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSdkInvites
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/sdktemplates.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/vpns.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSdkTemplates")  
-def getSdkTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgsVpns")  
+def getOrgsVpns(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSdkTemplates
+    API doc: https://doc.mist-lab.fr/#operation/listOrgsVpns
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -29,22 +29,22 @@
     org_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/sdktemplates"
+    uri = f"/api/v1/orgs/{org_id}/vpns"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSdkTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgsVpns(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSdkTemplates
+    API doc: https://doc.mist-lab.fr/#operation/listOrgsVpns
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -52,22 +52,22 @@
     org_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/sdktemplates"
+    uri = f"/api/v1/orgs/{org_id}/vpns"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createSdkTemplate(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def createOrgVpns(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createSdkTemplate
+    API doc: https://doc.mist-lab.fr/#operation/createOrgVpns
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -80,87 +80,87 @@
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/sdktemplates"
+    uri = f"/api/v1/orgs/{org_id}/vpns"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getSdkTemplate(mist_session:_APISession, org_id:str, sdktemplate_id:str) -> _APIResponse:
+def getOrgVpn(mist_session:_APISession, org_id:str, vpn_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSdkTemplate
+    API doc: https://doc.mist-lab.fr/#operation/getOrgVpn
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    sdktemplate_id : str        
+    vpn_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/sdktemplates/{sdktemplate_id}"
+    uri = f"/api/v1/orgs/{org_id}/vpns/{vpn_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteSdkTemplate(mist_session:_APISession, org_id:str, sdktemplate_id:str) -> _APIResponse:
+def deleteOrgVpn(mist_session:_APISession, org_id:str, vpn_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSdkTemplate
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrgVpn
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    sdktemplate_id : str        
+    vpn_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/sdktemplates/{sdktemplate_id}"
+    uri = f"/api/v1/orgs/{org_id}/vpns/{vpn_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateSdkTemplate(mist_session:_APISession, org_id:str, sdktemplate_id:str, body:object) -> _APIResponse:
+def updateOrgVpn(mist_session:_APISession, org_id:str, vpn_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSdkTemplate
+    API doc: https://doc.mist-lab.fr/#operation/updateOrgVpn
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    sdktemplate_id : str        
+    vpn_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/sdktemplates/{sdktemplate_id}"
+    uri = f"/api/v1/orgs/{org_id}/vpns/{vpn_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/secpolicies.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/secpolicies.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgSecPolicies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgSecPolicies")  
 def getOrgSecPolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSecPolicies
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/servicepolicies.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/servicepolicies.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgServicePolicies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgServicePolicies")  
 def getOrgServicePolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgServicePolicies
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/services.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgServices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgServices")  
 def getOrgServices(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgServices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/setting.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/setting.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/sitegroups.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/sitegroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgSiteGroups")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgSiteGroups")  
 def getOrgSiteGroups(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSiteGroups
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/sites.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/sites.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgSites")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgSites")  
 def getOrgSites(mist_session:_APISession, org_id:str, limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSites
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -218,40 +218,31 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def importOrgMapToSiteFile(mist_session:_APISession, org_id:str, site_name:str, csv:str=None, file:str=None) -> _APIResponse:
+def importOrgMapToSiteFile(mist_session:_APISession, org_id:str, site_name:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/importOrgMapToSite
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
     site_name : str        
     
-    BODY PARAMS
-    -----------
-    csv : str
-        path to the file to upload. 
-    file : str
-        path to the file to upload. 
-    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     multipart_form_data = {
-        "csv":csv,
-        "file":file,
     }
     uri = f"/api/v1/orgs/{org_id}/sites/{site_name}/maps/import"
     resp = mist_session.mist_post_file(uri=uri, multipart_form_data=multipart_form_data)
     return resp
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/sitetemplates.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/sitetemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgSiteTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgSiteTemplates")  
 def getOrgSiteTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSiteTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/ssoroles.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/ssoroles.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgSsoRoles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgSsoRoles")  
 def getOrgSsoRoles(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsoRoles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/ssos.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/ssos.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgSsos")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgSsos")  
 def getOrgSsos(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsos
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -160,15 +160,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/ssos/{sso_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgSsoLatestFailures")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgSsoLatestFailures")  
 def getOrgSsoLatestFailures(mist_session:_APISession, org_id:str, sso_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsoLatestFailures
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/ssr.py` & `mistapi-0.42.0/src/mistapi/api/v1/self/apitokens.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,160 +10,142 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getOrg128TRegistrationCommands(mist_session:_APISession, org_id:str) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listApiTokens")  
+def getApiTokens(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrg128TRegistrationCommands
+    API doc: https://doc.mist-lab.fr/#operation/listApiTokens
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
-    PATH PARAMS
-    -----------
-    org_id : str        
-    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/128routers/register_cmd"
+    uri = f"/api/v1/self/apitokens"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgSsrUpgrades")  
-def getOrgSsrUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listApiTokens(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgSsrUpgrades
+    API doc: https://doc.mist-lab.fr/#operation/listApiTokens
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
-    PATH PARAMS
-    -----------
-    org_id : str        
-    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/ssr/upgrade"
+    uri = f"/api/v1/self/apitokens"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listOrgSsrUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
+def createApiToken(mist_session:_APISession, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgSsrUpgrades
+    API doc: https://doc.mist-lab.fr/#operation/createApiToken
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
-    PATH PARAMS
+    BODY PARAMS
     -----------
-    org_id : str        
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/ssr/upgrade"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/self/apitokens"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def upgradeOrgSsrs(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def getApiToken(mist_session:_APISession, apitoken_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/upgradeOrgSsrs
+    API doc: https://doc.mist-lab.fr/#operation/getApiToken
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
-    
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
+    apitoken_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/ssr/upgrade"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/self/apitokens/{apitoken_id}"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def cancelOrgSsrUpgrade(mist_session:_APISession, org_id:str, upgrade_id:str, body:object) -> _APIResponse:
+def deleteApiToken(mist_session:_APISession, apitoken_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/cancelOrgSsrUpgrade
+    API doc: https://doc.mist-lab.fr/#operation/deleteApiToken
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str
-    upgrade_id : str        
-    
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
+    apitoken_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/ssr/upgrade/{upgrade_id}/cancel"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/self/apitokens/{apitoken_id}"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def getOrgSsrUpgradeInfo(mist_session:_APISession, org_id:str, channel:str=None) -> _APIResponse:
+def updateApiToken(mist_session:_APISession, apitoken_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgSsrUpgradeInfo
+    API doc: https://doc.mist-lab.fr/#operation/updateApiToken
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
+    apitoken_id : str        
     
-    QUERY PARAMS
-    ------------
-    channel : str        
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/ssr/versions"
-    query_params={}
-    if channel: query_params["channel"]=channel
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/self/apitokens/{apitoken_id}"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/stats.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgAssetsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgAssetsStats")  
 def getOrgAssetsStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAssetsStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -255,15 +255,15 @@
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/stats/bgp_peers/search"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgDevicesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgDevicesStats")  
 def getOrgDevicesStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", type:str="ap", status:str="all", site_id:str=None, mac:str=None, evpntopo_id:str=None, evpn_unused:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDevicesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -356,15 +356,15 @@
     if site_id: query_params["site_id"]=site_id
     if mac: query_params["mac"]=mac
     if evpntopo_id: query_params["evpntopo_id"]=evpntopo_id
     if evpn_unused: query_params["evpn_unused"]=evpn_unused
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgMxEdgesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgMxEdgesStats")  
 def getOrgMxEdgesStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", for_site:str="false") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/subscriptions.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/subscriptions.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/templates.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgTemplates")  
 def getOrgTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/tickets.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/tickets.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgTickets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgTickets")  
 def getOrgTickets(mist_session:_APISession, org_id:str, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgTickets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/troubleshoot.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/troubleshoot.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,31 +10,31 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def troubleshootOrgClient(mist_session:_APISession, org_id:str, mac:str=None, site_id:str=None, start:int=None, end:int=None, type:str=None) -> _APIResponse:
+def troubleshootOrg(mist_session:_APISession, org_id:str, mac:str=None, site_id:str=None, start:int=None, end:int=None, type:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/troubleshootOrgClient
+    API doc: https://doc.mist-lab.fr/#operation/troubleshootOrg
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     mac : str
-      **required** when troubleshooting device
+      **required** when troubleshooting device or a client
     site_id : str
       **required** when troubleshooting site
     start : int
     end : int
     type : str{'wireless', 'wired', 'wan'}
       when troubleshooting site, type of network to troubleshoot
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/vpns.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/beacons.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,157 +10,157 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgsVpns")  
-def getOrgsVpns(mist_session:_APISession, org_id:str) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteBeacons")  
+def getSiteBeacons(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgsVpns
+    API doc: https://doc.mist-lab.fr/#operation/listSiteBeacons
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
+    site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/vpns"
+    uri = f"/api/v1/sites/{site_id}/beacons"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listOrgsVpns(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listSiteBeacons(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgsVpns
+    API doc: https://doc.mist-lab.fr/#operation/listSiteBeacons
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
+    site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/vpns"
+    uri = f"/api/v1/sites/{site_id}/beacons"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createOrgVpns(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def createSiteBeacon(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createOrgVpns
+    API doc: https://doc.mist-lab.fr/#operation/createSiteBeacon
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
+    site_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/vpns"
+    uri = f"/api/v1/sites/{site_id}/beacons"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getOrgVpn(mist_session:_APISession, org_id:str, vpn_id:str) -> _APIResponse:
+def getSiteBeacon(mist_session:_APISession, site_id:str, beacon_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgVpn
+    API doc: https://doc.mist-lab.fr/#operation/getSiteBeacon
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str
-    vpn_id : str        
+    site_id : str
+    beacon_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/vpns/{vpn_id}"
+    uri = f"/api/v1/sites/{site_id}/beacons/{beacon_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteOrgVpn(mist_session:_APISession, org_id:str, vpn_id:str) -> _APIResponse:
+def deleteSiteBeacons(mist_session:_APISession, site_id:str, beacon_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteOrgVpn
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteBeacons
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str
-    vpn_id : str        
+    site_id : str
+    beacon_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/vpns/{vpn_id}"
+    uri = f"/api/v1/sites/{site_id}/beacons/{beacon_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateOrgVpn(mist_session:_APISession, org_id:str, vpn_id:str, body:object) -> _APIResponse:
+def updateSiteBeacons(mist_session:_APISession, site_id:str, beacon_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateOrgVpn
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteBeacons
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str
-    vpn_id : str        
+    site_id : str
+    beacon_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/vpns/{vpn_id}"
+    uri = f"/api/v1/sites/{site_id}/beacons/{beacon_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/wan_client.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/wan_client.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/wan_clients.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/wan_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/webhooks.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/rssizones.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,157 +10,157 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgWebhooks")  
-def getOrgWebhooks(mist_session:_APISession, org_id:str) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteRssiZones")  
+def getSiteRssiZones(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgWebhooks
+    API doc: https://doc.mist-lab.fr/#operation/listSiteRssiZones
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
+    site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/webhooks"
+    uri = f"/api/v1/sites/{site_id}/rssizones"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listOrgWebhooks(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listSiteRssiZones(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgWebhooks
+    API doc: https://doc.mist-lab.fr/#operation/listSiteRssiZones
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
+    site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/webhooks"
+    uri = f"/api/v1/sites/{site_id}/rssizones"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createOrgWebhook(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def createSiteRssiZone(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createOrgWebhook
+    API doc: https://doc.mist-lab.fr/#operation/createSiteRssiZone
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
+    site_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/webhooks"
+    uri = f"/api/v1/sites/{site_id}/rssizones"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getOrgWebhook(mist_session:_APISession, org_id:str, webhook_id:str) -> _APIResponse:
+def getSiteRssiZone(mist_session:_APISession, site_id:str, rssizone_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgWebhook
+    API doc: https://doc.mist-lab.fr/#operation/getSiteRssiZone
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str
-    webhook_id : str        
+    site_id : str
+    rssizone_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/webhooks/{webhook_id}"
+    uri = f"/api/v1/sites/{site_id}/rssizones/{rssizone_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteOrgWebhook(mist_session:_APISession, org_id:str, webhook_id:str) -> _APIResponse:
+def deleteSiteRssiZone(mist_session:_APISession, site_id:str, rssizone_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteOrgWebhook
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteRssiZone
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str
-    webhook_id : str        
+    site_id : str
+    rssizone_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/webhooks/{webhook_id}"
+    uri = f"/api/v1/sites/{site_id}/rssizones/{rssizone_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateOrgWebhook(mist_session:_APISession, org_id:str, webhook_id:str, body:object) -> _APIResponse:
+def updateSiteRssiZone(mist_session:_APISession, site_id:str, rssizone_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateOrgWebhook
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteRssiZone
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str
-    webhook_id : str        
+    site_id : str
+    rssizone_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/webhooks/{webhook_id}"
+    uri = f"/api/v1/sites/{site_id}/rssizones/{rssizone_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/wired_clients.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/wired_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/wlans.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/wlans.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgWlans")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgWlans")  
 def getOrgWlans(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWlans
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -84,43 +84,14 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/wlans"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getOrgWlanDerived(mist_session:_APISession, org_id:str, resolve:bool=None) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgWlanDerived
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    org_id : str        
-    
-    QUERY PARAMS
-    ------------
-    resolve : bool
-      whether to resolve SITE_VARS, default is false (as filter, optional)        
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/orgs/{org_id}/wlans/derived"
-    query_params={}
-    if resolve: query_params["resolve"]=resolve
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
 def getOrgWLAN(mist_session:_APISession, org_id:str, wlan_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/getOrgWLAN
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/wxrules.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/wxrules.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgWxRules")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgWxRules")  
 def getOrgWxRules(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxRules
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/wxtags.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/wxtags.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgWxTags")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgWxTags")  
 def getOrgWxTags(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxTags
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/orgs/wxtunnels.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/wxtunnels.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listOrgWxTunnels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgWxTunnels")  
 def getOrgWxTunnels(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxTunnels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/recover/recover.py` & `mistapi-0.42.0/src/mistapi/api/v1/recover/recover.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/recover/verify.py` & `mistapi-0.42.0/src/mistapi/api/v1/recover/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/register/register.py` & `mistapi-0.42.0/src/mistapi/api/v1/register/register.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/register/verify.py` & `mistapi-0.42.0/src/mistapi/api/v1/register/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/self/__init__.py` & `mistapi-0.42.0/src/mistapi/api/v1/self/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/self/apitokens.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/sites.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,92 +10,80 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listApiTokens")  
-def getApiTokens(mist_session:_APISession) -> _APIResponse:
+def getSiteInfo(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listApiTokens
+    API doc: https://doc.mist-lab.fr/#operation/getSiteInfo
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/self/apitokens"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
-def listApiTokens(mist_session:_APISession) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/listApiTokens
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
+    PATH PARAMS
+    -----------
+    site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/self/apitokens"
+    uri = f"/api/v1/sites/{site_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createApiToken(mist_session:_APISession, body:object) -> _APIResponse:
+def deleteSite(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createApiToken
+    API doc: https://doc.mist-lab.fr/#operation/deleteSite
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
-    BODY PARAMS
+    PATH PARAMS
     -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
+    site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/self/apitokens"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def deleteApiToken(mist_session:_APISession, apitoken_id:str) -> _APIResponse:
+def updateSiteInfo(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteApiToken
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteInfo
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    apitoken_id : str        
+    site_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/self/apitokens/{apitoken_id}"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    uri = f"/api/v1/sites/{site_id}"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/self/logs.py` & `mistapi-0.42.0/src/mistapi/api/v1/self/logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSelfAuditLogs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSelfAuditLogs")  
 def getSelfAuditLogs(mist_session:_APISession, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSelfAuditLogs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/self/oauth.py` & `mistapi-0.42.0/src/mistapi/api/v1/self/oauth.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/self/self.py` & `mistapi-0.42.0/src/mistapi/api/v1/self/self.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/self/subscriptions.py` & `mistapi-0.42.0/src/mistapi/api/v1/self/subscriptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listAlarmSubscriptions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listAlarmSubscriptions")  
 def getAlarmSubscriptions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listAlarmSubscriptions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/self/two_factor.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/licenses.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,54 +10,30 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def generateQrCodeForVerification(mist_session:_APISession, by:str="qrcode") -> _APIResponse:
+def getSiteLicenseUsage(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/generateQrCodeForVerification
+    API doc: https://doc.mist-lab.fr/#operation/getSiteLicenseUsage
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
-    QUERY PARAMS
-    ------------
-    by : str{'qrcode'}, default: qrcode        
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/self/two_factor/token"
-    query_params={}
-    if by: query_params["by"]=by
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
-def verifyTwoFactor(mist_session:_APISession, body:object) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/verifyTwoFactor
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    BODY PARAMS
+    PATH PARAMS
     -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
+    site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/self/two_factor/verify"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/licenses/usages"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/self/update.py` & `mistapi-0.42.0/src/mistapi/api/v1/self/update.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/__init__.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/alarms.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/alarms.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/anomaly.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/anomaly.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/apps.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/networks.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,54 +10,66 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteApps")  
-def getSiteApps(mist_session:_APISession, site_id:str) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteNetworksDerived")  
+def getSiteNetworksDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteApps
+    API doc: https://doc.mist-lab.fr/#operation/listSiteNetworksDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
+    QUERY PARAMS
+    ------------
+    resolve : bool
+      whether resolve the site variables        
+    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/apps"
-    query_params={}
+    uri = f"/api/v1/sites/{site_id}/networks/derived"
+    query_params={}
+    if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteApps(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listSiteNetworksDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteApps
+    API doc: https://doc.mist-lab.fr/#operation/listSiteNetworksDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
+    QUERY PARAMS
+    ------------
+    resolve : bool
+      whether resolve the site variables        
+    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/apps"
-    query_params={}
+    uri = f"/api/v1/sites/{site_id}/networks/derived"
+    query_params={}
+    if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/assetfilters.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/assetfilters.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteAssetFilters")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteAssetFilters")  
 def getSiteAssetFilters(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAssetFilters
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/assets.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteAssets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteAssets")  
 def getSiteAssets(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAssets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/beacons.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/uisettings.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteBeacons")  
-def getSiteBeacons(mist_session:_APISession, site_id:str) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteCurdSettings")  
+def getSiteCurdSettings(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteBeacons
+    API doc: https://doc.mist-lab.fr/#operation/listSiteCurdSettings
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -29,22 +29,22 @@
     site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/beacons"
+    uri = f"/api/v1/sites/{site_id}/uisettings"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteBeacons(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listSiteCurdSettings(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteBeacons
+    API doc: https://doc.mist-lab.fr/#operation/listSiteCurdSettings
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -52,22 +52,22 @@
     site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/beacons"
+    uri = f"/api/v1/sites/{site_id}/uisettings"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createSiteBeacon(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def createSiteCurdSettings(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createSiteBeacon
+    API doc: https://doc.mist-lab.fr/#operation/createSiteCurdSettings
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -80,87 +80,110 @@
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/beacons"
+    uri = f"/api/v1/sites/{site_id}/uisettings"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getSiteBeacon(mist_session:_APISession, site_id:str, beacon_id:str) -> _APIResponse:
+def getSiteCurdSettingDerived(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteBeacon
+    API doc: https://doc.mist-lab.fr/#operation/getSiteCurdSettingDerived
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/uisettings/derived"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def getSiteCurdSetting(mist_session:_APISession, site_id:str, uisetting_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/getSiteCurdSetting
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    beacon_id : str        
+    uisetting_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/beacons/{beacon_id}"
+    uri = f"/api/v1/sites/{site_id}/uisettings/{uisetting_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteSiteBeacons(mist_session:_APISession, site_id:str, beacon_id:str) -> _APIResponse:
+def deleteSiteCurdSetting(mist_session:_APISession, site_id:str, uisetting_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteBeacons
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteCurdSetting
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    beacon_id : str        
+    uisetting_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/beacons/{beacon_id}"
+    uri = f"/api/v1/sites/{site_id}/uisettings/{uisetting_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateSiteBeacons(mist_session:_APISession, site_id:str, beacon_id:str, body:object) -> _APIResponse:
+def updateSiteCurdSetting(mist_session:_APISession, site_id:str, uisetting_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteBeacons
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteCurdSetting
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    beacon_id : str        
+    uisetting_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/beacons/{beacon_id}"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/uisettings/{uisetting_id}"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/call.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/call.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/clients.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/count.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/count.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/deviceprofiles.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/deviceprofiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteDeviceProfilesDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteDeviceProfilesDerived")  
 def getSiteDeviceProfilesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDeviceProfilesDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/devices.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteDevices")  
 def getSiteDevices(mist_session:_APISession, site_id:str, type:str="ap", name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -550,15 +550,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/restart"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def searchSiteDevices(mist_session:_APISession, site_id:str, hostname:str=None, type:str="ap", model:str=None, mac:str=None, version:str=None, power_constrained:bool=None, ip_address:str=None, mxtunnel_status:str=None, mxedge_id:str=None, lldp_system_name:str=None, lldp_system_desc:str=None, lldp_port_id:str=None, lldp_mgmt_addr:str=None, band_24_channel:int=None, band_5_channel:int=None, band_6_channel:int=None, eth0_port_speed:int=None, sort:str="timestamp", desc_sort:str=None, stats:bool=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def searchSiteDevices(mist_session:_APISession, site_id:str, hostname:str=None, type:str="ap", model:str=None, mac:str=None, version:str=None, power_constrained:bool=None, ip_address:str=None, mxtunnel_status:str=None, mxedge_id:str=None, lldp_system_name:str=None, lldp_system_desc:str=None, lldp_port_id:str=None, lldp_mgmt_addr:str=None, band_24_channel:int=None, band_5_channel:int=None, band_6_channel:int=None, band_24_bandwith:int=None, band_5_bandwith:int=None, band_6_bandwith:int=None, eth0_port_speed:int=None, sort:str="timestamp", desc_sort:str=None, stats:bool=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/searchSiteDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -596,14 +596,20 @@
       LLDP management ip address
     band_24_channel : int
       Channel of band_24
     band_5_channel : int
       Channel of band_5
     band_6_channel : int
       Channel of band_6
+    band_24_bandwith : int
+      Bandwidth of band_24
+    band_5_bandwith : int
+      Bandwidth of band_5
+    band_6_bandwith : int
+      Bandwidth of band_6
     eth0_port_speed : int
       Port speed of eth0
     sort : str{'timestamp', 'mac', 'model', 'sku'}, default: timestamp
       sort options
     desc_sort : str{'timestamp', 'mac', 'model', 'sku'}
       sort options in reverse order
     stats : bool
@@ -632,28 +638,60 @@
     if lldp_system_name: query_params["lldp_system_name"]=lldp_system_name
     if lldp_system_desc: query_params["lldp_system_desc"]=lldp_system_desc
     if lldp_port_id: query_params["lldp_port_id"]=lldp_port_id
     if lldp_mgmt_addr: query_params["lldp_mgmt_addr"]=lldp_mgmt_addr
     if band_24_channel: query_params["band_24_channel"]=band_24_channel
     if band_5_channel: query_params["band_5_channel"]=band_5_channel
     if band_6_channel: query_params["band_6_channel"]=band_6_channel
+    if band_24_bandwith: query_params["band_24_bandwith"]=band_24_bandwith
+    if band_5_bandwith: query_params["band_5_bandwith"]=band_5_bandwith
+    if band_6_bandwith: query_params["band_6_bandwith"]=band_6_bandwith
     if eth0_port_speed: query_params["eth0_port_speed"]=eth0_port_speed
     if sort: query_params["sort"]=sort
     if desc_sort: query_params["desc_sort"]=desc_sort
     if stats: query_params["stats"]=stats
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteDevicesUpgrade")  
 def getSiteDevicesUpgrade(mist_session:_APISession, site_id:str, status:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteDevicesUpgrade
+    API doc: https://doc.mist-lab.fr/#operation/listSiteDevicesUpgrade
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str        
+    
+    QUERY PARAMS
+    ------------
+    status : str{'downloading', 'completed', 'created', 'downloaded', 'upgrading', 'cancelled', 'failed'}        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/devices/upgrade"
+    query_params={}
+    if status: query_params["status"]=status
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def listSiteDevicesUpgrade(mist_session:_APISession, site_id:str, status:str=None) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/listSiteDevicesUpgrade
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -745,15 +783,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/upgrade/{upgrade_id}/cancel"
     resp = mist_session.mist_post(uri=uri)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteAvailableDeviceVersions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteAvailableDeviceVersions")  
 def getSiteAvailableDeviceVersions(mist_session:_APISession, site_id:str, type:str="ap", model:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAvailableDeviceVersions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -1713,17 +1751,17 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/support"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def StartSiteDeviceSyntheticTest(mist_session:_APISession, site_id:str, device_id:str, body:object) -> _APIResponse:
+def triggerSiteDeviceSyntheticTest(mist_session:_APISession, site_id:str, device_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/StartSiteDeviceSyntheticTest
+    API doc: https://doc.mist-lab.fr/#operation/triggerSiteDeviceSyntheticTest
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/events.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/events.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/evpn_topologies.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/evpn_topologies.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/guests.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/guests.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteAllGuestAuthorizations")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteAllGuestAuthorizations")  
 def getSiteAllGuestAuthorizations(mist_session:_APISession, site_id:str, wlan_id:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAllGuestAuthorizations
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/insights.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/insights.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if interval: query_params["interval"]=interval
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteRogueAPs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteRogueAPs")  
 def getSiteRogueAPs(mist_session:_APISession, site_id:str, type:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d", interval:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteRogueAPs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -167,15 +167,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if interval: query_params["interval"]=interval
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteRogueClients")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteRogueClients")  
 def getSiteRogueClients(mist_session:_APISession, site_id:str, limit:int=100, start:int=None, end:int=None, duration:str="1d", interval:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteRogueClients
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/licenses.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/wan_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,30 +10,35 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getSiteLicenseUsage(mist_session:_APISession, site_id:str) -> _APIResponse:
+def countSiteWanClientEvents(mist_session:_APISession, site_id:str, distinct:str="type") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteLicenseUsage
+    API doc: https://doc.mist-lab.fr/#operation/countSiteWanClientEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
+    QUERY PARAMS
+    ------------
+    distinct : str{'type', 'hostname', 'ip', 'mfg', 'mac'}, default: type        
+    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/licenses/usages"
-    query_params={}
+    uri = f"/api/v1/sites/{site_id}/wan_client/events/count"
+    query_params={}
+    if distinct: query_params["distinct"]=distinct
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/location.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/location.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/maps.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/maps.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteMaps")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteMaps")  
 def getSiteMaps(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteMaps
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -84,51 +84,33 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/maps"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def importSiteMapsFile(mist_session:_APISession, site_id:str, auto_deviceprofile_assignment:bool=None, csv:str=None, file:str=None, json:dict=None) -> _APIResponse:
+def importSiteMapsFile(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/importSiteMaps
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
-    BODY PARAMS
-    -----------
-    auto_deviceprofile_assignment : bool
-        whether to auto assign device to deviceprofile by name
-    csv : str
-        path to the file to upload. csv file for ap name mapping, optional
-    file : str
-        path to the file to upload. ekahau or ibwave file
-    json : dict
-        import_all_floorplans : bool
-        import_height : bool, default: True
-        import_orientation : bool, default: True
-        vendor_name : {'ekahau', 'ibwave'}
-    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     multipart_form_data = {
-        "auto_deviceprofile_assignment":auto_deviceprofile_assignment,
-        "csv":csv,
-        "file":file,
-        "json":json,
     }
     uri = f"/api/v1/sites/{site_id}/maps/import"
     resp = mist_session.mist_post_file(uri=uri, multipart_form_data=multipart_form_data)
     return resp
 
 def getSiteMap(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
     """
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/mxedges.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/mxedges.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteMxEdges")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteMxEdges")  
 def getSiteMxEdges(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteMxEdges
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/mxtunnels.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/mxtunnels.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/networks.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/vpns.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteNetworksDerived")  
-def getSiteNetworksDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteVpnsDerived")  
+def getSiteVpnsDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteNetworksDerived
+    API doc: https://doc.mist-lab.fr/#operation/listSiteVpnsDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -34,23 +34,23 @@
       whether resolve the site variables        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/networks/derived"
+    uri = f"/api/v1/sites/{site_id}/vpns/derived"
     query_params={}
     if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteNetworksDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
+def listSiteVpnsDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteNetworksDerived
+    API doc: https://doc.mist-lab.fr/#operation/listSiteVpnsDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -63,13 +63,13 @@
       whether resolve the site variables        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/networks/derived"
+    uri = f"/api/v1/sites/{site_id}/vpns/derived"
     query_params={}
     if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/otherdevices.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/otherdevices.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteOtherDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteOtherDevices")  
 def getSiteOtherDevices(mist_session:_APISession, site_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteOtherDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/pcaps.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/pcaps.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSitePacketCaptures")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSitePacketCaptures")  
 def getSitePacketCaptures(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", client_mac:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSitePacketCaptures
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/psks.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/psks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSitePsks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSitePsks")  
 def getSitePsks(mist_session:_APISession, site_id:str, ssid:str=None, role:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSitePsks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/rfdiags.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/rfdiags.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/rogues.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/rogues.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     bssid : str
       bssid of the network detected as threat
     ap_mac : str
       mac of the device that had strongest signal strength for ssid/bssid pair
     channel : str
       channel over which ap_mac heard ssid/bssid pair
     seen_on_lan : bool
-      whether the reporting AP see a wireless client (on LAN) connecting to it  
+      whether the reporting AP see a wireless client (on LAN) connecting to it
     page : int, default: 1
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
@@ -90,15 +90,15 @@
     bssid : str
       bssid of the network detected as threat
     ap_mac : str
       mac of the device that had strongest signal strength for ssid/bssid pair
     channel : int
       channel over which ap_mac heard ssid/bssid pair
     seen_on_lan : bool
-      whether the reporting AP see a wireless client (on LAN) connecting to it  
+      whether the reporting AP see a wireless client (on LAN) connecting to it
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/rrm.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/rrm.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/rssizones.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/zones.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteRssiZones")  
-def getSiteRssiZones(mist_session:_APISession, site_id:str) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteZones")  
+def getSiteZones(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteRssiZones
+    API doc: https://doc.mist-lab.fr/#operation/listSiteZones
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -29,22 +29,22 @@
     site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/rssizones"
+    uri = f"/api/v1/sites/{site_id}/zones"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteRssiZones(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listSiteZones(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteRssiZones
+    API doc: https://doc.mist-lab.fr/#operation/listSiteZones
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -52,22 +52,22 @@
     site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/rssizones"
+    uri = f"/api/v1/sites/{site_id}/zones"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createSiteRssiZone(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def createSiteZone(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createSiteRssiZone
+    API doc: https://doc.mist-lab.fr/#operation/createSiteZone
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -80,87 +80,87 @@
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/rssizones"
+    uri = f"/api/v1/sites/{site_id}/zones"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getSiteRssiZone(mist_session:_APISession, site_id:str, rssizone_id:str) -> _APIResponse:
+def getSiteZone(mist_session:_APISession, site_id:str, zone_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteRssiZone
+    API doc: https://doc.mist-lab.fr/#operation/getSiteZone
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    rssizone_id : str        
+    zone_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/rssizones/{rssizone_id}"
+    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteSiteRssiZone(mist_session:_APISession, site_id:str, rssizone_id:str) -> _APIResponse:
+def deleteSiteZone(mist_session:_APISession, site_id:str, zone_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteRssiZone
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteZone
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    rssizone_id : str        
+    zone_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/rssizones/{rssizone_id}"
+    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateSiteRssiZone(mist_session:_APISession, site_id:str, rssizone_id:str, body:object) -> _APIResponse:
+def updateSiteZone(mist_session:_APISession, site_id:str, zone_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteRssiZone
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteZone
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    rssizone_id : str        
+    zone_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/rssizones/{rssizone_id}"
+    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/servicepolicies.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/servicepolicies.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteServicePoliciesDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteServicePoliciesDerived")  
 def getSiteServicePoliciesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteServicePoliciesDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/services.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/services.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteServicesDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteServicesDerived")  
 def getSiteServicesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteServicesDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/setting.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/setting.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/sites.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/subscriptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getSiteInfo(mist_session:_APISession, site_id:str) -> _APIResponse:
+def UnsubscribeSiteAlarms(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteInfo
+    API doc: https://doc.mist-lab.fr/#operation/UnsubscribeSiteAlarms
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -28,62 +28,34 @@
     site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
-def deleteSite(mist_session:_APISession, site_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSite
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    site_id : str        
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}"
+    uri = f"/api/v1/sites/{site_id}/subscriptions"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateSiteInfo(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def SubscribeSiteAlarms(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteInfo
+    API doc: https://doc.mist-lab.fr/#operation/SubscribeSiteAlarms
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
-    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/subscriptions"
+    resp = mist_session.mist_post(uri=uri)
     return resp
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/skyatp.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/skyatp.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/sle.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/sle.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     site_id : str
     scope : str
     scope_id : str
       * site_id if `scope`==`site`
 * device_id if `scope`==`ap`, `scope`==`switch` or `scope`==`gateway`
 * mac if `scope`==`client`
     metric : str
-       values from /api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metrics        
+      values from /api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metrics        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metric/{metric}/classifiers"
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/ssr.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/ssr.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/stats.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     if distinct: query_params["distinct"]=distinct
     if device_mac: query_params["device_mac"]=device_mac
     if app: query_params["app"]=app
     if wired: query_params["wired"]=wired
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteAssetsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteAssetsStats")  
 def getSiteAssetsStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAssetsStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -266,15 +266,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteBeaconsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteBeaconsStats")  
 def getSiteBeaconsStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteBeaconsStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -469,15 +469,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteWirelessClientsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteWirelessClientsStats")  
 def getSiteWirelessClientsStats(mist_session:_APISession, site_id:str, wired:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWirelessClientsStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -555,15 +555,15 @@
     """
     uri = f"/api/v1/sites/{site_id}/stats/clients/{client_mac}"
     query_params={}
     if wired: query_params["wired"]=wired
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteDevicesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteDevicesStats")  
 def getSiteDevicesStats(mist_session:_APISession, site_id:str, type:str="ap", status:str="all", page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDevicesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -672,15 +672,15 @@
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/devices/{device_id}/clients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteDiscoveredAssets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteDiscoveredAssets")  
 def getSiteDiscoveredAssets(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDiscoveredAssets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -1045,15 +1045,15 @@
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/maps/{map_id}/sdkclients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteUnconnectedClientStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteUnconnectedClientStats")  
 def getSiteUnconnectedClientStats(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteUnconnectedClientStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -1094,15 +1094,15 @@
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/maps/{map_id}/unconnected_clients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteMxEdgesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteMxEdgesStats")  
 def getSiteMxEdgesStats(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteMxEdgesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -1279,15 +1279,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchSiteSwOrGwPorts(mist_session:_APISession, site_id:str, full_duplex:bool=None, mac:str=None, neighbor_mac:str=None, neighbor_port_desc:str=None, neighbor_system_name:str=None, poe_disabled:bool=None, poe_mode:str=None, poe_on:bool=None, port_id:str=None, port_mac:str=None, power_draw:float=None, tx_pkts:int=None, rx_pkts:int=None, rx_bytes:int=None, tx_bps:int=None, rx_bps:int=None, tx_errors:int=None, rx_errors:int=None, tx_mcast_pkts:int=None, tx_bcast_pkts:int=None, rx_mcast_pkts:int=None, rx_bcast_pkts:int=None, speed:int=None, mac_limit:int=None, mac_count:int=None, up:bool=None, stp_state:str=None, stp_role:str=None, xcvr_part_number:str=None, auth_state:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def searchSiteSwOrGwPorts(mist_session:_APISession, site_id:str, full_duplex:bool=None, mac:str=None, type:str=None, neighbor_mac:str=None, neighbor_port_desc:str=None, neighbor_system_name:str=None, poe_disabled:bool=None, poe_mode:str=None, poe_on:bool=None, port_id:str=None, port_mac:str=None, power_draw:float=None, tx_pkts:int=None, rx_pkts:int=None, rx_bytes:int=None, tx_bps:int=None, rx_bps:int=None, tx_errors:int=None, rx_errors:int=None, tx_mcast_pkts:int=None, tx_bcast_pkts:int=None, rx_mcast_pkts:int=None, rx_bcast_pkts:int=None, speed:int=None, mac_limit:int=None, mac_count:int=None, up:bool=None, active:bool=None, jitter:float=None, loss:float=None, latency:float=None, stp_state:str=None, stp_role:str=None, xcvr_part_number:str=None, auth_state:str=None, lte_imsi:str=None, lte_iccid:str=None, lte_imei:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/searchSiteSwOrGwPorts
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -1298,14 +1298,16 @@
     
     QUERY PARAMS
     ------------
     full_duplex : bool
       indicates full or half duplex
     mac : str
       device identifier
+    type : str{'ap', 'ble', 'switch', 'gateway', 'mxedge', 'nac'}
+      device type
     neighbor_mac : str
       Chassis identifier of the chassis type listed
     neighbor_port_desc : str
       Description supplied by the system on the interface E.g. “GigabitEthernet2/0/39”
     neighbor_system_name : str
       Name supplied by the system on the interface E.g. neighbor system name E.g. “Kumar-Acc-SW.mist.local”
     poe_disabled : bool
@@ -1346,36 +1348,51 @@
       port speed
     mac_limit : int
       Limit on number of dynamically learned macs
     mac_count : int
       Number of mac addresses in the forwarding table
     up : bool
       indicates if interface is up
+    active : bool
+      indicates if interface is active/inactive
+    jitter : float
+      Last sampled jitter of the interface
+    loss : float
+      Last sampled loss of the interface
+    latency : float
+      Last sampled latency of the interface
     stp_state : str{'forwarding', 'blocking', 'learning', 'listening', 'disabled'}
       if `up`==`true`
     stp_role : str{'designated', 'backup', 'alternate', 'root', 'root-prevented'}
       if `up`==`true`
     xcvr_part_number : str
       Optic Slot Partnumber, Check for null/empty
     auth_state : str{'init', 'authenticated', 'authenticating', 'held'}
       if `up`==`true` && has Authenticator role
+    lte_imsi : str
+      LTE IMSI value, Check for null/empty
+    lte_iccid : str
+      LTE ICCID value, Check for null/empty
+    lte_imei : str
+      LTE IMEI value, Check for null/empty
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/ports/search"
     query_params={}
     if full_duplex: query_params["full_duplex"]=full_duplex
     if mac: query_params["mac"]=mac
+    if type: query_params["type"]=type
     if neighbor_mac: query_params["neighbor_mac"]=neighbor_mac
     if neighbor_port_desc: query_params["neighbor_port_desc"]=neighbor_port_desc
     if neighbor_system_name: query_params["neighbor_system_name"]=neighbor_system_name
     if poe_disabled: query_params["poe_disabled"]=poe_disabled
     if poe_mode: query_params["poe_mode"]=poe_mode
     if poe_on: query_params["poe_on"]=poe_on
     if port_id: query_params["port_id"]=port_id
@@ -1392,18 +1409,25 @@
     if tx_bcast_pkts: query_params["tx_bcast_pkts"]=tx_bcast_pkts
     if rx_mcast_pkts: query_params["rx_mcast_pkts"]=rx_mcast_pkts
     if rx_bcast_pkts: query_params["rx_bcast_pkts"]=rx_bcast_pkts
     if speed: query_params["speed"]=speed
     if mac_limit: query_params["mac_limit"]=mac_limit
     if mac_count: query_params["mac_count"]=mac_count
     if up: query_params["up"]=up
+    if active: query_params["active"]=active
+    if jitter: query_params["jitter"]=jitter
+    if loss: query_params["loss"]=loss
+    if latency: query_params["latency"]=latency
     if stp_state: query_params["stp_state"]=stp_state
     if stp_role: query_params["stp_role"]=stp_role
     if xcvr_part_number: query_params["xcvr_part_number"]=xcvr_part_number
     if auth_state: query_params["auth_state"]=auth_state
+    if lte_imsi: query_params["lte_imsi"]=lte_imsi
+    if lte_iccid: query_params["lte_iccid"]=lte_iccid
+    if lte_imei: query_params["lte_imei"]=lte_imei
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
@@ -1650,63 +1674,44 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteWiredClientAndParentInterface(mist_session:_APISession, site_id:str, device_id:str, port_id:str=None) -> _APIResponse:
+def getSiteSwitchesMetrics(mist_session:_APISession, site_id:str, type:str=None, scope:str=None, switch_mac:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteWiredClientAndParentInterface
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSwitchesMetrics
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str
-    device_id : str        
+    site_id : str        
     
     QUERY PARAMS
     ------------
-    port_id : str        
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/stats/switch_wired_clients/{device_id}/search"
-    query_params={}
-    if port_id: query_params["port_id"]=port_id
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
-def getSiteAdoptedSwitchesComplianceMetrics(mist_session:_APISession, site_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteAdoptedSwitchesComplianceMetrics
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    site_id : str        
+    type : str{'active_ports_summary'}
+    scope : str{'site', 'switch'}
+    switch_mac : str
+      switch mac, used only with metric `type`==`active_ports_summary`        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/switches/metrics"
-    query_params={}
+    query_params={}
+    if type: query_params["type"]=type
+    if scope: query_params["scope"]=scope
+    if switch_mac: query_params["switch_mac"]=switch_mac
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
 def getSiteWxRulesUsage(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/getSiteWxRulesUsage
     
@@ -1725,15 +1730,15 @@
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/wxrules"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteZonesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteZonesStats")  
 def getSiteZonesStats(mist_session:_APISession, site_id:str, map_id:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteZonesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/subscriptions.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/synthetic_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def UnsubscribeSite(mist_session:_APISession, site_id:str) -> _APIResponse:
+def getSiteSyntheticTestStatus(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/UnsubscribeSite
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSyntheticTestStatus
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -28,34 +28,39 @@
     site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/subscriptions"
+    uri = f"/api/v1/sites/{site_id}/synthetic_test"
     query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def SubscribeSite(mist_session:_APISession, site_id:str) -> _APIResponse:
+def triggerSiteSyntheticTest(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/SubscribeSite
+    API doc: https://doc.mist-lab.fr/#operation/triggerSiteSyntheticTest
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/subscriptions"
-    resp = mist_session.mist_post(uri=uri)
+    uri = f"/api/v1/sites/{site_id}/synthetic_test"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/uisettings.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/ssr.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,156 +10,189 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getSiteCurdSettings(mist_session:_APISession, site_id:str) -> _APIResponse:
+def getOrg128TRegistrationCommands(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteCurdSettings
+    API doc: https://doc.mist-lab.fr/#operation/getOrg128TRegistrationCommands
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str        
+    org_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/uisettings"
+    uri = f"/api/v1/orgs/{org_id}/128routers/register_cmd"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createSiteCurdSettings(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgSsrUpgrades")  
+def getOrgSsrUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createSiteCurdSettings
+    API doc: https://doc.mist-lab.fr/#operation/listOrgSsrUpgrades
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str        
-    
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
+    org_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/uisettings"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/orgs/{org_id}/ssr/upgrade"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteDerivedCurdSetting(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listOrgSsrUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteDerivedCurdSetting
+    API doc: https://doc.mist-lab.fr/#operation/listOrgSsrUpgrades
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str        
+    org_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/uisettings/derived"
+    uri = f"/api/v1/orgs/{org_id}/ssr/upgrade"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteCurdSetting(mist_session:_APISession, site_id:str, uisetting_id:str) -> _APIResponse:
+def upgradeOrgSsrs(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteCurdSetting
+    API doc: https://doc.mist-lab.fr/#operation/upgradeOrgSsrs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str
-    uisetting_id : str        
+    org_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/uisettings/{uisetting_id}"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/orgs/{org_id}/ssr/upgrade"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def deleteSiteCurdSetting(mist_session:_APISession, site_id:str, uisetting_id:str) -> _APIResponse:
+def cancelOrgSsrUpgrade(mist_session:_APISession, org_id:str, upgrade_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteCurdSetting
+    API doc: https://doc.mist-lab.fr/#operation/cancelOrgSsrUpgrade
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str
-    uisetting_id : str        
+    org_id : str
+    upgrade_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/uisettings/{uisetting_id}"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    uri = f"/api/v1/orgs/{org_id}/ssr/upgrade/{upgrade_id}/cancel"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def updateSiteCurdSetting(mist_session:_APISession, site_id:str, uisetting_id:str, body:object) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgAvailableSsrVersions")  
+def getOrgAvailableSsrVersions(mist_session:_APISession, org_id:str, channel:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteCurdSetting
+    API doc: https://doc.mist-lab.fr/#operation/listOrgAvailableSsrVersions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str
-    uisetting_id : str        
+    org_id : str        
     
-    BODY PARAMS
+    QUERY PARAMS
+    ------------
+    channel : str        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/orgs/{org_id}/ssr/versions"
+    query_params={}
+    if channel: query_params["channel"]=channel
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def listOrgAvailableSsrVersions(mist_session:_APISession, org_id:str, channel:str=None) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/listOrgAvailableSsrVersions
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
     -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
+    org_id : str        
+    
+    QUERY PARAMS
+    ------------
+    channel : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/uisettings/{uisetting_id}"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/orgs/{org_id}/ssr/versions"
+    query_params={}
+    if channel: query_params["channel"]=channel
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/vbeacons.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/vbeacons.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteVBeacons")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteVBeacons")  
 def getSiteVBeacons(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteVBeacons
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/visits.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/visits.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/wan_clients.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/wan_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/webhooks.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/webhooks.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteWebhooks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteWebhooks")  
 def getSiteWebhooks(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWebhooks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -160,14 +160,56 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/webhooks/{webhook_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
+def searchSiteWebhooksDeliveries(mist_session:_APISession, site_id:str, webhook_id:str, status_code:int=None, error:str=None, topic:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/searchSiteWebhooksDeliveries
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    webhook_id : str        
+    
+    QUERY PARAMS
+    ------------
+    status_code : int
+    error : str
+    topic : str{'alarms', 'audits', 'device-updowns', 'occupancy-alerts', 'ping'}
+      webhook topic
+    start : int
+    end : int
+    duration : str, default: 1d
+    limit : int, default: 100        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/webhooks/{webhook_id}/events/search"
+    query_params={}
+    if status_code: query_params["status_code"]=status_code
+    if error: query_params["error"]=error
+    if topic: query_params["topic"]=topic
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if limit: query_params["limit"]=limit
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
 def pingSiteWebhook(mist_session:_APISession, site_id:str, webhook_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/pingSiteWebhook
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/wired_clients.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/wired_clients.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def countSiteClientsWired(mist_session:_APISession, site_id:str, distinct:str="mac", mac:str=None, device_mac:str=None, port_id:str=None, vlan:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def countSiteWiredClients(mist_session:_APISession, site_id:str, distinct:str="mac", mac:str=None, device_mac:str=None, port_id:str=None, vlan:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countSiteClientsWired
+    API doc: https://doc.mist-lab.fr/#operation/countSiteWiredClients
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -60,17 +60,17 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchSiteClientsWired(mist_session:_APISession, site_id:str, device_mac:str=None, mac:str=None, port_id:str=None, vlan:str=None, ip_address:str=None, manufacture:str=None, text:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def searchSiteWiredClients(mist_session:_APISession, site_id:str, device_mac:str=None, mac:str=None, ip:str=None, port_id:str=None, vlan:str=None, manufacture:str=None, text:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/searchSiteClientsWired
+    API doc: https://doc.mist-lab.fr/#operation/searchSiteWiredClients
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -79,19 +79,20 @@
     
     QUERY PARAMS
     ------------
     device_mac : str
       device mac
     mac : str
       client mac
+    ip : str
+      client ip
     port_id : str
       port id
     vlan : str
       vlan
-    ip_address : str
     manufacture : str
       manufacture
     text : str
       single entry of hostname/mac
     limit : int, default: 100
     start : int
     end : int
@@ -102,17 +103,17 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/wired_clients/search"
     query_params={}
     if device_mac: query_params["device_mac"]=device_mac
     if mac: query_params["mac"]=mac
+    if ip: query_params["ip"]=ip
     if port_id: query_params["port_id"]=port_id
     if vlan: query_params["vlan"]=vlan
-    if ip_address: query_params["ip_address"]=ip_address
     if manufacture: query_params["manufacture"]=manufacture
     if text: query_params["text"]=text
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/wlans.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/wlans.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteWlans")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteWlans")  
 def getSiteWlans(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWlans
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -84,17 +84,47 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/wlans"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteWlanDerived")  
 def getSiteWlanDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteWlanDerived
+    API doc: https://doc.mist-lab.fr/#operation/listSiteWlanDerived
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str        
+    
+    QUERY PARAMS
+    ------------
+    resolve : bool
+      whether to resolve SITE_VARS        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/wlans/derived"
+    query_params={}
+    if resolve: query_params["resolve"]=resolve
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def listSiteWlanDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/listSiteWlanDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/wxrules.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/wxrules.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteWxRules")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteWxRules")  
 def getSiteWxRules(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWxRules
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/wxtags.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/wxtags.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteWxTags")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteWxTags")  
 def getSiteWxTags(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWxTags
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/wxtunnels.py` & `mistapi-0.42.0/src/mistapi/api/v1/sites/wxtunnels.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteWxTunnels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listSiteWxTunnels")  
 def getSiteWxTunnels(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWxTunnels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/sites/zones.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/idpprofiles.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,157 +10,157 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.41.9", details="function replaced with listSiteZones")  
-def getSiteZones(mist_session:_APISession, site_id:str) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.60.0", current_version="0.42.0", details="function replaced with listOrgIdpProfiles")  
+def getOrgIdpProfiles(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteZones
+    API doc: https://doc.mist-lab.fr/#operation/listOrgIdpProfiles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str        
+    org_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/zones"
+    uri = f"/api/v1/orgs/{org_id}/idpprofiles"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteZones(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listOrgIdpProfiles(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteZones
+    API doc: https://doc.mist-lab.fr/#operation/listOrgIdpProfiles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str        
+    org_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/zones"
+    uri = f"/api/v1/orgs/{org_id}/idpprofiles"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createSiteZone(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def createOrgIdpProfile(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createSiteZone
+    API doc: https://doc.mist-lab.fr/#operation/createOrgIdpProfile
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str        
+    org_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/zones"
+    uri = f"/api/v1/orgs/{org_id}/idpprofiles"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getSiteZone(mist_session:_APISession, site_id:str, zone_id:str) -> _APIResponse:
+def getOrgIdpProfile(mist_session:_APISession, org_id:str, idpprofile_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteZone
+    API doc: https://doc.mist-lab.fr/#operation/getOrgIdpProfile
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str
-    zone_id : str        
+    org_id : str
+    idpprofile_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
+    uri = f"/api/v1/orgs/{org_id}/idpprofiles/{idpprofile_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteSiteZone(mist_session:_APISession, site_id:str, zone_id:str) -> _APIResponse:
+def deleteOrgIdpProfile(mist_session:_APISession, org_id:str, idpprofile_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteZone
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrgIdpProfile
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str
-    zone_id : str        
+    org_id : str
+    idpprofile_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
+    uri = f"/api/v1/orgs/{org_id}/idpprofiles/{idpprofile_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateSiteZone(mist_session:_APISession, site_id:str, zone_id:str, body:object) -> _APIResponse:
+def updateOrgIdpProfile(mist_session:_APISession, org_id:str, idpprofile_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteZone
+    API doc: https://doc.mist-lab.fr/#operation/updateOrgIdpProfile
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str
-    zone_id : str        
+    org_id : str
+    idpprofile_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
+    uri = f"/api/v1/orgs/{org_id}/idpprofiles/{idpprofile_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/utils/test_telstra.py` & `mistapi-0.42.0/src/mistapi/api/v1/orgs/maps.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,26 +10,30 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def testSiteWlanTelstraSetup(mist_session:_APISession) -> _APIResponse:
+def importOrgMapsFile(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/testSiteWlanTelstraSetup
+    API doc: https://doc.mist-lab.fr/#operation/importOrgMaps
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
+    PATH PARAMS
+    -----------
+    org_id : str        
+    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/utils/test_telstra"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    multipart_form_data = {
+    }
+    uri = f"/api/v1/orgs/{org_id}/maps/import"
+    resp = mist_session.mist_post_file(uri=uri, multipart_form_data=multipart_form_data)
     return resp
-
```

### Comparing `mistapi-0.41.9/src/mistapi/api/v1/utils/test_twilio.py` & `mistapi-0.42.0/src/mistapi/api/v1/utils/test_twilio.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.41.9/src/mistapi/cli.py` & `mistapi-0.42.0/src/mistapi/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,17 @@
         msp_accounts = sorted(msp_accounts, key=lambda x: x["name"].lower())
         while True:
             i = -1
             print("\r\nAvailable MSP Accounts:")
             for privilege in msp_accounts:
                 i += 1
                 print(f"{i}) {privilege['name']} (id: {privilege['msp_id']})")
-
+            print()
+            print("n) Orgs not linked to an MSP account")
+            print()
             resp = input(
                 f'\r\nSelect the MSP Account to use (0 to {i}, "n" for None, or "q" to quit): '
             )
             if resp == "q":
                 sys.exit(0)
             elif resp.lower() == "n":
                 return [priv for priv in mist_session.privileges if not priv.get("msp_id")]
```

### Comparing `mistapi-0.41.9/src/mistapi.egg-info/PKG-INFO` & `mistapi-0.42.0/src/mistapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistapi
-Version: 0.41.9
+Version: 0.42.0
 Summary: Python package to simplify the Mist System APIs usage
 Author-email: Thomas Munzer <tmunzer@juniper.net>
 License: MIT
 Project-URL: Source, https://github.com/tmunzer/mistapi_python
 Project-URL: Bug Tracker, https://github.com/tmunzer/mistapi_python/issues
 Keywords: Mist,Juniper,API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mistapi-0.41.9/src/mistapi.egg-info/SOURCES.txt` & `mistapi-0.42.0/src/mistapi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 src/mistapi/api/__init__.py
 src/mistapi/api/v1/__init__.py
 src/mistapi/api/v1/const/__init__.py
 src/mistapi/api/v1/const/alarm_defs.py
 src/mistapi/api/v1/const/ap_channels.py
 src/mistapi/api/v1/const/ap_led_status.py
 src/mistapi/api/v1/const/applications.py
-src/mistapi/api/v1/const/call_events.py
 src/mistapi/api/v1/const/client_events.py
 src/mistapi/api/v1/const/countries.py
 src/mistapi/api/v1/const/default_gateway_config.py
 src/mistapi/api/v1/const/device_events.py
 src/mistapi/api/v1/const/device_models.py
 src/mistapi/api/v1/const/insight_metrics.py
 src/mistapi/api/v1/const/languages.py
@@ -91,14 +90,15 @@
 src/mistapi/api/v1/orgs/clone.py
 src/mistapi/api/v1/orgs/crl.py
 src/mistapi/api/v1/orgs/deviceprofiles.py
 src/mistapi/api/v1/orgs/devices.py
 src/mistapi/api/v1/orgs/evpn_topologies.py
 src/mistapi/api/v1/orgs/gatewaytemplates.py
 src/mistapi/api/v1/orgs/guests.py
+src/mistapi/api/v1/orgs/idpprofiles.py
 src/mistapi/api/v1/orgs/insights.py
 src/mistapi/api/v1/orgs/inventory.py
 src/mistapi/api/v1/orgs/invites.py
 src/mistapi/api/v1/orgs/jsi.py
 src/mistapi/api/v1/orgs/licenses.py
 src/mistapi/api/v1/orgs/logs.py
 src/mistapi/api/v1/orgs/maps.py
```

