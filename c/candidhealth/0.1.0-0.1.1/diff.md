# Comparing `tmp/candidhealth-0.1.0.tar.gz` & `tmp/candidhealth-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "candidhealth-0.1.0.tar", max compression
+gzip compressed data, was "candidhealth-0.1.1.tar", max compression
```

## Comparing `candidhealth-0.1.0.tar` & `candidhealth-0.1.1.tar`

### file list

```diff
@@ -1,236 +1,236 @@
--rw-r--r--   0        0        0        0 2023-05-25 18:31:54.583160 candidhealth-0.1.0/README.md
--rw-r--r--   0        0        0      373 2023-05-25 18:31:54.583160 candidhealth-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5601 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/__init__.py
--rw-r--r--   0        0        0     2009 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/client.py
--rw-r--r--   0        0        0      348 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/core/__init__.py
--rw-r--r--   0        0        0      426 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      227 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/environment.py
--rw-r--r--   0        0        0        0 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/py.typed
--rw-r--r--   0        0        0     5767 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/__init__.py
--rw-r--r--   0        0        0      111 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/auth/__init__.py
--rw-r--r--   0        0        0      820 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/auth/client.py
--rw-r--r--   0        0        0      102 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/auth/resources/__init__.py
--rw-r--r--   0        0        0      304 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/auth/resources/v_2/__init__.py
--rw-r--r--   0        0        0     3502 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/auth/resources/v_2/client.py
--rw-r--r--   0        0        0      159 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/auth/resources/v_2/errors/__init__.py
--rw-r--r--   0        0        0      330 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/auth/resources/v_2/errors/too_many_requests_error.py
--rw-r--r--   0        0        0      333 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/auth/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0      785 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_request.py
--rw-r--r--   0        0        0      806 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_response.py
--rw-r--r--   0        0        0      765 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/auth/resources/v_2/types/too_many_requests_error_type.py
--rw-r--r--   0        0        0      191 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/billing_notes/__init__.py
--rw-r--r--   0        0        0     2831 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/billing_notes/client.py
--rw-r--r--   0        0        0      256 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/billing_notes/types/__init__.py
--rw-r--r--   0        0        0     1136 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/billing_notes/types/billing_note.py
--rw-r--r--   0        0        0      813 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/billing_notes/types/billing_note_base.py
--rw-r--r--   0        0        0      104 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/billing_notes/types/billing_note_id.py
--rw-r--r--   0        0        0      139 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/claims/__init__.py
--rw-r--r--   0        0        0      164 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/claims/types/__init__.py
--rw-r--r--   0        0        0     1151 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/claims/types/claim.py
--rw-r--r--   0        0        0     2605 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/claims/types/claim_status.py
--rw-r--r--   0        0        0     1305 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/commons/__init__.py
--rw-r--r--   0        0        0     1928 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/commons/types/__init__.py
--rw-r--r--   0        0        0       79 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/commons/types/auth_0_id.py
--rw-r--r--   0        0        0       98 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/commons/types/claim_id.py
--rw-r--r--   0        0        0       90 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/commons/types/content_download_url.py
--rw-r--r--   0        0        0       76 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/commons/types/date.py
--rw-r--r--   0        0        0       91 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/commons/types/encounter_external_id.py
--rw-r--r--   0        0        0      102 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/commons/types/encounter_id.py
--rw-r--r--   0        0        0    11148 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/commons/types/facility_type_code.py
--rw-r--r--   0        0        0    15447 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/commons/types/insurance_type_code.py
--rw-r--r--   0        0        0       79 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/commons/types/link_url.py
--rw-r--r--   0        0        0       75 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/npi.py
--rw-r--r--   0        0        0      105 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/organization_id.py
--rw-r--r--   0        0        0       81 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/page_token.py
--rw-r--r--   0        0        0       89 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/patient_external_id.py
--rw-r--r--   0        0        0     4686 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py
--rw-r--r--   0        0        0    79514 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/procedure_modifier.py
--rw-r--r--   0        0        0      735 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/region_national.py
--rw-r--r--   0        0        0      790 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/region_states.py
--rw-r--r--   0        0        0      722 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/regions.py
--rw-r--r--   0        0        0      864 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/resource_page.py
--rw-r--r--   0        0        0      104 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/service_line_id.py
--rw-r--r--   0        0        0      432 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/service_line_units.py
--rw-r--r--   0        0        0     5065 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/source_of_payment_code.py
--rw-r--r--   0        0        0     6264 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/state.py
--rw-r--r--   0        0        0     1037 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/street_address_base.py
--rw-r--r--   0        0        0      985 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/street_address_long_zip.py
--rw-r--r--   0        0        0     1003 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/street_address_short_zip.py
--rw-r--r--   0        0        0       83 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/work_queue_id.py
--rw-r--r--   0        0        0      251 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/contracts/__init__.py
--rw-r--r--   0        0        0      365 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/contracts/types/__init__.py
--rw-r--r--   0        0        0      940 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/contracts/types/authorized_signatory.py
--rw-r--r--   0        0        0     1430 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/contracts/types/contract.py
--rw-r--r--   0        0        0     1517 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/contracts/types/contract_base.py
--rw-r--r--   0        0        0      101 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/contracts/types/contract_id.py
--rw-r--r--   0        0        0      986 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/contracts/types/contract_status.py
--rw-r--r--   0        0        0     1125 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/credentialing/__init__.py
--rw-r--r--   0        0        0     1472 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/credentialing/types/__init__.py
--rw-r--r--   0        0        0      886 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/credentialing/types/credentialed_encounter_status_result.py
--rw-r--r--   0        0        0      940 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/credentialing/types/credentialing_span_dates.py
--rw-r--r--   0        0        0      977 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/credentialing/types/credentialing_span_status.py
--rw-r--r--   0        0        0      881 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/credentialing/types/encounter_credentialing_status_result.py
--rw-r--r--   0        0        0      864 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/credentialing/types/non_required_credentialing_dates.py
--rw-r--r--   0        0        0     2210 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/credentialing/types/provider_credentialing_span.py
--rw-r--r--   0        0        0      958 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/credentialing/types/provider_credentialing_span_base.py
--rw-r--r--   0        0        0      118 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/credentialing/types/provider_credentialing_span_id.py
--rw-r--r--   0        0        0      827 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/credentialing/types/required_credentialing_dates.py
--rw-r--r--   0        0        0      279 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/diagnoses/__init__.py
--rw-r--r--   0        0        0      409 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/diagnoses/types/__init__.py
--rw-r--r--   0        0        0      958 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/diagnoses/types/diagnosis.py
--rw-r--r--   0        0        0     1904 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/diagnoses/types/diagnosis_create.py
--rw-r--r--   0        0        0      102 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/diagnoses/types/diagnosis_id.py
--rw-r--r--   0        0        0     1974 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/diagnoses/types/diagnosis_type_code.py
--rw-r--r--   0        0        0      903 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py
--rw-r--r--   0        0        0      111 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounter_providers/__init__.py
--rw-r--r--   0        0        0      102 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/__init__.py
--rw-r--r--   0        0        0      381 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/__init__.py
--rw-r--r--   0        0        0      516 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0     1988 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py
--rw-r--r--   0        0        0     1092 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py
--rw-r--r--   0        0        0     1284 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py
--rw-r--r--   0        0        0      101 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/provider_id.py
--rw-r--r--   0        0        0     1244 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py
--rw-r--r--   0        0        0     1244 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py
--rw-r--r--   0        0        0      111 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/__init__.py
--rw-r--r--   0        0        0      832 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/client.py
--rw-r--r--   0        0        0      102 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/__init__.py
--rw-r--r--   0        0        0     2507 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/__init__.py
--rw-r--r--   0        0        0    31263 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/client.py
--rw-r--r--   0        0        0     3652 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/__init__.py
--rw-r--r--   0        0        0      103 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/attachment_id.py
--rw-r--r--   0        0        0     1314 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/attributable_contracting_status_result.py
--rw-r--r--   0        0        0      944 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/base_attachment.py
--rw-r--r--   0        0        0      874 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/clinical_note.py
--rw-r--r--   0        0        0      944 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category.py
--rw-r--r--   0        0        0      894 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category_create.py
--rw-r--r--   0        0        0      659 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/coding_attribution_type.py
--rw-r--r--   0        0        0      713 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/contracting_out_of_of_network_reason.py
--rw-r--r--   0        0        0     2992 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/encounter.py
--rw-r--r--   0        0        0      920 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/encounter_attachment.py
--rw-r--r--   0        0        0      388 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/encounter_attachment_type.py
--rw-r--r--   0        0        0     4498 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/encounter_base.py
--rw-r--r--   0        0        0      885 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/encounter_page.py
--rw-r--r--   0        0        0     1025 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/encounter_sort_options.py
--rw-r--r--   0        0        0      659 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/generate_clinical_notes_pdf_response.py
--rw-r--r--   0        0        0      855 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/in_network_contracting_status_result.py
--rw-r--r--   0        0        0      845 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up.py
--rw-r--r--   0        0        0       88 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up_id.py
--rw-r--r--   0        0        0      969 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intake_question.py
--rw-r--r--   0        0        0       88 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intake_question_id.py
--rw-r--r--   0        0        0      891 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intake_response_and_follow_ups.py
--rw-r--r--   0        0        0     1303 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intervention.py
--rw-r--r--   0        0        0      865 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intervention_category.py
--rw-r--r--   0        0        0      855 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/lab.py
--rw-r--r--   0        0        0      457 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/lab_code_type.py
--rw-r--r--   0        0        0      834 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/mark_as_not_billable_response.py
--rw-r--r--   0        0        0      953 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/medication.py
--rw-r--r--   0        0        0      880 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/network_status.py
--rw-r--r--   0        0        0     1164 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/network_status_computation_results.py
--rw-r--r--   0        0        0     2615 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/note_category.py
--rw-r--r--   0        0        0      900 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/out_of_network_contracting_status_result.py
--rw-r--r--   0        0        0     1012 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category.py
--rw-r--r--   0        0        0      885 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category_enum.py
--rw-r--r--   0        0        0       96 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/prior_authorization_number.py
--rw-r--r--   0        0        0       77 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/rx_cui.py
--rw-r--r--   0        0        0      898 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/successful_generate_clinical_notes_pdf_response.py
--rw-r--r--   0        0        0      544 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/synchronicity_type.py
--rw-r--r--   0        0        0      893 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/vitals.py
--rw-r--r--   0        0        0      143 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/era/__init__.py
--rw-r--r--   0        0        0      181 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/era/types/__init__.py
--rw-r--r--   0        0        0      817 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/era/types/era.py
--rw-r--r--   0        0        0      811 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/era/types/era_base.py
--rw-r--r--   0        0        0       96 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/era/types/era_id.py
--rw-r--r--   0        0        0      207 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/expected_network_status/__init__.py
--rw-r--r--   0        0        0     5547 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/expected_network_status/client.py
--rw-r--r--   0        0        0      270 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/expected_network_status/types/__init__.py
--rw-r--r--   0        0        0      729 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/expected_network_status/types/expected_network_status.py
--rw-r--r--   0        0        0      981 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/expected_network_status/types/expected_network_status_response.py
--rw-r--r--   0        0        0      399 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/individual/__init__.py
--rw-r--r--   0        0        0      545 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/individual/types/__init__.py
--rw-r--r--   0        0        0      871 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/individual/types/gender.py
--rw-r--r--   0        0        0      821 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/individual/types/individual_base.py
--rw-r--r--   0        0        0      103 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/individual/types/individual_id.py
--rw-r--r--   0        0        0      867 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/individual/types/patient.py
--rw-r--r--   0        0        0     1515 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/individual/types/patient_create.py
--rw-r--r--   0        0        0      972 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/individual/types/subscriber.py
--rw-r--r--   0        0        0     1200 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/individual/types/subscriber_base.py
--rw-r--r--   0        0        0      925 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/individual/types/subscriber_create.py
--rw-r--r--   0        0        0      247 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/insurance_card/__init__.py
--rw-r--r--   0        0        0      352 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/insurance_card/types/__init__.py
--rw-r--r--   0        0        0     1106 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/insurance_card/types/insurance_card.py
--rw-r--r--   0        0        0     1122 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/insurance_card/types/insurance_card_base.py
--rw-r--r--   0        0        0     1026 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/insurance_card/types/insurance_card_create.py
--rw-r--r--   0        0        0      106 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/insurance_card/types/insurance_card_id.py
--rw-r--r--   0        0        0      199 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/invoices/__init__.py
--rw-r--r--   0        0        0      276 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/invoices/types/__init__.py
--rw-r--r--   0        0        0     1397 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/invoices/types/invoice.py
--rw-r--r--   0        0        0      100 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/invoices/types/invoice_id.py
--rw-r--r--   0        0        0      849 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/invoices/types/invoice_item.py
--rw-r--r--   0        0        0      908 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/invoices/types/invoice_status.py
--rw-r--r--   0        0        0      111 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/__init__.py
--rw-r--r--   0        0        0      102 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/resources/__init__.py
--rw-r--r--   0        0        0      501 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/__init__.py
--rw-r--r--   0        0        0      704 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0      334 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/address_type.py
--rw-r--r--   0        0        0      492 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/employment_status.py
--rw-r--r--   0        0        0     2857 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/license_type.py
--rw-r--r--   0        0        0     1562 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider.py
--rw-r--r--   0        0        0     1062 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py
--rw-r--r--   0        0        0     2853 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_base.py
--rw-r--r--   0        0        0      113 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_id.py
--rw-r--r--   0        0        0      510 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/provider_type.py
--rw-r--r--   0        0        0      111 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/patient_payments/__init__.py
--rw-r--r--   0        0        0      102 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/patient_payments/resources/__init__.py
--rw-r--r--   0        0        0      259 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/patient_payments/resources/v_2/__init__.py
--rw-r--r--   0        0        0      370 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/patient_payments/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0     1648 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/patient_payments/resources/v_2/types/patient_payment.py
--rw-r--r--   0        0        0       88 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_id.py
--rw-r--r--   0        0        0     2035 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_source.py
--rw-r--r--   0        0        0     2055 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_status.py
--rw-r--r--   0        0        0      135 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/payers/__init__.py
--rw-r--r--   0        0        0     4709 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/payers/client.py
--rw-r--r--   0        0        0      158 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/payers/types/__init__.py
--rw-r--r--   0        0        0     1043 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/payers/types/payer.py
--rw-r--r--   0        0        0      865 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/payers/types/payer_page.py
--rw-r--r--   0        0        0      251 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_facility/__init__.py
--rw-r--r--   0        0        0      348 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_facility/types/__init__.py
--rw-r--r--   0        0        0      975 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_facility/types/encounter_service_facility.py
--rw-r--r--   0        0        0     1574 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_facility/types/encounter_service_facility_base.py
--rw-r--r--   0        0        0      108 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_facility/types/service_facility_id.py
--rw-r--r--   0        0        0      671 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_lines/__init__.py
--rw-r--r--   0        0        0      978 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_lines/types/__init__.py
--rw-r--r--   0        0        0     6559 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_lines/types/denial_reason_content.py
--rw-r--r--   0        0        0     1104 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_lines/types/drug_identification.py
--rw-r--r--   0        0        0      996 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_lines/types/measurement_unit_code.py
--rw-r--r--   0        0        0     1659 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_lines/types/service_id_qualifier.py
--rw-r--r--   0        0        0     1144 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line.py
--rw-r--r--   0        0        0      960 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_adjustment.py
--rw-r--r--   0        0        0      866 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_base.py
--rw-r--r--   0        0        0     1899 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_base_with_optionals.py
--rw-r--r--   0        0        0     1618 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_create.py
--rw-r--r--   0        0        0     1099 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_denial_reason.py
--rw-r--r--   0        0        0      917 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_era_data.py
--rw-r--r--   0        0        0      177 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/tags/__init__.py
--rw-r--r--   0        0        0      244 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/tags/types/__init__.py
--rw-r--r--   0        0        0      799 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/tags/types/tag.py
--rw-r--r--   0        0        0     1527 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/tags/types/tag_color_enum.py
--rw-r--r--   0        0        0      861 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/tags/types/tag_create.py
--rw-r--r--   0        0        0       77 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/tags/types/tag_id.py
--rw-r--r--   0        0        0      113 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/tasks/__init__.py
--rw-r--r--   0        0        0      115 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/tasks/types/__init__.py
--rw-r--r--   0        0        0       97 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/tasks/types/task_id.py
--rw-r--r--   0        0        0      109 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/users/__init__.py
--rw-r--r--   0        0        0      108 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/users/types/__init__.py
--rw-r--r--   0        0        0      916 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/users/types/user.py
--rw-r--r--   0        0        0      111 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/work_queues/__init__.py
--rw-r--r--   0        0        0      102 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/work_queues/resources/__init__.py
--rw-r--r--   0        0        0      207 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/work_queues/resources/v_1/__init__.py
--rw-r--r--   0        0        0      281 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/work_queues/resources/v_1/types/__init__.py
--rw-r--r--   0        0        0     1052 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/work_queues/resources/v_1/types/work_queue.py
--rw-r--r--   0        0        0      893 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/work_queues/resources/v_1/types/work_queue_category.py
--rw-r--r--   0        0        0     1242 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/work_queues/resources/v_1/types/work_queue_category_type.py
--rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 candidhealth-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-26 17:29:39.259210 candidhealth-0.1.1/README.md
+-rw-r--r--   0        0        0      373 2023-05-26 17:29:39.259210 candidhealth-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5601 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/__init__.py
+-rw-r--r--   0        0        0     2009 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/client.py
+-rw-r--r--   0        0        0      348 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      227 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/environment.py
+-rw-r--r--   0        0        0        0 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/py.typed
+-rw-r--r--   0        0        0     5767 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/__init__.py
+-rw-r--r--   0        0        0      111 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/auth/__init__.py
+-rw-r--r--   0        0        0      820 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/auth/client.py
+-rw-r--r--   0        0        0      102 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/auth/resources/__init__.py
+-rw-r--r--   0        0        0      304 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/__init__.py
+-rw-r--r--   0        0        0     3502 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/client.py
+-rw-r--r--   0        0        0      159 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/errors/__init__.py
+-rw-r--r--   0        0        0      330 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      333 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0      785 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/types/auth_get_token_request.py
+-rw-r--r--   0        0        0      806 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/types/auth_get_token_response.py
+-rw-r--r--   0        0        0      765 2023-05-26 17:29:39.259210 candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/types/too_many_requests_error_type.py
+-rw-r--r--   0        0        0      191 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/billing_notes/__init__.py
+-rw-r--r--   0        0        0     2831 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/billing_notes/client.py
+-rw-r--r--   0        0        0      256 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/billing_notes/types/__init__.py
+-rw-r--r--   0        0        0     1136 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/billing_notes/types/billing_note.py
+-rw-r--r--   0        0        0      813 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/billing_notes/types/billing_note_base.py
+-rw-r--r--   0        0        0      104 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/billing_notes/types/billing_note_id.py
+-rw-r--r--   0        0        0      139 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/claims/__init__.py
+-rw-r--r--   0        0        0      164 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/claims/types/__init__.py
+-rw-r--r--   0        0        0     1151 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/claims/types/claim.py
+-rw-r--r--   0        0        0     2605 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/claims/types/claim_status.py
+-rw-r--r--   0        0        0     1305 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/__init__.py
+-rw-r--r--   0        0        0     1928 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0       79 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/auth_0_id.py
+-rw-r--r--   0        0        0       98 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/claim_id.py
+-rw-r--r--   0        0        0       90 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/content_download_url.py
+-rw-r--r--   0        0        0       76 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/date.py
+-rw-r--r--   0        0        0       91 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/encounter_external_id.py
+-rw-r--r--   0        0        0      102 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/encounter_id.py
+-rw-r--r--   0        0        0    11148 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/facility_type_code.py
+-rw-r--r--   0        0        0    15447 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/insurance_type_code.py
+-rw-r--r--   0        0        0       79 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/link_url.py
+-rw-r--r--   0        0        0       75 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/npi.py
+-rw-r--r--   0        0        0      105 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/organization_id.py
+-rw-r--r--   0        0        0       81 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/page_token.py
+-rw-r--r--   0        0        0       89 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/patient_external_id.py
+-rw-r--r--   0        0        0     4686 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py
+-rw-r--r--   0        0        0    79514 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/procedure_modifier.py
+-rw-r--r--   0        0        0      735 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/region_national.py
+-rw-r--r--   0        0        0      790 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/region_states.py
+-rw-r--r--   0        0        0      633 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/regions.py
+-rw-r--r--   0        0        0      864 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/resource_page.py
+-rw-r--r--   0        0        0      104 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/service_line_id.py
+-rw-r--r--   0        0        0      432 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/service_line_units.py
+-rw-r--r--   0        0        0     5065 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/source_of_payment_code.py
+-rw-r--r--   0        0        0     6264 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/state.py
+-rw-r--r--   0        0        0     1037 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/street_address_base.py
+-rw-r--r--   0        0        0      985 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/street_address_long_zip.py
+-rw-r--r--   0        0        0     1003 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/street_address_short_zip.py
+-rw-r--r--   0        0        0       83 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/commons/types/work_queue_id.py
+-rw-r--r--   0        0        0      251 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/contracts/__init__.py
+-rw-r--r--   0        0        0      365 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/contracts/types/__init__.py
+-rw-r--r--   0        0        0      940 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/contracts/types/authorized_signatory.py
+-rw-r--r--   0        0        0     1430 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/contracts/types/contract.py
+-rw-r--r--   0        0        0     1517 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/contracts/types/contract_base.py
+-rw-r--r--   0        0        0      101 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/contracts/types/contract_id.py
+-rw-r--r--   0        0        0      986 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/contracts/types/contract_status.py
+-rw-r--r--   0        0        0     1125 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/credentialing/__init__.py
+-rw-r--r--   0        0        0     1472 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/credentialing/types/__init__.py
+-rw-r--r--   0        0        0      886 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/credentialing/types/credentialed_encounter_status_result.py
+-rw-r--r--   0        0        0      846 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/credentialing/types/credentialing_span_dates.py
+-rw-r--r--   0        0        0      977 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/credentialing/types/credentialing_span_status.py
+-rw-r--r--   0        0        0      809 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/credentialing/types/encounter_credentialing_status_result.py
+-rw-r--r--   0        0        0      864 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/credentialing/types/non_required_credentialing_dates.py
+-rw-r--r--   0        0        0     2210 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/credentialing/types/provider_credentialing_span.py
+-rw-r--r--   0        0        0      958 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/credentialing/types/provider_credentialing_span_base.py
+-rw-r--r--   0        0        0      118 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/credentialing/types/provider_credentialing_span_id.py
+-rw-r--r--   0        0        0      827 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/credentialing/types/required_credentialing_dates.py
+-rw-r--r--   0        0        0      279 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/diagnoses/__init__.py
+-rw-r--r--   0        0        0      409 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/diagnoses/types/__init__.py
+-rw-r--r--   0        0        0      958 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/diagnoses/types/diagnosis.py
+-rw-r--r--   0        0        0     1904 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/diagnoses/types/diagnosis_create.py
+-rw-r--r--   0        0        0      102 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/diagnoses/types/diagnosis_id.py
+-rw-r--r--   0        0        0     1974 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/diagnoses/types/diagnosis_type_code.py
+-rw-r--r--   0        0        0      903 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py
+-rw-r--r--   0        0        0      111 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/encounter_providers/__init__.py
+-rw-r--r--   0        0        0      102 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/__init__.py
+-rw-r--r--   0        0        0      381 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/__init__.py
+-rw-r--r--   0        0        0      516 2023-05-26 17:29:39.263210 candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0     1988 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py
+-rw-r--r--   0        0        0     1092 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py
+-rw-r--r--   0        0        0     1284 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py
+-rw-r--r--   0        0        0      101 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/provider_id.py
+-rw-r--r--   0        0        0     1244 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py
+-rw-r--r--   0        0        0     1244 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py
+-rw-r--r--   0        0        0      111 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/__init__.py
+-rw-r--r--   0        0        0      832 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/client.py
+-rw-r--r--   0        0        0      102 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/__init__.py
+-rw-r--r--   0        0        0     2507 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/__init__.py
+-rw-r--r--   0        0        0    31263 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/client.py
+-rw-r--r--   0        0        0     3652 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/__init__.py
+-rw-r--r--   0        0        0      103 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/attachment_id.py
+-rw-r--r--   0        0        0     1206 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/attributable_contracting_status_result.py
+-rw-r--r--   0        0        0      944 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/base_attachment.py
+-rw-r--r--   0        0        0      874 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/clinical_note.py
+-rw-r--r--   0        0        0      944 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/clinical_note_category.py
+-rw-r--r--   0        0        0      894 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/clinical_note_category_create.py
+-rw-r--r--   0        0        0      659 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/coding_attribution_type.py
+-rw-r--r--   0        0        0      713 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/contracting_out_of_of_network_reason.py
+-rw-r--r--   0        0        0     2992 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/encounter.py
+-rw-r--r--   0        0        0      920 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/encounter_attachment.py
+-rw-r--r--   0        0        0      388 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/encounter_attachment_type.py
+-rw-r--r--   0        0        0     4498 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/encounter_base.py
+-rw-r--r--   0        0        0      885 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/encounter_page.py
+-rw-r--r--   0        0        0     1025 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/encounter_sort_options.py
+-rw-r--r--   0        0        0      568 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/generate_clinical_notes_pdf_response.py
+-rw-r--r--   0        0        0      855 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/in_network_contracting_status_result.py
+-rw-r--r--   0        0        0      845 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intake_follow_up.py
+-rw-r--r--   0        0        0       88 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intake_follow_up_id.py
+-rw-r--r--   0        0        0      969 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intake_question.py
+-rw-r--r--   0        0        0       88 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intake_question_id.py
+-rw-r--r--   0        0        0      891 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intake_response_and_follow_ups.py
+-rw-r--r--   0        0        0     1303 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intervention.py
+-rw-r--r--   0        0        0      865 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intervention_category.py
+-rw-r--r--   0        0        0      855 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/lab.py
+-rw-r--r--   0        0        0      457 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/lab_code_type.py
+-rw-r--r--   0        0        0      834 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/mark_as_not_billable_response.py
+-rw-r--r--   0        0        0      953 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/medication.py
+-rw-r--r--   0        0        0      880 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/network_status.py
+-rw-r--r--   0        0        0     1164 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/network_status_computation_results.py
+-rw-r--r--   0        0        0     2615 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/note_category.py
+-rw-r--r--   0        0        0      900 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/out_of_network_contracting_status_result.py
+-rw-r--r--   0        0        0     1012 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/patient_history_category.py
+-rw-r--r--   0        0        0      885 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/patient_history_category_enum.py
+-rw-r--r--   0        0        0       96 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/prior_authorization_number.py
+-rw-r--r--   0        0        0       77 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/rx_cui.py
+-rw-r--r--   0        0        0      898 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/successful_generate_clinical_notes_pdf_response.py
+-rw-r--r--   0        0        0      544 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/synchronicity_type.py
+-rw-r--r--   0        0        0      893 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/vitals.py
+-rw-r--r--   0        0        0      143 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/era/__init__.py
+-rw-r--r--   0        0        0      181 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/era/types/__init__.py
+-rw-r--r--   0        0        0      817 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/era/types/era.py
+-rw-r--r--   0        0        0      811 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/era/types/era_base.py
+-rw-r--r--   0        0        0       96 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/era/types/era_id.py
+-rw-r--r--   0        0        0      207 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/expected_network_status/__init__.py
+-rw-r--r--   0        0        0     5547 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/expected_network_status/client.py
+-rw-r--r--   0        0        0      270 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/expected_network_status/types/__init__.py
+-rw-r--r--   0        0        0      729 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/expected_network_status/types/expected_network_status.py
+-rw-r--r--   0        0        0      981 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/expected_network_status/types/expected_network_status_response.py
+-rw-r--r--   0        0        0      399 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/individual/__init__.py
+-rw-r--r--   0        0        0      545 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/individual/types/__init__.py
+-rw-r--r--   0        0        0      871 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/individual/types/gender.py
+-rw-r--r--   0        0        0      821 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/individual/types/individual_base.py
+-rw-r--r--   0        0        0      103 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/individual/types/individual_id.py
+-rw-r--r--   0        0        0      867 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/individual/types/patient.py
+-rw-r--r--   0        0        0     1515 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/individual/types/patient_create.py
+-rw-r--r--   0        0        0      972 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/individual/types/subscriber.py
+-rw-r--r--   0        0        0     1200 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/individual/types/subscriber_base.py
+-rw-r--r--   0        0        0      925 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/individual/types/subscriber_create.py
+-rw-r--r--   0        0        0      247 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/insurance_card/__init__.py
+-rw-r--r--   0        0        0      352 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/insurance_card/types/__init__.py
+-rw-r--r--   0        0        0     1106 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/insurance_card/types/insurance_card.py
+-rw-r--r--   0        0        0     1122 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/insurance_card/types/insurance_card_base.py
+-rw-r--r--   0        0        0     1026 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/insurance_card/types/insurance_card_create.py
+-rw-r--r--   0        0        0      106 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/insurance_card/types/insurance_card_id.py
+-rw-r--r--   0        0        0      199 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/invoices/__init__.py
+-rw-r--r--   0        0        0      276 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/invoices/types/__init__.py
+-rw-r--r--   0        0        0     1397 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/invoices/types/invoice.py
+-rw-r--r--   0        0        0      100 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/invoices/types/invoice_id.py
+-rw-r--r--   0        0        0      849 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/invoices/types/invoice_item.py
+-rw-r--r--   0        0        0      908 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/invoices/types/invoice_status.py
+-rw-r--r--   0        0        0      111 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/__init__.py
+-rw-r--r--   0        0        0      102 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/resources/__init__.py
+-rw-r--r--   0        0        0      501 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/__init__.py
+-rw-r--r--   0        0        0      704 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0      334 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/address_type.py
+-rw-r--r--   0        0        0      492 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/employment_status.py
+-rw-r--r--   0        0        0     2857 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/license_type.py
+-rw-r--r--   0        0        0     1562 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/organization_provider.py
+-rw-r--r--   0        0        0     1062 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py
+-rw-r--r--   0        0        0     2853 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_base.py
+-rw-r--r--   0        0        0      113 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_id.py
+-rw-r--r--   0        0        0      510 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/provider_type.py
+-rw-r--r--   0        0        0      111 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/patient_payments/__init__.py
+-rw-r--r--   0        0        0      102 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/patient_payments/resources/__init__.py
+-rw-r--r--   0        0        0      259 2023-05-26 17:29:39.267210 candidhealth-0.1.1/src/candid/resources/patient_payments/resources/v_2/__init__.py
+-rw-r--r--   0        0        0      370 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/patient_payments/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0     1648 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/patient_payments/resources/v_2/types/patient_payment.py
+-rw-r--r--   0        0        0       88 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_id.py
+-rw-r--r--   0        0        0     2035 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_source.py
+-rw-r--r--   0        0        0     2055 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_status.py
+-rw-r--r--   0        0        0      135 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/payers/__init__.py
+-rw-r--r--   0        0        0     4709 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/payers/client.py
+-rw-r--r--   0        0        0      158 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/payers/types/__init__.py
+-rw-r--r--   0        0        0     1043 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/payers/types/payer.py
+-rw-r--r--   0        0        0      865 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/payers/types/payer_page.py
+-rw-r--r--   0        0        0      251 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_facility/__init__.py
+-rw-r--r--   0        0        0      348 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_facility/types/__init__.py
+-rw-r--r--   0        0        0      975 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_facility/types/encounter_service_facility.py
+-rw-r--r--   0        0        0     1574 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_facility/types/encounter_service_facility_base.py
+-rw-r--r--   0        0        0      108 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_facility/types/service_facility_id.py
+-rw-r--r--   0        0        0      671 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/__init__.py
+-rw-r--r--   0        0        0      978 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/__init__.py
+-rw-r--r--   0        0        0     6559 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/denial_reason_content.py
+-rw-r--r--   0        0        0     1104 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/drug_identification.py
+-rw-r--r--   0        0        0      996 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/measurement_unit_code.py
+-rw-r--r--   0        0        0     1659 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/service_id_qualifier.py
+-rw-r--r--   0        0        0     1144 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line.py
+-rw-r--r--   0        0        0      960 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_adjustment.py
+-rw-r--r--   0        0        0      866 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_base.py
+-rw-r--r--   0        0        0     1899 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_base_with_optionals.py
+-rw-r--r--   0        0        0     1618 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_create.py
+-rw-r--r--   0        0        0     1099 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_denial_reason.py
+-rw-r--r--   0        0        0      917 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_era_data.py
+-rw-r--r--   0        0        0      177 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/tags/__init__.py
+-rw-r--r--   0        0        0      244 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/tags/types/__init__.py
+-rw-r--r--   0        0        0      799 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/tags/types/tag.py
+-rw-r--r--   0        0        0     1527 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/tags/types/tag_color_enum.py
+-rw-r--r--   0        0        0      861 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/tags/types/tag_create.py
+-rw-r--r--   0        0        0       77 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/tags/types/tag_id.py
+-rw-r--r--   0        0        0      113 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/tasks/__init__.py
+-rw-r--r--   0        0        0      115 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/tasks/types/__init__.py
+-rw-r--r--   0        0        0       97 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/tasks/types/task_id.py
+-rw-r--r--   0        0        0      109 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/users/__init__.py
+-rw-r--r--   0        0        0      108 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/users/types/__init__.py
+-rw-r--r--   0        0        0      916 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/users/types/user.py
+-rw-r--r--   0        0        0      111 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/work_queues/__init__.py
+-rw-r--r--   0        0        0      102 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/work_queues/resources/__init__.py
+-rw-r--r--   0        0        0      207 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/work_queues/resources/v_1/__init__.py
+-rw-r--r--   0        0        0      281 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/work_queues/resources/v_1/types/__init__.py
+-rw-r--r--   0        0        0     1052 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/work_queues/resources/v_1/types/work_queue.py
+-rw-r--r--   0        0        0      893 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/work_queues/resources/v_1/types/work_queue_category.py
+-rw-r--r--   0        0        0     1242 2023-05-26 17:29:39.271210 candidhealth-0.1.1/src/candid/resources/work_queues/resources/v_1/types/work_queue_category_type.py
+-rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 candidhealth-0.1.1/PKG-INFO
```

### Comparing `candidhealth-0.1.0/src/candid/__init__.py` & `candidhealth-0.1.1/src/candid/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/client.py` & `candidhealth-0.1.1/src/candid/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/core/datetime_utils.py` & `candidhealth-0.1.1/src/candid/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/core/jsonable_encoder.py` & `candidhealth-0.1.1/src/candid/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/__init__.py` & `candidhealth-0.1.1/src/candid/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/auth/client.py` & `candidhealth-0.1.1/src/candid/resources/auth/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/auth/resources/v_2/client.py` & `candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_request.py` & `candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/types/auth_get_token_request.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_response.py` & `candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/types/auth_get_token_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/auth/resources/v_2/types/too_many_requests_error_type.py` & `candidhealth-0.1.1/src/candid/resources/auth/resources/v_2/types/too_many_requests_error_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/billing_notes/client.py` & `candidhealth-0.1.1/src/candid/resources/billing_notes/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/billing_notes/types/billing_note.py` & `candidhealth-0.1.1/src/candid/resources/billing_notes/types/billing_note.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/billing_notes/types/billing_note_base.py` & `candidhealth-0.1.1/src/candid/resources/billing_notes/types/billing_note_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/claims/types/claim.py` & `candidhealth-0.1.1/src/candid/resources/claims/types/claim.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/claims/types/claim_status.py` & `candidhealth-0.1.1/src/candid/resources/claims/types/claim_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/commons/__init__.py` & `candidhealth-0.1.1/src/candid/resources/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/commons/types/__init__.py` & `candidhealth-0.1.1/src/candid/resources/commons/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/commons/types/facility_type_code.py` & `candidhealth-0.1.1/src/candid/resources/commons/types/facility_type_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/commons/types/insurance_type_code.py` & `candidhealth-0.1.1/src/candid/resources/commons/types/insurance_type_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py` & `candidhealth-0.1.1/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/commons/types/procedure_modifier.py` & `candidhealth-0.1.1/src/candid/resources/commons/types/procedure_modifier.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/commons/types/region_national.py` & `candidhealth-0.1.1/src/candid/resources/commons/types/region_national.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/commons/types/region_states.py` & `candidhealth-0.1.1/src/candid/resources/commons/types/region_states.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/commons/types/resource_page.py` & `candidhealth-0.1.1/src/candid/resources/commons/types/resource_page.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/commons/types/source_of_payment_code.py` & `candidhealth-0.1.1/src/candid/resources/commons/types/source_of_payment_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/commons/types/state.py` & `candidhealth-0.1.1/src/candid/resources/commons/types/state.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/commons/types/street_address_base.py` & `candidhealth-0.1.1/src/candid/resources/commons/types/street_address_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/commons/types/street_address_long_zip.py` & `candidhealth-0.1.1/src/candid/resources/commons/types/street_address_long_zip.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/commons/types/street_address_short_zip.py` & `candidhealth-0.1.1/src/candid/resources/commons/types/street_address_short_zip.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/contracts/types/authorized_signatory.py` & `candidhealth-0.1.1/src/candid/resources/contracts/types/authorized_signatory.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/contracts/types/contract.py` & `candidhealth-0.1.1/src/candid/resources/contracts/types/contract.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/contracts/types/contract_base.py` & `candidhealth-0.1.1/src/candid/resources/contracts/types/contract_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/contracts/types/contract_status.py` & `candidhealth-0.1.1/src/candid/resources/contracts/types/contract_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/credentialing/__init__.py` & `candidhealth-0.1.1/src/candid/resources/credentialing/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/credentialing/types/__init__.py` & `candidhealth-0.1.1/src/candid/resources/credentialing/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/credentialing/types/credentialed_encounter_status_result.py` & `candidhealth-0.1.1/src/candid/resources/credentialing/types/credentialed_encounter_status_result.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/credentialing/types/credentialing_span_dates.py` & `candidhealth-0.1.1/src/candid/resources/credentialing/types/credentialing_span_dates.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-import pydantic
 import typing_extensions
 
 from .non_required_credentialing_dates import NonRequiredCredentialingDates
 from .required_credentialing_dates import RequiredCredentialingDates
 
 
 class CredentialingSpanDates_RequiredDates(RequiredCredentialingDates):
