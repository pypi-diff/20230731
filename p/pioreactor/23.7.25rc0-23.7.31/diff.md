# Comparing `tmp/pioreactor-23.7.25rc0-py3-none-any.whl.zip` & `tmp/pioreactor-23.7.31-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,85 +1,85 @@
-Zip file size: 187736 bytes, number of entries: 83
--rw-r--r--  2.0 unx      117 b- defN 23-Jul-25 18:13 pioreactor/__init__.py
--rw-r--r--  2.0 unx     6887 b- defN 23-Jul-25 18:13 pioreactor/config.py
--rw-r--r--  2.0 unx      265 b- defN 23-Jul-25 18:13 pioreactor/error_codes.py
--rw-r--r--  2.0 unx      443 b- defN 23-Jul-25 18:13 pioreactor/exc.py
--rw-r--r--  2.0 unx     3105 b- defN 23-Jul-25 18:13 pioreactor/hardware.py
--rw-r--r--  2.0 unx     6618 b- defN 23-Jul-25 18:13 pioreactor/logging.py
--rw-r--r--  2.0 unx    15510 b- defN 23-Jul-25 18:13 pioreactor/mureq.py
--rw-r--r--  2.0 unx    12950 b- defN 23-Jul-25 18:13 pioreactor/pubsub.py
--rw-r--r--  2.0 unx     6391 b- defN 23-Jul-25 18:13 pioreactor/structs.py
--rw-r--r--  2.0 unx     2724 b- defN 23-Jul-25 18:13 pioreactor/types.py
--rw-r--r--  2.0 unx     2156 b- defN 23-Jul-25 18:13 pioreactor/version.py
--rw-r--r--  2.0 unx     4458 b- defN 23-Jul-25 18:13 pioreactor/whoami.py
--rw-r--r--  2.0 unx      540 b- defN 23-Jul-25 18:13 pioreactor/actions/__init__.py
--rw-r--r--  2.0 unx     8743 b- defN 23-Jul-25 18:13 pioreactor/actions/led_intensity.py
--rw-r--r--  2.0 unx     7755 b- defN 23-Jul-25 18:13 pioreactor/actions/od_blank.py
--rw-r--r--  2.0 unx    21010 b- defN 23-Jul-25 18:13 pioreactor/actions/od_calibration.py
--rw-r--r--  2.0 unx    17612 b- defN 23-Jul-25 18:13 pioreactor/actions/pump.py
--rw-r--r--  2.0 unx    21362 b- defN 23-Jul-25 18:13 pioreactor/actions/pump_calibration.py
--rw-r--r--  2.0 unx    17031 b- defN 23-Jul-25 18:13 pioreactor/actions/self_test.py
--rw-r--r--  2.0 unx     5175 b- defN 23-Jul-25 18:13 pioreactor/actions/stirring_calibration.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-25 18:13 pioreactor/actions/leader/__init__.py
--rw-r--r--  2.0 unx     4745 b- defN 23-Jul-25 18:13 pioreactor/actions/leader/backup_database.py
--rw-r--r--  2.0 unx     8717 b- defN 23-Jul-25 18:13 pioreactor/actions/leader/experiment_profile.py
--rw-r--r--  2.0 unx     6426 b- defN 23-Jul-25 18:13 pioreactor/actions/leader/export_experiment_data.py
--rw-r--r--  2.0 unx      445 b- defN 23-Jul-25 18:13 pioreactor/automations/__init__.py
--rw-r--r--  2.0 unx      496 b- defN 23-Jul-25 18:13 pioreactor/automations/dosing/__init__.py
--rw-r--r--  2.0 unx    28429 b- defN 23-Jul-25 18:13 pioreactor/automations/dosing/base.py
--rw-r--r--  2.0 unx     1404 b- defN 23-Jul-25 18:13 pioreactor/automations/dosing/chemostat.py
--rw-r--r--  2.0 unx     1194 b- defN 23-Jul-25 18:13 pioreactor/automations/dosing/fed_batch.py
--rw-r--r--  2.0 unx     2724 b- defN 23-Jul-25 18:13 pioreactor/automations/dosing/morbidostat.py
--rw-r--r--  2.0 unx     4880 b- defN 23-Jul-25 18:13 pioreactor/automations/dosing/pid_morbidostat.py
--rw-r--r--  2.0 unx      468 b- defN 23-Jul-25 18:13 pioreactor/automations/dosing/silent.py
--rw-r--r--  2.0 unx     2252 b- defN 23-Jul-25 18:13 pioreactor/automations/dosing/turbidostat.py
--rw-r--r--  2.0 unx      510 b- defN 23-Jul-25 18:13 pioreactor/automations/events/__init__.py
--rw-r--r--  2.0 unx      473 b- defN 23-Jul-25 18:13 pioreactor/automations/led/__init__.py
--rw-r--r--  2.0 unx    11868 b- defN 23-Jul-25 18:13 pioreactor/automations/led/base.py
--rw-r--r--  2.0 unx     3875 b- defN 23-Jul-25 18:13 pioreactor/automations/led/light_dark_cycle.py
--rw-r--r--  2.0 unx      205 b- defN 23-Jul-25 18:13 pioreactor/automations/temperature/__init__.py
--rw-r--r--  2.0 unx     9722 b- defN 23-Jul-25 18:13 pioreactor/automations/temperature/base.py
--rw-r--r--  2.0 unx      674 b- defN 23-Jul-25 18:13 pioreactor/automations/temperature/constant_duty_cycle.py
--rw-r--r--  2.0 unx      517 b- defN 23-Jul-25 18:13 pioreactor/automations/temperature/only_record_temperature.py
--rw-r--r--  2.0 unx     4086 b- defN 23-Jul-25 18:13 pioreactor/automations/temperature/thermostat.py
--rw-r--r--  2.0 unx      715 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/__init__.py
--rw-r--r--  2.0 unx    43584 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/base.py
--rw-r--r--  2.0 unx     6851 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/dosing_control.py
--rw-r--r--  2.0 unx    20247 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/growth_rate_calculating.py
--rw-r--r--  2.0 unx     5485 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/led_control.py
--rw-r--r--  2.0 unx    25386 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/monitor.py
--rw-r--r--  2.0 unx    48495 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/od_reading.py
--rw-r--r--  2.0 unx    17586 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/stirring.py
--rw-r--r--  2.0 unx    24346 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/temperature_control.py
--rw-r--r--  2.0 unx      605 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/leader/__init__.py
--rw-r--r--  2.0 unx    16378 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/leader/mqtt_to_db_streaming.py
--rw-r--r--  2.0 unx     4187 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/leader/watchdog.py
--rw-r--r--  2.0 unx      609 b- defN 23-Jul-25 18:13 pioreactor/background_jobs/subjobs/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-25 18:13 pioreactor/cli/__init__.py
--rw-r--r--  2.0 unx    30358 b- defN 23-Jul-25 18:13 pioreactor/cli/pio.py
--rw-r--r--  2.0 unx    24399 b- defN 23-Jul-25 18:13 pioreactor/cli/pios.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-25 18:13 pioreactor/experiment_profiles/__init__.py
--rw-r--r--  2.0 unx     1059 b- defN 23-Jul-25 18:13 pioreactor/experiment_profiles/profile_struct.py
--rw-r--r--  2.0 unx     3716 b- defN 23-Jul-25 18:13 pioreactor/plugin_management/__init__.py
--rw-r--r--  2.0 unx     1316 b- defN 23-Jul-25 18:13 pioreactor/plugin_management/install_plugin.py
--rw-r--r--  2.0 unx     1086 b- defN 23-Jul-25 18:13 pioreactor/plugin_management/list_plugins.py
--rw-r--r--  2.0 unx     1657 b- defN 23-Jul-25 18:13 pioreactor/plugin_management/uninstall_plugin.py
--rw-r--r--  2.0 unx      792 b- defN 23-Jul-25 18:13 pioreactor/plugin_management/utils.py
--rw-r--r--  2.0 unx    10998 b- defN 23-Jul-25 18:13 pioreactor/utils/__init__.py
--rw-r--r--  2.0 unx     4096 b- defN 23-Jul-25 18:13 pioreactor/utils/adcs.py
--rw-r--r--  2.0 unx     1930 b- defN 23-Jul-25 18:13 pioreactor/utils/dacs.py
--rw-r--r--  2.0 unx      976 b- defN 23-Jul-25 18:13 pioreactor/utils/gpio_helpers.py
--rw-r--r--  2.0 unx     2847 b- defN 23-Jul-25 18:13 pioreactor/utils/math_helpers.py
--rw-r--r--  2.0 unx     4122 b- defN 23-Jul-25 18:13 pioreactor/utils/mock.py
--rw-r--r--  2.0 unx     3951 b- defN 23-Jul-25 18:13 pioreactor/utils/networking.py
--rw-r--r--  2.0 unx     7559 b- defN 23-Jul-25 18:13 pioreactor/utils/pwm.py
--rw-r--r--  2.0 unx     3393 b- defN 23-Jul-25 18:13 pioreactor/utils/rpi_bad_power.py
--rw-r--r--  2.0 unx     7749 b- defN 23-Jul-25 18:13 pioreactor/utils/sqlite_worker.py
--rw-r--r--  2.0 unx    17179 b- defN 23-Jul-25 18:13 pioreactor/utils/streaming_calculations.py
--rw-r--r--  2.0 unx     5614 b- defN 23-Jul-25 18:13 pioreactor/utils/timing.py
--rw-r--r--  2.0 unx     1079 b- defN 23-Jul-25 18:14 pioreactor-23.7.25rc0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3778 b- defN 23-Jul-25 18:14 pioreactor-23.7.25rc0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 18:14 pioreactor-23.7.25rc0.dist-info/WHEEL
--rw-r--r--  2.0 unx       79 b- defN 23-Jul-25 18:14 pioreactor-23.7.25rc0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-25 18:14 pioreactor-23.7.25rc0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     7681 b- defN 23-Jul-25 18:14 pioreactor-23.7.25rc0.dist-info/RECORD
-83 files, 616953 bytes uncompressed, 175372 bytes compressed:  71.6%
+Zip file size: 187695 bytes, number of entries: 83
+-rw-r--r--  2.0 unx      117 b- defN 23-Jul-31 16:42 pioreactor/__init__.py
+-rw-r--r--  2.0 unx     6887 b- defN 23-Jul-31 16:42 pioreactor/config.py
+-rw-r--r--  2.0 unx      265 b- defN 23-Jul-31 16:42 pioreactor/error_codes.py
+-rw-r--r--  2.0 unx      443 b- defN 23-Jul-31 16:42 pioreactor/exc.py
+-rw-r--r--  2.0 unx     3105 b- defN 23-Jul-31 16:42 pioreactor/hardware.py
+-rw-r--r--  2.0 unx     6618 b- defN 23-Jul-31 16:42 pioreactor/logging.py
+-rw-r--r--  2.0 unx    15510 b- defN 23-Jul-31 16:42 pioreactor/mureq.py
+-rw-r--r--  2.0 unx    12950 b- defN 23-Jul-31 16:42 pioreactor/pubsub.py
+-rw-r--r--  2.0 unx     6391 b- defN 23-Jul-31 16:42 pioreactor/structs.py
+-rw-r--r--  2.0 unx     2724 b- defN 23-Jul-31 16:42 pioreactor/types.py
+-rw-r--r--  2.0 unx     2153 b- defN 23-Jul-31 16:42 pioreactor/version.py
+-rw-r--r--  2.0 unx     4458 b- defN 23-Jul-31 16:42 pioreactor/whoami.py
+-rw-r--r--  2.0 unx      540 b- defN 23-Jul-31 16:42 pioreactor/actions/__init__.py
+-rw-r--r--  2.0 unx     8743 b- defN 23-Jul-31 16:42 pioreactor/actions/led_intensity.py
+-rw-r--r--  2.0 unx     7755 b- defN 23-Jul-31 16:42 pioreactor/actions/od_blank.py
+-rw-r--r--  2.0 unx    21010 b- defN 23-Jul-31 16:42 pioreactor/actions/od_calibration.py
+-rw-r--r--  2.0 unx    17612 b- defN 23-Jul-31 16:42 pioreactor/actions/pump.py
+-rw-r--r--  2.0 unx    21362 b- defN 23-Jul-31 16:42 pioreactor/actions/pump_calibration.py
+-rw-r--r--  2.0 unx    17031 b- defN 23-Jul-31 16:42 pioreactor/actions/self_test.py
+-rw-r--r--  2.0 unx     5175 b- defN 23-Jul-31 16:42 pioreactor/actions/stirring_calibration.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-31 16:42 pioreactor/actions/leader/__init__.py
+-rw-r--r--  2.0 unx     4745 b- defN 23-Jul-31 16:42 pioreactor/actions/leader/backup_database.py
+-rw-r--r--  2.0 unx     8717 b- defN 23-Jul-31 16:42 pioreactor/actions/leader/experiment_profile.py
+-rw-r--r--  2.0 unx     6426 b- defN 23-Jul-31 16:42 pioreactor/actions/leader/export_experiment_data.py
+-rw-r--r--  2.0 unx      445 b- defN 23-Jul-31 16:42 pioreactor/automations/__init__.py
+-rw-r--r--  2.0 unx      496 b- defN 23-Jul-31 16:42 pioreactor/automations/dosing/__init__.py
+-rw-r--r--  2.0 unx    28429 b- defN 23-Jul-31 16:42 pioreactor/automations/dosing/base.py
+-rw-r--r--  2.0 unx     1404 b- defN 23-Jul-31 16:42 pioreactor/automations/dosing/chemostat.py
+-rw-r--r--  2.0 unx     1194 b- defN 23-Jul-31 16:42 pioreactor/automations/dosing/fed_batch.py
+-rw-r--r--  2.0 unx     2724 b- defN 23-Jul-31 16:42 pioreactor/automations/dosing/morbidostat.py
+-rw-r--r--  2.0 unx     4880 b- defN 23-Jul-31 16:42 pioreactor/automations/dosing/pid_morbidostat.py
+-rw-r--r--  2.0 unx      468 b- defN 23-Jul-31 16:42 pioreactor/automations/dosing/silent.py
+-rw-r--r--  2.0 unx     2252 b- defN 23-Jul-31 16:42 pioreactor/automations/dosing/turbidostat.py
+-rw-r--r--  2.0 unx      510 b- defN 23-Jul-31 16:42 pioreactor/automations/events/__init__.py
+-rw-r--r--  2.0 unx      473 b- defN 23-Jul-31 16:42 pioreactor/automations/led/__init__.py
+-rw-r--r--  2.0 unx    11868 b- defN 23-Jul-31 16:42 pioreactor/automations/led/base.py
+-rw-r--r--  2.0 unx     3875 b- defN 23-Jul-31 16:42 pioreactor/automations/led/light_dark_cycle.py
+-rw-r--r--  2.0 unx      205 b- defN 23-Jul-31 16:42 pioreactor/automations/temperature/__init__.py
+-rw-r--r--  2.0 unx     9722 b- defN 23-Jul-31 16:42 pioreactor/automations/temperature/base.py
+-rw-r--r--  2.0 unx      674 b- defN 23-Jul-31 16:42 pioreactor/automations/temperature/constant_duty_cycle.py
+-rw-r--r--  2.0 unx      517 b- defN 23-Jul-31 16:42 pioreactor/automations/temperature/only_record_temperature.py
+-rw-r--r--  2.0 unx     4086 b- defN 23-Jul-31 16:42 pioreactor/automations/temperature/thermostat.py
+-rw-r--r--  2.0 unx      715 b- defN 23-Jul-31 16:42 pioreactor/background_jobs/__init__.py
+-rw-r--r--  2.0 unx    43584 b- defN 23-Jul-31 16:42 pioreactor/background_jobs/base.py
+-rw-r--r--  2.0 unx     6851 b- defN 23-Jul-31 16:42 pioreactor/background_jobs/dosing_control.py
+-rw-r--r--  2.0 unx    20247 b- defN 23-Jul-31 16:42 pioreactor/background_jobs/growth_rate_calculating.py
+-rw-r--r--  2.0 unx     5485 b- defN 23-Jul-31 16:42 pioreactor/background_jobs/led_control.py
+-rw-r--r--  2.0 unx    25386 b- defN 23-Jul-31 16:42 pioreactor/background_jobs/monitor.py
+-rw-r--r--  2.0 unx    48495 b- defN 23-Jul-31 16:42 pioreactor/background_jobs/od_reading.py
+-rw-r--r--  2.0 unx    17586 b- defN 23-Jul-31 16:42 pioreactor/background_jobs/stirring.py
+-rw-r--r--  2.0 unx    24346 b- defN 23-Jul-31 16:42 pioreactor/background_jobs/temperature_control.py
+-rw-r--r--  2.0 unx      605 b- defN 23-Jul-31 16:42 pioreactor/background_jobs/leader/__init__.py
+-rw-r--r--  2.0 unx    16378 b- defN 23-Jul-31 16:42 pioreactor/background_jobs/leader/mqtt_to_db_streaming.py
+-rw-r--r--  2.0 unx     4187 b- defN 23-Jul-31 16:42 pioreactor/background_jobs/leader/watchdog.py
+-rw-r--r--  2.0 unx      609 b- defN 23-Jul-31 16:42 pioreactor/background_jobs/subjobs/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-31 16:42 pioreactor/cli/__init__.py
+-rw-r--r--  2.0 unx    30358 b- defN 23-Jul-31 16:42 pioreactor/cli/pio.py
+-rw-r--r--  2.0 unx    24399 b- defN 23-Jul-31 16:42 pioreactor/cli/pios.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-31 16:42 pioreactor/experiment_profiles/__init__.py
+-rw-r--r--  2.0 unx     1059 b- defN 23-Jul-31 16:42 pioreactor/experiment_profiles/profile_struct.py
+-rw-r--r--  2.0 unx     3716 b- defN 23-Jul-31 16:42 pioreactor/plugin_management/__init__.py
+-rw-r--r--  2.0 unx     1316 b- defN 23-Jul-31 16:42 pioreactor/plugin_management/install_plugin.py
+-rw-r--r--  2.0 unx     1086 b- defN 23-Jul-31 16:42 pioreactor/plugin_management/list_plugins.py
+-rw-r--r--  2.0 unx     1657 b- defN 23-Jul-31 16:42 pioreactor/plugin_management/uninstall_plugin.py
+-rw-r--r--  2.0 unx      792 b- defN 23-Jul-31 16:42 pioreactor/plugin_management/utils.py
+-rw-r--r--  2.0 unx    10998 b- defN 23-Jul-31 16:42 pioreactor/utils/__init__.py
+-rw-r--r--  2.0 unx     4096 b- defN 23-Jul-31 16:42 pioreactor/utils/adcs.py
+-rw-r--r--  2.0 unx     1930 b- defN 23-Jul-31 16:42 pioreactor/utils/dacs.py
+-rw-r--r--  2.0 unx      976 b- defN 23-Jul-31 16:42 pioreactor/utils/gpio_helpers.py
+-rw-r--r--  2.0 unx     2847 b- defN 23-Jul-31 16:42 pioreactor/utils/math_helpers.py
+-rw-r--r--  2.0 unx     4122 b- defN 23-Jul-31 16:42 pioreactor/utils/mock.py
+-rw-r--r--  2.0 unx     3951 b- defN 23-Jul-31 16:42 pioreactor/utils/networking.py
+-rw-r--r--  2.0 unx     7559 b- defN 23-Jul-31 16:42 pioreactor/utils/pwm.py
+-rw-r--r--  2.0 unx     3393 b- defN 23-Jul-31 16:42 pioreactor/utils/rpi_bad_power.py
+-rw-r--r--  2.0 unx     7749 b- defN 23-Jul-31 16:42 pioreactor/utils/sqlite_worker.py
+-rw-r--r--  2.0 unx    17179 b- defN 23-Jul-31 16:42 pioreactor/utils/streaming_calculations.py
+-rw-r--r--  2.0 unx     5614 b- defN 23-Jul-31 16:42 pioreactor/utils/timing.py
+-rw-r--r--  2.0 unx     1079 b- defN 23-Jul-31 16:42 pioreactor-23.7.31.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3775 b- defN 23-Jul-31 16:42 pioreactor-23.7.31.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-31 16:42 pioreactor-23.7.31.dist-info/WHEEL
+-rw-r--r--  2.0 unx       79 b- defN 23-Jul-31 16:42 pioreactor-23.7.31.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-31 16:42 pioreactor-23.7.31.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     7663 b- defN 23-Jul-31 16:42 pioreactor-23.7.31.dist-info/RECORD
+83 files, 616929 bytes uncompressed, 175367 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -225,26 +225,26 @@
 
 Filename: pioreactor/utils/streaming_calculations.py
 Comment: 
 
 Filename: pioreactor/utils/timing.py
 Comment: 
 
