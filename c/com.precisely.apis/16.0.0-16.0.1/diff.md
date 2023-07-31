# Comparing `tmp/com.precisely.apis-16.0.0.tar.gz` & `tmp/com.precisely.apis-16.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.precisely.apis-16.0.0.tar", last modified: Tue May  2 10:27:06 2023, max compression
+gzip compressed data, was "com.precisely.apis-16.0.1.tar", last modified: Mon Jul 31 09:15:06 2023, max compression
```

## Comparing `com.precisely.apis-16.0.0.tar` & `com.precisely.apis-16.0.1.tar`

### file list

```diff
@@ -1,410 +1,411 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 10:27:06.765631 com.precisely.apis-16.0.0/
--rw-rw-rw-   0        0        0    11558 2023-05-02 10:12:45.000000 com.precisely.apis-16.0.0/LICENSE
--rw-rw-rw-   0        0        0      451 2023-05-02 10:27:06.766631 com.precisely.apis-16.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    49358 2023-05-02 10:24:46.000000 com.precisely.apis-16.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 10:27:05.981965 com.precisely.apis-16.0.0/com/
--rw-rw-rw-   0        0        0        0 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 10:27:06.022633 com.precisely.apis-16.0.0/com/precisely/
--rw-rw-rw-   0        0        0        0 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 10:27:06.031631 com.precisely.apis-16.0.0/com/precisely/apis/
--rw-rw-rw-   0        0        0      828 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 10:27:06.102631 com.precisely.apis-16.0.0/com/precisely/apis/api/
--rw-rw-rw-   0        0        0      251 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/api/__init__.py
--rw-rw-rw-   0        0        0    16087 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/api/address_autocomplete_enterprise_service_api.py
--rw-rw-rw-   0        0        0    10596 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/api/address_autocomplete_service_api.py
--rw-rw-rw-   0        0        0    30342 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/api/address_verification_service_api.py
--rw-rw-rw-   0        0        0    23486 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/api/addresses_service__api.py
--rw-rw-rw-   0        0        0    43156 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/api/demographics_service_api.py
--rw-rw-rw-   0        0        0     5850 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/api/email_verification_service_api.py
--rw-rw-rw-   0        0        0    47771 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/api/geocode_service_api.py
--rw-rw-rw-   0        0        0    11824 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/api/geolocation_service_api.py
--rw-rw-rw-   0        0        0    53765 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/api/local_tax_service_api.py
--rw-rw-rw-   0        0        0     6043 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/api/neighborhoods_service__api.py
--rw-rw-rw-   0        0        0     5902 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/api/phone_verification_service_api.py
--rw-rw-rw-   0        0        0    66565 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/api/places_service__api.py
--rw-rw-rw-   0        0        0    11086 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/api/property_information_service_api.py
--rw-rw-rw-   0        0        0    20787 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/api/psap_911_service_api.py
--rw-rw-rw-   0        0        0   130591 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/api/risks_service_api.py
--rw-rw-rw-   0        0        0    57552 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/api/routing_service_api.py
--rw-rw-rw-   0        0        0    10365 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/api/schools_service_api.py
--rw-rw-rw-   0        0        0    19115 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/api/streets_service_api.py
--rw-rw-rw-   0        0        0    11525 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/api/telecomm_info_service_api.py
--rw-rw-rw-   0        0        0    21579 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/api/time_zone_service_api.py
--rw-rw-rw-   0        0        0    54012 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/api/zones_service_api.py
--rw-rw-rw-   0        0        0    38586 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/api_client.py
-drwxrwxrwx   0        0        0        0 2023-05-02 10:27:06.103630 com.precisely.apis-16.0.0/com/precisely/apis/apis/
--rw-rw-rw-   0        0        0     2215 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/apis/__init__.py
--rw-rw-rw-   0        0        0    16559 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/configuration.py
--rw-rw-rw-   0        0        0     5117 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-02 10:27:06.763634 com.precisely.apis-16.0.0/com/precisely/apis/model/
--rw-rw-rw-   0        0        0      348 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/__init__.py
--rw-rw-rw-   0        0        0    11256 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/absentee_owner.py
--rw-rw-rw-   0        0        0    11241 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/accuracy.py
--rw-rw-rw-   0        0        0    17255 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/address.py
--rw-rw-rw-   0        0        0    11453 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/address_time.py
--rw-rw-rw-   0        0        0    11285 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/address_type.py
--rw-rw-rw-   0        0        0    13513 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/addresses_by_boundary_request.py
--rw-rw-rw-   0        0        0    11159 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/addresses_count.py
--rw-rw-rw-   0        0        0    14966 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/addresses_dto.py
--rw-rw-rw-   0        0        0    11321 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/addresses_preferences.py
--rw-rw-rw-   0        0        0    11720 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/addresses_response.py
--rw-rw-rw-   0        0        0    17285 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/ah_jmailing_address.py
--rw-rw-rw-   0        0        0    13338 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/ahj.py
--rw-rw-rw-   0        0        0    11201 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/ahj_list.py
--rw-rw-rw-   0        0        0    11761 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/ahj_plus_psap_response.py
--rw-rw-rw-   0        0        0    11244 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/amenities.py
--rw-rw-rw-   0        0        0    11229 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/area.py
--rw-rw-rw-   0        0        0    12644 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/area_code_info.py
--rw-rw-rw-   0        0        0    12082 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/assets_and_wealth_theme.py
--rw-rw-rw-   0        0        0    11271 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/base_flood_elevation.py
--rw-rw-rw-   0        0        0    11253 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/basement_type.py
--rw-rw-rw-   0        0        0    12377 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/basic_boundary.py
--rw-rw-rw-   0        0        0    11770 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/boundaries.py
--rw-rw-rw-   0        0        0    12162 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/boundary.py
--rw-rw-rw-   0        0        0    11763 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/boundary_buffer.py
--rw-rw-rw-   0        0        0    11298 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/boundary_point.py
--rw-rw-rw-   0        0        0    11294 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/buffer_relation.py
--rw-rw-rw-   0        0        0    11250 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/buildg_class.py
--rw-rw-rw-   0        0        0    11262 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/buildg_condition.py
--rw-rw-rw-   0        0        0    11595 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/buildg_features_sqft.py
--rw-rw-rw-   0        0        0    11564 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/buildg_improve_area.py
--rw-rw-rw-   0        0        0    11268 2023-05-02 08:13:02.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/buildg_improve_type.py
--rw-rw-rw-   0        0        0    11256 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/buildg_quality.py
--rw-rw-rw-   0        0        0    11250 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/buildg_style.py
--rw-rw-rw-   0        0        0    11247 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/buildg_type.py
--rw-rw-rw-   0        0        0    11247 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/buildg_view.py
--rw-rw-rw-   0        0        0    11271 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/building_sqft_source.py
--rw-rw-rw-   0        0        0    11247 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/business_id.py
--rw-rw-rw-   0        0        0    11253 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/ca_exemptions.py
--rw-rw-rw-   0        0        0    13761 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/candidate.py
--rw-rw-rw-   0        0        0    13101 2023-05-02 10:22:26.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/candidate_range.py
--rw-rw-rw-   0        0        0    12226 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/candidate_range_unit.py
--rw-rw-rw-   0        0        0    11233 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/carrier.py
--rw-rw-rw-   0        0        0    11930 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/category.py
--rw-rw-rw-   0        0        0    12296 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/category_metadata.py
--rw-rw-rw-   0        0        0    11224 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/cbsa.py
--rw-rw-rw-   0        0        0    12050 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/census.py
--rw-rw-rw-   0        0        0    11277 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/center.py
--rw-rw-rw-   0        0        0    11259 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/city.py
--rw-rw-rw-   0        0        0    11893 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/common_geometry.py
--rw-rw-rw-   0        0        0    11420 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/community.py
--rw-rw-rw-   0        0        0    11297 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/consistency_code.py
--rw-rw-rw-   0        0        0    11253 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/construction.py
--rw-rw-rw-   0        0        0    12222 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/contact_details.py
--rw-rw-rw-   0        0        0    12861 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/contact_person.py
--rw-rw-rw-   0        0        0    11250 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/cooling_type.py
--rw-rw-rw-   0        0        0    11691 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/cost.py
--rw-rw-rw-   0        0        0    11230 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/county.py
--rw-rw-rw-   0        0        0    11464 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/coverage.py
--rw-rw-rw-   0        0        0    11830 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/crime_boundary.py
--rw-rw-rw-   0        0        0    11750 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/crime_index_theme.py
--rw-rw-rw-   0        0        0    11834 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/crime_risk_by_address_batch_request.py
--rw-rw-rw-   0        0        0    11851 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/crime_risk_by_location_batch_request.py
--rw-rw-rw-   0        0        0    11331 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/crime_risk_preferences.py
--rw-rw-rw-   0        0        0    12263 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/crime_risk_response.py
--rw-rw-rw-   0        0        0    11372 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/crime_risk_response_list.py
--rw-rw-rw-   0        0        0    11530 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/crs.py
--rw-rw-rw-   0        0        0    12065 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/demographics.py
--rw-rw-rw-   0        0        0    11567 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/demographics_advanced_preferences.py
--rw-rw-rw-   0        0        0    12118 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/demographics_advanced_request.py
--rw-rw-rw-   0        0        0    11960 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/demographics_geometry.py
--rw-rw-rw-   0        0        0    11557 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/demographics_geometry_crc.py
--rw-rw-rw-   0        0        0    15660 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/demographics_themes_v2.py
--rw-rw-rw-   0        0        0    11232 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/depth.py
--rw-rw-rw-   0        0        0    11328 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/direction_geometry.py
--rw-rw-rw-   0        0        0    11241 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/distance.py
--rw-rw-rw-   0        0        0    11265 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/distance_to_border.py
--rw-rw-rw-   0        0        0    11863 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/distance_to_flood_hazard_address_request.py
--rw-rw-rw-   0        0        0    11880 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/distance_to_flood_hazard_location_request.py
--rw-rw-rw-   0        0        0    11406 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/distance_to_flood_hazard_response.py
--rw-rw-rw-   0        0        0    11288 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/district_type.py
--rw-rw-rw-   0        0        0    11635 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/domestic_ultimate_business.py
--rw-rw-rw-   0        0        0    11266 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/earthquake_date_time.py
--rw-rw-rw-   0        0        0    13648 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/earthquake_event.py
--rw-rw-rw-   0        0        0    11621 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/earthquake_events_response.py
--rw-rw-rw-   0        0        0    11981 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/earthquake_history.py
--rw-rw-rw-   0        0        0    11313 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/earthquake_location.py
--rw-rw-rw-   0        0        0    11798 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/earthquake_risk_by_address_request.py
--rw-rw-rw-   0        0        0    11815 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/earthquake_risk_by_location_request.py
--rw-rw-rw-   0        0        0    12371 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/earthquake_risk_response.py
--rw-rw-rw-   0        0        0    11447 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/earthquake_risk_response_list.py
--rw-rw-rw-   0        0        0    12064 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/education_theme.py
--rw-rw-rw-   0        0        0    11358 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/employee_count.py
--rw-rw-rw-   0        0        0    12067 2023-05-02 08:13:03.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/employment_theme.py
--rw-rw-rw-   0        0        0    11247 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/energy_type.py
--rw-rw-rw-   0        0        0    11332 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/error_code.py
--rw-rw-rw-   0        0        0    11260 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/error_info.py
--rw-rw-rw-   0        0        0    13880 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/events_count.py
--rw-rw-rw-   0        0        0    12070 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/expenditure_theme.py
--rw-rw-rw-   0        0        0    11256 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/exterior_walls.py
--rw-rw-rw-   0        0        0    11589 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/extra_feature_sqft.py
--rw-rw-rw-   0        0        0    11445 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/field.py
--rw-rw-rw-   0        0        0    14301 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/fields_matching.py
--rw-rw-rw-   0        0        0    12318 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/fire_department.py
--rw-rw-rw-   0        0        0    12050 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/fire_event.py
--rw-rw-rw-   0        0        0    11282 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/fire_events_response.py
--rw-rw-rw-   0        0        0    11733 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/fire_history.py
--rw-rw-rw-   0        0        0    11780 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/fire_risk_by_address_request.py
--rw-rw-rw-   0        0        0    11797 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/fire_risk_by_location_request.py
--rw-rw-rw-   0        0        0    12122 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/fire_risk_response.py
--rw-rw-rw-   0        0        0    11357 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/fire_risk_response_list.py
--rw-rw-rw-   0        0        0    11725 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/fire_shed.py
--rw-rw-rw-   0        0        0    13259 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/fire_station.py
--rw-rw-rw-   0        0        0    11677 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/fire_station_contact_details.py
--rw-rw-rw-   0        0        0    11677 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/fire_stations.py
--rw-rw-rw-   0        0        0    11256 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/fireplace_type.py
--rw-rw-rw-   0        0        0    11868 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/flood_hazard_preferences.py
--rw-rw-rw-   0        0        0    11819 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/flood_risk_by_address_request.py
--rw-rw-rw-   0        0        0    11836 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/flood_risk_by_location_request.py
--rw-rw-rw-   0        0        0    11616 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/flood_risk_preferences.py
--rw-rw-rw-   0        0        0    12803 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/flood_risk_response.py
--rw-rw-rw-   0        0        0    11372 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/flood_risk_response_list.py
--rw-rw-rw-   0        0        0    12555 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/flood_zone.py
--rw-rw-rw-   0        0        0    11244 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/floor_type.py
--rw-rw-rw-   0        0        0    13506 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/formatted_tax_address.py
--rw-rw-rw-   0        0        0    11247 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/foundation.py
--rw-rw-rw-   0        0        0    11679 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/free_or_reduced_price_lunches.py
--rw-rw-rw-   0        0        0    11241 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/fuel_type.py
--rw-rw-rw-   0        0        0    11247 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/garage_type.py
--rw-rw-rw-   0        0        0    11682 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/geo_location_access_point.py
--rw-rw-rw-   0        0        0    11479 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/geo_location_country.py
--rw-rw-rw-   0        0        0    11957 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/geo_location_ip_addr.py
--rw-rw-rw-   0        0        0    13204 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/geo_location_place.py
--rw-rw-rw-   0        0        0    11295 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/geo_location_state.py
--rw-rw-rw-   0        0        0    11638 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/geo_pos.py
--rw-rw-rw-   0        0        0    14446 2023-05-02 10:21:44.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/geocode_address.py
--rw-rw-rw-   0        0        0    18616 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/geocode_preferences.py
--rw-rw-rw-   0        0        0    11970 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/geocode_request.py
--rw-rw-rw-   0        0        0    12023 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/geocode_service_response.py
--rw-rw-rw-   0        0        0    11418 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/geocode_service_response_list.py
--rw-rw-rw-   0        0        0    11316 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/geolocation_geometry.py
--rw-rw-rw-   0        0        0    11283 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/geometry.py
--rw-rw-rw-   0        0        0    11521 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/geometry_crc.py
--rw-rw-rw-   0        0        0    11088 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/geometry_properties.py
--rw-rw-rw-   0        0        0    11461 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/get_city_state_province_api_input.py
--rw-rw-rw-   0        0        0    11984 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/get_city_state_province_api_input_row.py
--rw-rw-rw-   0        0        0    12600 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/get_city_state_province_api_options.py
--rw-rw-rw-   0        0        0    13593 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/get_city_state_province_api_output.py
--rw-rw-rw-   0        0        0    11912 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/get_city_state_province_api_request.py
--rw-rw-rw-   0        0        0    11470 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/get_city_state_province_api_response.py
--rw-rw-rw-   0        0        0    11400 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/get_postal_codes_api_input.py
--rw-rw-rw-   0        0        0    12159 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/get_postal_codes_api_input_row.py
--rw-rw-rw-   0        0        0    11710 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/get_postal_codes_api_options.py
--rw-rw-rw-   0        0        0    13110 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/get_postal_codes_api_output.py
--rw-rw-rw-   0        0        0    11316 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/get_postal_codes_api_output_user_fields.py
--rw-rw-rw-   0        0        0    11808 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/get_postal_codes_api_request.py
--rw-rw-rw-   0        0        0    11409 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/get_postal_codes_api_response.py
--rw-rw-rw-   0        0        0    11629 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/global_ultimate_business.py
--rw-rw-rw-   0        0        0    13489 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/grade_levels_taught.py
--rw-rw-rw-   0        0        0    11435 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/greatschools.py
--rw-rw-rw-   0        0        0    11462 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/grid.py
--rw-rw-rw-   0        0        0    12055 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/health_theme.py
--rw-rw-rw-   0        0        0    11250 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/heating_type.py
--rw-rw-rw-   0        0        0    12067 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/households_theme.py
--rw-rw-rw-   0        0        0    12058 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/housing_theme.py
--rw-rw-rw-   0        0        0    12055 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/income_theme.py
--rw-rw-rw-   0        0        0    11874 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/index_variable.py
--rw-rw-rw-   0        0        0    11677 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/individual_value_variable.py
--rw-rw-rw-   0        0        0    11253 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/interior_wall.py
--rw-rw-rw-   0        0        0    11319 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/intermediate_points.py
--rw-rw-rw-   0        0        0    12291 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/intersection.py
--rw-rw-rw-   0        0        0    11679 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/intersection_response.py
--rw-rw-rw-   0        0        0    12067 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/ip_info.py
--rw-rw-rw-   0        0        0    13054 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/ipd.py
--rw-rw-rw-   0        0        0    11890 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/ipd_tax_by_address_batch_request.py
--rw-rw-rw-   0        0        0    11871 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/ipd_tax_jurisdiction.py
--rw-rw-rw-   0        0        0    11808 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/key_lookup_request.py
--rw-rw-rw-   0        0        0    11446 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/keys.py
--rw-rw-rw-   0        0        0    11238 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/land_use.py
--rw-rw-rw-   0        0        0    12232 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/lat_long_fields.py
--rw-rw-rw-   0        0        0    12064 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/life_style_theme.py
--rw-rw-rw-   0        0        0    11238 2023-05-02 08:13:04.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/loc_code.py
--rw-rw-rw-   0        0        0    11343 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/local_tax_geometry.py
--rw-rw-rw-   0        0        0    14407 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/local_tax_preferences.py
--rw-rw-rw-   0        0        0    11217 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/location.py
--rw-rw-rw-   0        0        0    12025 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/location_time.py
--rw-rw-rw-   0        0        0    12175 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/magnitude.py
--rw-rw-rw-   0        0        0    11972 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/match.py
--rw-rw-rw-   0        0        0    17276 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/matched_address.py
--rw-rw-rw-   0        0        0    12342 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/matrix.py
--rw-rw-rw-   0        0        0    11221 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/mcd.py
--rw-rw-rw-   0        0        0    11652 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/metadata_response.py
--rw-rw-rw-   0        0        0    11474 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/name.py
--rw-rw-rw-   0        0        0    11298 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/neighborhoods_response.py
--rw-rw-rw-   0        0        0    13019 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/network.py
--rw-rw-rw-   0        0        0    11496 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/organization_type.py
--rw-rw-rw-   0        0        0    11247 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/other_rooms.py
--rw-rw-rw-   0        0        0    11256 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/owner_vest_type.py
--rw-rw-rw-   0        0        0    11899 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/owners.py
--rw-rw-rw-   0        0        0    11605 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/parent_business.py
--rw-rw-rw-   0        0        0    11412 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/pb_key_address_request.py
--rw-rw-rw-   0        0        0    11468 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/pb_key_response.py
--rw-rw-rw-   0        0        0    11250 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/pb_key_response_list.py
--rw-rw-rw-   0        0        0    11646 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/pbkey.py
--rw-rw-rw-   0        0        0    11383 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/phone_verification.py
--rw-rw-rw-   0        0        0    12826 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/phone_verification_output.py
--rw-rw-rw-   0        0        0    11592 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/place.py
--rw-rw-rw-   0        0        0    12220 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/places_response.py
--rw-rw-rw-   0        0        0    20808 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/poi.py
--rw-rw-rw-   0        0        0    12870 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/poi_boundary.py
--rw-rw-rw-   0        0        0    11840 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/poi_boundary_address_request.py
--rw-rw-rw-   0        0        0    11900 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/poi_boundary_location_request.py
--rw-rw-rw-   0        0        0    11825 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/poi_boundary_locations.py
--rw-rw-rw-   0        0        0    11548 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/poi_boundary_preferences.py
--rw-rw-rw-   0        0        0    11333 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/poi_boundary_response.py
--rw-rw-rw-   0        0        0    11800 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/poi_classification.py
--rw-rw-rw-   0        0        0    11116 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/poi_count.py
--rw-rw-rw-   0        0        0    12954 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/poi_count_request.py
--rw-rw-rw-   0        0        0    13374 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/poiby_geometry_request.py
--rw-rw-rw-   0        0        0    11725 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/points.py
--rw-rw-rw-   0        0        0    11241 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/pool_type.py
--rw-rw-rw-   0        0        0    12067 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/population_theme.py
--rw-rw-rw-   0        0        0    11114 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/preferenc_time_zone.py
--rw-rw-rw-   0        0        0    11280 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/primary_zone.py
--rw-rw-rw-   0        0        0    11256 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/prior_sale_code.py
--rw-rw-rw-   0        0        0    11265 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/prop_site_influene.py
--rw-rw-rw-   0        0        0    11106 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/properties.py
--rw-rw-rw-   0        0        0    46206 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/property_attributes.py
--rw-rw-rw-   0        0        0    11349 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/property_geometry.py
--rw-rw-rw-   0        0        0    11918 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/property_info_address_request.py
--rw-rw-rw-   0        0        0    11133 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/property_info_preferences.py
--rw-rw-rw-   0        0        0    12002 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/property_info_response.py
--rw-rw-rw-   0        0        0    11457 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/property_info_responses.py
--rw-rw-rw-   0        0        0    11696 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/proxy.py
--rw-rw-rw-   0        0        0    13793 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/psap_response.py
--rw-rw-rw-   0        0        0    12085 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/race_and_ethnicity_theme.py
--rw-rw-rw-   0        0        0    12626 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/range_variable.py
--rw-rw-rw-   0        0        0    11664 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/rate.py
--rw-rw-rw-   0        0        0    13755 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/rate_center_response.py
--rw-rw-rw-   0        0        0    12337 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/return_fields_descriptor.py
--rw-rw-rw-   0        0        0    11723 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/reverse_geocode_request.py
--rw-rw-rw-   0        0        0    14978 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/risk.py
--rw-rw-rw-   0        0        0    17267 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/risk_address.py
--rw-rw-rw-   0        0        0    11337 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/risk_geometry.py
--rw-rw-rw-   0        0        0    11797 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/risk_locations.py
--rw-rw-rw-   0        0        0    11601 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/risk_preferences.py
--rw-rw-rw-   0        0        0    11316 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/risks_boundaries.py
--rw-rw-rw-   0        0        0    11368 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/risks_crime_theme.py
--rw-rw-rw-   0        0        0    11536 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/risks_geometry_crc.py
--rw-rw-rw-   0        0        0    13324 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/road.py
--rw-rw-rw-   0        0        0    11256 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/roof_cover_type.py
--rw-rw-rw-   0        0        0    11256 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/roof_frame_type.py
--rw-rw-rw-   0        0        0    11256 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/roof_shape_type.py
--rw-rw-rw-   0        0        0    12381 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/route_direction.py
--rw-rw-rw-   0        0        0    11304 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/route_geometry.py
--rw-rw-rw-   0        0        0    13382 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/route_response.py
--rw-rw-rw-   0        0        0    13904 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/sales_tax.py
--rw-rw-rw-   0        0        0    11569 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/sales_volume.py
--rw-rw-rw-   0        0        0    19109 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/school.py
--rw-rw-rw-   0        0        0    12879 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/school_district.py
--rw-rw-rw-   0        0        0    13410 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/school_profile.py
--rw-rw-rw-   0        0        0    12471 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/school_ranking.py
--rw-rw-rw-   0        0        0    11996 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/schools_near_by_response.py
--rw-rw-rw-   0        0        0    11761 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/segmentation.py
--rw-rw-rw-   0        0        0    11365 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/segmentation_themes.py
--rw-rw-rw-   0        0        0    11268 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/shore_line_distance.py
--rw-rw-rw-   0        0        0    12022 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/sic.py
--rw-rw-rw-   0        0        0    12330 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/sic_metadata.py
--rw-rw-rw-   0        0        0    12078 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/site_details.py
--rw-rw-rw-   0        0        0    13485 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/situs_address.py
--rw-rw-rw-   0        0        0    12476 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/special_purpose_district.py
--rw-rw-rw-   0        0        0    11579 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/special_purpose_district_tax.py
--rw-rw-rw-   0        0        0    13049 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/speed_limit.py
--rw-rw-rw-   0        0        0    11298 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/start_end_point.py
--rw-rw-rw-   0        0        0    11227 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/state.py
--rw-rw-rw-   0        0        0    11265 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/status.py
--rw-rw-rw-   0        0        0    11273 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/stories.py
--rw-rw-rw-   0        0        0    12424 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/student_ethnicity.py
--rw-rw-rw-   0        0        0    12082 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/supply_and_demand_theme.py
--rw-rw-rw-   0        0        0    18388 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/tax_address.py
--rw-rw-rw-   0        0        0    11824 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/tax_address_request.py
--rw-rw-rw-   0        0        0    11239 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/tax_county.py
--rw-rw-rw-   0        0        0    13607 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/tax_district_response.py
--rw-rw-rw-   0        0        0    11446 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/tax_district_response_list.py
--rw-rw-rw-   0        0        0    11247 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/tax_doc_type.py
--rw-rw-rw-   0        0        0    11253 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/tax_exemption.py
--rw-rw-rw-   0        0        0    11334 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/tax_geometry.py
--rw-rw-rw-   0        0        0    12257 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/tax_jurisdiction.py
--rw-rw-rw-   0        0        0    11798 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/tax_location_request.py
--rw-rw-rw-   0        0        0    11787 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/tax_locations.py
--rw-rw-rw-   0        0        0    12845 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/tax_place.py
--rw-rw-rw-   0        0        0    18168 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/tax_rate_address.py
--rw-rw-rw-   0        0        0    11919 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/tax_rate_address_request.py
--rw-rw-rw-   0        0        0    11810 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/tax_rate_location_request.py
--rw-rw-rw-   0        0        0    17504 2023-05-02 08:13:05.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/tax_rate_matched_address.py
--rw-rw-rw-   0        0        0    14126 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/tax_rate_response.py
--rw-rw-rw-   0        0        0    11346 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/tax_responses.py
--rw-rw-rw-   0        0        0    11268 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/tax_sales_price_code.py
--rw-rw-rw-   0        0        0    11236 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/tax_state.py
--rw-rw-rw-   0        0        0    11229 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/time.py
--rw-rw-rw-   0        0        0    11731 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/timezone_address_request.py
--rw-rw-rw-   0        0        0    11349 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/timezone_geometry.py
--rw-rw-rw-   0        0        0    11357 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/timezone_location_request.py
--rw-rw-rw-   0        0        0    15245 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/timezone_response.py
--rw-rw-rw-   0        0        0    11352 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/timezone_response_list.py
--rw-rw-rw-   0        0        0    11354 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/travel_boundaries.py
--rw-rw-rw-   0        0        0    11234 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/travel_boundary.py
--rw-rw-rw-   0        0        0    11283 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/travel_cost_matrix_response.py
--rw-rw-rw-   0        0        0    11229 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/type.py
--rw-rw-rw-   0        0        0    13867 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/typeahead_location.py
--rw-rw-rw-   0        0        0    11353 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/typeahead_locations.py
--rw-rw-rw-   0        0        0    11505 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/typeahead_range.py
--rw-rw-rw-   0        0        0    11363 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/typeahead_unit.py
--rw-rw-rw-   0        0        0    11235 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/unit.py
--rw-rw-rw-   0        0        0    13898 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/use_tax.py
--rw-rw-rw-   0        0        0    11238 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/vacancy.py
--rw-rw-rw-   0        0        0    11817 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_email_address_api_request.py
--rw-rw-rw-   0        0        0    11447 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_email_address_api_response.py
--rw-rw-rw-   0        0        0    11429 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_email_address_input.py
--rw-rw-rw-   0        0        0    16658 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_email_address_input_row.py
--rw-rw-rw-   0        0        0    15324 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_email_address_output.py
--rw-rw-rw-   0        0        0    11449 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_input.py
--rw-rw-rw-   0        0        0    13503 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_input_row.py
--rw-rw-rw-   0        0        0    11357 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_options.py
--rw-rw-rw-   0        0        0    15940 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_output.py
--rw-rw-rw-   0        0        0    11520 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_premium_input.py
--rw-rw-rw-   0        0        0    14342 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_premium_input_row.py
--rw-rw-rw-   0        0        0    15105 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_premium_options.py
--rw-rw-rw-   0        0        0    39660 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_premium_output.py
--rw-rw-rw-   0        0        0    12012 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_premium_request.py
--rw-rw-rw-   0        0        0    11529 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_premium_response.py
--rw-rw-rw-   0        0        0    11480 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_pro_input.py
--rw-rw-rw-   0        0        0    13512 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_pro_input_row.py
--rw-rw-rw-   0        0        0    14100 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_pro_options.py
--rw-rw-rw-   0        0        0    18611 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_pro_output.py
--rw-rw-rw-   0        0        0    11944 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_pro_request.py
--rw-rw-rw-   0        0        0    11489 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_pro_response.py
--rw-rw-rw-   0        0        0    11891 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_request.py
--rw-rw-rw-   0        0        0    11458 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_response.py
--rw-rw-rw-   0        0        0    11530 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_input.py
--rw-rw-rw-   0        0        0    14701 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_input_row.py
--rw-rw-rw-   0        0        0    36257 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_options.py
--rw-rw-rw-   0        0        0    49413 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_output.py
--rw-rw-rw-   0        0        0    12029 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_request.py
--rw-rw-rw-   0        0        0    11539 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_response.py
--rw-rw-rw-   0        0        0    11488 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_phone_number_api_request.py
--rw-rw-rw-   0        0        0    11521 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_phone_number_api_request_input.py
--rw-rw-rw-   0        0        0    11377 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/validate_phone_number_api_request_input_row.py
--rw-rw-rw-   0        0        0    11760 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/water_body.py
--rw-rw-rw-   0        0        0    11870 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/water_body_response.py
--rw-rw-rw-   0        0        0    17270 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/zones_address.py
--rw-rw-rw-   0        0        0    11334 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/zones_boundary_geometry.py
--rw-rw-rw-   0        0        0    11574 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/zones_contact_details.py
--rw-rw-rw-   0        0        0    11340 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/zones_geometry.py
--rw-rw-rw-   0        0        0    11091 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/zones_parent_business.py
--rw-rw-rw-   0        0        0    14879 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/zones_poi.py
--rw-rw-rw-   0        0        0    11851 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/zones_poi_classification.py
--rw-rw-rw-   0        0        0    11863 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/zones_poi_geometry.py
--rw-rw-rw-   0        0        0    11791 2023-05-02 08:13:06.000000 com.precisely.apis-16.0.0/com/precisely/apis/model/zones_sic.py
--rw-rw-rw-   0        0        0    81943 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/model_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 10:27:06.764631 com.precisely.apis-16.0.0/com/precisely/apis/models/
--rw-rw-rw-   0        0        0    26774 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/models/__init__.py
--rw-rw-rw-   0        0        0    14245 2023-05-02 08:13:07.000000 com.precisely.apis-16.0.0/com/precisely/apis/rest.py
-drwxrwxrwx   0        0        0        0 2023-05-02 10:27:06.020630 com.precisely.apis-16.0.0/com.precisely.apis.egg-info/
--rw-rw-rw-   0        0        0      451 2023-05-02 10:27:05.000000 com.precisely.apis-16.0.0/com.precisely.apis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    18612 2023-05-02 10:27:05.000000 com.precisely.apis-16.0.0/com.precisely.apis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 10:27:05.000000 com.precisely.apis-16.0.0/com.precisely.apis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-02 10:27:05.000000 com.precisely.apis-16.0.0/com.precisely.apis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-02 10:27:05.000000 com.precisely.apis-16.0.0/com.precisely.apis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       76 2023-05-02 10:27:06.767630 com.precisely.apis-16.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-05-02 10:19:59.000000 com.precisely.apis-16.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:15:06.338000 com.precisely.apis-16.0.1/
+-rw-rw-rw-   0        0        0    11558 2023-05-02 10:12:45.000000 com.precisely.apis-16.0.1/LICENSE
+-rw-rw-rw-   0        0        0      451 2023-07-31 09:15:06.338000 com.precisely.apis-16.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    49391 2023-07-31 09:13:13.000000 com.precisely.apis-16.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 09:15:05.519645 com.precisely.apis-16.0.1/com/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:15:05.549001 com.precisely.apis-16.0.1/com/precisely/
+-rw-rw-rw-   0        0        0        0 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/precisely/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:15:05.581002 com.precisely.apis-16.0.1/com/precisely/apis/
+-rw-rw-rw-   0        0        0      828 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/precisely/apis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:15:05.628002 com.precisely.apis-16.0.1/com/precisely/apis/api/
+-rw-rw-rw-   0        0        0      251 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/precisely/apis/api/__init__.py
+-rw-rw-rw-   0        0        0    16087 2023-07-31 07:09:12.000000 com.precisely.apis-16.0.1/com/precisely/apis/api/address_autocomplete_enterprise_service_api.py
+-rw-rw-rw-   0        0        0    10596 2023-07-31 07:09:12.000000 com.precisely.apis-16.0.1/com/precisely/apis/api/address_autocomplete_service_api.py
+-rw-rw-rw-   0        0        0    30342 2023-07-31 07:09:12.000000 com.precisely.apis-16.0.1/com/precisely/apis/api/address_verification_service_api.py
+-rw-rw-rw-   0        0        0    23486 2023-07-31 07:09:12.000000 com.precisely.apis-16.0.1/com/precisely/apis/api/addresses_service__api.py
+-rw-rw-rw-   0        0        0    43156 2023-07-31 07:09:12.000000 com.precisely.apis-16.0.1/com/precisely/apis/api/demographics_service_api.py
+-rw-rw-rw-   0        0        0     5850 2023-07-31 07:09:12.000000 com.precisely.apis-16.0.1/com/precisely/apis/api/email_verification_service_api.py
+-rw-rw-rw-   0        0        0    47771 2023-07-31 07:09:12.000000 com.precisely.apis-16.0.1/com/precisely/apis/api/geocode_service_api.py
+-rw-rw-rw-   0        0        0    11824 2023-07-31 07:09:12.000000 com.precisely.apis-16.0.1/com/precisely/apis/api/geolocation_service_api.py
+-rw-rw-rw-   0        0        0    53765 2023-07-31 07:09:12.000000 com.precisely.apis-16.0.1/com/precisely/apis/api/local_tax_service_api.py
+-rw-rw-rw-   0        0        0     6043 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/precisely/apis/api/neighborhoods_service__api.py
+-rw-rw-rw-   0        0        0     5902 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/precisely/apis/api/phone_verification_service_api.py
+-rw-rw-rw-   0        0        0    66565 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/precisely/apis/api/places_service__api.py
+-rw-rw-rw-   0        0        0    11086 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/precisely/apis/api/property_information_service_api.py
+-rw-rw-rw-   0        0        0    20787 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/precisely/apis/api/psap_911_service_api.py
+-rw-rw-rw-   0        0        0   130591 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/precisely/apis/api/risks_service_api.py
+-rw-rw-rw-   0        0        0    57552 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/precisely/apis/api/routing_service_api.py
+-rw-rw-rw-   0        0        0    10365 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/precisely/apis/api/schools_service_api.py
+-rw-rw-rw-   0        0        0    19115 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/precisely/apis/api/streets_service_api.py
+-rw-rw-rw-   0        0        0    11525 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/precisely/apis/api/telecomm_info_service_api.py
+-rw-rw-rw-   0        0        0    21579 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/precisely/apis/api/time_zone_service_api.py
+-rw-rw-rw-   0        0        0    54012 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/precisely/apis/api/zones_service_api.py
+-rw-rw-rw-   0        0        0    38586 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/precisely/apis/api_client.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:15:05.631000 com.precisely.apis-16.0.1/com/precisely/apis/apis/
+-rw-rw-rw-   0        0        0     2215 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/precisely/apis/apis/__init__.py
+-rw-rw-rw-   0        0        0    16559 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/precisely/apis/configuration.py
+-rw-rw-rw-   0        0        0     5117 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/precisely/apis/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:15:06.334999 com.precisely.apis-16.0.1/com/precisely/apis/model/
+-rw-rw-rw-   0        0        0      348 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/__init__.py
+-rw-rw-rw-   0        0        0    11256 2023-07-31 07:09:05.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/absentee_owner.py
+-rw-rw-rw-   0        0        0    11241 2023-07-31 07:09:05.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/accuracy.py
+-rw-rw-rw-   0        0        0    17255 2023-07-31 07:09:05.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/address.py
+-rw-rw-rw-   0        0        0    17940 2023-07-31 07:09:05.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/address1.py
+-rw-rw-rw-   0        0        0    11453 2023-07-31 07:09:05.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/address_time.py
+-rw-rw-rw-   0        0        0    11285 2023-07-31 07:09:05.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/address_type.py
+-rw-rw-rw-   0        0        0    13513 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/addresses_by_boundary_request.py
+-rw-rw-rw-   0        0        0    11159 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/addresses_count.py
+-rw-rw-rw-   0        0        0    14966 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/addresses_dto.py
+-rw-rw-rw-   0        0        0    11321 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/addresses_preferences.py
+-rw-rw-rw-   0        0        0    11720 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/addresses_response.py
+-rw-rw-rw-   0        0        0    17285 2023-07-31 07:09:05.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/ah_jmailing_address.py
+-rw-rw-rw-   0        0        0    13338 2023-07-31 07:09:05.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/ahj.py
+-rw-rw-rw-   0        0        0    11201 2023-07-31 07:09:05.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/ahj_list.py
+-rw-rw-rw-   0        0        0    11761 2023-07-31 07:09:05.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/ahj_plus_psap_response.py
+-rw-rw-rw-   0        0        0    11244 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/amenities.py
+-rw-rw-rw-   0        0        0    11229 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/area.py
+-rw-rw-rw-   0        0        0    12644 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/area_code_info.py
+-rw-rw-rw-   0        0        0    12082 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/assets_and_wealth_theme.py
+-rw-rw-rw-   0        0        0    11271 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/base_flood_elevation.py
+-rw-rw-rw-   0        0        0    11253 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/basement_type.py
+-rw-rw-rw-   0        0        0    12377 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/basic_boundary.py
+-rw-rw-rw-   0        0        0    11770 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/boundaries.py
+-rw-rw-rw-   0        0        0    12162 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/boundary.py
+-rw-rw-rw-   0        0        0    11763 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/boundary_buffer.py
+-rw-rw-rw-   0        0        0    11298 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/boundary_point.py
+-rw-rw-rw-   0        0        0    11294 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/buffer_relation.py
+-rw-rw-rw-   0        0        0    11250 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/buildg_class.py
+-rw-rw-rw-   0        0        0    11262 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/buildg_condition.py
+-rw-rw-rw-   0        0        0    11595 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/buildg_features_sqft.py
+-rw-rw-rw-   0        0        0    11564 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/buildg_improve_area.py
+-rw-rw-rw-   0        0        0    11268 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/buildg_improve_type.py
+-rw-rw-rw-   0        0        0    11256 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/buildg_quality.py
+-rw-rw-rw-   0        0        0    11250 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/buildg_style.py
+-rw-rw-rw-   0        0        0    11247 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/buildg_type.py
+-rw-rw-rw-   0        0        0    11247 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/buildg_view.py
+-rw-rw-rw-   0        0        0    11271 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/building_sqft_source.py
+-rw-rw-rw-   0        0        0    11247 2023-07-31 07:09:06.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/business_id.py
+-rw-rw-rw-   0        0        0    11253 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/ca_exemptions.py
+-rw-rw-rw-   0        0        0    13761 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/candidate.py
+-rw-rw-rw-   0        0        0    13399 2023-07-31 09:10:00.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/candidate_range.py
+-rw-rw-rw-   0        0        0    12226 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/candidate_range_unit.py
+-rw-rw-rw-   0        0        0    11233 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/carrier.py
+-rw-rw-rw-   0        0        0    11930 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/category.py
+-rw-rw-rw-   0        0        0    12296 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/category_metadata.py
+-rw-rw-rw-   0        0        0    11224 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/cbsa.py
+-rw-rw-rw-   0        0        0    12050 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/census.py
+-rw-rw-rw-   0        0        0    11277 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/center.py
+-rw-rw-rw-   0        0        0    11259 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/city.py
+-rw-rw-rw-   0        0        0    11893 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/common_geometry.py
+-rw-rw-rw-   0        0        0    11420 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/community.py
+-rw-rw-rw-   0        0        0    11297 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/consistency_code.py
+-rw-rw-rw-   0        0        0    11253 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/construction.py
+-rw-rw-rw-   0        0        0    12222 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/contact_details.py
+-rw-rw-rw-   0        0        0    12861 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/contact_person.py
+-rw-rw-rw-   0        0        0    11250 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/cooling_type.py
+-rw-rw-rw-   0        0        0    11691 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/cost.py
+-rw-rw-rw-   0        0        0    11230 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/county.py
+-rw-rw-rw-   0        0        0    11464 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/coverage.py
+-rw-rw-rw-   0        0        0    11830 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/crime_boundary.py
+-rw-rw-rw-   0        0        0    11750 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/crime_index_theme.py
+-rw-rw-rw-   0        0        0    11834 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/crime_risk_by_address_batch_request.py
+-rw-rw-rw-   0        0        0    11851 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/crime_risk_by_location_batch_request.py
+-rw-rw-rw-   0        0        0    11331 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/crime_risk_preferences.py
+-rw-rw-rw-   0        0        0    12263 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/crime_risk_response.py
+-rw-rw-rw-   0        0        0    11372 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/crime_risk_response_list.py
+-rw-rw-rw-   0        0        0    11530 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/crs.py
+-rw-rw-rw-   0        0        0    12065 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/demographics.py
+-rw-rw-rw-   0        0        0    11567 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/demographics_advanced_preferences.py
+-rw-rw-rw-   0        0        0    12118 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/demographics_advanced_request.py
+-rw-rw-rw-   0        0        0    11960 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/demographics_geometry.py
+-rw-rw-rw-   0        0        0    11557 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/demographics_geometry_crc.py
+-rw-rw-rw-   0        0        0    15660 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/demographics_themes_v2.py
+-rw-rw-rw-   0        0        0    11232 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/depth.py
+-rw-rw-rw-   0        0        0    11328 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/direction_geometry.py
+-rw-rw-rw-   0        0        0    11241 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/distance.py
+-rw-rw-rw-   0        0        0    11265 2023-07-31 07:09:07.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/distance_to_border.py
+-rw-rw-rw-   0        0        0    11863 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/distance_to_flood_hazard_address_request.py
+-rw-rw-rw-   0        0        0    11880 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/distance_to_flood_hazard_location_request.py
+-rw-rw-rw-   0        0        0    11406 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/distance_to_flood_hazard_response.py
+-rw-rw-rw-   0        0        0    11288 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/district_type.py
+-rw-rw-rw-   0        0        0    11635 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/domestic_ultimate_business.py
+-rw-rw-rw-   0        0        0    11266 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/earthquake_date_time.py
+-rw-rw-rw-   0        0        0    13648 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/earthquake_event.py
+-rw-rw-rw-   0        0        0    11621 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/earthquake_events_response.py
+-rw-rw-rw-   0        0        0    11981 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/earthquake_history.py
+-rw-rw-rw-   0        0        0    11313 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/earthquake_location.py
+-rw-rw-rw-   0        0        0    11798 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/earthquake_risk_by_address_request.py
+-rw-rw-rw-   0        0        0    11815 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/earthquake_risk_by_location_request.py
+-rw-rw-rw-   0        0        0    12371 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/earthquake_risk_response.py
+-rw-rw-rw-   0        0        0    11447 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/earthquake_risk_response_list.py
+-rw-rw-rw-   0        0        0    12064 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/education_theme.py
+-rw-rw-rw-   0        0        0    11358 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/employee_count.py
+-rw-rw-rw-   0        0        0    12067 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/employment_theme.py
+-rw-rw-rw-   0        0        0    11247 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/energy_type.py
+-rw-rw-rw-   0        0        0    11332 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/error_code.py
+-rw-rw-rw-   0        0        0    11260 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/error_info.py
+-rw-rw-rw-   0        0        0    13880 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/events_count.py
+-rw-rw-rw-   0        0        0    12070 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/expenditure_theme.py
+-rw-rw-rw-   0        0        0    11256 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/exterior_walls.py
+-rw-rw-rw-   0        0        0    11589 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/extra_feature_sqft.py
+-rw-rw-rw-   0        0        0    11445 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/field.py
+-rw-rw-rw-   0        0        0    14301 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/fields_matching.py
+-rw-rw-rw-   0        0        0    12318 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/fire_department.py
+-rw-rw-rw-   0        0        0    12050 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/fire_event.py
+-rw-rw-rw-   0        0        0    11282 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/fire_events_response.py
+-rw-rw-rw-   0        0        0    11733 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/fire_history.py
+-rw-rw-rw-   0        0        0    11780 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/fire_risk_by_address_request.py
+-rw-rw-rw-   0        0        0    11797 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/fire_risk_by_location_request.py
+-rw-rw-rw-   0        0        0    12122 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/fire_risk_response.py
+-rw-rw-rw-   0        0        0    11357 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/fire_risk_response_list.py
+-rw-rw-rw-   0        0        0    11725 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/fire_shed.py
+-rw-rw-rw-   0        0        0    13259 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/fire_station.py
+-rw-rw-rw-   0        0        0    11677 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/fire_station_contact_details.py
+-rw-rw-rw-   0        0        0    11677 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/fire_stations.py
+-rw-rw-rw-   0        0        0    11256 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/fireplace_type.py
+-rw-rw-rw-   0        0        0    11868 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/flood_hazard_preferences.py
+-rw-rw-rw-   0        0        0    11819 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/flood_risk_by_address_request.py
+-rw-rw-rw-   0        0        0    11836 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/flood_risk_by_location_request.py
+-rw-rw-rw-   0        0        0    11616 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/flood_risk_preferences.py
+-rw-rw-rw-   0        0        0    12803 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/flood_risk_response.py
+-rw-rw-rw-   0        0        0    11372 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/flood_risk_response_list.py
+-rw-rw-rw-   0        0        0    12555 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/flood_zone.py
+-rw-rw-rw-   0        0        0    11244 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/floor_type.py
+-rw-rw-rw-   0        0        0    13506 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/formatted_tax_address.py
+-rw-rw-rw-   0        0        0    11247 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/foundation.py
+-rw-rw-rw-   0        0        0    11679 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/free_or_reduced_price_lunches.py
+-rw-rw-rw-   0        0        0    11241 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/fuel_type.py
+-rw-rw-rw-   0        0        0    11247 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/garage_type.py
+-rw-rw-rw-   0        0        0    11682 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/geo_location_access_point.py
+-rw-rw-rw-   0        0        0    11479 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/geo_location_country.py
+-rw-rw-rw-   0        0        0    11957 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/geo_location_ip_addr.py
+-rw-rw-rw-   0        0        0    13204 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/geo_location_place.py
+-rw-rw-rw-   0        0        0    11295 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/geo_location_state.py
+-rw-rw-rw-   0        0        0    11638 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/geo_pos.py
+-rw-rw-rw-   0        0        0    14761 2023-07-31 09:09:53.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/geocode_address.py
+-rw-rw-rw-   0        0        0    18616 2023-07-31 07:09:08.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/geocode_preferences.py
+-rw-rw-rw-   0        0        0    11970 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/geocode_request.py
+-rw-rw-rw-   0        0        0    12023 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/geocode_service_response.py
+-rw-rw-rw-   0        0        0    11418 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/geocode_service_response_list.py
+-rw-rw-rw-   0        0        0    11316 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/geolocation_geometry.py
+-rw-rw-rw-   0        0        0    11283 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/geometry.py
+-rw-rw-rw-   0        0        0    11521 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/geometry_crc.py
+-rw-rw-rw-   0        0        0    11088 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/geometry_properties.py
+-rw-rw-rw-   0        0        0    11461 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/get_city_state_province_api_input.py
+-rw-rw-rw-   0        0        0    11984 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/get_city_state_province_api_input_row.py
+-rw-rw-rw-   0        0        0    12600 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/get_city_state_province_api_options.py
+-rw-rw-rw-   0        0        0    13593 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/get_city_state_province_api_output.py
+-rw-rw-rw-   0        0        0    11912 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/get_city_state_province_api_request.py
+-rw-rw-rw-   0        0        0    11470 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/get_city_state_province_api_response.py
+-rw-rw-rw-   0        0        0    11400 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/get_postal_codes_api_input.py
+-rw-rw-rw-   0        0        0    12159 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/get_postal_codes_api_input_row.py
+-rw-rw-rw-   0        0        0    11710 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/get_postal_codes_api_options.py
+-rw-rw-rw-   0        0        0    13110 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/get_postal_codes_api_output.py
+-rw-rw-rw-   0        0        0    11316 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/get_postal_codes_api_output_user_fields.py
+-rw-rw-rw-   0        0        0    11808 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/get_postal_codes_api_request.py
+-rw-rw-rw-   0        0        0    11409 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/get_postal_codes_api_response.py
+-rw-rw-rw-   0        0        0    11629 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/global_ultimate_business.py
+-rw-rw-rw-   0        0        0    13489 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/grade_levels_taught.py
+-rw-rw-rw-   0        0        0    11435 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/greatschools.py
+-rw-rw-rw-   0        0        0    11462 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/grid.py
+-rw-rw-rw-   0        0        0    12055 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/health_theme.py
+-rw-rw-rw-   0        0        0    11250 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/heating_type.py
+-rw-rw-rw-   0        0        0    12067 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/households_theme.py
+-rw-rw-rw-   0        0        0    12058 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/housing_theme.py
+-rw-rw-rw-   0        0        0    12055 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/income_theme.py
+-rw-rw-rw-   0        0        0    11874 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/index_variable.py
+-rw-rw-rw-   0        0        0    11677 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/individual_value_variable.py
+-rw-rw-rw-   0        0        0    11253 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/interior_wall.py
+-rw-rw-rw-   0        0        0    11319 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/intermediate_points.py
+-rw-rw-rw-   0        0        0    12291 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/intersection.py
+-rw-rw-rw-   0        0        0    11679 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/intersection_response.py
+-rw-rw-rw-   0        0        0    12067 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/ip_info.py
+-rw-rw-rw-   0        0        0    13054 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/ipd.py
+-rw-rw-rw-   0        0        0    11890 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/ipd_tax_by_address_batch_request.py
+-rw-rw-rw-   0        0        0    11871 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/ipd_tax_jurisdiction.py
+-rw-rw-rw-   0        0        0    11808 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/key_lookup_request.py
+-rw-rw-rw-   0        0        0    11446 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/keys.py
+-rw-rw-rw-   0        0        0    11238 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/land_use.py
+-rw-rw-rw-   0        0        0    12232 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/lat_long_fields.py
+-rw-rw-rw-   0        0        0    12064 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/life_style_theme.py
+-rw-rw-rw-   0        0        0    11238 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/loc_code.py
+-rw-rw-rw-   0        0        0    11343 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/local_tax_geometry.py
+-rw-rw-rw-   0        0        0    14407 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/local_tax_preferences.py
+-rw-rw-rw-   0        0        0    11217 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/location.py
+-rw-rw-rw-   0        0        0    12025 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/location_time.py
+-rw-rw-rw-   0        0        0    12175 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/magnitude.py
+-rw-rw-rw-   0        0        0    11972 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/match.py
+-rw-rw-rw-   0        0        0    17276 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/matched_address.py
+-rw-rw-rw-   0        0        0    12342 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/matrix.py
+-rw-rw-rw-   0        0        0    11221 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/mcd.py
+-rw-rw-rw-   0        0        0    11652 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/metadata_response.py
+-rw-rw-rw-   0        0        0    11474 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/name.py
+-rw-rw-rw-   0        0        0    11298 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/neighborhoods_response.py
+-rw-rw-rw-   0        0        0    13019 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/network.py
+-rw-rw-rw-   0        0        0    11496 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/organization_type.py
+-rw-rw-rw-   0        0        0    11247 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/other_rooms.py
+-rw-rw-rw-   0        0        0    11256 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/owner_vest_type.py
+-rw-rw-rw-   0        0        0    11899 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/owners.py
+-rw-rw-rw-   0        0        0    11605 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/parent_business.py
+-rw-rw-rw-   0        0        0    11412 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/pb_key_address_request.py
+-rw-rw-rw-   0        0        0    11468 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/pb_key_response.py
+-rw-rw-rw-   0        0        0    11250 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/pb_key_response_list.py
+-rw-rw-rw-   0        0        0    11646 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/pbkey.py
+-rw-rw-rw-   0        0        0    11383 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/phone_verification.py
+-rw-rw-rw-   0        0        0    12826 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/phone_verification_output.py
+-rw-rw-rw-   0        0        0    11592 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/place.py
+-rw-rw-rw-   0        0        0    12220 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/places_response.py
+-rw-rw-rw-   0        0        0    20808 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/poi.py
+-rw-rw-rw-   0        0        0    12870 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/poi_boundary.py
+-rw-rw-rw-   0        0        0    11840 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/poi_boundary_address_request.py
+-rw-rw-rw-   0        0        0    11900 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/poi_boundary_location_request.py
+-rw-rw-rw-   0        0        0    11825 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/poi_boundary_locations.py
+-rw-rw-rw-   0        0        0    11548 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/poi_boundary_preferences.py
+-rw-rw-rw-   0        0        0    11333 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/poi_boundary_response.py
+-rw-rw-rw-   0        0        0    11800 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/poi_classification.py
+-rw-rw-rw-   0        0        0    11116 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/poi_count.py
+-rw-rw-rw-   0        0        0    12954 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/poi_count_request.py
+-rw-rw-rw-   0        0        0    13374 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/poiby_geometry_request.py
+-rw-rw-rw-   0        0        0    11725 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/points.py
+-rw-rw-rw-   0        0        0    11241 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/pool_type.py
+-rw-rw-rw-   0        0        0    12067 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/population_theme.py
+-rw-rw-rw-   0        0        0    11114 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/preferenc_time_zone.py
+-rw-rw-rw-   0        0        0    11280 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/primary_zone.py
+-rw-rw-rw-   0        0        0    11256 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/prior_sale_code.py
+-rw-rw-rw-   0        0        0    11265 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/prop_site_influene.py
+-rw-rw-rw-   0        0        0    11106 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/properties.py
+-rw-rw-rw-   0        0        0    46206 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/property_attributes.py
+-rw-rw-rw-   0        0        0    11349 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/property_geometry.py
+-rw-rw-rw-   0        0        0    11918 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/property_info_address_request.py
+-rw-rw-rw-   0        0        0    11133 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/property_info_preferences.py
+-rw-rw-rw-   0        0        0    12002 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/property_info_response.py
+-rw-rw-rw-   0        0        0    11457 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/property_info_responses.py
+-rw-rw-rw-   0        0        0    11696 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/proxy.py
+-rw-rw-rw-   0        0        0    13793 2023-07-31 07:09:09.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/psap_response.py
+-rw-rw-rw-   0        0        0    12085 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/race_and_ethnicity_theme.py
+-rw-rw-rw-   0        0        0    12626 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/range_variable.py
+-rw-rw-rw-   0        0        0    11664 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/rate.py
+-rw-rw-rw-   0        0        0    13755 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/rate_center_response.py
+-rw-rw-rw-   0        0        0    12337 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/return_fields_descriptor.py
+-rw-rw-rw-   0        0        0    11723 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/reverse_geocode_request.py
+-rw-rw-rw-   0        0        0    14978 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/risk.py
+-rw-rw-rw-   0        0        0    17267 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/risk_address.py
+-rw-rw-rw-   0        0        0    11337 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/risk_geometry.py
+-rw-rw-rw-   0        0        0    11797 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/risk_locations.py
+-rw-rw-rw-   0        0        0    11601 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/risk_preferences.py
+-rw-rw-rw-   0        0        0    11316 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/risks_boundaries.py
+-rw-rw-rw-   0        0        0    11368 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/risks_crime_theme.py
+-rw-rw-rw-   0        0        0    11536 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/risks_geometry_crc.py
+-rw-rw-rw-   0        0        0    13324 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/road.py
+-rw-rw-rw-   0        0        0    11256 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/roof_cover_type.py
+-rw-rw-rw-   0        0        0    11256 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/roof_frame_type.py
+-rw-rw-rw-   0        0        0    11256 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/roof_shape_type.py
+-rw-rw-rw-   0        0        0    12381 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/route_direction.py
+-rw-rw-rw-   0        0        0    11304 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/route_geometry.py
+-rw-rw-rw-   0        0        0    13382 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/route_response.py
+-rw-rw-rw-   0        0        0    13904 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/sales_tax.py
+-rw-rw-rw-   0        0        0    11569 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/sales_volume.py
+-rw-rw-rw-   0        0        0    19109 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/school.py
+-rw-rw-rw-   0        0        0    12879 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/school_district.py
+-rw-rw-rw-   0        0        0    13410 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/school_profile.py
+-rw-rw-rw-   0        0        0    12471 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/school_ranking.py
+-rw-rw-rw-   0        0        0    11996 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/schools_near_by_response.py
+-rw-rw-rw-   0        0        0    11761 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/segmentation.py
+-rw-rw-rw-   0        0        0    11365 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/segmentation_themes.py
+-rw-rw-rw-   0        0        0    11268 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/shore_line_distance.py
+-rw-rw-rw-   0        0        0    12022 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/sic.py
+-rw-rw-rw-   0        0        0    12330 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/sic_metadata.py
+-rw-rw-rw-   0        0        0    12078 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/site_details.py
+-rw-rw-rw-   0        0        0    13485 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/situs_address.py
+-rw-rw-rw-   0        0        0    12476 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/special_purpose_district.py
+-rw-rw-rw-   0        0        0    11579 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/special_purpose_district_tax.py
+-rw-rw-rw-   0        0        0    13049 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/speed_limit.py
+-rw-rw-rw-   0        0        0    11298 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/start_end_point.py
+-rw-rw-rw-   0        0        0    11227 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/state.py
+-rw-rw-rw-   0        0        0    11265 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/status.py
+-rw-rw-rw-   0        0        0    11273 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/stories.py
+-rw-rw-rw-   0        0        0    12424 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/student_ethnicity.py
+-rw-rw-rw-   0        0        0    12082 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/supply_and_demand_theme.py
+-rw-rw-rw-   0        0        0    18388 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/tax_address.py
+-rw-rw-rw-   0        0        0    11824 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/tax_address_request.py
+-rw-rw-rw-   0        0        0    11239 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/tax_county.py
+-rw-rw-rw-   0        0        0    13607 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/tax_district_response.py
+-rw-rw-rw-   0        0        0    11446 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/tax_district_response_list.py
+-rw-rw-rw-   0        0        0    11247 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/tax_doc_type.py
+-rw-rw-rw-   0        0        0    11253 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/tax_exemption.py
+-rw-rw-rw-   0        0        0    11334 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/tax_geometry.py
+-rw-rw-rw-   0        0        0    12257 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/tax_jurisdiction.py
+-rw-rw-rw-   0        0        0    11798 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/tax_location_request.py
+-rw-rw-rw-   0        0        0    11787 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/tax_locations.py
+-rw-rw-rw-   0        0        0    12845 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/tax_place.py
+-rw-rw-rw-   0        0        0    18168 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/tax_rate_address.py
+-rw-rw-rw-   0        0        0    11919 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/tax_rate_address_request.py
+-rw-rw-rw-   0        0        0    11810 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/tax_rate_location_request.py
+-rw-rw-rw-   0        0        0    17504 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/tax_rate_matched_address.py
+-rw-rw-rw-   0        0        0    14126 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/tax_rate_response.py
+-rw-rw-rw-   0        0        0    11346 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/tax_responses.py
+-rw-rw-rw-   0        0        0    11268 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/tax_sales_price_code.py
+-rw-rw-rw-   0        0        0    11236 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/tax_state.py
+-rw-rw-rw-   0        0        0    11229 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/time.py
+-rw-rw-rw-   0        0        0    11731 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/timezone_address_request.py
+-rw-rw-rw-   0        0        0    11349 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/timezone_geometry.py
+-rw-rw-rw-   0        0        0    11357 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/timezone_location_request.py
+-rw-rw-rw-   0        0        0    15245 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/timezone_response.py
+-rw-rw-rw-   0        0        0    11352 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/timezone_response_list.py
+-rw-rw-rw-   0        0        0    11354 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/travel_boundaries.py
+-rw-rw-rw-   0        0        0    11234 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/travel_boundary.py
+-rw-rw-rw-   0        0        0    11283 2023-07-31 07:09:10.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/travel_cost_matrix_response.py
+-rw-rw-rw-   0        0        0    11229 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/type.py
+-rw-rw-rw-   0        0        0    13874 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/typeahead_location.py
+-rw-rw-rw-   0        0        0    11353 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/typeahead_locations.py
+-rw-rw-rw-   0        0        0    11505 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/typeahead_range.py
+-rw-rw-rw-   0        0        0    11595 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/typeahead_unit.py
+-rw-rw-rw-   0        0        0    11235 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/unit.py
+-rw-rw-rw-   0        0        0    13898 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/use_tax.py
+-rw-rw-rw-   0        0        0    11238 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/vacancy.py
+-rw-rw-rw-   0        0        0    11817 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_email_address_api_request.py
+-rw-rw-rw-   0        0        0    11447 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_email_address_api_response.py
+-rw-rw-rw-   0        0        0    11429 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_email_address_input.py
+-rw-rw-rw-   0        0        0    16658 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_email_address_input_row.py
+-rw-rw-rw-   0        0        0    15324 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_email_address_output.py
+-rw-rw-rw-   0        0        0    11449 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_input.py
+-rw-rw-rw-   0        0        0    13503 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_input_row.py
+-rw-rw-rw-   0        0        0    11357 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_options.py
+-rw-rw-rw-   0        0        0    15940 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_output.py
+-rw-rw-rw-   0        0        0    11520 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_premium_input.py
+-rw-rw-rw-   0        0        0    14342 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_premium_input_row.py
+-rw-rw-rw-   0        0        0    15105 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_premium_options.py
+-rw-rw-rw-   0        0        0    39660 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_premium_output.py
+-rw-rw-rw-   0        0        0    12012 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_premium_request.py
+-rw-rw-rw-   0        0        0    11529 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_premium_response.py
+-rw-rw-rw-   0        0        0    11480 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_pro_input.py
+-rw-rw-rw-   0        0        0    13512 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_pro_input_row.py
+-rw-rw-rw-   0        0        0    14100 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_pro_options.py
+-rw-rw-rw-   0        0        0    18611 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_pro_output.py
+-rw-rw-rw-   0        0        0    11944 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_pro_request.py
+-rw-rw-rw-   0        0        0    11489 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_pro_response.py
+-rw-rw-rw-   0        0        0    11891 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_request.py
+-rw-rw-rw-   0        0        0    11458 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_response.py
+-rw-rw-rw-   0        0        0    11530 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_input.py
+-rw-rw-rw-   0        0        0    14701 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_input_row.py
+-rw-rw-rw-   0        0        0    36257 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_options.py
+-rw-rw-rw-   0        0        0    49413 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_output.py
+-rw-rw-rw-   0        0        0    12029 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_request.py
+-rw-rw-rw-   0        0        0    11539 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_response.py
+-rw-rw-rw-   0        0        0    11488 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_phone_number_api_request.py
+-rw-rw-rw-   0        0        0    11521 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_phone_number_api_request_input.py
+-rw-rw-rw-   0        0        0    11377 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/validate_phone_number_api_request_input_row.py
+-rw-rw-rw-   0        0        0    11760 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/water_body.py
+-rw-rw-rw-   0        0        0    11870 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/water_body_response.py
+-rw-rw-rw-   0        0        0    17270 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/zones_address.py
+-rw-rw-rw-   0        0        0    11334 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/zones_boundary_geometry.py
+-rw-rw-rw-   0        0        0    11574 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/zones_contact_details.py
+-rw-rw-rw-   0        0        0    11340 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/zones_geometry.py
+-rw-rw-rw-   0        0        0    11091 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/zones_parent_business.py
+-rw-rw-rw-   0        0        0    14879 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/zones_poi.py
+-rw-rw-rw-   0        0        0    11851 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/zones_poi_classification.py
+-rw-rw-rw-   0        0        0    11863 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/zones_poi_geometry.py
+-rw-rw-rw-   0        0        0    11791 2023-07-31 07:09:11.000000 com.precisely.apis-16.0.1/com/precisely/apis/model/zones_sic.py
+-rw-rw-rw-   0        0        0    81943 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/precisely/apis/model_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:15:06.336000 com.precisely.apis-16.0.1/com/precisely/apis/models/
+-rw-rw-rw-   0        0        0    26829 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/precisely/apis/models/__init__.py
+-rw-rw-rw-   0        0        0    14245 2023-07-31 07:09:13.000000 com.precisely.apis-16.0.1/com/precisely/apis/rest.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:15:05.547998 com.precisely.apis-16.0.1/com.precisely.apis.egg-info/
+-rw-rw-rw-   0        0        0      451 2023-07-31 09:15:05.000000 com.precisely.apis-16.0.1/com.precisely.apis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    18649 2023-07-31 09:15:05.000000 com.precisely.apis-16.0.1/com.precisely.apis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 09:15:05.000000 com.precisely.apis-16.0.1/com.precisely.apis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-31 09:15:05.000000 com.precisely.apis-16.0.1/com.precisely.apis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-31 09:15:05.000000 com.precisely.apis-16.0.1/com.precisely.apis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       76 2023-07-31 09:15:06.339998 com.precisely.apis-16.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-07-31 09:08:09.000000 com.precisely.apis-16.0.1/setup.py
```

### Comparing `com.precisely.apis-16.0.0/LICENSE` & `com.precisely.apis-16.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-16.0.0/README.md` & `com.precisely.apis-16.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 [Click here](https://docs.precisely.com/docs/sftw/precisely-apis/main/en-us/webhelp/apis/About%20Document/about_this_doc.html) for detailed Documentation on Precisely APIs 
 # PreciselyAPIsPythonSDK
 Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- Package version: 16.0.0
+- Package version: 16.0.1
 
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 For more information, please visit [https://support.precisely.com](https://support.precisely.com)
 
 ## Requirements.
 
@@ -265,14 +265,15 @@
  - [AHJ](docs/AHJ.md)
  - [AHJList](docs/AHJList.md)
  - [AHJPlusPSAPResponse](docs/AHJPlusPSAPResponse.md)
  - [AHJmailingAddress](docs/AHJmailingAddress.md)
  - [AbsenteeOwner](docs/AbsenteeOwner.md)
  - [Accuracy](docs/Accuracy.md)
  - [Address](docs/Address.md)
+ - [Address1](docs/Address1.md)
  - [AddressTime](docs/AddressTime.md)
  - [AddressType](docs/AddressType.md)
  - [AddressesByBoundaryRequest](docs/AddressesByBoundaryRequest.md)
  - [AddressesCount](docs/AddressesCount.md)
  - [AddressesDTO](docs/AddressesDTO.md)
  - [AddressesPreferences](docs/AddressesPreferences.md)
  - [AddressesResponse](docs/AddressesResponse.md)
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/__init__.py` & `com.precisely.apis-16.0.1/com/precisely/apis/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # flake8: noqa
 
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "16.0.0"
+__version__ = "16.0.1"
 
 # import ApiClient
 from com.precisely.apis.api_client import ApiClient
 
 # import Configuration
 from com.precisely.apis.configuration import Configuration
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/api/address_autocomplete_enterprise_service_api.py` & `com.precisely.apis-16.0.1/com/precisely/apis/api/address_autocomplete_enterprise_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/api/address_autocomplete_service_api.py` & `com.precisely.apis-16.0.1/com/precisely/apis/api/address_autocomplete_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/api/address_verification_service_api.py` & `com.precisely.apis-16.0.1/com/precisely/apis/api/address_verification_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/api/addresses_service__api.py` & `com.precisely.apis-16.0.1/com/precisely/apis/api/addresses_service__api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/api/demographics_service_api.py` & `com.precisely.apis-16.0.1/com/precisely/apis/api/demographics_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/api/email_verification_service_api.py` & `com.precisely.apis-16.0.1/com/precisely/apis/api/email_verification_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/api/geocode_service_api.py` & `com.precisely.apis-16.0.1/com/precisely/apis/api/geocode_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/api/geolocation_service_api.py` & `com.precisely.apis-16.0.1/com/precisely/apis/api/geolocation_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/api/local_tax_service_api.py` & `com.precisely.apis-16.0.1/com/precisely/apis/api/local_tax_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/api/neighborhoods_service__api.py` & `com.precisely.apis-16.0.1/com/precisely/apis/api/neighborhoods_service__api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/api/phone_verification_service_api.py` & `com.precisely.apis-16.0.1/com/precisely/apis/api/phone_verification_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/api/places_service__api.py` & `com.precisely.apis-16.0.1/com/precisely/apis/api/places_service__api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/api/property_information_service_api.py` & `com.precisely.apis-16.0.1/com/precisely/apis/api/property_information_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/api/psap_911_service_api.py` & `com.precisely.apis-16.0.1/com/precisely/apis/api/psap_911_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/api/risks_service_api.py` & `com.precisely.apis-16.0.1/com/precisely/apis/api/risks_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/api/routing_service_api.py` & `com.precisely.apis-16.0.1/com/precisely/apis/api/routing_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/api/schools_service_api.py` & `com.precisely.apis-16.0.1/com/precisely/apis/api/schools_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/api/streets_service_api.py` & `com.precisely.apis-16.0.1/com/precisely/apis/api/streets_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/api/telecomm_info_service_api.py` & `com.precisely.apis-16.0.1/com/precisely/apis/api/telecomm_info_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/api/time_zone_service_api.py` & `com.precisely.apis-16.0.1/com/precisely/apis/api/time_zone_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/api/zones_service_api.py` & `com.precisely.apis-16.0.1/com/precisely/apis/api/zones_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/api_client.py` & `com.precisely.apis-16.0.1/com/precisely/apis/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
 import mimetypes
@@ -80,15 +80,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/16.0.0/python'
+        self.user_agent = 'OpenAPI-Generator/16.0.1/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/apis/__init__.py` & `com.precisely.apis-16.0.1/com/precisely/apis/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/configuration.py` & `com.precisely.apis-16.0.1/com/precisely/apis/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
 import multiprocessing
@@ -383,16 +383,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 16.0.0\n"\
-               "SDK Package Version: 16.0.0".\
+               "Version of the API: 16.0.1\n"\
+               "SDK Package Version: 16.0.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/exceptions.py` & `com.precisely.apis-16.0.1/com/precisely/apis/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/absentee_owner.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/absentee_owner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/accuracy.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/accuracy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/address.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/address_time.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/address_time.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/address_type.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/address_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/addresses_by_boundary_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/addresses_by_boundary_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/addresses_count.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/addresses_count.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/addresses_dto.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/addresses_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/addresses_preferences.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/addresses_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/addresses_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/addresses_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/ah_jmailing_address.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/ah_jmailing_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/ahj.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/ahj.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/ahj_list.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/ahj_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/ahj_plus_psap_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/ahj_plus_psap_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/amenities.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/amenities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/area.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/area.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/area_code_info.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/area_code_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/assets_and_wealth_theme.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/assets_and_wealth_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/base_flood_elevation.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/base_flood_elevation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/basement_type.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/basement_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/basic_boundary.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/basic_boundary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/boundaries.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/boundaries.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/boundary.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/boundary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/boundary_buffer.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/boundary_buffer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/boundary_point.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/boundary_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/buffer_relation.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/buffer_relation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/buildg_class.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/buildg_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/buildg_condition.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/buildg_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/buildg_features_sqft.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/buildg_features_sqft.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/buildg_improve_area.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/buildg_improve_area.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/buildg_improve_type.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/buildg_improve_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/buildg_quality.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/buildg_quality.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/buildg_style.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/buildg_style.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/buildg_type.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/buildg_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/buildg_view.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/buildg_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/building_sqft_source.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/building_sqft_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/business_id.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/business_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/ca_exemptions.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/ca_exemptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/candidate.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/candidate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/candidate_range.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/contact_person.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from com.precisely.apis.model.candidate_range_unit import CandidateRangeUnit
-    globals()['CandidateRangeUnit'] = CandidateRangeUnit
 
-
-class CandidateRange(ModelNormal):
+class ContactPerson(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,88 +51,79 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('side',): {
-            'UNKNOWN': "UNKNOWN",
-            'LEFT': "LEFT",
-            'RIGHT': "RIGHT",
-            'BOTH': "BOTH",
-        },
-        ('odd_even_indicator',): {
-            'UNKNOWN': "UNKNOWN",
-            'BOTH': "BOTH",
-            'ODD': "ODD",
-            'EVEN': "EVEN",
-            'IRREGULAR': "IRREGULAR",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'place_name': (str,),  # noqa: E501
-            'low_house': (str,),  # noqa: E501
-            'high_house': (str,),  # noqa: E501
-            'side': (str,),  # noqa: E501
-            'odd_even_indicator': (str,),  # noqa: E501
-            'units': ([CandidateRangeUnit],),  # noqa: E501
-            'custom_values': (dict,),  # noqa: E501
+            'title': (str,),  # noqa: E501
+            'full_name': (str,),  # noqa: E501
+            'prefix': (str,),  # noqa: E501
+            'first_name': (str,),  # noqa: E501
+            'last_name': (str,),  # noqa: E501
+            'phone': (str,),  # noqa: E501
+            'fax': (str,),  # noqa: E501
+            'email': (str,),  # noqa: E501
+            'comments': (str,),  # noqa: E501
+            'additional_details': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'place_name': 'placeName',  # noqa: E501
-        'low_house': 'lowHouse',  # noqa: E501
-        'high_house': 'highHouse',  # noqa: E501
-        'side': 'side',  # noqa: E501
-        'odd_even_indicator': 'oddEvenIndicator',  # noqa: E501
-        'units': 'units',  # noqa: E501
-        'custom_values': 'customValues',  # noqa: E501
+        'title': 'title',  # noqa: E501
+        'full_name': 'fullName',  # noqa: E501
+        'prefix': 'prefix',  # noqa: E501
+        'first_name': 'firstName',  # noqa: E501
+        'last_name': 'lastName',  # noqa: E501
+        'phone': 'phone',  # noqa: E501
+        'fax': 'fax',  # noqa: E501
+        'email': 'email',  # noqa: E501
+        'comments': 'comments',  # noqa: E501
+        'additional_details': 'additionalDetails',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CandidateRange - a model defined in OpenAPI
+        """ContactPerson - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -161,21 +148,24 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            place_name (str): [optional]  # noqa: E501
-            low_house (str): [optional]  # noqa: E501
-            high_house (str): [optional]  # noqa: E501
-            side (str): [optional]  # noqa: E501
-            odd_even_indicator (str): [optional]  # noqa: E501
-            units ([CandidateRangeUnit]): [optional]  # noqa: E501
-            custom_values ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)}): [optional]  # noqa: E501
+            title (str): [optional]  # noqa: E501
+            full_name (str): [optional]  # noqa: E501
+            prefix (str): [optional]  # noqa: E501
+            first_name (str): [optional]  # noqa: E501
+            last_name (str): [optional]  # noqa: E501
+            phone (str): [optional]  # noqa: E501
+            fax (str): [optional]  # noqa: E501
+            email (str): [optional]  # noqa: E501
+            comments (str): [optional]  # noqa: E501
+            additional_details (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -216,15 +206,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """CandidateRange - a model defined in OpenAPI
+        """ContactPerson - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -249,21 +239,24 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            place_name (str): [optional]  # noqa: E501
-            low_house (str): [optional]  # noqa: E501
-            high_house (str): [optional]  # noqa: E501
-            side (str): [optional]  # noqa: E501
-            odd_even_indicator (str): [optional]  # noqa: E501
-            units ([CandidateRangeUnit]): [optional]  # noqa: E501
-            custom_values ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)}): [optional]  # noqa: E501
+            title (str): [optional]  # noqa: E501
+            full_name (str): [optional]  # noqa: E501
+            prefix (str): [optional]  # noqa: E501
+            first_name (str): [optional]  # noqa: E501
+            last_name (str): [optional]  # noqa: E501
+            phone (str): [optional]  # noqa: E501
+            fax (str): [optional]  # noqa: E501
+            email (str): [optional]  # noqa: E501
+            comments (str): [optional]  # noqa: E501
+            additional_details (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/candidate_range_unit.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/candidate_range_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/carrier.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/carrier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/category.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/category.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/category_metadata.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/category_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/cbsa.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/cbsa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/census.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/census.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/center.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/center.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/city.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/city.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/common_geometry.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/common_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/community.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/community.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/consistency_code.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/consistency_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/construction.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/construction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/contact_details.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/contact_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/contact_person.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/tax_place.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class ContactPerson(ModelNormal):
+class TaxPlace(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,53 +77,51 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'title': (str,),  # noqa: E501
-            'full_name': (str,),  # noqa: E501
-            'prefix': (str,),  # noqa: E501
-            'first_name': (str,),  # noqa: E501
-            'last_name': (str,),  # noqa: E501
-            'phone': (str,),  # noqa: E501
-            'fax': (str,),  # noqa: E501
-            'email': (str,),  # noqa: E501
-            'comments': (str,),  # noqa: E501
-            'additional_details': (str,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'code': (str,),  # noqa: E501
+            'gnis_code': (str,),  # noqa: E501
+            'self_collected': (bool,),  # noqa: E501
+            'class_code': (str,),  # noqa: E501
+            'incorporated_flag': (str,),  # noqa: E501
+            'last_annexed_date': (str,),  # noqa: E501
+            'last_updated_date': (str,),  # noqa: E501
+            'last_verified_date': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'title': 'title',  # noqa: E501
-        'full_name': 'fullName',  # noqa: E501
-        'prefix': 'prefix',  # noqa: E501
-        'first_name': 'firstName',  # noqa: E501
-        'last_name': 'lastName',  # noqa: E501
-        'phone': 'phone',  # noqa: E501
-        'fax': 'fax',  # noqa: E501
-        'email': 'email',  # noqa: E501
-        'comments': 'comments',  # noqa: E501
-        'additional_details': 'additionalDetails',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'code': 'code',  # noqa: E501
+        'gnis_code': 'gnisCode',  # noqa: E501
+        'self_collected': 'selfCollected',  # noqa: E501
+        'class_code': 'classCode',  # noqa: E501
+        'incorporated_flag': 'incorporatedFlag',  # noqa: E501
+        'last_annexed_date': 'lastAnnexedDate',  # noqa: E501
+        'last_updated_date': 'lastUpdatedDate',  # noqa: E501
+        'last_verified_date': 'lastVerifiedDate',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ContactPerson - a model defined in OpenAPI
+        """TaxPlace - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -148,24 +146,23 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            title (str): [optional]  # noqa: E501
-            full_name (str): [optional]  # noqa: E501
-            prefix (str): [optional]  # noqa: E501
-            first_name (str): [optional]  # noqa: E501
-            last_name (str): [optional]  # noqa: E501
-            phone (str): [optional]  # noqa: E501
-            fax (str): [optional]  # noqa: E501
-            email (str): [optional]  # noqa: E501
-            comments (str): [optional]  # noqa: E501
-            additional_details (str): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            code (str): [optional]  # noqa: E501
+            gnis_code (str): [optional]  # noqa: E501
+            self_collected (bool): [optional]  # noqa: E501
+            class_code (str): [optional]  # noqa: E501
+            incorporated_flag (str): [optional]  # noqa: E501
+            last_annexed_date (str): [optional]  # noqa: E501
+            last_updated_date (str): [optional]  # noqa: E501
+            last_verified_date (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -206,15 +203,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ContactPerson - a model defined in OpenAPI
+        """TaxPlace - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -239,24 +236,23 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            title (str): [optional]  # noqa: E501
-            full_name (str): [optional]  # noqa: E501
-            prefix (str): [optional]  # noqa: E501
-            first_name (str): [optional]  # noqa: E501
-            last_name (str): [optional]  # noqa: E501
-            phone (str): [optional]  # noqa: E501
-            fax (str): [optional]  # noqa: E501
-            email (str): [optional]  # noqa: E501
-            comments (str): [optional]  # noqa: E501
-            additional_details (str): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            code (str): [optional]  # noqa: E501
+            gnis_code (str): [optional]  # noqa: E501
+            self_collected (bool): [optional]  # noqa: E501
+            class_code (str): [optional]  # noqa: E501
+            incorporated_flag (str): [optional]  # noqa: E501
+            last_annexed_date (str): [optional]  # noqa: E501
+            last_updated_date (str): [optional]  # noqa: E501
+            last_verified_date (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/cooling_type.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/cooling_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/cost.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/cost.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/county.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/county.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/coverage.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/coverage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/crime_boundary.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/crime_boundary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/crime_index_theme.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/crime_index_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/crime_risk_by_address_batch_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/crime_risk_by_address_batch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/crime_risk_by_location_batch_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/crime_risk_by_location_batch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/crime_risk_preferences.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/crime_risk_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/crime_risk_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/crime_risk_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/crime_risk_response_list.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/crime_risk_response_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/crs.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/crs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/demographics.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/demographics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/demographics_advanced_preferences.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/demographics_advanced_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/demographics_advanced_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/demographics_advanced_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/demographics_geometry.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/demographics_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/demographics_geometry_crc.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/demographics_geometry_crc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/demographics_themes_v2.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/demographics_themes_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/depth.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/depth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/direction_geometry.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/direction_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/distance.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/distance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/distance_to_border.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/distance_to_border.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/distance_to_flood_hazard_address_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/distance_to_flood_hazard_address_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/distance_to_flood_hazard_location_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/distance_to_flood_hazard_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/distance_to_flood_hazard_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/distance_to_flood_hazard_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/district_type.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/district_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/domestic_ultimate_business.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/domestic_ultimate_business.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/earthquake_date_time.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/earthquake_date_time.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/earthquake_event.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/earthquake_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/earthquake_events_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/earthquake_events_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/earthquake_history.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/earthquake_history.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/earthquake_location.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/earthquake_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/earthquake_risk_by_address_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/earthquake_risk_by_address_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/earthquake_risk_by_location_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/earthquake_risk_by_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/earthquake_risk_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/earthquake_risk_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/earthquake_risk_response_list.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/earthquake_risk_response_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/education_theme.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/education_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/employee_count.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/employee_count.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/employment_theme.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/employment_theme.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/energy_type.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/energy_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/error_code.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/error_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/error_info.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/error_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/events_count.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/events_count.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/expenditure_theme.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/expenditure_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/exterior_walls.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/exterior_walls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/extra_feature_sqft.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/extra_feature_sqft.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/field.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/fields_matching.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/fields_matching.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/fire_department.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/fire_department.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/fire_event.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/fire_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/fire_events_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/fire_events_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/fire_history.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/fire_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/fire_risk_by_address_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/fire_risk_by_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/fire_risk_by_location_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/fire_risk_by_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/fire_risk_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/fire_risk_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/fire_risk_response_list.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/fire_risk_response_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/fire_shed.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/fire_shed.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/fire_station.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/fire_station.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/fire_station_contact_details.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/fire_station_contact_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/fire_stations.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/fire_stations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/fireplace_type.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/fireplace_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/flood_hazard_preferences.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/flood_hazard_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/flood_risk_by_address_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/flood_risk_by_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/flood_risk_by_location_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/flood_risk_by_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/flood_risk_preferences.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/flood_risk_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/flood_risk_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/flood_risk_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/flood_risk_response_list.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/flood_risk_response_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/flood_zone.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/flood_zone.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/floor_type.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/floor_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/formatted_tax_address.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/formatted_tax_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/foundation.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/foundation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/free_or_reduced_price_lunches.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/free_or_reduced_price_lunches.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/fuel_type.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/fuel_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/garage_type.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/garage_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/geo_location_access_point.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/geo_location_access_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/geo_location_country.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/geo_location_country.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/geo_location_ip_addr.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/geo_location_ip_addr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/geo_location_place.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/geo_location_place.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/geo_location_state.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/geo_location_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/geo_pos.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/geo_pos.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/geocode_address.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/grade_levels_taught.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class GeocodeAddress(ModelNormal):
+class GradeLevelsTaught(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,65 +77,61 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'object_id': (str,),  # noqa: E501
-            'main_address_line': (str,),  # noqa: E501
-            'address_last_line': (str,),  # noqa: E501
-            'place_name': (str,),  # noqa: E501
-            'area_name1': (str,),  # noqa: E501
-            'area_name2': (str,),  # noqa: E501
-            'area_name3': (str,),  # noqa: E501
-            'area_name4': (str,),  # noqa: E501
-            'post_code1': (str,),  # noqa: E501
-            'post_code2': (str,),  # noqa: E501
-            'country': (str,),  # noqa: E501
-            'address_number': (str,),  # noqa: E501
-            'street_name': (str,),  # noqa: E501
-            'unit_type': (str,),  # noqa: E501
-            'unit_value': (str,),  # noqa: E501
-            'custom_values': (dict,), # noqa: E501
+            'pk': (str,),  # noqa: E501
+            'kg': (str,),  # noqa: E501
+            'first': (str,),  # noqa: E501
+            'second': (str,),  # noqa: E501
+            'third': (str,),  # noqa: E501
+            'fourth': (str,),  # noqa: E501
+            'fifth': (str,),  # noqa: E501
+            'sixth': (str,),  # noqa: E501
+            'seventh': (str,),  # noqa: E501
+            'eighth': (str,),  # noqa: E501
+            'ninth': (str,),  # noqa: E501
+            'tenth': (str,),  # noqa: E501
+            'eleventh': (str,),  # noqa: E501
+            'twelfth': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'object_id': 'objectId',  # noqa: E501
-        'main_address_line': 'mainAddressLine',  # noqa: E501
-        'address_last_line': 'addressLastLine',  # noqa: E501
-        'place_name': 'placeName',  # noqa: E501
-        'area_name1': 'areaName1',  # noqa: E501
-        'area_name2': 'areaName2',  # noqa: E501
-        'area_name3': 'areaName3',  # noqa: E501
-        'area_name4': 'areaName4',  # noqa: E501
-        'post_code1': 'postCode1',  # noqa: E501
-        'post_code2': 'postCode2',  # noqa: E501
-        'country': 'country',  # noqa: E501
-        'address_number': 'addressNumber',  # noqa: E501
-        'street_name': 'streetName',  # noqa: E501
-        'unit_type': 'unitType',  # noqa: E501
-        'unit_value': 'unitValue',  # noqa: E501
-        'custom_fields': 'customFields',  # noqa: E501
+        'pk': 'pk',  # noqa: E501
+        'kg': 'kg',  # noqa: E501
+        'first': 'first',  # noqa: E501
+        'second': 'second',  # noqa: E501
+        'third': 'third',  # noqa: E501
+        'fourth': 'fourth',  # noqa: E501
+        'fifth': 'fifth',  # noqa: E501
+        'sixth': 'sixth',  # noqa: E501
+        'seventh': 'seventh',  # noqa: E501
+        'eighth': 'eighth',  # noqa: E501
+        'ninth': 'ninth',  # noqa: E501
+        'tenth': 'tenth',  # noqa: E501
+        'eleventh': 'eleventh',  # noqa: E501
+        'twelfth': 'twelfth',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """GeocodeAddress - a model defined in OpenAPI
+        """GradeLevelsTaught - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -160,30 +156,28 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            object_id (str): [optional]  # noqa: E501
-            main_address_line (str): [optional]  # noqa: E501
-            address_last_line (str): [optional]  # noqa: E501
-            place_name (str): [optional]  # noqa: E501
-            area_name1 (str): [optional]  # noqa: E501
-            area_name2 (str): [optional]  # noqa: E501
-            area_name3 (str): [optional]  # noqa: E501
-            area_name4 (str): [optional]  # noqa: E501
-            post_code1 (str): [optional]  # noqa: E501
-            post_code2 (str): [optional]  # noqa: E501
-            country (str): [optional]  # noqa: E501
-            address_number (str): [optional]  # noqa: E501
-            street_name (str): [optional]  # noqa: E501
-            unit_type (str): [optional]  # noqa: E501
-            unit_value (str): [optional]  # noqa: E501
-            custom_fields ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)}): [optional]  # noqa: E501
+            pk (str): [optional]  # noqa: E501
+            kg (str): [optional]  # noqa: E501
+            first (str): [optional]  # noqa: E501
+            second (str): [optional]  # noqa: E501
+            third (str): [optional]  # noqa: E501
+            fourth (str): [optional]  # noqa: E501
+            fifth (str): [optional]  # noqa: E501
+            sixth (str): [optional]  # noqa: E501
+            seventh (str): [optional]  # noqa: E501
+            eighth (str): [optional]  # noqa: E501
+            ninth (str): [optional]  # noqa: E501
+            tenth (str): [optional]  # noqa: E501
+            eleventh (str): [optional]  # noqa: E501
+            twelfth (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -224,15 +218,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """GeocodeAddress - a model defined in OpenAPI
+        """GradeLevelsTaught - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -257,30 +251,28 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            object_id (str): [optional]  # noqa: E501
-            main_address_line (str): [optional]  # noqa: E501
-            address_last_line (str): [optional]  # noqa: E501
-            place_name (str): [optional]  # noqa: E501
-            area_name1 (str): [optional]  # noqa: E501
-            area_name2 (str): [optional]  # noqa: E501
-            area_name3 (str): [optional]  # noqa: E501
-            area_name4 (str): [optional]  # noqa: E501
-            post_code1 (str): [optional]  # noqa: E501
-            post_code2 (str): [optional]  # noqa: E501
-            country (str): [optional]  # noqa: E501
-            address_number (str): [optional]  # noqa: E501
-            street_name (str): [optional]  # noqa: E501
-            unit_type (str): [optional]  # noqa: E501
-            unit_value (str): [optional]  # noqa: E501
-            custom_fields ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)}): [optional]  # noqa: E501
+            pk (str): [optional]  # noqa: E501
+            kg (str): [optional]  # noqa: E501
+            first (str): [optional]  # noqa: E501
+            second (str): [optional]  # noqa: E501
+            third (str): [optional]  # noqa: E501
+            fourth (str): [optional]  # noqa: E501
+            fifth (str): [optional]  # noqa: E501
+            sixth (str): [optional]  # noqa: E501
+            seventh (str): [optional]  # noqa: E501
+            eighth (str): [optional]  # noqa: E501
+            ninth (str): [optional]  # noqa: E501
+            tenth (str): [optional]  # noqa: E501
+            eleventh (str): [optional]  # noqa: E501
+            twelfth (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/geocode_preferences.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/geocode_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/geocode_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/geocode_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/geocode_service_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/geocode_service_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/geocode_service_response_list.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/geocode_service_response_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/geolocation_geometry.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/geolocation_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/geometry.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/geometry_crc.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/geometry_crc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/geometry_properties.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/geometry_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/get_city_state_province_api_input.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/get_city_state_province_api_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/get_city_state_province_api_input_row.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/get_city_state_province_api_input_row.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/get_city_state_province_api_options.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/get_city_state_province_api_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/get_city_state_province_api_output.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/get_city_state_province_api_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/get_city_state_province_api_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/get_city_state_province_api_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/get_city_state_province_api_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/get_city_state_province_api_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/get_postal_codes_api_input.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/get_postal_codes_api_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/get_postal_codes_api_input_row.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/get_postal_codes_api_input_row.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/get_postal_codes_api_options.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/get_postal_codes_api_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/get_postal_codes_api_output.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/get_postal_codes_api_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/get_postal_codes_api_output_user_fields.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/get_postal_codes_api_output_user_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/get_postal_codes_api_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/get_postal_codes_api_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/get_postal_codes_api_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/get_postal_codes_api_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/global_ultimate_business.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/global_ultimate_business.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/grade_levels_taught.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/situs_address.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class GradeLevelsTaught(ModelNormal):
+class SitusAddress(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,61 +77,57 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'pk': (str,),  # noqa: E501
-            'kg': (str,),  # noqa: E501
-            'first': (str,),  # noqa: E501
-            'second': (str,),  # noqa: E501
-            'third': (str,),  # noqa: E501
-            'fourth': (str,),  # noqa: E501
-            'fifth': (str,),  # noqa: E501
-            'sixth': (str,),  # noqa: E501
-            'seventh': (str,),  # noqa: E501
-            'eighth': (str,),  # noqa: E501
-            'ninth': (str,),  # noqa: E501
-            'tenth': (str,),  # noqa: E501
-            'eleventh': (str,),  # noqa: E501
-            'twelfth': (str,),  # noqa: E501
+            'main_address_line': (str,),  # noqa: E501
+            'address_number': (str,),  # noqa: E501
+            'street_pre_direction': (str,),  # noqa: E501
+            'street_name': (str,),  # noqa: E501
+            'street_type': (str,),  # noqa: E501
+            'street_post_direction': (str,),  # noqa: E501
+            'unit_type': (str,),  # noqa: E501
+            'unit_value': (str,),  # noqa: E501
+            'city': (str,),  # noqa: E501
+            'state': (str,),  # noqa: E501
+            'post_code1': (str,),  # noqa: E501
+            'post_code2': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'pk': 'pk',  # noqa: E501
-        'kg': 'kg',  # noqa: E501
-        'first': 'first',  # noqa: E501
-        'second': 'second',  # noqa: E501
-        'third': 'third',  # noqa: E501
-        'fourth': 'fourth',  # noqa: E501
-        'fifth': 'fifth',  # noqa: E501
-        'sixth': 'sixth',  # noqa: E501
-        'seventh': 'seventh',  # noqa: E501
-        'eighth': 'eighth',  # noqa: E501
-        'ninth': 'ninth',  # noqa: E501
-        'tenth': 'tenth',  # noqa: E501
-        'eleventh': 'eleventh',  # noqa: E501
-        'twelfth': 'twelfth',  # noqa: E501
+        'main_address_line': 'mainAddressLine',  # noqa: E501
+        'address_number': 'addressNumber',  # noqa: E501
+        'street_pre_direction': 'streetPreDirection',  # noqa: E501
+        'street_name': 'streetName',  # noqa: E501
+        'street_type': 'streetType',  # noqa: E501
+        'street_post_direction': 'streetPostDirection',  # noqa: E501
+        'unit_type': 'unitType',  # noqa: E501
+        'unit_value': 'unitValue',  # noqa: E501
+        'city': 'city',  # noqa: E501
+        'state': 'state',  # noqa: E501
+        'post_code1': 'postCode1',  # noqa: E501
+        'post_code2': 'postCode2',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """GradeLevelsTaught - a model defined in OpenAPI
+        """SitusAddress - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -156,28 +152,26 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            pk (str): [optional]  # noqa: E501
-            kg (str): [optional]  # noqa: E501
-            first (str): [optional]  # noqa: E501
-            second (str): [optional]  # noqa: E501
-            third (str): [optional]  # noqa: E501
-            fourth (str): [optional]  # noqa: E501
-            fifth (str): [optional]  # noqa: E501
-            sixth (str): [optional]  # noqa: E501
-            seventh (str): [optional]  # noqa: E501
-            eighth (str): [optional]  # noqa: E501
-            ninth (str): [optional]  # noqa: E501
-            tenth (str): [optional]  # noqa: E501
-            eleventh (str): [optional]  # noqa: E501
-            twelfth (str): [optional]  # noqa: E501
+            main_address_line (str): [optional]  # noqa: E501
+            address_number (str): [optional]  # noqa: E501
+            street_pre_direction (str): [optional]  # noqa: E501
+            street_name (str): [optional]  # noqa: E501
+            street_type (str): [optional]  # noqa: E501
+            street_post_direction (str): [optional]  # noqa: E501
+            unit_type (str): [optional]  # noqa: E501
+            unit_value (str): [optional]  # noqa: E501
+            city (str): [optional]  # noqa: E501
+            state (str): [optional]  # noqa: E501
+            post_code1 (str): [optional]  # noqa: E501
+            post_code2 (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -218,15 +212,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """GradeLevelsTaught - a model defined in OpenAPI
+        """SitusAddress - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -251,28 +245,26 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            pk (str): [optional]  # noqa: E501
-            kg (str): [optional]  # noqa: E501
-            first (str): [optional]  # noqa: E501
-            second (str): [optional]  # noqa: E501
-            third (str): [optional]  # noqa: E501
-            fourth (str): [optional]  # noqa: E501
-            fifth (str): [optional]  # noqa: E501
-            sixth (str): [optional]  # noqa: E501
-            seventh (str): [optional]  # noqa: E501
-            eighth (str): [optional]  # noqa: E501
-            ninth (str): [optional]  # noqa: E501
-            tenth (str): [optional]  # noqa: E501
-            eleventh (str): [optional]  # noqa: E501
-            twelfth (str): [optional]  # noqa: E501
+            main_address_line (str): [optional]  # noqa: E501
+            address_number (str): [optional]  # noqa: E501
+            street_pre_direction (str): [optional]  # noqa: E501
+            street_name (str): [optional]  # noqa: E501
+            street_type (str): [optional]  # noqa: E501
+            street_post_direction (str): [optional]  # noqa: E501
+            unit_type (str): [optional]  # noqa: E501
+            unit_value (str): [optional]  # noqa: E501
+            city (str): [optional]  # noqa: E501
+            state (str): [optional]  # noqa: E501
+            post_code1 (str): [optional]  # noqa: E501
+            post_code2 (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/greatschools.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/greatschools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/grid.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/health_theme.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/health_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/heating_type.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/heating_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/households_theme.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/households_theme.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/housing_theme.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/housing_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/income_theme.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/income_theme.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/index_variable.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/index_variable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/individual_value_variable.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/individual_value_variable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/interior_wall.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/interior_wall.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/intermediate_points.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/intermediate_points.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/intersection.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/intersection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/intersection_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/intersection_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/ip_info.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/ip_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/ipd.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/ipd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/ipd_tax_by_address_batch_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/ipd_tax_by_address_batch_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/ipd_tax_jurisdiction.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/ipd_tax_jurisdiction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/key_lookup_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/key_lookup_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/keys.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/keys.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/land_use.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/land_use.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/lat_long_fields.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/lat_long_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/life_style_theme.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/life_style_theme.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/loc_code.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/loc_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/local_tax_geometry.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/local_tax_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/local_tax_preferences.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/local_tax_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/location.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/location_time.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/location_time.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/magnitude.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/magnitude.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/match.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/match.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/matched_address.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/matched_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/matrix.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/mcd.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/mcd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/metadata_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/metadata_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/name.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/name.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/neighborhoods_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/neighborhoods_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/network.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/organization_type.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/organization_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/other_rooms.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/other_rooms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/owner_vest_type.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/owner_vest_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/owners.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/owners.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/parent_business.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/parent_business.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/pb_key_address_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/pb_key_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/pb_key_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/pb_key_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/pb_key_response_list.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/pb_key_response_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/pbkey.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/pbkey.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/phone_verification.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/phone_verification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/phone_verification_output.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/phone_verification_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/place.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/place.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/places_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/places_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/poi.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/poi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/poi_boundary.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/poi_boundary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/poi_boundary_address_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/poi_boundary_address_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/poi_boundary_location_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/poi_boundary_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/poi_boundary_locations.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/poi_boundary_locations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/poi_boundary_preferences.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/poi_boundary_preferences.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/poi_boundary_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/poi_boundary_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/poi_classification.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/poi_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/poi_count.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/poi_count.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/poi_count_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/poi_count_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/poiby_geometry_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/poiby_geometry_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/points.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/points.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/pool_type.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/pool_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/population_theme.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/population_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/preferenc_time_zone.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/preferenc_time_zone.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/primary_zone.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/primary_zone.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/prior_sale_code.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/prior_sale_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/prop_site_influene.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/prop_site_influene.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/properties.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/property_attributes.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/property_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/property_geometry.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/property_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/property_info_address_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/property_info_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/property_info_preferences.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/property_info_preferences.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/property_info_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/property_info_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/property_info_responses.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/property_info_responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/proxy.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/psap_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/psap_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/race_and_ethnicity_theme.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/race_and_ethnicity_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/range_variable.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/range_variable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/rate.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/rate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/rate_center_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/rate_center_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/return_fields_descriptor.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/return_fields_descriptor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/reverse_geocode_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/reverse_geocode_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/risk.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/risk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/risk_address.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/risk_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/risk_geometry.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/risk_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/risk_locations.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/risk_locations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/risk_preferences.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/risk_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/risks_boundaries.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/risks_boundaries.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/risks_crime_theme.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/risks_crime_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/risks_geometry_crc.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/risks_geometry_crc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/road.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/road.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/roof_cover_type.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/roof_cover_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/roof_frame_type.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/roof_frame_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/roof_shape_type.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/roof_shape_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/route_direction.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/route_direction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/route_geometry.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/route_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/route_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/route_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/sales_tax.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/sales_tax.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/sales_volume.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/sales_volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/school.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/school.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/school_district.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/school_district.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/school_profile.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/school_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/school_ranking.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/school_ranking.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/schools_near_by_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/schools_near_by_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/segmentation.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/segmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/segmentation_themes.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/segmentation_themes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/shore_line_distance.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/shore_line_distance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/sic.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/sic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/sic_metadata.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/sic_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/site_details.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/site_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/situs_address.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/typeahead_location.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,16 +25,32 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from com.precisely.apis.model.address1 import Address1
+    from com.precisely.apis.model.distance import Distance
+    from com.precisely.apis.model.geometry import Geometry
+    from com.precisely.apis.model.match import Match
+    from com.precisely.apis.model.place import Place
+    from com.precisely.apis.model.poi import Poi
+    from com.precisely.apis.model.typeahead_range import TypeaheadRange
+    globals()['Address1'] = Address1
+    globals()['Distance'] = Distance
+    globals()['Geometry'] = Geometry
+    globals()['Match'] = Match
+    globals()['Place'] = Place
+    globals()['Poi'] = Poi
+    globals()['TypeaheadRange'] = TypeaheadRange
 
-class SitusAddress(ModelNormal):
+
+class TypeaheadLocation(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,72 +78,72 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'main_address_line': (str,),  # noqa: E501
-            'address_number': (str,),  # noqa: E501
-            'street_pre_direction': (str,),  # noqa: E501
-            'street_name': (str,),  # noqa: E501
-            'street_type': (str,),  # noqa: E501
-            'street_post_direction': (str,),  # noqa: E501
-            'unit_type': (str,),  # noqa: E501
-            'unit_value': (str,),  # noqa: E501
-            'city': (str,),  # noqa: E501
-            'state': (str,),  # noqa: E501
-            'post_code1': (str,),  # noqa: E501
-            'post_code2': (str,),  # noqa: E501
+            'dataset': (str,),  # noqa: E501
+            'match': (Match,),  # noqa: E501
+            'address': (Address1,),  # noqa: E501
+            'poi': (Poi,),  # noqa: E501
+            'distance': (Distance,),  # noqa: E501
+            'unit_temp': (str,),  # noqa: E501
+            'value_temp': (str,),  # noqa: E501
+            'geometry': (Geometry,),  # noqa: E501
+            'total_unit_count': (int,),  # noqa: E501
+            'ranges': ([TypeaheadRange],),  # noqa: E501
+            'place': (Place,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'main_address_line': 'mainAddressLine',  # noqa: E501
-        'address_number': 'addressNumber',  # noqa: E501
-        'street_pre_direction': 'streetPreDirection',  # noqa: E501
-        'street_name': 'streetName',  # noqa: E501
-        'street_type': 'streetType',  # noqa: E501
-        'street_post_direction': 'streetPostDirection',  # noqa: E501
-        'unit_type': 'unitType',  # noqa: E501
-        'unit_value': 'unitValue',  # noqa: E501
-        'city': 'city',  # noqa: E501
-        'state': 'state',  # noqa: E501
-        'post_code1': 'postCode1',  # noqa: E501
-        'post_code2': 'postCode2',  # noqa: E501
+        'dataset': 'dataset',  # noqa: E501
+        'match': 'match',  # noqa: E501
+        'address': 'address',  # noqa: E501
+        'poi': 'poi',  # noqa: E501
+        'distance': 'distance',  # noqa: E501
+        'unit_temp': 'unitTemp',  # noqa: E501
+        'value_temp': 'valueTemp',  # noqa: E501
+        'geometry': 'geometry',  # noqa: E501
+        'total_unit_count': 'totalUnitCount',  # noqa: E501
+        'ranges': 'ranges',  # noqa: E501
+        'place': 'place',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SitusAddress - a model defined in OpenAPI
+        """TypeaheadLocation - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -152,26 +168,25 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            main_address_line (str): [optional]  # noqa: E501
-            address_number (str): [optional]  # noqa: E501
-            street_pre_direction (str): [optional]  # noqa: E501
-            street_name (str): [optional]  # noqa: E501
-            street_type (str): [optional]  # noqa: E501
-            street_post_direction (str): [optional]  # noqa: E501
-            unit_type (str): [optional]  # noqa: E501
-            unit_value (str): [optional]  # noqa: E501
-            city (str): [optional]  # noqa: E501
-            state (str): [optional]  # noqa: E501
-            post_code1 (str): [optional]  # noqa: E501
-            post_code2 (str): [optional]  # noqa: E501
+            dataset (str): [optional]  # noqa: E501
+            match (Match): [optional]  # noqa: E501
+            address (Address1): [optional]  # noqa: E501
+            poi (Poi): [optional]  # noqa: E501
+            distance (Distance): [optional]  # noqa: E501
+            unit_temp (str): [optional]  # noqa: E501
+            value_temp (str): [optional]  # noqa: E501
+            geometry (Geometry): [optional]  # noqa: E501
+            total_unit_count (int): [optional]  # noqa: E501
+            ranges ([TypeaheadRange]): [optional]  # noqa: E501
+            place (Place): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -212,15 +227,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SitusAddress - a model defined in OpenAPI
+        """TypeaheadLocation - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -245,26 +260,25 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            main_address_line (str): [optional]  # noqa: E501
-            address_number (str): [optional]  # noqa: E501
-            street_pre_direction (str): [optional]  # noqa: E501
-            street_name (str): [optional]  # noqa: E501
-            street_type (str): [optional]  # noqa: E501
-            street_post_direction (str): [optional]  # noqa: E501
-            unit_type (str): [optional]  # noqa: E501
-            unit_value (str): [optional]  # noqa: E501
-            city (str): [optional]  # noqa: E501
-            state (str): [optional]  # noqa: E501
-            post_code1 (str): [optional]  # noqa: E501
-            post_code2 (str): [optional]  # noqa: E501
+            dataset (str): [optional]  # noqa: E501
+            match (Match): [optional]  # noqa: E501
+            address (Address1): [optional]  # noqa: E501
+            poi (Poi): [optional]  # noqa: E501
+            distance (Distance): [optional]  # noqa: E501
+            unit_temp (str): [optional]  # noqa: E501
+            value_temp (str): [optional]  # noqa: E501
+            geometry (Geometry): [optional]  # noqa: E501
+            total_unit_count (int): [optional]  # noqa: E501
+            ranges ([TypeaheadRange]): [optional]  # noqa: E501
+            place (Place): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/special_purpose_district.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/special_purpose_district.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/special_purpose_district_tax.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/special_purpose_district_tax.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/speed_limit.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/speed_limit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/start_end_point.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/start_end_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/state.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/status.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/stories.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/stories.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/student_ethnicity.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/student_ethnicity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/supply_and_demand_theme.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/supply_and_demand_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/tax_address.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/tax_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/tax_address_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/tax_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/tax_county.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/tax_county.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/tax_district_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/tax_district_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/tax_district_response_list.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/tax_district_response_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/tax_doc_type.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/tax_doc_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/tax_exemption.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/tax_exemption.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/tax_geometry.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/tax_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/tax_jurisdiction.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/tax_jurisdiction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/tax_location_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/tax_location_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/tax_locations.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/tax_locations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/tax_place.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/tax_rate_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,16 +25,30 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from com.precisely.apis.model.census import Census
+    from com.precisely.apis.model.lat_long_fields import LatLongFields
+    from com.precisely.apis.model.sales_tax import SalesTax
+    from com.precisely.apis.model.tax_jurisdiction import TaxJurisdiction
+    from com.precisely.apis.model.tax_rate_matched_address import TaxRateMatchedAddress
+    from com.precisely.apis.model.use_tax import UseTax
+    globals()['Census'] = Census
+    globals()['LatLongFields'] = LatLongFields
+    globals()['SalesTax'] = SalesTax
+    globals()['TaxJurisdiction'] = TaxJurisdiction
+    globals()['TaxRateMatchedAddress'] = TaxRateMatchedAddress
+    globals()['UseTax'] = UseTax
 
-class TaxPlace(ModelNormal):
+
+class TaxRateResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,66 +76,72 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'name': (str,),  # noqa: E501
-            'code': (str,),  # noqa: E501
+            'object_id': (str,),  # noqa: E501
+            'vendor_name': (str,),  # noqa: E501
             'gnis_code': (str,),  # noqa: E501
-            'self_collected': (bool,),  # noqa: E501
-            'class_code': (str,),  # noqa: E501
-            'incorporated_flag': (str,),  # noqa: E501
-            'last_annexed_date': (str,),  # noqa: E501
-            'last_updated_date': (str,),  # noqa: E501
-            'last_verified_date': (str,),  # noqa: E501
+            'confidence': (float,),  # noqa: E501
+            'jurisdiction': (TaxJurisdiction,),  # noqa: E501
+            'matched_address': (TaxRateMatchedAddress,),  # noqa: E501
+            'sales_tax': (SalesTax,),  # noqa: E501
+            'use_tax': (UseTax,),  # noqa: E501
+            'census': (Census,),  # noqa: E501
+            'lat_long_fields': (LatLongFields,),  # noqa: E501
+            'address': (TaxRateMatchedAddress,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
-        'code': 'code',  # noqa: E501
+        'object_id': 'objectId',  # noqa: E501
+        'vendor_name': 'vendorName',  # noqa: E501
         'gnis_code': 'gnisCode',  # noqa: E501
-        'self_collected': 'selfCollected',  # noqa: E501
-        'class_code': 'classCode',  # noqa: E501
-        'incorporated_flag': 'incorporatedFlag',  # noqa: E501
-        'last_annexed_date': 'lastAnnexedDate',  # noqa: E501
-        'last_updated_date': 'lastUpdatedDate',  # noqa: E501
-        'last_verified_date': 'lastVerifiedDate',  # noqa: E501
+        'confidence': 'confidence',  # noqa: E501
+        'jurisdiction': 'jurisdiction',  # noqa: E501
+        'matched_address': 'matchedAddress',  # noqa: E501
+        'sales_tax': 'salesTax',  # noqa: E501
+        'use_tax': 'useTax',  # noqa: E501
+        'census': 'census',  # noqa: E501
+        'lat_long_fields': 'latLongFields',  # noqa: E501
+        'address': 'address',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TaxPlace - a model defined in OpenAPI
+        """TaxRateResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -146,23 +166,25 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            code (str): [optional]  # noqa: E501
+            object_id (str): [optional]  # noqa: E501
+            vendor_name (str): [optional]  # noqa: E501
             gnis_code (str): [optional]  # noqa: E501
-            self_collected (bool): [optional]  # noqa: E501
-            class_code (str): [optional]  # noqa: E501
-            incorporated_flag (str): [optional]  # noqa: E501
-            last_annexed_date (str): [optional]  # noqa: E501
-            last_updated_date (str): [optional]  # noqa: E501
-            last_verified_date (str): [optional]  # noqa: E501
+            confidence (float): [optional]  # noqa: E501
+            jurisdiction (TaxJurisdiction): [optional]  # noqa: E501
+            matched_address (TaxRateMatchedAddress): [optional]  # noqa: E501
+            sales_tax (SalesTax): [optional]  # noqa: E501
+            use_tax (UseTax): [optional]  # noqa: E501
+            census (Census): [optional]  # noqa: E501
+            lat_long_fields (LatLongFields): [optional]  # noqa: E501
+            address (TaxRateMatchedAddress): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -203,15 +225,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TaxPlace - a model defined in OpenAPI
+        """TaxRateResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -236,23 +258,25 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): [optional]  # noqa: E501
-            code (str): [optional]  # noqa: E501
+            object_id (str): [optional]  # noqa: E501
+            vendor_name (str): [optional]  # noqa: E501
             gnis_code (str): [optional]  # noqa: E501
-            self_collected (bool): [optional]  # noqa: E501
-            class_code (str): [optional]  # noqa: E501
-            incorporated_flag (str): [optional]  # noqa: E501
-            last_annexed_date (str): [optional]  # noqa: E501
-            last_updated_date (str): [optional]  # noqa: E501
-            last_verified_date (str): [optional]  # noqa: E501
+            confidence (float): [optional]  # noqa: E501
+            jurisdiction (TaxJurisdiction): [optional]  # noqa: E501
+            matched_address (TaxRateMatchedAddress): [optional]  # noqa: E501
+            sales_tax (SalesTax): [optional]  # noqa: E501
+            use_tax (UseTax): [optional]  # noqa: E501
+            census (Census): [optional]  # noqa: E501
+            lat_long_fields (LatLongFields): [optional]  # noqa: E501
+            address (TaxRateMatchedAddress): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/tax_rate_address.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/tax_rate_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/tax_rate_address_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/tax_rate_address_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/tax_rate_location_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/tax_rate_location_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/tax_rate_matched_address.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/tax_rate_matched_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/tax_rate_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_input_row.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,29 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from com.precisely.apis.model.census import Census
-    from com.precisely.apis.model.lat_long_fields import LatLongFields
-    from com.precisely.apis.model.sales_tax import SalesTax
-    from com.precisely.apis.model.tax_jurisdiction import TaxJurisdiction
-    from com.precisely.apis.model.tax_rate_matched_address import TaxRateMatchedAddress
-    from com.precisely.apis.model.use_tax import UseTax
-    globals()['Census'] = Census
-    globals()['LatLongFields'] = LatLongFields
-    globals()['SalesTax'] = SalesTax
-    globals()['TaxJurisdiction'] = TaxJurisdiction
-    globals()['TaxRateMatchedAddress'] = TaxRateMatchedAddress
-    globals()['UseTax'] = UseTax
+    from com.precisely.apis.model.get_postal_codes_api_output_user_fields import GetPostalCodesAPIOutputUserFields
+    globals()['GetPostalCodesAPIOutputUserFields'] = GetPostalCodesAPIOutputUserFields
 
 
-class TaxRateResponse(ModelNormal):
+class ValidateMailingAddressUSCANAPIInputRow(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -93,55 +83,57 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'object_id': (str,),  # noqa: E501
-            'vendor_name': (str,),  # noqa: E501
-            'gnis_code': (str,),  # noqa: E501
-            'confidence': (float,),  # noqa: E501
-            'jurisdiction': (TaxJurisdiction,),  # noqa: E501
-            'matched_address': (TaxRateMatchedAddress,),  # noqa: E501
-            'sales_tax': (SalesTax,),  # noqa: E501
-            'use_tax': (UseTax,),  # noqa: E501
-            'census': (Census,),  # noqa: E501
-            'lat_long_fields': (LatLongFields,),  # noqa: E501
-            'address': (TaxRateMatchedAddress,),  # noqa: E501
+            'user_fields': ([GetPostalCodesAPIOutputUserFields],),  # noqa: E501
+            'address_line1': (str,),  # noqa: E501
+            'address_line2': (str,),  # noqa: E501
+            'address_line3': (str,),  # noqa: E501
+            'address_line4': (str,),  # noqa: E501
+            'firm_name': (str,),  # noqa: E501
+            'city': (str,),  # noqa: E501
+            'state_province': (str,),  # noqa: E501
+            'country': (str,),  # noqa: E501
+            'postal_code': (str,),  # noqa: E501
+            'us_urban_name': (str,),  # noqa: E501
+            'can_language': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'object_id': 'objectId',  # noqa: E501
-        'vendor_name': 'vendorName',  # noqa: E501
-        'gnis_code': 'gnisCode',  # noqa: E501
-        'confidence': 'confidence',  # noqa: E501
-        'jurisdiction': 'jurisdiction',  # noqa: E501
-        'matched_address': 'matchedAddress',  # noqa: E501
-        'sales_tax': 'salesTax',  # noqa: E501
-        'use_tax': 'useTax',  # noqa: E501
-        'census': 'census',  # noqa: E501
-        'lat_long_fields': 'latLongFields',  # noqa: E501
-        'address': 'address',  # noqa: E501
+        'user_fields': 'user_fields',  # noqa: E501
+        'address_line1': 'AddressLine1',  # noqa: E501
+        'address_line2': 'AddressLine2',  # noqa: E501
+        'address_line3': 'AddressLine3',  # noqa: E501
+        'address_line4': 'AddressLine4',  # noqa: E501
+        'firm_name': 'FirmName',  # noqa: E501
+        'city': 'City',  # noqa: E501
+        'state_province': 'StateProvince',  # noqa: E501
+        'country': 'Country',  # noqa: E501
+        'postal_code': 'PostalCode',  # noqa: E501
+        'us_urban_name': 'USUrbanName',  # noqa: E501
+        'can_language': 'CanLanguage',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TaxRateResponse - a model defined in OpenAPI
+        """ValidateMailingAddressUSCANAPIInputRow - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -166,25 +158,26 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            object_id (str): [optional]  # noqa: E501
-            vendor_name (str): [optional]  # noqa: E501
-            gnis_code (str): [optional]  # noqa: E501
-            confidence (float): [optional]  # noqa: E501
-            jurisdiction (TaxJurisdiction): [optional]  # noqa: E501
-            matched_address (TaxRateMatchedAddress): [optional]  # noqa: E501
-            sales_tax (SalesTax): [optional]  # noqa: E501
-            use_tax (UseTax): [optional]  # noqa: E501
-            census (Census): [optional]  # noqa: E501
-            lat_long_fields (LatLongFields): [optional]  # noqa: E501
-            address (TaxRateMatchedAddress): [optional]  # noqa: E501
+            user_fields ([GetPostalCodesAPIOutputUserFields]): These fields are returned, unmodified, in the user_fields section of the response.. [optional]  # noqa: E501
+            address_line1 (str): The first address line.. [optional]  # noqa: E501
+            address_line2 (str): The second address line.. [optional]  # noqa: E501
+            address_line3 (str): The third address line.. [optional]  # noqa: E501
+            address_line4 (str): The fourth address line.. [optional]  # noqa: E501
+            firm_name (str): The company or firm name.. [optional]  # noqa: E501
+            city (str): The city name.. [optional]  # noqa: E501
+            state_province (str): The state or province.. [optional]  # noqa: E501
+            country (str): The country code or name.. [optional]  # noqa: E501
+            postal_code (str): The postal code for the address.. [optional]  # noqa: E501
+            us_urban_name (str): U.S. address urbanization name. Used primarily for Puerto Rico addresses.. [optional]  # noqa: E501
+            can_language (str): Canadian language.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -225,15 +218,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TaxRateResponse - a model defined in OpenAPI
+        """ValidateMailingAddressUSCANAPIInputRow - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -258,25 +251,26 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            object_id (str): [optional]  # noqa: E501
-            vendor_name (str): [optional]  # noqa: E501
-            gnis_code (str): [optional]  # noqa: E501
-            confidence (float): [optional]  # noqa: E501
-            jurisdiction (TaxJurisdiction): [optional]  # noqa: E501
-            matched_address (TaxRateMatchedAddress): [optional]  # noqa: E501
-            sales_tax (SalesTax): [optional]  # noqa: E501
-            use_tax (UseTax): [optional]  # noqa: E501
-            census (Census): [optional]  # noqa: E501
-            lat_long_fields (LatLongFields): [optional]  # noqa: E501
-            address (TaxRateMatchedAddress): [optional]  # noqa: E501
+            user_fields ([GetPostalCodesAPIOutputUserFields]): These fields are returned, unmodified, in the user_fields section of the response.. [optional]  # noqa: E501
+            address_line1 (str): The first address line.. [optional]  # noqa: E501
+            address_line2 (str): The second address line.. [optional]  # noqa: E501
+            address_line3 (str): The third address line.. [optional]  # noqa: E501
+            address_line4 (str): The fourth address line.. [optional]  # noqa: E501
+            firm_name (str): The company or firm name.. [optional]  # noqa: E501
+            city (str): The city name.. [optional]  # noqa: E501
+            state_province (str): The state or province.. [optional]  # noqa: E501
+            country (str): The country code or name.. [optional]  # noqa: E501
+            postal_code (str): The postal code for the address.. [optional]  # noqa: E501
+            us_urban_name (str): U.S. address urbanization name. Used primarily for Puerto Rico addresses.. [optional]  # noqa: E501
+            can_language (str): Canadian language.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/tax_responses.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/tax_responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/tax_sales_price_code.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/tax_sales_price_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/tax_state.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/tax_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/time.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/time.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/timezone_address_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/timezone_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/timezone_geometry.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/timezone_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/timezone_location_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/timezone_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/timezone_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/timezone_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/timezone_response_list.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/timezone_response_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/travel_boundaries.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/travel_boundaries.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/travel_boundary.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/travel_boundary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/travel_cost_matrix_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/travel_cost_matrix_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/type.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/typeahead_location.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/use_tax.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,31 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from com.precisely.apis.model.address import Address
-    from com.precisely.apis.model.distance import Distance
-    from com.precisely.apis.model.geometry import Geometry
-    from com.precisely.apis.model.match import Match
-    from com.precisely.apis.model.place import Place
-    from com.precisely.apis.model.poi import Poi
-    from com.precisely.apis.model.typeahead_range import TypeaheadRange
-    globals()['Address'] = Address
-    globals()['Distance'] = Distance
-    globals()['Geometry'] = Geometry
-    globals()['Match'] = Match
-    globals()['Place'] = Place
-    globals()['Poi'] = Poi
-    globals()['TypeaheadRange'] = TypeaheadRange
+    from com.precisely.apis.model.special_purpose_district_tax import SpecialPurposeDistrictTax
+    globals()['SpecialPurposeDistrictTax'] = SpecialPurposeDistrictTax
 
 
-class TypeaheadLocation(ModelNormal):
+class UseTax(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -95,55 +83,55 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'dataset': (str,),  # noqa: E501
-            'match': (Match,),  # noqa: E501
-            'address': (Address,),  # noqa: E501
-            'poi': (Poi,),  # noqa: E501
-            'distance': (Distance,),  # noqa: E501
-            'unit_temp': (str,),  # noqa: E501
-            'value_temp': (str,),  # noqa: E501
-            'geometry': (Geometry,),  # noqa: E501
-            'total_unit_count': (int,),  # noqa: E501
-            'ranges': ([TypeaheadRange],),  # noqa: E501
-            'place': (Place,),  # noqa: E501
+            'special_tax_rules_applied': (bool,),  # noqa: E501
+            'special_tax_rules_descriptor': (str,),  # noqa: E501
+            'total_tax_rate': (float,),  # noqa: E501
+            'total_tax_amount': (float,),  # noqa: E501
+            'state_tax_rate': (float,),  # noqa: E501
+            'state_tax_amount': (float,),  # noqa: E501
+            'county_tax_rate': (float,),  # noqa: E501
+            'county_tax_amount': (float,),  # noqa: E501
+            'municipal_tax_rate': (float,),  # noqa: E501
+            'municipal_tax_amount': (float,),  # noqa: E501
+            'spds_tax': ([SpecialPurposeDistrictTax],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'dataset': 'dataset',  # noqa: E501
-        'match': 'match',  # noqa: E501
-        'address': 'address',  # noqa: E501
-        'poi': 'poi',  # noqa: E501
-        'distance': 'distance',  # noqa: E501
-        'unit_temp': 'unitTemp',  # noqa: E501
-        'value_temp': 'valueTemp',  # noqa: E501
-        'geometry': 'geometry',  # noqa: E501
-        'total_unit_count': 'totalUnitCount',  # noqa: E501
-        'ranges': 'ranges',  # noqa: E501
-        'place': 'place',  # noqa: E501
+        'special_tax_rules_applied': 'specialTaxRulesApplied',  # noqa: E501
+        'special_tax_rules_descriptor': 'specialTaxRulesDescriptor',  # noqa: E501
+        'total_tax_rate': 'totalTaxRate',  # noqa: E501
+        'total_tax_amount': 'totalTaxAmount',  # noqa: E501
+        'state_tax_rate': 'stateTaxRate',  # noqa: E501
+        'state_tax_amount': 'stateTaxAmount',  # noqa: E501
+        'county_tax_rate': 'countyTaxRate',  # noqa: E501
+        'county_tax_amount': 'countyTaxAmount',  # noqa: E501
+        'municipal_tax_rate': 'municipalTaxRate',  # noqa: E501
+        'municipal_tax_amount': 'municipalTaxAmount',  # noqa: E501
+        'spds_tax': 'spdsTax',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TypeaheadLocation - a model defined in OpenAPI
+        """UseTax - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -168,25 +156,25 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            dataset (str): [optional]  # noqa: E501
-            match (Match): [optional]  # noqa: E501
-            address (Address): [optional]  # noqa: E501
-            poi (Poi): [optional]  # noqa: E501
-            distance (Distance): [optional]  # noqa: E501
-            unit_temp (str): [optional]  # noqa: E501
-            value_temp (str): [optional]  # noqa: E501
-            geometry (Geometry): [optional]  # noqa: E501
-            total_unit_count (int): [optional]  # noqa: E501
-            ranges ([TypeaheadRange]): [optional]  # noqa: E501
-            place (Place): [optional]  # noqa: E501
+            special_tax_rules_applied (bool): [optional]  # noqa: E501
+            special_tax_rules_descriptor (str): [optional]  # noqa: E501
+            total_tax_rate (float): [optional]  # noqa: E501
+            total_tax_amount (float): [optional]  # noqa: E501
+            state_tax_rate (float): [optional]  # noqa: E501
+            state_tax_amount (float): [optional]  # noqa: E501
+            county_tax_rate (float): [optional]  # noqa: E501
+            county_tax_amount (float): [optional]  # noqa: E501
+            municipal_tax_rate (float): [optional]  # noqa: E501
+            municipal_tax_amount (float): [optional]  # noqa: E501
+            spds_tax ([SpecialPurposeDistrictTax]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -227,15 +215,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TypeaheadLocation - a model defined in OpenAPI
+        """UseTax - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -260,25 +248,25 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            dataset (str): [optional]  # noqa: E501
-            match (Match): [optional]  # noqa: E501
-            address (Address): [optional]  # noqa: E501
-            poi (Poi): [optional]  # noqa: E501
-            distance (Distance): [optional]  # noqa: E501
-            unit_temp (str): [optional]  # noqa: E501
-            value_temp (str): [optional]  # noqa: E501
-            geometry (Geometry): [optional]  # noqa: E501
-            total_unit_count (int): [optional]  # noqa: E501
-            ranges ([TypeaheadRange]): [optional]  # noqa: E501
-            place (Place): [optional]  # noqa: E501
+            special_tax_rules_applied (bool): [optional]  # noqa: E501
+            special_tax_rules_descriptor (str): [optional]  # noqa: E501
+            total_tax_rate (float): [optional]  # noqa: E501
+            total_tax_amount (float): [optional]  # noqa: E501
+            state_tax_rate (float): [optional]  # noqa: E501
+            state_tax_amount (float): [optional]  # noqa: E501
+            county_tax_rate (float): [optional]  # noqa: E501
+            county_tax_amount (float): [optional]  # noqa: E501
+            municipal_tax_rate (float): [optional]  # noqa: E501
+            municipal_tax_amount (float): [optional]  # noqa: E501
+            spds_tax ([SpecialPurposeDistrictTax]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/typeahead_locations.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/typeahead_locations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/typeahead_range.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/typeahead_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/typeahead_unit.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/typeahead_unit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -79,24 +79,26 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'unit_info': (str,),  # noqa: E501
             'formatted_unit_address': (str,),  # noqa: E501
+            'postal_verified': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'unit_info': 'unitInfo',  # noqa: E501
         'formatted_unit_address': 'formattedUnitAddress',  # noqa: E501
+        'postal_verified': 'postalVerified',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -134,14 +136,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             unit_info (str): [optional]  # noqa: E501
             formatted_unit_address (str): [optional]  # noqa: E501
+            postal_verified (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -217,14 +220,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             unit_info (str): [optional]  # noqa: E501
             formatted_unit_address (str): [optional]  # noqa: E501
+            postal_verified (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/unit.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/use_tax.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_output.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from com.precisely.apis.model.special_purpose_district_tax import SpecialPurposeDistrictTax
-    globals()['SpecialPurposeDistrictTax'] = SpecialPurposeDistrictTax
+    from com.precisely.apis.model.get_postal_codes_api_output_user_fields import GetPostalCodesAPIOutputUserFields
+    globals()['GetPostalCodesAPIOutputUserFields'] = GetPostalCodesAPIOutputUserFields
 
 
-class UseTax(ModelNormal):
+class ValidateMailingAddressOutput(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,55 +83,63 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'special_tax_rules_applied': (bool,),  # noqa: E501
-            'special_tax_rules_descriptor': (str,),  # noqa: E501
-            'total_tax_rate': (float,),  # noqa: E501
-            'total_tax_amount': (float,),  # noqa: E501
-            'state_tax_rate': (float,),  # noqa: E501
-            'state_tax_amount': (float,),  # noqa: E501
-            'county_tax_rate': (float,),  # noqa: E501
-            'county_tax_amount': (float,),  # noqa: E501
-            'municipal_tax_rate': (float,),  # noqa: E501
-            'municipal_tax_amount': (float,),  # noqa: E501
-            'spds_tax': ([SpecialPurposeDistrictTax],),  # noqa: E501
+            'user_fields': ([GetPostalCodesAPIOutputUserFields],),  # noqa: E501
+            'address_line1': (str,),  # noqa: E501
+            'address_line2': (str,),  # noqa: E501
+            'firm_name': (str,),  # noqa: E501
+            'city': (str,),  # noqa: E501
+            'postal_code': (str,),  # noqa: E501
+            'country': (str,),  # noqa: E501
+            'state_province': (str,),  # noqa: E501
+            'block_address': (str,),  # noqa: E501
+            'additional_input_data': (str,),  # noqa: E501
+            'postal_code_base': (str,),  # noqa: E501
+            'postal_code_add_on': (str,),  # noqa: E501
+            'status': (str,),  # noqa: E501
+            'status_code': (str,),  # noqa: E501
+            'status_description': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'special_tax_rules_applied': 'specialTaxRulesApplied',  # noqa: E501
-        'special_tax_rules_descriptor': 'specialTaxRulesDescriptor',  # noqa: E501
-        'total_tax_rate': 'totalTaxRate',  # noqa: E501
-        'total_tax_amount': 'totalTaxAmount',  # noqa: E501
-        'state_tax_rate': 'stateTaxRate',  # noqa: E501
-        'state_tax_amount': 'stateTaxAmount',  # noqa: E501
-        'county_tax_rate': 'countyTaxRate',  # noqa: E501
-        'county_tax_amount': 'countyTaxAmount',  # noqa: E501
-        'municipal_tax_rate': 'municipalTaxRate',  # noqa: E501
-        'municipal_tax_amount': 'municipalTaxAmount',  # noqa: E501
-        'spds_tax': 'spdsTax',  # noqa: E501
+        'user_fields': 'user_fields',  # noqa: E501
+        'address_line1': 'AddressLine1',  # noqa: E501
+        'address_line2': 'AddressLine2',  # noqa: E501
+        'firm_name': 'FirmName',  # noqa: E501
+        'city': 'City',  # noqa: E501
+        'postal_code': 'PostalCode',  # noqa: E501
+        'country': 'Country',  # noqa: E501
+        'state_province': 'StateProvince',  # noqa: E501
+        'block_address': 'BlockAddress',  # noqa: E501
+        'additional_input_data': 'AdditionalInputData',  # noqa: E501
+        'postal_code_base': 'PostalCode.Base',  # noqa: E501
+        'postal_code_add_on': 'PostalCode.AddOn',  # noqa: E501
+        'status': 'Status',  # noqa: E501
+        'status_code': 'Status.Code',  # noqa: E501
+        'status_description': 'Status.Description',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UseTax - a model defined in OpenAPI
+        """ValidateMailingAddressOutput - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -156,25 +164,29 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            special_tax_rules_applied (bool): [optional]  # noqa: E501
-            special_tax_rules_descriptor (str): [optional]  # noqa: E501
-            total_tax_rate (float): [optional]  # noqa: E501
-            total_tax_amount (float): [optional]  # noqa: E501
-            state_tax_rate (float): [optional]  # noqa: E501
-            state_tax_amount (float): [optional]  # noqa: E501
-            county_tax_rate (float): [optional]  # noqa: E501
-            county_tax_amount (float): [optional]  # noqa: E501
-            municipal_tax_rate (float): [optional]  # noqa: E501
-            municipal_tax_amount (float): [optional]  # noqa: E501
-            spds_tax ([SpecialPurposeDistrictTax]): [optional]  # noqa: E501
+            user_fields ([GetPostalCodesAPIOutputUserFields]): These fields are returned, unmodified, in the user_fields section of the response.. [optional]  # noqa: E501
+            address_line1 (str): The first line of the validated address.. [optional]  # noqa: E501
+            address_line2 (str): The second line of the validated address.. [optional]  # noqa: E501
+            firm_name (str): The validated firm or company name.. [optional]  # noqa: E501
+            city (str): The validated city name.. [optional]  # noqa: E501
+            postal_code (str): The validated ZIP Code or postal code.. [optional]  # noqa: E501
+            country (str): The country name in English.. [optional]  # noqa: E501
+            state_province (str): The validated state or province abbreviation.. [optional]  # noqa: E501
+            block_address (str): The formatted address, as it would appear on a physical mail piece.. [optional]  # noqa: E501
+            additional_input_data (str): Input data not used by the address validation process.. [optional]  # noqa: E501
+            postal_code_base (str): The 5-digit ZIP Code.. [optional]  # noqa: E501
+            postal_code_add_on (str): The 4-digit add-on part of the ZIP Code.. [optional]  # noqa: E501
+            status (str): Reports the success or failure of the match attempt.. [optional]  # noqa: E501
+            status_code (str): Reason for failure, if there is one.. [optional]  # noqa: E501
+            status_description (str): Description of the problem, if there is one.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -215,15 +227,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """UseTax - a model defined in OpenAPI
+        """ValidateMailingAddressOutput - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -248,25 +260,29 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            special_tax_rules_applied (bool): [optional]  # noqa: E501
-            special_tax_rules_descriptor (str): [optional]  # noqa: E501
-            total_tax_rate (float): [optional]  # noqa: E501
-            total_tax_amount (float): [optional]  # noqa: E501
-            state_tax_rate (float): [optional]  # noqa: E501
-            state_tax_amount (float): [optional]  # noqa: E501
-            county_tax_rate (float): [optional]  # noqa: E501
-            county_tax_amount (float): [optional]  # noqa: E501
-            municipal_tax_rate (float): [optional]  # noqa: E501
-            municipal_tax_amount (float): [optional]  # noqa: E501
-            spds_tax ([SpecialPurposeDistrictTax]): [optional]  # noqa: E501
+            user_fields ([GetPostalCodesAPIOutputUserFields]): These fields are returned, unmodified, in the user_fields section of the response.. [optional]  # noqa: E501
+            address_line1 (str): The first line of the validated address.. [optional]  # noqa: E501
+            address_line2 (str): The second line of the validated address.. [optional]  # noqa: E501
+            firm_name (str): The validated firm or company name.. [optional]  # noqa: E501
+            city (str): The validated city name.. [optional]  # noqa: E501
+            postal_code (str): The validated ZIP Code or postal code.. [optional]  # noqa: E501
+            country (str): The country name in English.. [optional]  # noqa: E501
+            state_province (str): The validated state or province abbreviation.. [optional]  # noqa: E501
+            block_address (str): The formatted address, as it would appear on a physical mail piece.. [optional]  # noqa: E501
+            additional_input_data (str): Input data not used by the address validation process.. [optional]  # noqa: E501
+            postal_code_base (str): The 5-digit ZIP Code.. [optional]  # noqa: E501
+            postal_code_add_on (str): The 4-digit add-on part of the ZIP Code.. [optional]  # noqa: E501
+            status (str): Reports the success or failure of the match attempt.. [optional]  # noqa: E501
+            status_code (str): Reason for failure, if there is one.. [optional]  # noqa: E501
+            status_description (str): Description of the problem, if there is one.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/vacancy.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/vacancy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_email_address_api_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_email_address_api_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_email_address_api_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_email_address_api_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_email_address_input.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_email_address_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_email_address_input_row.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_email_address_input_row.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_email_address_output.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_email_address_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_input.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_input_row.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_input_row.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_options.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_output.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/zones_poi.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,19 +26,25 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from com.precisely.apis.model.get_postal_codes_api_output_user_fields import GetPostalCodesAPIOutputUserFields
-    globals()['GetPostalCodesAPIOutputUserFields'] = GetPostalCodesAPIOutputUserFields
+    from com.precisely.apis.model.employee_count import EmployeeCount
+    from com.precisely.apis.model.zones_contact_details import ZonesContactDetails
+    from com.precisely.apis.model.zones_parent_business import ZonesParentBusiness
+    from com.precisely.apis.model.zones_poi_classification import ZonesPoiClassification
+    globals()['EmployeeCount'] = EmployeeCount
+    globals()['ZonesContactDetails'] = ZonesContactDetails
+    globals()['ZonesParentBusiness'] = ZonesParentBusiness
+    globals()['ZonesPoiClassification'] = ZonesPoiClassification
 
 
-class ValidateMailingAddressOutput(ModelNormal):
+class ZonesPoi(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,63 +89,61 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'user_fields': ([GetPostalCodesAPIOutputUserFields],),  # noqa: E501
-            'address_line1': (str,),  # noqa: E501
-            'address_line2': (str,),  # noqa: E501
-            'firm_name': (str,),  # noqa: E501
-            'city': (str,),  # noqa: E501
-            'postal_code': (str,),  # noqa: E501
-            'country': (str,),  # noqa: E501
-            'state_province': (str,),  # noqa: E501
-            'block_address': (str,),  # noqa: E501
-            'additional_input_data': (str,),  # noqa: E501
-            'postal_code_base': (str,),  # noqa: E501
-            'postal_code_add_on': (str,),  # noqa: E501
-            'status': (str,),  # noqa: E501
-            'status_code': (str,),  # noqa: E501
-            'status_description': (str,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'brand_name': (str,),  # noqa: E501
+            'trade_name': (str,),  # noqa: E501
+            'franchise_name': (str,),  # noqa: E501
+            'open24_hours': (str,),  # noqa: E501
+            'contact_details': (ZonesContactDetails,),  # noqa: E501
+            'poi_classification': (ZonesPoiClassification,),  # noqa: E501
+            'employee_count': (EmployeeCount,),  # noqa: E501
+            'organization_status_code': (str,),  # noqa: E501
+            'organization_status_code_description': (str,),  # noqa: E501
+            'parent_business': (ZonesParentBusiness,),  # noqa: E501
+            'ticker_symbol': (str,),  # noqa: E501
+            'exchange_name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'user_fields': 'user_fields',  # noqa: E501
-        'address_line1': 'AddressLine1',  # noqa: E501
-        'address_line2': 'AddressLine2',  # noqa: E501
-        'firm_name': 'FirmName',  # noqa: E501
-        'city': 'City',  # noqa: E501
-        'postal_code': 'PostalCode',  # noqa: E501
-        'country': 'Country',  # noqa: E501
-        'state_province': 'StateProvince',  # noqa: E501
-        'block_address': 'BlockAddress',  # noqa: E501
-        'additional_input_data': 'AdditionalInputData',  # noqa: E501
-        'postal_code_base': 'PostalCode.Base',  # noqa: E501
-        'postal_code_add_on': 'PostalCode.AddOn',  # noqa: E501
-        'status': 'Status',  # noqa: E501
-        'status_code': 'Status.Code',  # noqa: E501
-        'status_description': 'Status.Description',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'brand_name': 'brandName',  # noqa: E501
+        'trade_name': 'tradeName',  # noqa: E501
+        'franchise_name': 'franchiseName',  # noqa: E501
+        'open24_hours': 'open24Hours',  # noqa: E501
+        'contact_details': 'contactDetails',  # noqa: E501
+        'poi_classification': 'poiClassification',  # noqa: E501
+        'employee_count': 'employeeCount',  # noqa: E501
+        'organization_status_code': 'organizationStatusCode',  # noqa: E501
+        'organization_status_code_description': 'organizationStatusCodeDescription',  # noqa: E501
+        'parent_business': 'parentBusiness',  # noqa: E501
+        'ticker_symbol': 'tickerSymbol',  # noqa: E501
+        'exchange_name': 'exchangeName',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ValidateMailingAddressOutput - a model defined in OpenAPI
+        """ZonesPoi - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -164,29 +168,28 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            user_fields ([GetPostalCodesAPIOutputUserFields]): These fields are returned, unmodified, in the user_fields section of the response.. [optional]  # noqa: E501
-            address_line1 (str): The first line of the validated address.. [optional]  # noqa: E501
-            address_line2 (str): The second line of the validated address.. [optional]  # noqa: E501
-            firm_name (str): The validated firm or company name.. [optional]  # noqa: E501
-            city (str): The validated city name.. [optional]  # noqa: E501
-            postal_code (str): The validated ZIP Code or postal code.. [optional]  # noqa: E501
-            country (str): The country name in English.. [optional]  # noqa: E501
-            state_province (str): The validated state or province abbreviation.. [optional]  # noqa: E501
-            block_address (str): The formatted address, as it would appear on a physical mail piece.. [optional]  # noqa: E501
-            additional_input_data (str): Input data not used by the address validation process.. [optional]  # noqa: E501
-            postal_code_base (str): The 5-digit ZIP Code.. [optional]  # noqa: E501
-            postal_code_add_on (str): The 4-digit add-on part of the ZIP Code.. [optional]  # noqa: E501
-            status (str): Reports the success or failure of the match attempt.. [optional]  # noqa: E501
-            status_code (str): Reason for failure, if there is one.. [optional]  # noqa: E501
-            status_description (str): Description of the problem, if there is one.. [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            brand_name (str): [optional]  # noqa: E501
+            trade_name (str): [optional]  # noqa: E501
+            franchise_name (str): [optional]  # noqa: E501
+            open24_hours (str): [optional]  # noqa: E501
+            contact_details (ZonesContactDetails): [optional]  # noqa: E501
+            poi_classification (ZonesPoiClassification): [optional]  # noqa: E501
+            employee_count (EmployeeCount): [optional]  # noqa: E501
+            organization_status_code (str): [optional]  # noqa: E501
+            organization_status_code_description (str): [optional]  # noqa: E501
+            parent_business (ZonesParentBusiness): [optional]  # noqa: E501
+            ticker_symbol (str): [optional]  # noqa: E501
+            exchange_name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -227,15 +230,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ValidateMailingAddressOutput - a model defined in OpenAPI
+        """ZonesPoi - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -260,29 +263,28 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            user_fields ([GetPostalCodesAPIOutputUserFields]): These fields are returned, unmodified, in the user_fields section of the response.. [optional]  # noqa: E501
-            address_line1 (str): The first line of the validated address.. [optional]  # noqa: E501
-            address_line2 (str): The second line of the validated address.. [optional]  # noqa: E501
-            firm_name (str): The validated firm or company name.. [optional]  # noqa: E501
-            city (str): The validated city name.. [optional]  # noqa: E501
-            postal_code (str): The validated ZIP Code or postal code.. [optional]  # noqa: E501
-            country (str): The country name in English.. [optional]  # noqa: E501
-            state_province (str): The validated state or province abbreviation.. [optional]  # noqa: E501
-            block_address (str): The formatted address, as it would appear on a physical mail piece.. [optional]  # noqa: E501
-            additional_input_data (str): Input data not used by the address validation process.. [optional]  # noqa: E501
-            postal_code_base (str): The 5-digit ZIP Code.. [optional]  # noqa: E501
-            postal_code_add_on (str): The 4-digit add-on part of the ZIP Code.. [optional]  # noqa: E501
-            status (str): Reports the success or failure of the match attempt.. [optional]  # noqa: E501
-            status_code (str): Reason for failure, if there is one.. [optional]  # noqa: E501
-            status_description (str): Description of the problem, if there is one.. [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            brand_name (str): [optional]  # noqa: E501
+            trade_name (str): [optional]  # noqa: E501
+            franchise_name (str): [optional]  # noqa: E501
+            open24_hours (str): [optional]  # noqa: E501
+            contact_details (ZonesContactDetails): [optional]  # noqa: E501
+            poi_classification (ZonesPoiClassification): [optional]  # noqa: E501
+            employee_count (EmployeeCount): [optional]  # noqa: E501
+            organization_status_code (str): [optional]  # noqa: E501
+            organization_status_code_description (str): [optional]  # noqa: E501
+            parent_business (ZonesParentBusiness): [optional]  # noqa: E501
+            ticker_symbol (str): [optional]  # noqa: E501
+            exchange_name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_premium_input.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_premium_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_premium_input_row.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_premium_input_row.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_premium_options.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_premium_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_premium_output.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_premium_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_premium_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_premium_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_premium_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_premium_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_pro_input.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_pro_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_pro_input_row.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_pro_input_row.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_pro_options.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_pro_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_pro_output.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_pro_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_pro_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_pro_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_pro_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_pro_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_input.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_input_row.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/zones_sic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from com.precisely.apis.model.get_postal_codes_api_output_user_fields import GetPostalCodesAPIOutputUserFields
-    globals()['GetPostalCodesAPIOutputUserFields'] = GetPostalCodesAPIOutputUserFields
 
-
-class ValidateMailingAddressUSCANAPIInputRow(ModelNormal):
+class ZonesSic(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -66,74 +62,56 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'user_fields': ([GetPostalCodesAPIOutputUserFields],),  # noqa: E501
-            'address_line1': (str,),  # noqa: E501
-            'address_line2': (str,),  # noqa: E501
-            'address_line3': (str,),  # noqa: E501
-            'address_line4': (str,),  # noqa: E501
-            'firm_name': (str,),  # noqa: E501
-            'city': (str,),  # noqa: E501
-            'state_province': (str,),  # noqa: E501
-            'country': (str,),  # noqa: E501
-            'postal_code': (str,),  # noqa: E501
-            'us_urban_name': (str,),  # noqa: E501
-            'can_language': (str,),  # noqa: E501
+            'business_line': (str,),  # noqa: E501
+            'sic_code': (str,),  # noqa: E501
+            'sic_code_description': (str,),  # noqa: E501
+            'primary_sic_code': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'user_fields': 'user_fields',  # noqa: E501
-        'address_line1': 'AddressLine1',  # noqa: E501
-        'address_line2': 'AddressLine2',  # noqa: E501
-        'address_line3': 'AddressLine3',  # noqa: E501
-        'address_line4': 'AddressLine4',  # noqa: E501
-        'firm_name': 'FirmName',  # noqa: E501
-        'city': 'City',  # noqa: E501
-        'state_province': 'StateProvince',  # noqa: E501
-        'country': 'Country',  # noqa: E501
-        'postal_code': 'PostalCode',  # noqa: E501
-        'us_urban_name': 'USUrbanName',  # noqa: E501
-        'can_language': 'CanLanguage',  # noqa: E501
+        'business_line': 'businessLine',  # noqa: E501
+        'sic_code': 'sicCode',  # noqa: E501
+        'sic_code_description': 'sicCodeDescription',  # noqa: E501
+        'primary_sic_code': 'primarySicCode',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ValidateMailingAddressUSCANAPIInputRow - a model defined in OpenAPI
+        """ZonesSic - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -158,26 +136,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            user_fields ([GetPostalCodesAPIOutputUserFields]): These fields are returned, unmodified, in the user_fields section of the response.. [optional]  # noqa: E501
-            address_line1 (str): The first address line.. [optional]  # noqa: E501
-            address_line2 (str): The second address line.. [optional]  # noqa: E501
-            address_line3 (str): The third address line.. [optional]  # noqa: E501
-            address_line4 (str): The fourth address line.. [optional]  # noqa: E501
-            firm_name (str): The company or firm name.. [optional]  # noqa: E501
-            city (str): The city name.. [optional]  # noqa: E501
-            state_province (str): The state or province.. [optional]  # noqa: E501
-            country (str): The country code or name.. [optional]  # noqa: E501
-            postal_code (str): The postal code for the address.. [optional]  # noqa: E501
-            us_urban_name (str): U.S. address urbanization name. Used primarily for Puerto Rico addresses.. [optional]  # noqa: E501
-            can_language (str): Canadian language.. [optional]  # noqa: E501
+            business_line (str): [optional]  # noqa: E501
+            sic_code (str): [optional]  # noqa: E501
+            sic_code_description (str): [optional]  # noqa: E501
+            primary_sic_code (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -218,15 +188,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ValidateMailingAddressUSCANAPIInputRow - a model defined in OpenAPI
+        """ZonesSic - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -251,26 +221,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            user_fields ([GetPostalCodesAPIOutputUserFields]): These fields are returned, unmodified, in the user_fields section of the response.. [optional]  # noqa: E501
-            address_line1 (str): The first address line.. [optional]  # noqa: E501
-            address_line2 (str): The second address line.. [optional]  # noqa: E501
-            address_line3 (str): The third address line.. [optional]  # noqa: E501
-            address_line4 (str): The fourth address line.. [optional]  # noqa: E501
-            firm_name (str): The company or firm name.. [optional]  # noqa: E501
-            city (str): The city name.. [optional]  # noqa: E501
-            state_province (str): The state or province.. [optional]  # noqa: E501
-            country (str): The country code or name.. [optional]  # noqa: E501
-            postal_code (str): The postal code for the address.. [optional]  # noqa: E501
-            us_urban_name (str): U.S. address urbanization name. Used primarily for Puerto Rico addresses.. [optional]  # noqa: E501
-            can_language (str): Canadian language.. [optional]  # noqa: E501
+            business_line (str): [optional]  # noqa: E501
+            sic_code (str): [optional]  # noqa: E501
+            sic_code_description (str): [optional]  # noqa: E501
+            primary_sic_code (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_options.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_output.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_phone_number_api_request.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_phone_number_api_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_phone_number_api_request_input.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_phone_number_api_request_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/validate_phone_number_api_request_input_row.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/validate_phone_number_api_request_input_row.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/water_body.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/water_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/water_body_response.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/water_body_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/zones_address.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/zones_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/zones_boundary_geometry.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/zones_boundary_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/zones_contact_details.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/zones_contact_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/zones_geometry.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/zones_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/zones_parent_business.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/zones_parent_business.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/zones_poi.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/geocode_address.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,319 +1,315 @@
-"""
-    Precisely APIs
-
-    Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
-
-    The version of the OpenAPI document: 16.0.0
-    Generated by: https://openapi-generator.tech
-"""
-
-
-import re  # noqa: F401
-import sys  # noqa: F401
-
-from com.precisely.apis.model_utils import (  # noqa: F401
-    ApiTypeError,
-    ModelComposed,
-    ModelNormal,
-    ModelSimple,
-    cached_property,
-    change_keys_js_to_python,
-    convert_js_args_to_python_args,
-    date,
-    datetime,
-    file_type,
-    none_type,
-    validate_get_composed_info,
-    OpenApiModel
-)
-from com.precisely.apis.exceptions import ApiAttributeError
-
-
-def lazy_import():
-    from com.precisely.apis.model.employee_count import EmployeeCount
-    from com.precisely.apis.model.zones_contact_details import ZonesContactDetails
-    from com.precisely.apis.model.zones_parent_business import ZonesParentBusiness
-    from com.precisely.apis.model.zones_poi_classification import ZonesPoiClassification
-    globals()['EmployeeCount'] = EmployeeCount
-    globals()['ZonesContactDetails'] = ZonesContactDetails
-    globals()['ZonesParentBusiness'] = ZonesParentBusiness
-    globals()['ZonesPoiClassification'] = ZonesPoiClassification
-
-
-class ZonesPoi(ModelNormal):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-
-    Attributes:
-      allowed_values (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          with a capitalized key describing the allowed value and an allowed
-          value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
-      validations (dict): The key is the tuple path to the attribute
-          and the for var_name this is (var_name,). The value is a dict
-          that stores validations for max_length, min_length, max_items,
-          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
-          inclusive_minimum, and regex.
-      additional_properties_type (tuple): A tuple of classes accepted
-          as additional properties values.
-    """
-
-    allowed_values = {
-    }
-
-    validations = {
-    }
-
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
-
-    _nullable = False
-
-    @cached_property
-    def openapi_types():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-
-        Returns
-            openapi_types (dict): The key is attribute name
-                and the value is attribute type.
-        """
-        lazy_import()
-        return {
-            'id': (str,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'brand_name': (str,),  # noqa: E501
-            'trade_name': (str,),  # noqa: E501
-            'franchise_name': (str,),  # noqa: E501
-            'open24_hours': (str,),  # noqa: E501
-            'contact_details': (ZonesContactDetails,),  # noqa: E501
-            'poi_classification': (ZonesPoiClassification,),  # noqa: E501
-            'employee_count': (EmployeeCount,),  # noqa: E501
-            'organization_status_code': (str,),  # noqa: E501
-            'organization_status_code_description': (str,),  # noqa: E501
-            'parent_business': (ZonesParentBusiness,),  # noqa: E501
-            'ticker_symbol': (str,),  # noqa: E501
-            'exchange_name': (str,),  # noqa: E501
-        }
-
-    @cached_property
-    def discriminator():
-        return None
-
-
-    attribute_map = {
-        'id': 'id',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'brand_name': 'brandName',  # noqa: E501
-        'trade_name': 'tradeName',  # noqa: E501
-        'franchise_name': 'franchiseName',  # noqa: E501
-        'open24_hours': 'open24Hours',  # noqa: E501
-        'contact_details': 'contactDetails',  # noqa: E501
-        'poi_classification': 'poiClassification',  # noqa: E501
-        'employee_count': 'employeeCount',  # noqa: E501
-        'organization_status_code': 'organizationStatusCode',  # noqa: E501
-        'organization_status_code_description': 'organizationStatusCodeDescription',  # noqa: E501
-        'parent_business': 'parentBusiness',  # noqa: E501
-        'ticker_symbol': 'tickerSymbol',  # noqa: E501
-        'exchange_name': 'exchangeName',  # noqa: E501
-    }
-
-    read_only_vars = {
-    }
-
-    _composed_schemas = {}
-
-    @classmethod
-    @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ZonesPoi - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            brand_name (str): [optional]  # noqa: E501
-            trade_name (str): [optional]  # noqa: E501
-            franchise_name (str): [optional]  # noqa: E501
-            open24_hours (str): [optional]  # noqa: E501
-            contact_details (ZonesContactDetails): [optional]  # noqa: E501
-            poi_classification (ZonesPoiClassification): [optional]  # noqa: E501
-            employee_count (EmployeeCount): [optional]  # noqa: E501
-            organization_status_code (str): [optional]  # noqa: E501
-            organization_status_code_description (str): [optional]  # noqa: E501
-            parent_business (ZonesParentBusiness): [optional]  # noqa: E501
-            ticker_symbol (str): [optional]  # noqa: E501
-            exchange_name (str): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        self = super(OpenApiModel, cls).__new__(cls)
-
-        if args:
-            raise ApiTypeError(
-                "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                    args,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-        return self
-
-    required_properties = set([
-        '_data_store',
-        '_check_type',
-        '_spec_property_naming',
-        '_path_to_item',
-        '_configuration',
-        '_visited_composed_classes',
-    ])
-
-    @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """ZonesPoi - a model defined in OpenAPI
-
-        Keyword Args:
-            _check_type (bool): if True, values for parameters in openapi_types
-                                will be type checked and a TypeError will be
-                                raised if the wrong type is input.
-                                Defaults to True
-            _path_to_item (tuple/list): This is a list of keys or values to
-                                drill down to the model in received_data
-                                when deserializing a response
-            _spec_property_naming (bool): True if the variable names in the input data
-                                are serialized names, as specified in the OpenAPI document.
-                                False if the variable names in the input data
-                                are pythonic names, e.g. snake case (default)
-            _configuration (Configuration): the instance to use when
-                                deserializing a file_type parameter.
-                                If passed, type conversion is attempted
-                                If omitted no type conversion is done.
-            _visited_composed_classes (tuple): This stores a tuple of
-                                classes that we have traveled through so that
-                                if we see that class again we will not use its
-                                discriminator again.
-                                When traveling through a discriminator, the
-                                composed schema that is
-                                is traveled through is added to this set.
-                                For example if Animal has a discriminator
-                                petType and we pass in "Dog", and the class Dog
-                                allOf includes Animal, we move through Animal
-                                once using the discriminator, and pick Dog.
-                                Then in Dog, we will make an instance of the
-                                Animal class but this time we won't travel
-                                through its discriminator because we passed in
-                                _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            brand_name (str): [optional]  # noqa: E501
-            trade_name (str): [optional]  # noqa: E501
-            franchise_name (str): [optional]  # noqa: E501
-            open24_hours (str): [optional]  # noqa: E501
-            contact_details (ZonesContactDetails): [optional]  # noqa: E501
-            poi_classification (ZonesPoiClassification): [optional]  # noqa: E501
-            employee_count (EmployeeCount): [optional]  # noqa: E501
-            organization_status_code (str): [optional]  # noqa: E501
-            organization_status_code_description (str): [optional]  # noqa: E501
-            parent_business (ZonesParentBusiness): [optional]  # noqa: E501
-            ticker_symbol (str): [optional]  # noqa: E501
-            exchange_name (str): [optional]  # noqa: E501
-        """
-
-        _check_type = kwargs.pop('_check_type', True)
-        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
-        _configuration = kwargs.pop('_configuration', None)
-        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
-
-        if args:
-            raise ApiTypeError(
-                "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
-                    args,
-                    self.__class__.__name__,
-                ),
-                path_to_item=_path_to_item,
-                valid_classes=(self.__class__,),
-            )
-
-        self._data_store = {}
-        self._check_type = _check_type
-        self._spec_property_naming = _spec_property_naming
-        self._path_to_item = _path_to_item
-        self._configuration = _configuration
-        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
-            if var_name in self.read_only_vars:
-                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                                     f"class with read only attributes.")
+"""
+    Precisely APIs
+
+    Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
+
+    The version of the OpenAPI document: 16.0.0
+    Generated by: https://openapi-generator.tech
+"""
+
+
+import re  # noqa: F401
+import sys  # noqa: F401
+
+from com.precisely.apis.model_utils import (  # noqa: F401
+    ApiTypeError,
+    ModelComposed,
+    ModelNormal,
+    ModelSimple,
+    cached_property,
+    change_keys_js_to_python,
+    convert_js_args_to_python_args,
+    date,
+    datetime,
+    file_type,
+    none_type,
+    validate_get_composed_info,
+    OpenApiModel
+)
+from com.precisely.apis.exceptions import ApiAttributeError
+
+
+
+class GeocodeAddress(ModelNormal):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Attributes:
+      allowed_values (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          with a capitalized key describing the allowed value and an allowed
+          value. These dicts store the allowed enum values.
+      attribute_map (dict): The key is attribute name
+          and the value is json key in definition.
+      discriminator_value_class_map (dict): A dict to go from the discriminator
+          variable value to the discriminator class name.
+      validations (dict): The key is the tuple path to the attribute
+          and the for var_name this is (var_name,). The value is a dict
+          that stores validations for max_length, min_length, max_items,
+          min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
+          inclusive_minimum, and regex.
+      additional_properties_type (tuple): A tuple of classes accepted
+          as additional properties values.
+    """
+
+    allowed_values = {
+    }
+
+    validations = {
+    }
+
+    @cached_property
+    def additional_properties_type():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+
+    _nullable = False
+
+    @cached_property
+    def openapi_types():
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+
+        Returns
+            openapi_types (dict): The key is attribute name
+                and the value is attribute type.
+        """
+        return {
+            'object_id': (str,),  # noqa: E501
+            'main_address_line': (str,),  # noqa: E501
+            'address_last_line': (str,),  # noqa: E501
+            'place_name': (str,),  # noqa: E501
+            'area_name1': (str,),  # noqa: E501
+            'area_name2': (str,),  # noqa: E501
+            'area_name3': (str,),  # noqa: E501
+            'area_name4': (str,),  # noqa: E501
+            'post_code1': (str,),  # noqa: E501
+            'post_code2': (str,),  # noqa: E501
+            'country': (str,),  # noqa: E501
+            'address_number': (str,),  # noqa: E501
+            'street_name': (str,),  # noqa: E501
+            'unit_type': (str,),  # noqa: E501
+            'unit_value': (str,),  # noqa: E501
+            'custom_values': (dict,), # noqa: E501
+        }
+
+    @cached_property
+    def discriminator():
+        return None
+
+
+    attribute_map = {
+        'object_id': 'objectId',  # noqa: E501
+        'main_address_line': 'mainAddressLine',  # noqa: E501
+        'address_last_line': 'addressLastLine',  # noqa: E501
+        'place_name': 'placeName',  # noqa: E501
+        'area_name1': 'areaName1',  # noqa: E501
+        'area_name2': 'areaName2',  # noqa: E501
+        'area_name3': 'areaName3',  # noqa: E501
+        'area_name4': 'areaName4',  # noqa: E501
+        'post_code1': 'postCode1',  # noqa: E501
+        'post_code2': 'postCode2',  # noqa: E501
+        'country': 'country',  # noqa: E501
+        'address_number': 'addressNumber',  # noqa: E501
+        'street_name': 'streetName',  # noqa: E501
+        'unit_type': 'unitType',  # noqa: E501
+        'unit_value': 'unitValue',  # noqa: E501
+        'custom_fields': 'customFields',  # noqa: E501
+    }
+
+    read_only_vars = {
+    }
+
+    _composed_schemas = {}
+
+    @classmethod
+    @convert_js_args_to_python_args
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """GeocodeAddress - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            object_id (str): [optional]  # noqa: E501
+            main_address_line (str): [optional]  # noqa: E501
+            address_last_line (str): [optional]  # noqa: E501
+            place_name (str): [optional]  # noqa: E501
+            area_name1 (str): [optional]  # noqa: E501
+            area_name2 (str): [optional]  # noqa: E501
+            area_name3 (str): [optional]  # noqa: E501
+            area_name4 (str): [optional]  # noqa: E501
+            post_code1 (str): [optional]  # noqa: E501
+            post_code2 (str): [optional]  # noqa: E501
+            country (str): [optional]  # noqa: E501
+            address_number (str): [optional]  # noqa: E501
+            street_name (str): [optional]  # noqa: E501
+            unit_type (str): [optional]  # noqa: E501
+            unit_value (str): [optional]  # noqa: E501
+            custom_fields ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)}): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        self = super(OpenApiModel, cls).__new__(cls)
+
+        if args:
+            raise ApiTypeError(
+                "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                    args,
+                    self.__class__.__name__,
+                ),
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+        return self
+
+    required_properties = set([
+        '_data_store',
+        '_check_type',
+        '_spec_property_naming',
+        '_path_to_item',
+        '_configuration',
+        '_visited_composed_classes',
+    ])
+
+    @convert_js_args_to_python_args
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """GeocodeAddress - a model defined in OpenAPI
+
+        Keyword Args:
+            _check_type (bool): if True, values for parameters in openapi_types
+                                will be type checked and a TypeError will be
+                                raised if the wrong type is input.
+                                Defaults to True
+            _path_to_item (tuple/list): This is a list of keys or values to
+                                drill down to the model in received_data
+                                when deserializing a response
+            _spec_property_naming (bool): True if the variable names in the input data
+                                are serialized names, as specified in the OpenAPI document.
+                                False if the variable names in the input data
+                                are pythonic names, e.g. snake case (default)
+            _configuration (Configuration): the instance to use when
+                                deserializing a file_type parameter.
+                                If passed, type conversion is attempted
+                                If omitted no type conversion is done.
+            _visited_composed_classes (tuple): This stores a tuple of
+                                classes that we have traveled through so that
+                                if we see that class again we will not use its
+                                discriminator again.
+                                When traveling through a discriminator, the
+                                composed schema that is
+                                is traveled through is added to this set.
+                                For example if Animal has a discriminator
+                                petType and we pass in "Dog", and the class Dog
+                                allOf includes Animal, we move through Animal
+                                once using the discriminator, and pick Dog.
+                                Then in Dog, we will make an instance of the
+                                Animal class but this time we won't travel
+                                through its discriminator because we passed in
+                                _visited_composed_classes = (Animal,)
+            object_id (str): [optional]  # noqa: E501
+            main_address_line (str): [optional]  # noqa: E501
+            address_last_line (str): [optional]  # noqa: E501
+            place_name (str): [optional]  # noqa: E501
+            area_name1 (str): [optional]  # noqa: E501
+            area_name2 (str): [optional]  # noqa: E501
+            area_name3 (str): [optional]  # noqa: E501
+            area_name4 (str): [optional]  # noqa: E501
+            post_code1 (str): [optional]  # noqa: E501
+            post_code2 (str): [optional]  # noqa: E501
+            country (str): [optional]  # noqa: E501
+            address_number (str): [optional]  # noqa: E501
+            street_name (str): [optional]  # noqa: E501
+            unit_type (str): [optional]  # noqa: E501
+            unit_value (str): [optional]  # noqa: E501
+            custom_fields ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)}): [optional]  # noqa: E501
+        """
+
+        _check_type = kwargs.pop('_check_type', True)
+        _spec_property_naming = kwargs.pop('_spec_property_naming', False)
+        _path_to_item = kwargs.pop('_path_to_item', ())
+        _configuration = kwargs.pop('_configuration', None)
+        _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
+
+        if args:
+            raise ApiTypeError(
+                "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
+                    args,
+                    self.__class__.__name__,
+                ),
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
+
+        self._data_store = {}
+        self._check_type = _check_type
+        self._spec_property_naming = _spec_property_naming
+        self._path_to_item = _path_to_item
+        self._configuration = _configuration
+        self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
+
+        for var_name, var_value in kwargs.items():
+            if var_name not in self.attribute_map and \
+                        self._configuration is not None and \
+                        self._configuration.discard_unknown_keys and \
+                        self.additional_properties_type is None:
+                # discard variable.
+                continue
+            setattr(self, var_name, var_value)
+            if var_name in self.read_only_vars:
+                raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
+                                     f"class with read only attributes.")
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/zones_poi_classification.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/zones_poi_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model/zones_poi_geometry.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model/zones_poi_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/model_utils.py` & `com.precisely.apis-16.0.1/com/precisely/apis/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/models/__init__.py` & `com.precisely.apis-16.0.1/com/precisely/apis/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from com.precisely.apis.model.ahj import AHJ
 from com.precisely.apis.model.ahj_list import AHJList
 from com.precisely.apis.model.ahj_plus_psap_response import AHJPlusPSAPResponse
 from com.precisely.apis.model.ah_jmailing_address import AHJmailingAddress
 from com.precisely.apis.model.absentee_owner import AbsenteeOwner
 from com.precisely.apis.model.accuracy import Accuracy
 from com.precisely.apis.model.address import Address
+from com.precisely.apis.model.address1 import Address1
 from com.precisely.apis.model.address_time import AddressTime
 from com.precisely.apis.model.address_type import AddressType
 from com.precisely.apis.model.addresses_by_boundary_request import AddressesByBoundaryRequest
 from com.precisely.apis.model.addresses_count import AddressesCount
 from com.precisely.apis.model.addresses_dto import AddressesDTO
 from com.precisely.apis.model.addresses_preferences import AddressesPreferences
 from com.precisely.apis.model.addresses_response import AddressesResponse
```

### Comparing `com.precisely.apis-16.0.0/com/precisely/apis/rest.py` & `com.precisely.apis-16.0.1/com/precisely/apis/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

### Comparing `com.precisely.apis-16.0.0/com.precisely.apis.egg-info/SOURCES.txt` & `com.precisely.apis-16.0.1/com.precisely.apis.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 com/precisely/apis/api/time_zone_service_api.py
 com/precisely/apis/api/zones_service_api.py
 com/precisely/apis/apis/__init__.py
 com/precisely/apis/model/__init__.py
 com/precisely/apis/model/absentee_owner.py
 com/precisely/apis/model/accuracy.py
 com/precisely/apis/model/address.py
+com/precisely/apis/model/address1.py
 com/precisely/apis/model/address_time.py
 com/precisely/apis/model/address_type.py
 com/precisely/apis/model/addresses_by_boundary_request.py
 com/precisely/apis/model/addresses_count.py
 com/precisely/apis/model/addresses_dto.py
 com/precisely/apis/model/addresses_preferences.py
 com/precisely/apis/model/addresses_response.py
```

### Comparing `com.precisely.apis-16.0.0/setup.py` & `com.precisely.apis-16.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 16.0.0
+    The version of the OpenAPI document: 16.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "com.precisely.apis"
-VERSION = "16.0.0"
+VERSION = "16.0.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