@@ -23,11 +22,8 @@
     type: typing_extensions.Literal["non_required_dates"]
 
     class Config:
         frozen = True
         allow_population_by_field_name = True
 
 
-CredentialingSpanDates = typing_extensions.Annotated[
-    typing.Union[CredentialingSpanDates_RequiredDates, CredentialingSpanDates_NonRequiredDates],
-    pydantic.Field(discriminator="type"),
-]
+CredentialingSpanDates = typing.Union[CredentialingSpanDates_RequiredDates, CredentialingSpanDates_NonRequiredDates]
```

### Comparing `candidhealth-0.1.0/src/candid/resources/credentialing/types/credentialing_span_status.py` & `candidhealth-0.1.1/src/candid/resources/credentialing/types/credentialing_span_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/credentialing/types/encounter_credentialing_status_result.py` & `candidhealth-0.1.1/src/candid/resources/credentialing/types/encounter_credentialing_status_result.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,11 +21,10 @@
 class EncounterCredentialingStatusResult_NotCredentialed(pydantic.BaseModel):
     type: typing_extensions.Literal["not_credentialed"]
 
     class Config:
         frozen = True
 
 
-EncounterCredentialingStatusResult = typing_extensions.Annotated[
-    typing.Union[EncounterCredentialingStatusResult_Credentialed, EncounterCredentialingStatusResult_NotCredentialed],
-    pydantic.Field(discriminator="type"),
+EncounterCredentialingStatusResult = typing.Union[
+    EncounterCredentialingStatusResult_Credentialed, EncounterCredentialingStatusResult_NotCredentialed
 ]
```

### Comparing `candidhealth-0.1.0/src/candid/resources/credentialing/types/non_required_credentialing_dates.py` & `candidhealth-0.1.1/src/candid/resources/credentialing/types/non_required_credentialing_dates.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/credentialing/types/provider_credentialing_span.py` & `candidhealth-0.1.1/src/candid/resources/credentialing/types/provider_credentialing_span.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/credentialing/types/provider_credentialing_span_base.py` & `candidhealth-0.1.1/src/candid/resources/credentialing/types/provider_credentialing_span_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/credentialing/types/required_credentialing_dates.py` & `candidhealth-0.1.1/src/candid/resources/credentialing/types/required_credentialing_dates.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/diagnoses/types/diagnosis.py` & `candidhealth-0.1.1/src/candid/resources/diagnoses/types/diagnosis.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/diagnoses/types/diagnosis_create.py` & `candidhealth-0.1.1/src/candid/resources/diagnoses/types/diagnosis_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/diagnoses/types/diagnosis_type_code.py` & `candidhealth-0.1.1/src/candid/resources/diagnoses/types/diagnosis_type_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py` & `candidhealth-0.1.1/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py` & `candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py` & `candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py` & `candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py` & `candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py` & `candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py` & `candidhealth-0.1.1/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/client.py` & `candidhealth-0.1.1/src/candid/resources/encounters/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/__init__.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/client.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/__init__.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/attributable_contracting_status_result.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/attributable_contracting_status_result.py`

 * *Files 24% similar despite different names*

```diff
@@ -30,15 +30,12 @@
 class AttributableContractingStatusResult_Unknown(pydantic.BaseModel):
     contracting_status: typing_extensions.Literal["unknown"]
 
     class Config:
         frozen = True
 
 
-AttributableContractingStatusResult = typing_extensions.Annotated[
-    typing.Union[
-        AttributableContractingStatusResult_OutOfNetwork,
-        AttributableContractingStatusResult_InNetwork,
-        AttributableContractingStatusResult_Unknown,
-    ],
-    pydantic.Field(discriminator="contracting_status"),
+AttributableContractingStatusResult = typing.Union[
+    AttributableContractingStatusResult_OutOfNetwork,
+    AttributableContractingStatusResult_InNetwork,
+    AttributableContractingStatusResult_Unknown,
 ]
```

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/base_attachment.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/base_attachment.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/clinical_note.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/clinical_note.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/clinical_note_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category_create.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/clinical_note_category_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/coding_attribution_type.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/coding_attribution_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/contracting_out_of_of_network_reason.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/contracting_out_of_of_network_reason.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/encounter.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/encounter.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/encounter_attachment.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/encounter_attachment.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/encounter_base.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/encounter_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/encounter_page.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/encounter_page.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/encounter_sort_options.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/encounter_sort_options.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/in_network_contracting_status_result.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/in_network_contracting_status_result.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intake_follow_up.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intake_question.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intake_question.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intake_response_and_follow_ups.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intake_response_and_follow_ups.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intervention.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intervention.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intervention_category.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/intervention_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/lab.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/lab.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/mark_as_not_billable_response.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/mark_as_not_billable_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/medication.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/medication.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/network_status.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/network_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/network_status_computation_results.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/network_status_computation_results.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/note_category.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/note_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/out_of_network_contracting_status_result.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/out_of_network_contracting_status_result.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/patient_history_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category_enum.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/patient_history_category_enum.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/successful_generate_clinical_notes_pdf_response.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/successful_generate_clinical_notes_pdf_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/synchronicity_type.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/synchronicity_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/vitals.py` & `candidhealth-0.1.1/src/candid/resources/encounters/resources/v_4/types/vitals.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/era/types/era.py` & `candidhealth-0.1.1/src/candid/resources/era/types/era.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/era/types/era_base.py` & `candidhealth-0.1.1/src/candid/resources/era/types/era_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/expected_network_status/client.py` & `candidhealth-0.1.1/src/candid/resources/expected_network_status/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/expected_network_status/types/expected_network_status.py` & `candidhealth-0.1.1/src/candid/resources/expected_network_status/types/expected_network_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/expected_network_status/types/expected_network_status_response.py` & `candidhealth-0.1.1/src/candid/resources/expected_network_status/types/expected_network_status_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/individual/types/__init__.py` & `candidhealth-0.1.1/src/candid/resources/individual/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/individual/types/gender.py` & `candidhealth-0.1.1/src/candid/resources/individual/types/gender.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/individual/types/individual_base.py` & `candidhealth-0.1.1/src/candid/resources/individual/types/individual_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/individual/types/patient.py` & `candidhealth-0.1.1/src/candid/resources/individual/types/patient.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/individual/types/patient_create.py` & `candidhealth-0.1.1/src/candid/resources/individual/types/patient_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/individual/types/subscriber.py` & `candidhealth-0.1.1/src/candid/resources/individual/types/subscriber.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/individual/types/subscriber_base.py` & `candidhealth-0.1.1/src/candid/resources/individual/types/subscriber_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/individual/types/subscriber_create.py` & `candidhealth-0.1.1/src/candid/resources/individual/types/subscriber_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/insurance_card/types/insurance_card.py` & `candidhealth-0.1.1/src/candid/resources/insurance_card/types/insurance_card.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/insurance_card/types/insurance_card_base.py` & `candidhealth-0.1.1/src/candid/resources/insurance_card/types/insurance_card_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/insurance_card/types/insurance_card_create.py` & `candidhealth-0.1.1/src/candid/resources/insurance_card/types/insurance_card_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/invoices/types/invoice.py` & `candidhealth-0.1.1/src/candid/resources/invoices/types/invoice.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/invoices/types/invoice_item.py` & `candidhealth-0.1.1/src/candid/resources/invoices/types/invoice_item.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/invoices/types/invoice_status.py` & `candidhealth-0.1.1/src/candid/resources/invoices/types/invoice_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/__init__.py` & `candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/license_type.py` & `candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/license_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider.py` & `candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/organization_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py` & `candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_base.py` & `candidhealth-0.1.1/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/patient_payments/resources/v_2/types/patient_payment.py` & `candidhealth-0.1.1/src/candid/resources/patient_payments/resources/v_2/types/patient_payment.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_source.py` & `candidhealth-0.1.1/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_source.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_status.py` & `candidhealth-0.1.1/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/payers/client.py` & `candidhealth-0.1.1/src/candid/resources/payers/client.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/payers/types/payer.py` & `candidhealth-0.1.1/src/candid/resources/payers/types/payer.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/payers/types/payer_page.py` & `candidhealth-0.1.1/src/candid/resources/payers/types/payer_page.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/service_facility/types/encounter_service_facility.py` & `candidhealth-0.1.1/src/candid/resources/service_facility/types/encounter_service_facility.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/service_facility/types/encounter_service_facility_base.py` & `candidhealth-0.1.1/src/candid/resources/service_facility/types/encounter_service_facility_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/service_lines/__init__.py` & `candidhealth-0.1.1/src/candid/resources/service_lines/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/service_lines/types/__init__.py` & `candidhealth-0.1.1/src/candid/resources/service_lines/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/service_lines/types/denial_reason_content.py` & `candidhealth-0.1.1/src/candid/resources/service_lines/types/denial_reason_content.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/service_lines/types/drug_identification.py` & `candidhealth-0.1.1/src/candid/resources/service_lines/types/drug_identification.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/service_lines/types/measurement_unit_code.py` & `candidhealth-0.1.1/src/candid/resources/service_lines/types/measurement_unit_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/service_lines/types/service_id_qualifier.py` & `candidhealth-0.1.1/src/candid/resources/service_lines/types/service_id_qualifier.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line.py` & `candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_adjustment.py` & `candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_adjustment.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_base.py` & `candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_base_with_optionals.py` & `candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_base_with_optionals.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_create.py` & `candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_denial_reason.py` & `candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_denial_reason.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_era_data.py` & `candidhealth-0.1.1/src/candid/resources/service_lines/types/service_line_era_data.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/tags/types/tag.py` & `candidhealth-0.1.1/src/candid/resources/tags/types/tag.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/tags/types/tag_color_enum.py` & `candidhealth-0.1.1/src/candid/resources/tags/types/tag_color_enum.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/tags/types/tag_create.py` & `candidhealth-0.1.1/src/candid/resources/tags/types/tag_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/users/types/user.py` & `candidhealth-0.1.1/src/candid/resources/users/types/user.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/work_queues/resources/v_1/types/work_queue.py` & `candidhealth-0.1.1/src/candid/resources/work_queues/resources/v_1/types/work_queue.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/work_queues/resources/v_1/types/work_queue_category.py` & `candidhealth-0.1.1/src/candid/resources/work_queues/resources/v_1/types/work_queue_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.1.0/src/candid/resources/work_queues/resources/v_1/types/work_queue_category_type.py` & `candidhealth-0.1.1/src/candid/resources/work_queues/resources/v_1/types/work_queue_category_type.py`

 * *Files identical despite different names*