-Filename: pioreactor-23.7.25rc0.dist-info/LICENSE
+Filename: pioreactor-23.7.31.dist-info/LICENSE
 Comment: 
 
-Filename: pioreactor-23.7.25rc0.dist-info/METADATA
+Filename: pioreactor-23.7.31.dist-info/METADATA
 Comment: 
 
-Filename: pioreactor-23.7.25rc0.dist-info/WHEEL
+Filename: pioreactor-23.7.31.dist-info/WHEEL
 Comment: 
 
-Filename: pioreactor-23.7.25rc0.dist-info/entry_points.txt
+Filename: pioreactor-23.7.31.dist-info/entry_points.txt
 Comment: 
 
-Filename: pioreactor-23.7.25rc0.dist-info/top_level.txt
+Filename: pioreactor-23.7.31.dist-info/top_level.txt
 Comment: 
 
-Filename: pioreactor-23.7.25rc0.dist-info/RECORD
+Filename: pioreactor-23.7.31.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pioreactor/version.py

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import os
 
 # Append "dev" if a dev version
 # Append "rc0" if a rc version
-__version__ = "23.7.25rc0"
+__version__ = "23.7.31"
 
 
 def _get_hardware_version() -> tuple[int, int] | tuple[int, int, str]:
     if os.environ.get("HARDWARE") is not None:
         # ex: > HARDWARE=1.1 pio ...
         return int(os.environ["HARDWARE"].split(".")[0]), int(os.environ["HARDWARE"].split(".")[1])
```

## Comparing `pioreactor-23.7.25rc0.dist-info/LICENSE` & `pioreactor-23.7.31.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pioreactor-23.7.25rc0.dist-info/METADATA` & `pioreactor-23.7.31.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pioreactor
-Version: 23.7.25rc0
+Version: 23.7.31
 Summary: The core Python app of the Pioreactor. Control your bioreactor through Python.
 Home-page: https://github.com/pioreactor/pioreactor
 Author: Pioreactor
 Author-email: hello@pioreactor.com
 License: MIT
 Keywords: microbiology,bioreactor,turbidostat,raspberry pi,education,research
 Classifier: Topic :: Scientific/Engineering
```

## Comparing `pioreactor-23.7.25rc0.dist-info/RECORD` & `pioreactor-23.7.31.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 pioreactor/exc.py,sha256=GvNp0vvgeAclxB2eIGZMnhYU3bFIYKz_AGOU9hKYstM,443
 pioreactor/hardware.py,sha256=c7IpkPCcsxtfvgUSpxv3TCltzCVSsIybDGzuWTn6N8g,3105
 pioreactor/logging.py,sha256=uTX088TydO4UMDgBwBI8oVenr9t24xw4ju-ZR-Pnf6U,6618
 pioreactor/mureq.py,sha256=DpE7wqRwVe8FOz_mAcAAn9-GXCiRQ6VTSvcyUhF7pUU,15510
 pioreactor/pubsub.py,sha256=kFM6M3fmG1gG6hfNv8UB1LLcm9gJLzhLSM6hBHbL9NY,12950
 pioreactor/structs.py,sha256=ShLwXOezEK_dB7Hqim9jKob3dA86BYjs8kxePfypnZo,6391
 pioreactor/types.py,sha256=l5JwLlj9YFcq1RC-IrIPsBaGwwFuNs1GAputHLwl1aI,2724
-pioreactor/version.py,sha256=CBJIGjN6CHzGdXGZx2xOpgXcjL2-EikWBs5BlwW4T5M,2156
+pioreactor/version.py,sha256=6vpTS3cTzwAJIvvRdNGB3n5RMQ8-t_RW4a_rT1VAEqw,2153
 pioreactor/whoami.py,sha256=XoXUci2kAxqNfPr8C9YaeaOQJvPkn_DP4c8HskGcKPg,4458
 pioreactor/actions/__init__.py,sha256=VuwIL8llFFqBspvBRgC9yNm-Blu9tsE2kwgIJEs786o,540
 pioreactor/actions/led_intensity.py,sha256=C705sRk7_rQsdlgmYC8YB_w3Iq30aSeJ_Bq2QHhGJAQ,8743
 pioreactor/actions/od_blank.py,sha256=-4k03BQC1i0T3rMQUicicKBufzYRC4QZD829P_XRu-Q,7755
 pioreactor/actions/od_calibration.py,sha256=WCXa3sLtI38CJHdO4y4xV-o5gQx56VwcAp8zF03mXE0,21010
 pioreactor/actions/pump.py,sha256=iVAVqzNSJKWfj1thiJMAV04SSSOV20k8bb7BA7dEOZo,17612
 pioreactor/actions/pump_calibration.py,sha256=SdnQ2AWbVNEdWtG00cxG_TtkYSNc_4RHDAxfH_cE0sM,21362
@@ -71,13 +71,13 @@
 pioreactor/utils/mock.py,sha256=V1_RqiD6gNctW-HxpCI0aDXepULIGWzD0tJUcfelONA,4122
 pioreactor/utils/networking.py,sha256=ePepmhpvP3uiVLhearQBeBe-csNjSqCzz81ylzDZ11g,3951
 pioreactor/utils/pwm.py,sha256=7KAdMF0w9YQbnI7swhZE_gfBLIkCOEYnQIrbHuoLxqo,7559
 pioreactor/utils/rpi_bad_power.py,sha256=CbtzIi9x8pvtVAX6aID8MG5YXNzkeIRFYfhri4qI-Xo,3393
 pioreactor/utils/sqlite_worker.py,sha256=69vb6s9bFdku7W7Akvb7dI0qYFW1ByhC_RECBRDwKPc,7749
 pioreactor/utils/streaming_calculations.py,sha256=QIkdiyysILvH4f6tHTzgLKbX4nkH6_oSLFLIH-zpR7k,17179
 pioreactor/utils/timing.py,sha256=Yc4pG9FB9Ix5fLT98LwuK6jQawzgMaM8AB09zPWKkTM,5614
-pioreactor-23.7.25rc0.dist-info/LICENSE,sha256=RTnFva3sXKEPtRcFEvpWgg6NqscwpXrZ0ckNz9x2tlo,1079
-pioreactor-23.7.25rc0.dist-info/METADATA,sha256=Y5JEaJ4xRmP4BHI-q2nbDncrpinfihpwoGPQmIkL6kU,3778
-pioreactor-23.7.25rc0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-pioreactor-23.7.25rc0.dist-info/entry_points.txt,sha256=1vQa-58PTH44hOQBeYFJdO3Tdfzea7_pYDxv5KQWvZ4,79
-pioreactor-23.7.25rc0.dist-info/top_level.txt,sha256=xhd14Ee_KR74whX88OzvljqlGXmfpBUHOSIqDrbs9_0,11
-pioreactor-23.7.25rc0.dist-info/RECORD,,
+pioreactor-23.7.31.dist-info/LICENSE,sha256=RTnFva3sXKEPtRcFEvpWgg6NqscwpXrZ0ckNz9x2tlo,1079
+pioreactor-23.7.31.dist-info/METADATA,sha256=dKgDlpLT6STCc1pJsl1W8bxzvy0Mvi3K_hkOEjPQTmk,3775
+pioreactor-23.7.31.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+pioreactor-23.7.31.dist-info/entry_points.txt,sha256=1vQa-58PTH44hOQBeYFJdO3Tdfzea7_pYDxv5KQWvZ4,79
+pioreactor-23.7.31.dist-info/top_level.txt,sha256=xhd14Ee_KR74whX88OzvljqlGXmfpBUHOSIqDrbs9_0,11
+pioreactor-23.7.31.dist-info/RECORD,,
```

