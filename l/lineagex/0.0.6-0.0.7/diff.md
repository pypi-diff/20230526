# Comparing `tmp/lineagex-0.0.6.tar.gz` & `tmp/lineagex-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lineagex-0.0.6.tar", max compression
+gzip compressed data, was "lineagex-0.0.7.tar", max compression
```

## Comparing `lineagex-0.0.6.tar` & `lineagex-0.0.7.tar`

### file list

```diff
@@ -1,165 +1,165 @@
--rw-r--r--   0        0        0       55 2023-05-24 01:42:09.254432 lineagex-0.0.6/lineagex/__init__.py
--rw-r--r--   0        0        0    54175 2023-04-22 19:33:20.371862 lineagex-0.0.6/lineagex/app.js
--rw-r--r--   0        0        0    32350 2023-05-20 01:29:26.901284 lineagex-0.0.6/lineagex/ColumnLineage.py
--rw-r--r--   0        0        0    26326 2023-05-24 02:44:48.730666 lineagex-0.0.6/lineagex/ColumnLineageNoConn.py
--rw-r--r--   0        0        0     2124 2023-05-24 02:45:03.592600 lineagex-0.0.6/lineagex/example.py
--rw-r--r--   0        0        0       75 2022-10-26 09:03:26.188175 lineagex-0.0.6/lineagex/examples/dependency_example/a_table.sql
--rw-r--r--   0        0        0      251 2022-12-02 00:51:03.820262 lineagex-0.0.6/lineagex/examples/dependency_example/aa_table.sql
--rw-r--r--   0        0        0      523 2022-07-21 07:17:33.218837 lineagex-0.0.6/lineagex/examples/dependency_example/basic_patient_info.sql
--rw-r--r--   0        0        0       25 2023-05-24 02:27:29.985792 lineagex-0.0.6/lineagex/examples/dependency_example/from_aa_table.sql
--rw-r--r--   0        0        0       92 2022-10-26 09:03:35.427267 lineagex-0.0.6/lineagex/examples/dependency_example/no_dob.sql
--rw-r--r--   0        0        0       46 2023-05-23 21:49:30.792377 lineagex-0.0.6/lineagex/examples/github_example/desktop.ini
--rw-r--r--   0        0        0       77 2023-05-14 05:13:01.960169 lineagex-0.0.6/lineagex/examples/github_example/table1.sql
--rw-r--r--   0        0        0       76 2023-05-14 05:13:16.805234 lineagex-0.0.6/lineagex/examples/github_example/table2.sql
--rw-r--r--   0        0        0     2984 2023-05-17 19:49:22.688529 lineagex-0.0.6/lineagex/examples/mimic-iii/code_status.sql
--rw-r--r--   0        0        0    31332 2023-05-17 19:49:22.688529 lineagex-0.0.6/lineagex/examples/mimic-iii/comorbidity/elixhauser_ahrq_v37.sql
--rw-r--r--   0        0        0    18975 2023-05-17 19:49:22.688529 lineagex-0.0.6/lineagex/examples/mimic-iii/comorbidity/elixhauser_ahrq_v37_no_drg.sql
--rw-r--r--   0        0        0    10347 2023-05-17 19:49:22.689529 lineagex-0.0.6/lineagex/examples/mimic-iii/comorbidity/elixhauser_quan.sql
--rw-r--r--   0        0        0     2938 2023-05-17 19:49:22.689529 lineagex-0.0.6/lineagex/examples/mimic-iii/comorbidity/elixhauser_score_ahrq.sql
--rw-r--r--   0        0        0     2925 2023-05-17 19:49:22.689529 lineagex-0.0.6/lineagex/examples/mimic-iii/comorbidity/elixhauser_score_quan.sql
--rw-r--r--   0        0        0     3506 2023-05-23 23:50:36.510324 lineagex-0.0.6/lineagex/examples/mimic-iii/demographics/heightweight.sql
--rw-r--r--   0        0        0     3891 2023-05-17 19:49:22.689529 lineagex-0.0.6/lineagex/examples/mimic-iii/demographics/icustay_detail.sql
--rw-r--r--   0        0        0     1396 2023-05-17 19:49:22.690529 lineagex-0.0.6/lineagex/examples/mimic-iii/demographics/icustay_hours.sql
--rw-r--r--   0        0        0     1808 2023-05-17 19:49:22.690529 lineagex-0.0.6/lineagex/examples/mimic-iii/demographics/icustay_times.sql
--rw-r--r--   0        0        0     6521 2023-05-17 19:49:22.690529 lineagex-0.0.6/lineagex/examples/mimic-iii/demographics/note_counts.sql
--rw-r--r--   0        0        0      143 2023-05-17 19:49:22.690529 lineagex-0.0.6/lineagex/examples/mimic-iii/demographics/weight_durations.sql
--rw-r--r--   0        0        0    63797 2023-05-17 19:49:22.691529 lineagex-0.0.6/lineagex/examples/mimic-iii/diagnosis/ccs_multi_dx.csv.gz
--rw-r--r--   0        0        0     2172 2023-05-17 19:49:22.690529 lineagex-0.0.6/lineagex/examples/mimic-iii/diagnosis/README.md
--rw-r--r--   0        0        0     7140 2023-05-17 19:49:22.691529 lineagex-0.0.6/lineagex/examples/mimic-iii/durations/adenosine_durations.sql
--rw-r--r--   0        0        0     6273 2023-05-17 19:49:22.692529 lineagex-0.0.6/lineagex/examples/mimic-iii/durations/arterial_line_durations.sql
--rw-r--r--   0        0        0     7217 2023-05-17 19:49:22.692529 lineagex-0.0.6/lineagex/examples/mimic-iii/durations/central_line_durations.sql
--rw-r--r--   0        0        0     6331 2023-05-17 19:49:22.692529 lineagex-0.0.6/lineagex/examples/mimic-iii/durations/crrt_durations.sql
--rw-r--r--   0        0        0     7521 2023-05-17 19:49:22.692529 lineagex-0.0.6/lineagex/examples/mimic-iii/durations/dobutamine_dose.sql
--rw-r--r--   0        0        0     7051 2023-05-17 19:49:22.692529 lineagex-0.0.6/lineagex/examples/mimic-iii/durations/dobutamine_durations.sql
--rw-r--r--   0        0        0     7526 2023-05-17 19:49:22.693529 lineagex-0.0.6/lineagex/examples/mimic-iii/durations/dopamine_dose.sql
--rw-r--r--   0        0        0     7056 2023-05-17 19:49:22.693529 lineagex-0.0.6/lineagex/examples/mimic-iii/durations/dopamine_durations.sql
--rw-r--r--   0        0        0     8067 2023-05-17 19:49:22.693529 lineagex-0.0.6/lineagex/examples/mimic-iii/durations/epinephrine_dose.sql
--rw-r--r--   0        0        0     7110 2023-05-17 19:49:22.693529 lineagex-0.0.6/lineagex/examples/mimic-iii/durations/epinephrine_durations.sql
--rw-r--r--   0        0        0     6979 2023-05-17 19:49:22.693529 lineagex-0.0.6/lineagex/examples/mimic-iii/durations/isuprel_durations.sql
--rw-r--r--   0        0        0     6991 2023-05-17 19:49:22.693529 lineagex-0.0.6/lineagex/examples/mimic-iii/durations/milrinone_durations.sql
--rw-r--r--   0        0        0     9660 2023-05-17 19:49:22.693529 lineagex-0.0.6/lineagex/examples/mimic-iii/durations/neuroblock_dose.sql
--rw-r--r--   0        0        0     8192 2023-05-17 19:49:22.694529 lineagex-0.0.6/lineagex/examples/mimic-iii/durations/norepinephrine_dose.sql
--rw-r--r--   0        0        0     7080 2023-05-17 19:49:22.694529 lineagex-0.0.6/lineagex/examples/mimic-iii/durations/norepinephrine_durations.sql
--rw-r--r--   0        0        0     7541 2023-05-17 19:49:22.694529 lineagex-0.0.6/lineagex/examples/mimic-iii/durations/phenylephrine_dose.sql
--rw-r--r--   0        0        0     7086 2023-05-17 19:49:22.694529 lineagex-0.0.6/lineagex/examples/mimic-iii/durations/phenylephrine_durations.sql
--rw-r--r--   0        0        0     7531 2023-05-17 19:49:22.694529 lineagex-0.0.6/lineagex/examples/mimic-iii/durations/vasopressin_dose.sql
--rw-r--r--   0        0        0     7003 2023-05-17 19:49:22.694529 lineagex-0.0.6/lineagex/examples/mimic-iii/durations/vasopressin_durations.sql
--rw-r--r--   0        0        0     9595 2023-05-17 19:49:22.694529 lineagex-0.0.6/lineagex/examples/mimic-iii/durations/vasopressor_durations.sql
--rw-r--r--   0        0        0     5576 2023-05-17 19:49:22.695529 lineagex-0.0.6/lineagex/examples/mimic-iii/durations/ventilation_classification.sql
--rw-r--r--   0        0        0     4521 2023-05-17 19:49:22.695529 lineagex-0.0.6/lineagex/examples/mimic-iii/durations/ventilation_durations.sql
--rw-r--r--   0        0        0     6839 2023-05-17 19:49:22.695529 lineagex-0.0.6/lineagex/examples/mimic-iii/durations/weight_durations.sql
--rw-r--r--   0        0        0     2346 2023-05-17 19:49:22.695529 lineagex-0.0.6/lineagex/examples/mimic-iii/echo_data.sql
--rw-r--r--   0        0        0     5885 2023-05-23 23:51:44.365020 lineagex-0.0.6/lineagex/examples/mimic-iii/firstday/blood_gas_first_day.sql
--rw-r--r--   0        0        0     5385 2023-05-23 23:24:51.648101 lineagex-0.0.6/lineagex/examples/mimic-iii/firstday/blood_gas_first_day_arterial.sql
--rw-r--r--   0        0        0      139 2023-05-17 19:49:22.696529 lineagex-0.0.6/lineagex/examples/mimic-iii/firstday/first_day_sofa.sql
--rw-r--r--   0        0        0     5015 2023-05-17 19:49:22.696529 lineagex-0.0.6/lineagex/examples/mimic-iii/firstday/gcs_first_day.sql
--rw-r--r--   0        0        0     2415 2023-05-17 19:49:22.696529 lineagex-0.0.6/lineagex/examples/mimic-iii/firstday/height_first_day.sql
--rw-r--r--   0        0        0     9180 2023-05-17 19:49:22.696529 lineagex-0.0.6/lineagex/examples/mimic-iii/firstday/labs_first_day.sql
--rw-r--r--   0        0        0     9357 2023-05-17 19:49:22.697528 lineagex-0.0.6/lineagex/examples/mimic-iii/firstday/rrt_first_day.sql
--rw-r--r--   0        0        0     2205 2023-05-17 19:49:22.697528 lineagex-0.0.6/lineagex/examples/mimic-iii/firstday/urine_output_first_day.sql
--rw-r--r--   0        0        0     1148 2023-05-17 19:49:22.697528 lineagex-0.0.6/lineagex/examples/mimic-iii/firstday/ventilation_first_day.sql
--rw-r--r--   0        0        0     5200 2023-05-17 19:49:22.697528 lineagex-0.0.6/lineagex/examples/mimic-iii/firstday/vitals_first_day.sql
--rw-r--r--   0        0        0     3766 2023-05-17 19:49:22.697528 lineagex-0.0.6/lineagex/examples/mimic-iii/firstday/weight_first_day.sql
--rw-r--r--   0        0        0     3117 2023-05-17 19:49:22.698529 lineagex-0.0.6/lineagex/examples/mimic-iii/fluid_balance/colloid_bolus.sql
--rw-r--r--   0        0        0     4388 2023-05-17 19:49:22.698529 lineagex-0.0.6/lineagex/examples/mimic-iii/fluid_balance/crystalloid_bolus.sql
--rw-r--r--   0        0        0     2669 2023-05-17 19:49:22.698529 lineagex-0.0.6/lineagex/examples/mimic-iii/fluid_balance/ffp_transfusion.sql
--rw-r--r--   0        0        0     2500 2023-05-17 19:49:22.698529 lineagex-0.0.6/lineagex/examples/mimic-iii/fluid_balance/rbc_transfusion.sql
--rw-r--r--   0        0        0     1555 2023-05-17 19:49:22.698529 lineagex-0.0.6/lineagex/examples/mimic-iii/fluid_balance/urine_output.sql
--rw-r--r--   0        0        0      135 2023-05-17 19:49:22.698529 lineagex-0.0.6/lineagex/examples/mimic-iii/measurement/urine_output.sql
--rw-r--r--   0        0        0      171 2023-05-17 19:49:22.699531 lineagex-0.0.6/lineagex/examples/mimic-iii/medication/norepinephrine_equivalent_dose.sql
--rw-r--r--   0        0        0      143 2023-05-17 19:49:22.699531 lineagex-0.0.6/lineagex/examples/mimic-iii/medication/vasoactive_agent.sql
--rw-r--r--   0        0        0     1411 2023-05-17 19:49:22.699531 lineagex-0.0.6/lineagex/examples/mimic-iii/organfailure/kdigo_creatinine.sql
--rw-r--r--   0        0        0     3085 2023-05-17 19:49:22.699531 lineagex-0.0.6/lineagex/examples/mimic-iii/organfailure/kdigo_stages.sql
--rw-r--r--   0        0        0     2229 2023-05-17 19:49:22.699531 lineagex-0.0.6/lineagex/examples/mimic-iii/organfailure/kdigo_stages_48hr.sql
--rw-r--r--   0        0        0     2223 2023-05-17 19:49:22.700528 lineagex-0.0.6/lineagex/examples/mimic-iii/organfailure/kdigo_stages_7day.sql
--rw-r--r--   0        0        0     3287 2023-05-17 19:49:22.700528 lineagex-0.0.6/lineagex/examples/mimic-iii/organfailure/kdigo_uo.sql
--rw-r--r--   0        0        0     4829 2023-05-17 19:49:22.700528 lineagex-0.0.6/lineagex/examples/mimic-iii/organfailure/meld.sql
--rw-r--r--   0        0        0     3516 2023-05-17 19:49:22.701529 lineagex-0.0.6/lineagex/examples/mimic-iii/sepsis/angus.sql
--rw-r--r--   0        0        0     1035 2023-05-17 19:49:22.701529 lineagex-0.0.6/lineagex/examples/mimic-iii/sepsis/explicit.sql
--rw-r--r--   0        0        0     3954 2023-05-17 19:49:22.701529 lineagex-0.0.6/lineagex/examples/mimic-iii/sepsis/martin.sql
--rw-r--r--   0        0        0      125 2023-05-17 19:49:22.701529 lineagex-0.0.6/lineagex/examples/mimic-iii/sepsis/sepsis3.sql
--rw-r--r--   0        0        0    28187 2023-05-17 19:49:22.702529 lineagex-0.0.6/lineagex/examples/mimic-iii/severityscores/apsiii.sql
--rw-r--r--   0        0        0     7370 2023-05-17 19:49:22.702529 lineagex-0.0.6/lineagex/examples/mimic-iii/severityscores/lods.sql
--rw-r--r--   0        0        0     6878 2023-05-17 19:49:22.702529 lineagex-0.0.6/lineagex/examples/mimic-iii/severityscores/mlods.sql
--rw-r--r--   0        0        0     9670 2023-05-17 19:49:22.702529 lineagex-0.0.6/lineagex/examples/mimic-iii/severityscores/oasis.sql
--rw-r--r--   0        0        0     2594 2023-05-17 19:49:22.703529 lineagex-0.0.6/lineagex/examples/mimic-iii/severityscores/qsofa.sql
--rw-r--r--   0        0        0    10867 2023-05-17 19:49:22.703529 lineagex-0.0.6/lineagex/examples/mimic-iii/severityscores/saps.sql
--rw-r--r--   0        0        0    12484 2023-05-17 19:49:22.703529 lineagex-0.0.6/lineagex/examples/mimic-iii/severityscores/sapsii.sql
--rw-r--r--   0        0        0     3790 2023-05-17 19:49:22.703529 lineagex-0.0.6/lineagex/examples/mimic-iii/severityscores/sirs.sql
--rw-r--r--   0        0        0    10302 2023-05-17 19:49:22.704529 lineagex-0.0.6/lineagex/examples/mimic-iii/severityscores/sofa.sql
--rw-r--r--   0        0        0     8176 2023-05-17 19:49:22.704529 lineagex-0.0.6/lineagex/examples/mimic-iii/treatment/abx_prescriptions_list.sql
--rw-r--r--   0        0        0     4490 2023-05-17 19:49:22.704529 lineagex-0.0.6/lineagex/examples/mimic-iii/treatment/suspicion_of_infection.sql
--rw-r--r--   0        0        0    14187 2023-05-17 19:49:22.831516 lineagex-0.0.6/lineagex/examples/mimic-iv/comorbidity/charlson.sql
--rw-r--r--   0        0        0     6645 2023-05-17 19:49:22.831516 lineagex-0.0.6/lineagex/examples/mimic-iv/comorbidity/first_day_lab.sql
--rw-r--r--   0        0        0     1645 2023-05-17 19:49:22.831516 lineagex-0.0.6/lineagex/examples/mimic-iv/demographics/age.sql
--rw-r--r--   0        0        0     1816 2023-05-17 19:49:22.831516 lineagex-0.0.6/lineagex/examples/mimic-iv/demographics/icustay_detail.sql
--rw-r--r--   0        0        0     1732 2023-05-17 19:49:22.831516 lineagex-0.0.6/lineagex/examples/mimic-iv/demographics/icustay_hourly.sql
--rw-r--r--   0        0        0      803 2023-05-17 19:49:22.832517 lineagex-0.0.6/lineagex/examples/mimic-iv/demographics/icustay_times.sql
--rw-r--r--   0        0        0     3921 2023-05-17 19:49:22.832517 lineagex-0.0.6/lineagex/examples/mimic-iv/demographics/weight_durations.sql
--rw-r--r--   0        0        0     2030 2023-05-17 19:49:22.832517 lineagex-0.0.6/lineagex/examples/mimic-iv/firstday/first_day_bg.sql
--rw-r--r--   0        0        0     2039 2023-05-17 19:49:22.832517 lineagex-0.0.6/lineagex/examples/mimic-iv/firstday/first_day_bg_art.sql
--rw-r--r--   0        0        0     1758 2023-05-17 19:49:22.832517 lineagex-0.0.6/lineagex/examples/mimic-iv/firstday/first_day_gcs.sql
--rw-r--r--   0        0        0      757 2023-05-17 19:49:22.832517 lineagex-0.0.6/lineagex/examples/mimic-iv/firstday/first_day_height.sql
--rw-r--r--   0        0        0     7164 2023-05-17 19:49:22.833516 lineagex-0.0.6/lineagex/examples/mimic-iv/firstday/first_day_lab.sql
--rw-r--r--   0        0        0      715 2023-05-17 19:49:22.833516 lineagex-0.0.6/lineagex/examples/mimic-iv/firstday/first_day_rrt.sql
--rw-r--r--   0        0        0     9485 2023-05-17 19:49:22.833516 lineagex-0.0.6/lineagex/examples/mimic-iv/firstday/first_day_sofa.sql
--rw-r--r--   0        0        0      686 2023-05-17 19:49:22.833516 lineagex-0.0.6/lineagex/examples/mimic-iv/firstday/first_day_urine_output.sql
--rw-r--r--   0        0        0     1389 2023-05-17 19:49:22.833516 lineagex-0.0.6/lineagex/examples/mimic-iv/firstday/first_day_vitalsign.sql
--rw-r--r--   0        0        0      987 2023-05-17 19:49:22.834516 lineagex-0.0.6/lineagex/examples/mimic-iv/firstday/first_day_weight.sql
--rw-r--r--   0        0        0     8614 2023-05-17 19:49:22.834516 lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/bg.sql
--rw-r--r--   0        0        0     7196 2023-05-17 19:49:22.834516 lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/blood_differential.sql
--rw-r--r--   0        0        0     1000 2023-05-17 19:49:22.835515 lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/cardiac_marker.sql
--rw-r--r--   0        0        0     3165 2023-05-17 19:49:22.835515 lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/chemistry.sql
--rw-r--r--   0        0        0     1310 2023-05-17 19:49:22.835515 lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/coagulation.sql
--rw-r--r--   0        0        0     1578 2023-05-17 19:49:22.835515 lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/complete_blood_count.sql
--rw-r--r--   0        0        0     2136 2023-05-17 19:49:22.835515 lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/creatinine_baseline.sql
--rw-r--r--   0        0        0     1835 2023-05-17 19:49:22.836515 lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/enzyme.sql
--rw-r--r--   0        0        0     4839 2023-05-18 04:41:01.815148 lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/gcs.sql
--rw-r--r--   0        0        0     1443 2023-05-17 19:49:22.836515 lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/height.sql
--rw-r--r--   0        0        0      770 2023-05-17 19:49:22.837515 lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/icp.sql
--rw-r--r--   0        0        0      654 2023-05-17 19:49:22.837515 lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/inflammation.sql
--rw-r--r--   0        0        0      116 2023-05-17 19:49:22.837515 lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/kdigo_uo.sql
--rw-r--r--   0        0        0     3793 2023-05-17 19:49:22.837515 lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/oxygen_delivery.sql
--rw-r--r--   0        0        0     1000 2023-05-17 19:49:22.837515 lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/rhythm.sql
--rw-r--r--   0        0        0     1323 2023-05-17 19:49:22.837515 lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/urine_output.sql
--rw-r--r--   0        0        0     4550 2023-05-17 19:49:22.837515 lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/urine_output_rate.sql
--rw-r--r--   0        0        0     3415 2023-05-17 19:49:22.837515 lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/ventilator_setting.sql
--rw-r--r--   0        0        0     3709 2023-05-17 19:49:22.838515 lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/vitalsign.sql
--rw-r--r--   0        0        0    10373 2023-05-17 19:49:22.838515 lineagex-0.0.6/lineagex/examples/mimic-iv/medication/antibiotic.sql
--rw-r--r--   0        0        0      493 2023-05-17 19:49:22.838515 lineagex-0.0.6/lineagex/examples/mimic-iv/medication/dobutamine.sql
--rw-r--r--   0        0        0      486 2023-05-17 19:49:22.838515 lineagex-0.0.6/lineagex/examples/mimic-iv/medication/dopamine.sql
--rw-r--r--   0        0        0      499 2023-05-17 19:49:22.838515 lineagex-0.0.6/lineagex/examples/mimic-iv/medication/epinephrine.sql
--rw-r--r--   0        0        0      471 2023-05-17 19:49:22.838515 lineagex-0.0.6/lineagex/examples/mimic-iv/medication/milrinone.sql
--rw-r--r--   0        0        0      561 2023-05-17 19:49:22.838515 lineagex-0.0.6/lineagex/examples/mimic-iv/medication/neuroblock.sql
--rw-r--r--   0        0        0      865 2023-05-17 19:49:22.839516 lineagex-0.0.6/lineagex/examples/mimic-iv/medication/norepinephrine.sql
--rw-r--r--   0        0        0     1644 2023-05-17 19:49:22.839516 lineagex-0.0.6/lineagex/examples/mimic-iv/medication/norepinephrine_equivalent_dose.sql
--rw-r--r--   0        0        0      601 2023-05-17 19:49:22.839516 lineagex-0.0.6/lineagex/examples/mimic-iv/medication/phenylephrine.sql
--rw-r--r--   0        0        0     4576 2023-05-17 19:49:22.839516 lineagex-0.0.6/lineagex/examples/mimic-iv/medication/vasoactive_agent.sql
--rw-r--r--   0        0        0      722 2023-05-17 19:49:22.839516 lineagex-0.0.6/lineagex/examples/mimic-iv/medication/vasopressin.sql
--rw-r--r--   0        0        0     2036 2023-05-17 19:49:22.840515 lineagex-0.0.6/lineagex/examples/mimic-iv/organfailure/kdigo_creatinine.sql
--rw-r--r--   0        0        0     5580 2023-05-17 19:49:22.840515 lineagex-0.0.6/lineagex/examples/mimic-iv/organfailure/kdigo_stages.sql
--rw-r--r--   0        0        0     3802 2023-05-17 19:49:22.840515 lineagex-0.0.6/lineagex/examples/mimic-iv/organfailure/kdigo_uo.sql
--rw-r--r--   0        0        0     5701 2023-05-17 19:49:22.840515 lineagex-0.0.6/lineagex/examples/mimic-iv/organfailure/meld.sql
--rw-r--r--   0        0        0      675 2023-05-17 19:49:22.831516 lineagex-0.0.6/lineagex/examples/mimic-iv/README.md
--rw-r--r--   0        0        0    33864 2023-05-17 19:49:22.841515 lineagex-0.0.6/lineagex/examples/mimic-iv/score/apsiii.sql
--rw-r--r--   0        0        0     7695 2023-05-17 19:49:22.842515 lineagex-0.0.6/lineagex/examples/mimic-iv/score/lods.sql
--rw-r--r--   0        0        0    11246 2023-05-17 19:49:22.842515 lineagex-0.0.6/lineagex/examples/mimic-iv/score/oasis.sql
--rw-r--r--   0        0        0    17903 2023-05-17 19:49:22.842515 lineagex-0.0.6/lineagex/examples/mimic-iv/score/sapsii.sql
--rw-r--r--   0        0        0     3517 2023-05-17 19:49:22.842515 lineagex-0.0.6/lineagex/examples/mimic-iv/score/sirs.sql
--rw-r--r--   0        0        0    12603 2023-05-17 19:49:22.842515 lineagex-0.0.6/lineagex/examples/mimic-iv/score/sofa.sql
--rw-r--r--   0        0        0     2994 2023-05-17 19:49:22.843516 lineagex-0.0.6/lineagex/examples/mimic-iv/sepsis/sepsis3.sql
--rw-r--r--   0        0        0     6418 2023-05-17 19:49:22.843516 lineagex-0.0.6/lineagex/examples/mimic-iv/sepsis/suspicion_of_infection.sql
--rw-r--r--   0        0        0     6011 2023-05-17 19:49:22.843516 lineagex-0.0.6/lineagex/examples/mimic-iv/treatment/crrt.sql
--rw-r--r--   0        0        0     4777 2023-05-17 19:49:22.843516 lineagex-0.0.6/lineagex/examples/mimic-iv/treatment/invasive_line.sql
--rw-r--r--   0        0        0    13683 2023-05-18 23:24:29.938626 lineagex-0.0.6/lineagex/examples/mimic-iv/treatment/rrt.sql
--rw-r--r--   0        0        0     9285 2023-05-17 19:49:22.843516 lineagex-0.0.6/lineagex/examples/mimic-iv/treatment/ventilation.sql
--rw-r--r--   0        0        0     1802 2023-05-24 01:42:19.469427 lineagex-0.0.6/lineagex/lineagex.py
--rw-r--r--   0        0        0     4792 2023-05-24 02:45:19.755079 lineagex-0.0.6/lineagex/LineageXNoConn.py
--rw-r--r--   0        0        0    13522 2023-05-23 21:34:23.590817 lineagex-0.0.6/lineagex/LineageXWithConn.py
--rw-r--r--   0        0        0     7176 2023-05-23 22:40:25.559899 lineagex-0.0.6/lineagex/SqlToDict.py
--rw-r--r--   0        0        0     1460 2023-05-08 20:36:59.378380 lineagex-0.0.6/lineagex/stack.py
--rw-r--r--   0        0        0     7305 2023-05-19 22:10:39.261810 lineagex-0.0.6/lineagex/utils.py
--rw-r--r--   0        0        0  3761177 2023-04-22 19:33:20.645016 lineagex-0.0.6/lineagex/vendor.js
--rw-r--r--   0        0        0      448 2023-05-24 02:45:54.582891 lineagex-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4158 2023-05-17 20:42:55.789941 lineagex-0.0.6/README.md
--rw-r--r--   0        0        0     4863 1970-01-01 00:00:00.000000 lineagex-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-05-24 01:42:09.254432 lineagex-0.0.7/lineagex/__init__.py
+-rw-r--r--   0        0        0    54175 2023-04-22 19:33:20.371862 lineagex-0.0.7/lineagex/app.js
+-rw-r--r--   0        0        0    32350 2023-05-20 01:29:26.901284 lineagex-0.0.7/lineagex/ColumnLineage.py
+-rw-r--r--   0        0        0    28808 2023-05-24 23:58:27.489215 lineagex-0.0.7/lineagex/ColumnLineageNoConn.py
+-rw-r--r--   0        0        0     2124 2023-05-24 23:58:40.000867 lineagex-0.0.7/lineagex/example.py
+-rw-r--r--   0        0        0       75 2022-10-26 09:03:26.188175 lineagex-0.0.7/lineagex/examples/dependency_example/a_table.sql
+-rw-r--r--   0        0        0      251 2022-12-02 00:51:03.820262 lineagex-0.0.7/lineagex/examples/dependency_example/aa_table.sql
+-rw-r--r--   0        0        0      523 2022-07-21 07:17:33.218837 lineagex-0.0.7/lineagex/examples/dependency_example/basic_patient_info.sql
+-rw-r--r--   0        0        0       25 2023-05-24 02:27:29.985792 lineagex-0.0.7/lineagex/examples/dependency_example/from_aa_table.sql
+-rw-r--r--   0        0        0       92 2022-10-26 09:03:35.427267 lineagex-0.0.7/lineagex/examples/dependency_example/no_dob.sql
+-rw-r--r--   0        0        0       46 2023-05-23 21:49:30.792377 lineagex-0.0.7/lineagex/examples/github_example/desktop.ini
+-rw-r--r--   0        0        0       77 2023-05-14 05:13:01.960169 lineagex-0.0.7/lineagex/examples/github_example/table1.sql
+-rw-r--r--   0        0        0       76 2023-05-14 05:13:16.805234 lineagex-0.0.7/lineagex/examples/github_example/table2.sql
+-rw-r--r--   0        0        0     2984 2023-05-17 19:49:22.688529 lineagex-0.0.7/lineagex/examples/mimic-iii/code_status.sql
+-rw-r--r--   0        0        0    31332 2023-05-17 19:49:22.688529 lineagex-0.0.7/lineagex/examples/mimic-iii/comorbidity/elixhauser_ahrq_v37.sql
+-rw-r--r--   0        0        0    18975 2023-05-17 19:49:22.688529 lineagex-0.0.7/lineagex/examples/mimic-iii/comorbidity/elixhauser_ahrq_v37_no_drg.sql
+-rw-r--r--   0        0        0    10347 2023-05-17 19:49:22.689529 lineagex-0.0.7/lineagex/examples/mimic-iii/comorbidity/elixhauser_quan.sql
+-rw-r--r--   0        0        0     2938 2023-05-17 19:49:22.689529 lineagex-0.0.7/lineagex/examples/mimic-iii/comorbidity/elixhauser_score_ahrq.sql
+-rw-r--r--   0        0        0     2925 2023-05-17 19:49:22.689529 lineagex-0.0.7/lineagex/examples/mimic-iii/comorbidity/elixhauser_score_quan.sql
+-rw-r--r--   0        0        0     3506 2023-05-23 23:50:36.510324 lineagex-0.0.7/lineagex/examples/mimic-iii/demographics/heightweight.sql
+-rw-r--r--   0        0        0     3891 2023-05-17 19:49:22.689529 lineagex-0.0.7/lineagex/examples/mimic-iii/demographics/icustay_detail.sql
+-rw-r--r--   0        0        0     1396 2023-05-17 19:49:22.690529 lineagex-0.0.7/lineagex/examples/mimic-iii/demographics/icustay_hours.sql
+-rw-r--r--   0        0        0     1808 2023-05-17 19:49:22.690529 lineagex-0.0.7/lineagex/examples/mimic-iii/demographics/icustay_times.sql
+-rw-r--r--   0        0        0     6521 2023-05-17 19:49:22.690529 lineagex-0.0.7/lineagex/examples/mimic-iii/demographics/note_counts.sql
+-rw-r--r--   0        0        0      143 2023-05-17 19:49:22.690529 lineagex-0.0.7/lineagex/examples/mimic-iii/demographics/weight_durations.sql
+-rw-r--r--   0        0        0    63797 2023-05-17 19:49:22.691529 lineagex-0.0.7/lineagex/examples/mimic-iii/diagnosis/ccs_multi_dx.csv.gz
+-rw-r--r--   0        0        0     2172 2023-05-17 19:49:22.690529 lineagex-0.0.7/lineagex/examples/mimic-iii/diagnosis/README.md
+-rw-r--r--   0        0        0     7140 2023-05-17 19:49:22.691529 lineagex-0.0.7/lineagex/examples/mimic-iii/durations/adenosine_durations.sql
+-rw-r--r--   0        0        0     6273 2023-05-17 19:49:22.692529 lineagex-0.0.7/lineagex/examples/mimic-iii/durations/arterial_line_durations.sql
+-rw-r--r--   0        0        0     7217 2023-05-17 19:49:22.692529 lineagex-0.0.7/lineagex/examples/mimic-iii/durations/central_line_durations.sql
+-rw-r--r--   0        0        0     6331 2023-05-17 19:49:22.692529 lineagex-0.0.7/lineagex/examples/mimic-iii/durations/crrt_durations.sql
+-rw-r--r--   0        0        0     7521 2023-05-17 19:49:22.692529 lineagex-0.0.7/lineagex/examples/mimic-iii/durations/dobutamine_dose.sql
+-rw-r--r--   0        0        0     7051 2023-05-17 19:49:22.692529 lineagex-0.0.7/lineagex/examples/mimic-iii/durations/dobutamine_durations.sql
+-rw-r--r--   0        0        0     7526 2023-05-17 19:49:22.693529 lineagex-0.0.7/lineagex/examples/mimic-iii/durations/dopamine_dose.sql
+-rw-r--r--   0        0        0     7056 2023-05-17 19:49:22.693529 lineagex-0.0.7/lineagex/examples/mimic-iii/durations/dopamine_durations.sql
+-rw-r--r--   0        0        0     8067 2023-05-17 19:49:22.693529 lineagex-0.0.7/lineagex/examples/mimic-iii/durations/epinephrine_dose.sql
+-rw-r--r--   0        0        0     7110 2023-05-17 19:49:22.693529 lineagex-0.0.7/lineagex/examples/mimic-iii/durations/epinephrine_durations.sql
+-rw-r--r--   0        0        0     6979 2023-05-17 19:49:22.693529 lineagex-0.0.7/lineagex/examples/mimic-iii/durations/isuprel_durations.sql
+-rw-r--r--   0        0        0     6991 2023-05-17 19:49:22.693529 lineagex-0.0.7/lineagex/examples/mimic-iii/durations/milrinone_durations.sql
+-rw-r--r--   0        0        0     9660 2023-05-17 19:49:22.693529 lineagex-0.0.7/lineagex/examples/mimic-iii/durations/neuroblock_dose.sql
+-rw-r--r--   0        0        0     8192 2023-05-17 19:49:22.694529 lineagex-0.0.7/lineagex/examples/mimic-iii/durations/norepinephrine_dose.sql
+-rw-r--r--   0        0        0     7080 2023-05-17 19:49:22.694529 lineagex-0.0.7/lineagex/examples/mimic-iii/durations/norepinephrine_durations.sql
+-rw-r--r--   0        0        0     7541 2023-05-17 19:49:22.694529 lineagex-0.0.7/lineagex/examples/mimic-iii/durations/phenylephrine_dose.sql
+-rw-r--r--   0        0        0     7086 2023-05-17 19:49:22.694529 lineagex-0.0.7/lineagex/examples/mimic-iii/durations/phenylephrine_durations.sql
+-rw-r--r--   0        0        0     7531 2023-05-17 19:49:22.694529 lineagex-0.0.7/lineagex/examples/mimic-iii/durations/vasopressin_dose.sql
+-rw-r--r--   0        0        0     7003 2023-05-17 19:49:22.694529 lineagex-0.0.7/lineagex/examples/mimic-iii/durations/vasopressin_durations.sql
+-rw-r--r--   0        0        0     9595 2023-05-17 19:49:22.694529 lineagex-0.0.7/lineagex/examples/mimic-iii/durations/vasopressor_durations.sql
+-rw-r--r--   0        0        0     5576 2023-05-17 19:49:22.695529 lineagex-0.0.7/lineagex/examples/mimic-iii/durations/ventilation_classification.sql
+-rw-r--r--   0        0        0     4521 2023-05-17 19:49:22.695529 lineagex-0.0.7/lineagex/examples/mimic-iii/durations/ventilation_durations.sql
+-rw-r--r--   0        0        0     6839 2023-05-17 19:49:22.695529 lineagex-0.0.7/lineagex/examples/mimic-iii/durations/weight_durations.sql
+-rw-r--r--   0        0        0     2346 2023-05-17 19:49:22.695529 lineagex-0.0.7/lineagex/examples/mimic-iii/echo_data.sql
+-rw-r--r--   0        0        0     5885 2023-05-23 23:51:44.365020 lineagex-0.0.7/lineagex/examples/mimic-iii/firstday/blood_gas_first_day.sql
+-rw-r--r--   0        0        0     5385 2023-05-23 23:24:51.648101 lineagex-0.0.7/lineagex/examples/mimic-iii/firstday/blood_gas_first_day_arterial.sql
+-rw-r--r--   0        0        0      139 2023-05-17 19:49:22.696529 lineagex-0.0.7/lineagex/examples/mimic-iii/firstday/first_day_sofa.sql
+-rw-r--r--   0        0        0     5015 2023-05-17 19:49:22.696529 lineagex-0.0.7/lineagex/examples/mimic-iii/firstday/gcs_first_day.sql
+-rw-r--r--   0        0        0     2415 2023-05-17 19:49:22.696529 lineagex-0.0.7/lineagex/examples/mimic-iii/firstday/height_first_day.sql
+-rw-r--r--   0        0        0     9180 2023-05-17 19:49:22.696529 lineagex-0.0.7/lineagex/examples/mimic-iii/firstday/labs_first_day.sql
+-rw-r--r--   0        0        0     9357 2023-05-17 19:49:22.697528 lineagex-0.0.7/lineagex/examples/mimic-iii/firstday/rrt_first_day.sql
+-rw-r--r--   0        0        0     2205 2023-05-17 19:49:22.697528 lineagex-0.0.7/lineagex/examples/mimic-iii/firstday/urine_output_first_day.sql
+-rw-r--r--   0        0        0     1148 2023-05-17 19:49:22.697528 lineagex-0.0.7/lineagex/examples/mimic-iii/firstday/ventilation_first_day.sql
+-rw-r--r--   0        0        0     5200 2023-05-17 19:49:22.697528 lineagex-0.0.7/lineagex/examples/mimic-iii/firstday/vitals_first_day.sql
+-rw-r--r--   0        0        0     3766 2023-05-17 19:49:22.697528 lineagex-0.0.7/lineagex/examples/mimic-iii/firstday/weight_first_day.sql
+-rw-r--r--   0        0        0     3117 2023-05-17 19:49:22.698529 lineagex-0.0.7/lineagex/examples/mimic-iii/fluid_balance/colloid_bolus.sql
+-rw-r--r--   0        0        0     4388 2023-05-17 19:49:22.698529 lineagex-0.0.7/lineagex/examples/mimic-iii/fluid_balance/crystalloid_bolus.sql
+-rw-r--r--   0        0        0     2669 2023-05-17 19:49:22.698529 lineagex-0.0.7/lineagex/examples/mimic-iii/fluid_balance/ffp_transfusion.sql
+-rw-r--r--   0        0        0     2500 2023-05-17 19:49:22.698529 lineagex-0.0.7/lineagex/examples/mimic-iii/fluid_balance/rbc_transfusion.sql
+-rw-r--r--   0        0        0     1555 2023-05-17 19:49:22.698529 lineagex-0.0.7/lineagex/examples/mimic-iii/fluid_balance/urine_output.sql
+-rw-r--r--   0        0        0      135 2023-05-17 19:49:22.698529 lineagex-0.0.7/lineagex/examples/mimic-iii/measurement/urine_output.sql
+-rw-r--r--   0        0        0      171 2023-05-17 19:49:22.699531 lineagex-0.0.7/lineagex/examples/mimic-iii/medication/norepinephrine_equivalent_dose.sql
+-rw-r--r--   0        0        0      143 2023-05-17 19:49:22.699531 lineagex-0.0.7/lineagex/examples/mimic-iii/medication/vasoactive_agent.sql
+-rw-r--r--   0        0        0     1411 2023-05-17 19:49:22.699531 lineagex-0.0.7/lineagex/examples/mimic-iii/organfailure/kdigo_creatinine.sql
+-rw-r--r--   0        0        0     3085 2023-05-17 19:49:22.699531 lineagex-0.0.7/lineagex/examples/mimic-iii/organfailure/kdigo_stages.sql
+-rw-r--r--   0        0        0     2229 2023-05-17 19:49:22.699531 lineagex-0.0.7/lineagex/examples/mimic-iii/organfailure/kdigo_stages_48hr.sql
+-rw-r--r--   0        0        0     2223 2023-05-17 19:49:22.700528 lineagex-0.0.7/lineagex/examples/mimic-iii/organfailure/kdigo_stages_7day.sql
+-rw-r--r--   0        0        0     3287 2023-05-17 19:49:22.700528 lineagex-0.0.7/lineagex/examples/mimic-iii/organfailure/kdigo_uo.sql
+-rw-r--r--   0        0        0     4829 2023-05-17 19:49:22.700528 lineagex-0.0.7/lineagex/examples/mimic-iii/organfailure/meld.sql
+-rw-r--r--   0        0        0     3516 2023-05-17 19:49:22.701529 lineagex-0.0.7/lineagex/examples/mimic-iii/sepsis/angus.sql
+-rw-r--r--   0        0        0     1035 2023-05-17 19:49:22.701529 lineagex-0.0.7/lineagex/examples/mimic-iii/sepsis/explicit.sql
+-rw-r--r--   0        0        0     3954 2023-05-17 19:49:22.701529 lineagex-0.0.7/lineagex/examples/mimic-iii/sepsis/martin.sql
+-rw-r--r--   0        0        0      125 2023-05-17 19:49:22.701529 lineagex-0.0.7/lineagex/examples/mimic-iii/sepsis/sepsis3.sql
+-rw-r--r--   0        0        0    28187 2023-05-17 19:49:22.702529 lineagex-0.0.7/lineagex/examples/mimic-iii/severityscores/apsiii.sql
+-rw-r--r--   0        0        0     7370 2023-05-17 19:49:22.702529 lineagex-0.0.7/lineagex/examples/mimic-iii/severityscores/lods.sql
+-rw-r--r--   0        0        0     6878 2023-05-17 19:49:22.702529 lineagex-0.0.7/lineagex/examples/mimic-iii/severityscores/mlods.sql
+-rw-r--r--   0        0        0     9670 2023-05-17 19:49:22.702529 lineagex-0.0.7/lineagex/examples/mimic-iii/severityscores/oasis.sql
+-rw-r--r--   0        0        0     2594 2023-05-17 19:49:22.703529 lineagex-0.0.7/lineagex/examples/mimic-iii/severityscores/qsofa.sql
+-rw-r--r--   0        0        0    10867 2023-05-17 19:49:22.703529 lineagex-0.0.7/lineagex/examples/mimic-iii/severityscores/saps.sql
+-rw-r--r--   0        0        0    12484 2023-05-17 19:49:22.703529 lineagex-0.0.7/lineagex/examples/mimic-iii/severityscores/sapsii.sql
+-rw-r--r--   0        0        0     3790 2023-05-17 19:49:22.703529 lineagex-0.0.7/lineagex/examples/mimic-iii/severityscores/sirs.sql
+-rw-r--r--   0        0        0    10302 2023-05-17 19:49:22.704529 lineagex-0.0.7/lineagex/examples/mimic-iii/severityscores/sofa.sql
+-rw-r--r--   0        0        0     8176 2023-05-17 19:49:22.704529 lineagex-0.0.7/lineagex/examples/mimic-iii/treatment/abx_prescriptions_list.sql
+-rw-r--r--   0        0        0     4490 2023-05-17 19:49:22.704529 lineagex-0.0.7/lineagex/examples/mimic-iii/treatment/suspicion_of_infection.sql
+-rw-r--r--   0        0        0    14187 2023-05-17 19:49:22.831516 lineagex-0.0.7/lineagex/examples/mimic-iv/comorbidity/charlson.sql
+-rw-r--r--   0        0        0     6645 2023-05-17 19:49:22.831516 lineagex-0.0.7/lineagex/examples/mimic-iv/comorbidity/first_day_lab.sql
+-rw-r--r--   0        0        0     1645 2023-05-17 19:49:22.831516 lineagex-0.0.7/lineagex/examples/mimic-iv/demographics/age.sql
+-rw-r--r--   0        0        0     1816 2023-05-17 19:49:22.831516 lineagex-0.0.7/lineagex/examples/mimic-iv/demographics/icustay_detail.sql
+-rw-r--r--   0        0        0     1732 2023-05-17 19:49:22.831516 lineagex-0.0.7/lineagex/examples/mimic-iv/demographics/icustay_hourly.sql
+-rw-r--r--   0        0        0      803 2023-05-17 19:49:22.832517 lineagex-0.0.7/lineagex/examples/mimic-iv/demographics/icustay_times.sql
+-rw-r--r--   0        0        0     3921 2023-05-17 19:49:22.832517 lineagex-0.0.7/lineagex/examples/mimic-iv/demographics/weight_durations.sql
+-rw-r--r--   0        0        0     2030 2023-05-17 19:49:22.832517 lineagex-0.0.7/lineagex/examples/mimic-iv/firstday/first_day_bg.sql
+-rw-r--r--   0        0        0     2039 2023-05-17 19:49:22.832517 lineagex-0.0.7/lineagex/examples/mimic-iv/firstday/first_day_bg_art.sql
+-rw-r--r--   0        0        0     1758 2023-05-17 19:49:22.832517 lineagex-0.0.7/lineagex/examples/mimic-iv/firstday/first_day_gcs.sql
+-rw-r--r--   0        0        0      757 2023-05-17 19:49:22.832517 lineagex-0.0.7/lineagex/examples/mimic-iv/firstday/first_day_height.sql
+-rw-r--r--   0        0        0     7164 2023-05-17 19:49:22.833516 lineagex-0.0.7/lineagex/examples/mimic-iv/firstday/first_day_lab.sql
+-rw-r--r--   0        0        0      715 2023-05-17 19:49:22.833516 lineagex-0.0.7/lineagex/examples/mimic-iv/firstday/first_day_rrt.sql
+-rw-r--r--   0        0        0     9485 2023-05-17 19:49:22.833516 lineagex-0.0.7/lineagex/examples/mimic-iv/firstday/first_day_sofa.sql
+-rw-r--r--   0        0        0      686 2023-05-17 19:49:22.833516 lineagex-0.0.7/lineagex/examples/mimic-iv/firstday/first_day_urine_output.sql
+-rw-r--r--   0        0        0     1389 2023-05-17 19:49:22.833516 lineagex-0.0.7/lineagex/examples/mimic-iv/firstday/first_day_vitalsign.sql
+-rw-r--r--   0        0        0      987 2023-05-17 19:49:22.834516 lineagex-0.0.7/lineagex/examples/mimic-iv/firstday/first_day_weight.sql
+-rw-r--r--   0        0        0     8614 2023-05-17 19:49:22.834516 lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/bg.sql
+-rw-r--r--   0        0        0     7196 2023-05-17 19:49:22.834516 lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/blood_differential.sql
+-rw-r--r--   0        0        0     1000 2023-05-17 19:49:22.835515 lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/cardiac_marker.sql
+-rw-r--r--   0        0        0     3165 2023-05-17 19:49:22.835515 lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/chemistry.sql
+-rw-r--r--   0        0        0     1310 2023-05-17 19:49:22.835515 lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/coagulation.sql
+-rw-r--r--   0        0        0     1578 2023-05-17 19:49:22.835515 lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/complete_blood_count.sql
+-rw-r--r--   0        0        0     2136 2023-05-17 19:49:22.835515 lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/creatinine_baseline.sql
+-rw-r--r--   0        0        0     1835 2023-05-17 19:49:22.836515 lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/enzyme.sql
+-rw-r--r--   0        0        0     4839 2023-05-18 04:41:01.815148 lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/gcs.sql
+-rw-r--r--   0        0        0     1443 2023-05-17 19:49:22.836515 lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/height.sql
+-rw-r--r--   0        0        0      770 2023-05-17 19:49:22.837515 lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/icp.sql
+-rw-r--r--   0        0        0      654 2023-05-17 19:49:22.837515 lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/inflammation.sql
+-rw-r--r--   0        0        0      116 2023-05-17 19:49:22.837515 lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/kdigo_uo.sql
+-rw-r--r--   0        0        0     3793 2023-05-17 19:49:22.837515 lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/oxygen_delivery.sql
+-rw-r--r--   0        0        0     1000 2023-05-17 19:49:22.837515 lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/rhythm.sql
+-rw-r--r--   0        0        0     1323 2023-05-17 19:49:22.837515 lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/urine_output.sql
+-rw-r--r--   0        0        0     4550 2023-05-17 19:49:22.837515 lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/urine_output_rate.sql
+-rw-r--r--   0        0        0     3415 2023-05-17 19:49:22.837515 lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/ventilator_setting.sql
+-rw-r--r--   0        0        0     3709 2023-05-17 19:49:22.838515 lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/vitalsign.sql
+-rw-r--r--   0        0        0    10373 2023-05-17 19:49:22.838515 lineagex-0.0.7/lineagex/examples/mimic-iv/medication/antibiotic.sql
+-rw-r--r--   0        0        0      493 2023-05-17 19:49:22.838515 lineagex-0.0.7/lineagex/examples/mimic-iv/medication/dobutamine.sql
+-rw-r--r--   0        0        0      486 2023-05-17 19:49:22.838515 lineagex-0.0.7/lineagex/examples/mimic-iv/medication/dopamine.sql
+-rw-r--r--   0        0        0      499 2023-05-17 19:49:22.838515 lineagex-0.0.7/lineagex/examples/mimic-iv/medication/epinephrine.sql
+-rw-r--r--   0        0        0      471 2023-05-17 19:49:22.838515 lineagex-0.0.7/lineagex/examples/mimic-iv/medication/milrinone.sql
+-rw-r--r--   0        0        0      561 2023-05-17 19:49:22.838515 lineagex-0.0.7/lineagex/examples/mimic-iv/medication/neuroblock.sql
+-rw-r--r--   0        0        0      865 2023-05-17 19:49:22.839516 lineagex-0.0.7/lineagex/examples/mimic-iv/medication/norepinephrine.sql
+-rw-r--r--   0        0        0     1644 2023-05-17 19:49:22.839516 lineagex-0.0.7/lineagex/examples/mimic-iv/medication/norepinephrine_equivalent_dose.sql
+-rw-r--r--   0        0        0      601 2023-05-17 19:49:22.839516 lineagex-0.0.7/lineagex/examples/mimic-iv/medication/phenylephrine.sql
+-rw-r--r--   0        0        0     4576 2023-05-17 19:49:22.839516 lineagex-0.0.7/lineagex/examples/mimic-iv/medication/vasoactive_agent.sql
+-rw-r--r--   0        0        0      722 2023-05-17 19:49:22.839516 lineagex-0.0.7/lineagex/examples/mimic-iv/medication/vasopressin.sql
+-rw-r--r--   0        0        0     2036 2023-05-17 19:49:22.840515 lineagex-0.0.7/lineagex/examples/mimic-iv/organfailure/kdigo_creatinine.sql
+-rw-r--r--   0        0        0     5580 2023-05-17 19:49:22.840515 lineagex-0.0.7/lineagex/examples/mimic-iv/organfailure/kdigo_stages.sql
+-rw-r--r--   0        0        0     3802 2023-05-17 19:49:22.840515 lineagex-0.0.7/lineagex/examples/mimic-iv/organfailure/kdigo_uo.sql
+-rw-r--r--   0        0        0     5701 2023-05-17 19:49:22.840515 lineagex-0.0.7/lineagex/examples/mimic-iv/organfailure/meld.sql
+-rw-r--r--   0        0        0      675 2023-05-17 19:49:22.831516 lineagex-0.0.7/lineagex/examples/mimic-iv/README.md
+-rw-r--r--   0        0        0    33864 2023-05-17 19:49:22.841515 lineagex-0.0.7/lineagex/examples/mimic-iv/score/apsiii.sql
+-rw-r--r--   0        0        0     7695 2023-05-17 19:49:22.842515 lineagex-0.0.7/lineagex/examples/mimic-iv/score/lods.sql
+-rw-r--r--   0        0        0    11246 2023-05-17 19:49:22.842515 lineagex-0.0.7/lineagex/examples/mimic-iv/score/oasis.sql
+-rw-r--r--   0        0        0    17903 2023-05-17 19:49:22.842515 lineagex-0.0.7/lineagex/examples/mimic-iv/score/sapsii.sql
+-rw-r--r--   0        0        0     3517 2023-05-17 19:49:22.842515 lineagex-0.0.7/lineagex/examples/mimic-iv/score/sirs.sql
+-rw-r--r--   0        0        0    12603 2023-05-17 19:49:22.842515 lineagex-0.0.7/lineagex/examples/mimic-iv/score/sofa.sql
+-rw-r--r--   0        0        0     2994 2023-05-17 19:49:22.843516 lineagex-0.0.7/lineagex/examples/mimic-iv/sepsis/sepsis3.sql
+-rw-r--r--   0        0        0     6418 2023-05-17 19:49:22.843516 lineagex-0.0.7/lineagex/examples/mimic-iv/sepsis/suspicion_of_infection.sql
+-rw-r--r--   0        0        0     6011 2023-05-17 19:49:22.843516 lineagex-0.0.7/lineagex/examples/mimic-iv/treatment/crrt.sql
+-rw-r--r--   0        0        0     4777 2023-05-17 19:49:22.843516 lineagex-0.0.7/lineagex/examples/mimic-iv/treatment/invasive_line.sql
+-rw-r--r--   0        0        0    13683 2023-05-18 23:24:29.938626 lineagex-0.0.7/lineagex/examples/mimic-iv/treatment/rrt.sql
+-rw-r--r--   0        0        0     9285 2023-05-17 19:49:22.843516 lineagex-0.0.7/lineagex/examples/mimic-iv/treatment/ventilation.sql
+-rw-r--r--   0        0        0     2179 2023-05-25 21:16:42.019016 lineagex-0.0.7/lineagex/lineagex.py
+-rw-r--r--   0        0        0     4792 2023-05-24 22:21:05.454503 lineagex-0.0.7/lineagex/LineageXNoConn.py
+-rw-r--r--   0        0        0    14199 2023-05-26 20:54:14.280069 lineagex-0.0.7/lineagex/LineageXWithConn.py
+-rw-r--r--   0        0        0     7176 2023-05-23 22:40:25.559899 lineagex-0.0.7/lineagex/SqlToDict.py
+-rw-r--r--   0        0        0     1460 2023-05-08 20:36:59.378380 lineagex-0.0.7/lineagex/stack.py
+-rw-r--r--   0        0        0     7305 2023-05-19 22:10:39.261810 lineagex-0.0.7/lineagex/utils.py
+-rw-r--r--   0        0        0  3761177 2023-04-22 19:33:20.645016 lineagex-0.0.7/lineagex/vendor.js
+-rw-r--r--   0        0        0      448 2023-05-26 20:55:43.810146 lineagex-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3017 2023-05-26 19:08:04.665328 lineagex-0.0.7/README.md
+-rw-r--r--   0        0        0     3690 1970-01-01 00:00:00.000000 lineagex-0.0.7/PKG-INFO
```

### Comparing `lineagex-0.0.6/lineagex/app.js` & `lineagex-0.0.7/lineagex/app.js`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/ColumnLineage.py` & `lineagex-0.0.7/lineagex/ColumnLineage.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/ColumnLineageNoConn.py` & `lineagex-0.0.7/lineagex/ColumnLineageNoConn.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,26 @@
     exp.EQ,
     exp.Group,
     exp.Having,
     exp.Order,
     exp.From,
     exp.Join,
 ]
+from_join_exp = [exp.From, exp.Join]
 
 
 class ColumnLineageNoConn:
     def __init__(
         self, sql: Optional[str] = "", input_table_dict: Optional[dict] = None
     ):
         self.column_dict = {}
         self.table_alias_dict = {}
         self.cte_table_dict = {}
         self.cte_dict = {}
+        self.unnest_dict = {}
         self.input_table_dict = input_table_dict
         self.sql_ast = parse_one(sql, read="postgres")
         self.all_used_col = []
         self.table_list = []
         self.all_subquery_table = []
         self.sub_tables = []
         self.sub_cols = []
@@ -34,15 +36,15 @@
         # Everything other than CTEs, and pop the CTE tree
         for with_sql in self.sql_ast.find_all(exp.With):
             with_sql.pop()
         self._sub_shared_col_conds(sql_ast=self.sql_ast)
         self._run_lineage(self.sql_ast, False)
         # print(self.cte_dict)
         # print(self.column_dict)
-        # print(self.table_list)
+        # print(self.cte_table_dict)
 
     def _run_lineage(
         self, sql_ast: expressions = None, subquery_flag: bool = False
     ) -> None:
         """
         Run the lineage after all the cte and subquery are resolved
         :param sql_ast: the ast for the sql
@@ -100,15 +102,15 @@
 
     def _sub_shared_col_conds(self, sql_ast: expressions = None) -> None:
         """
         After the cte are resolved, run the subquery ast that is with the shared conditions(WHERE, GROUP BY, etc)
         :param sql_ast: the ast without the cte
         """
         # add in more conditions, including FROM/JOIN
-        for cond in shared_conditions_with_table:
+        for cond in shared_conditions + from_join_exp:
             for cond_sql in sql_ast.find_all(cond):
                 for sub_ast in cond_sql.find_all(exp.Subquery):
                     self.sub_tables = self._resolve_table(part_ast=sub_ast)
                     self.all_subquery_table.extend(
                         self._find_all_tables(temp_table_list=self.sub_tables)
                     )
                     self._run_lineage(sub_ast, True)
@@ -120,17 +122,17 @@
         """
         Run the subquery inside the cte first that is with the shared conditions(WHERE, GROUP BY, etc)
         :param sql_ast: the ast for the cte
         """
         all_cte_sub_table = []
         all_cte_sub_cols = []
         # add in more conditions, including FROM/JOIN
-        for cond in shared_conditions_with_table:
+        for cond in shared_conditions + from_join_exp:
             for cond_sql in sql_ast.find_all(cond):
-                for sub_ast in cond_sql.find_all(exp.Select):
+                for sub_ast in cond_sql.find_all(exp.Subquery):
                     temp_sub_table = self._resolve_table(part_ast=sub_ast)
                     temp_sub_cols = []
                     temp_dict = {}
                     for col in sub_ast.find_all(exp.Column):
                         if col.find(exp.Star):
                             temp_dict = self._resolve_agg_star(
                                 col_name="*",
@@ -208,15 +210,15 @@
         Resolve the projection given the projection expression
         :param projection: the given projection
         :param col_name: the column name
         :param target_dict: the dict it is outputting to
         :param source_table: all the source tables that this column might originate from
         """
         # Resolve count(*) with no alias, potentially other aggregations, MIN, MAX, SUM
-        if projection.find(exp.Star):
+        if projection.find(exp.Star) and not isinstance(projection.unalias(), exp.Array) and not isinstance(projection, exp.Array):
             if isinstance(projection, exp.Count):
                 col_name = "count"
                 target_dict = self._resolve_agg_star(
                     col_name=col_name,
                     projection=projection,
                     used_tables=source_table,
                     target_dict=target_dict,
@@ -256,14 +258,27 @@
             else:
                 target_dict = self._resolve_agg_star(
                     col_name=col_name,
                     projection=projection.unalias(),
                     used_tables=source_table,
                     target_dict=target_dict,
                 )
+        elif isinstance(projection.unalias(), exp.Array) or isinstance(projection, exp.Array):
+            temp_col = []
+            proj_columns = []
+            for p in projection.find_all(exp.Column):
+                temp_col.append(p.sql())
+            for p in temp_col:
+                proj_columns.extend(self._find_alias_col(
+                                col_sql=p,
+                                temp_table=source_table,
+                            ))
+            target_dict[col_name] = sorted(
+                list(set(proj_columns).union(self.all_used_col))
+                )
         else:
             proj_columns = []
             # Resolve only *
             if not isinstance(projection, exp.Column) and projection.find(exp.Star):
                 for t_name in source_table:
                     if t_name in self.input_table_dict.keys():
                         star_cols = self.input_table_dict[t_name]
@@ -342,26 +357,50 @@
 
     def _resolve_table(self, part_ast: expressions = None) -> List:
         """
         Find the tables in the given ast
         :param part_ast: the ast to find the table
         """
         temp_table_list = []
-        # Resolve FROM
-        for table_sql in part_ast.find_all(exp.From):
-            for table in table_sql.find_all(exp.Table):
-                temp_table_list = self._find_table(
-                    table=table, temp_table_list=temp_table_list
-                )
-        # Resolve JOIN
-        for table_sql in part_ast.find_all(exp.Join):
-            for table in table_sql.find_all(exp.Table):
-                temp_table_list = self._find_table(
-                    table=table, temp_table_list=temp_table_list
-                )
+        for cond in from_join_exp:
+            # Resolve FROM and JOIN
+            for table_sql in part_ast.find_all(cond):
+                # Skip GenerateSeries as a Table
+                if table_sql.find(exp.GenerateSeries):
+                    if table_sql.find(exp.GenerateSeries).depth <= table_sql.depth + 2:
+                        continue
+                # Resolve Unnest for creating tables
+                elif table_sql.find(exp.Unnest):
+                    temp_col_name = []
+                    for t in table_sql.find_all(exp.Identifier):
+                        temp_col_name.append(t.text("this"))
+                        dep_tables = []
+                        if len(temp_col_name) == 2:
+                            dep_cols = self._find_alias_col(
+                                col_sql=temp_col_name[1] + "." + temp_col_name[0],
+                                temp_table=[temp_col_name[1]],
+                            )
+                            self.all_used_col.extend(dep_cols)
+                            for x in dep_cols:
+                                if len(x.split(".")) == 3:
+                                    idx = x.rfind(".")
+                                    dep_tables.append(x[:idx])
+                                elif len(x.split(".")) == 2:
+                                    dep_tables.append(x)
+                            dep_tables = list(set(dep_tables))
+                            self.table_alias_dict[temp_col_name[0]] = dep_tables
+                            self.unnest_dict[temp_col_name[0]] = dep_cols
+                            if table_sql.find(exp.TableAlias):
+                                self.table_alias_dict[table_sql.find(exp.TableAlias).text("this")] = dep_tables
+                                self.unnest_dict[table_sql.find(exp.TableAlias).text("this")] = dep_cols
+                        temp_table_list.extend(dep_tables)
+                for table in table_sql.find_all(exp.Table):
+                    temp_table_list = self._find_table(
+                        table=table, temp_table_list=temp_table_list
+                    )
         return temp_table_list
 
     def _find_table(
         self, table: expressions = None, temp_table_list: Optional[List] = None
     ) -> List:
         """
         Update table alias and find all aliased used table names
@@ -422,14 +461,16 @@
         :param col_sql: the sql to the column
         :param temp_table: the table that the sql uses
         :return:
         """
         temp = col_sql.split(".")
         # trying to deduce the table if all possible tables are eliminated
         elim_table = []
+        if col_sql in self.unnest_dict.keys():
+            return self.unnest_dict[col_sql]
         if len(temp) < 2:
             for t in temp_table:
                 if t in self.input_table_dict.keys():
                     if col_sql in self.input_table_dict[t]:
                         return [t + "." + col_sql]
                     else:
                         elim_table.append(t)
```

### Comparing `lineagex-0.0.6/lineagex/example.py` & `lineagex-0.0.7/lineagex/example.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/dependency_example/basic_patient_info.sql` & `lineagex-0.0.7/lineagex/examples/dependency_example/basic_patient_info.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/code_status.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/code_status.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/comorbidity/elixhauser_ahrq_v37.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/comorbidity/elixhauser_ahrq_v37.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/comorbidity/elixhauser_ahrq_v37_no_drg.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/comorbidity/elixhauser_ahrq_v37_no_drg.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/comorbidity/elixhauser_quan.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/comorbidity/elixhauser_quan.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/comorbidity/elixhauser_score_ahrq.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/comorbidity/elixhauser_score_ahrq.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/comorbidity/elixhauser_score_quan.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/comorbidity/elixhauser_score_quan.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/demographics/heightweight.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/demographics/heightweight.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/demographics/icustay_detail.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/demographics/icustay_detail.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/demographics/icustay_hours.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/demographics/icustay_hours.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/demographics/icustay_times.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/demographics/icustay_times.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/demographics/note_counts.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/demographics/note_counts.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/diagnosis/ccs_multi_dx.csv.gz` & `lineagex-0.0.7/lineagex/examples/mimic-iii/diagnosis/ccs_multi_dx.csv.gz`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/diagnosis/README.md` & `lineagex-0.0.7/lineagex/examples/mimic-iii/diagnosis/README.md`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/durations/adenosine_durations.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/durations/adenosine_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/durations/arterial_line_durations.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/durations/arterial_line_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/durations/central_line_durations.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/durations/central_line_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/durations/crrt_durations.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/durations/crrt_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/durations/dobutamine_dose.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/durations/dobutamine_dose.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/durations/dobutamine_durations.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/durations/dobutamine_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/durations/dopamine_dose.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/durations/dopamine_dose.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/durations/dopamine_durations.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/durations/dopamine_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/durations/epinephrine_dose.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/durations/epinephrine_dose.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/durations/epinephrine_durations.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/durations/epinephrine_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/durations/isuprel_durations.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/durations/isuprel_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/durations/milrinone_durations.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/durations/milrinone_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/durations/neuroblock_dose.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/durations/neuroblock_dose.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/durations/norepinephrine_dose.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/durations/norepinephrine_dose.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/durations/norepinephrine_durations.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/durations/norepinephrine_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/durations/phenylephrine_dose.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/durations/phenylephrine_dose.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/durations/phenylephrine_durations.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/durations/phenylephrine_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/durations/vasopressin_dose.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/durations/vasopressin_dose.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/durations/vasopressin_durations.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/durations/vasopressin_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/durations/vasopressor_durations.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/durations/vasopressor_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/durations/ventilation_classification.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/durations/ventilation_classification.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/durations/ventilation_durations.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/durations/ventilation_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/durations/weight_durations.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/durations/weight_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/echo_data.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/echo_data.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/firstday/blood_gas_first_day.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/firstday/blood_gas_first_day.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/firstday/blood_gas_first_day_arterial.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/firstday/blood_gas_first_day_arterial.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/firstday/gcs_first_day.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/firstday/gcs_first_day.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/firstday/height_first_day.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/firstday/height_first_day.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/firstday/labs_first_day.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/firstday/labs_first_day.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/firstday/rrt_first_day.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/firstday/rrt_first_day.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/firstday/urine_output_first_day.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/firstday/urine_output_first_day.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/firstday/ventilation_first_day.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/firstday/ventilation_first_day.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/firstday/vitals_first_day.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/firstday/vitals_first_day.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/firstday/weight_first_day.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/firstday/weight_first_day.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/fluid_balance/colloid_bolus.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/fluid_balance/colloid_bolus.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/fluid_balance/crystalloid_bolus.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/fluid_balance/crystalloid_bolus.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/fluid_balance/ffp_transfusion.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/fluid_balance/ffp_transfusion.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/fluid_balance/rbc_transfusion.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/fluid_balance/rbc_transfusion.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/fluid_balance/urine_output.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/fluid_balance/urine_output.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/organfailure/kdigo_creatinine.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/organfailure/kdigo_creatinine.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/organfailure/kdigo_stages.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/organfailure/kdigo_stages.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/organfailure/kdigo_stages_48hr.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/organfailure/kdigo_stages_48hr.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/organfailure/kdigo_stages_7day.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/organfailure/kdigo_stages_7day.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/organfailure/kdigo_uo.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/organfailure/kdigo_uo.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/organfailure/meld.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/organfailure/meld.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/sepsis/angus.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/sepsis/angus.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/sepsis/explicit.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/sepsis/explicit.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/sepsis/martin.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/sepsis/martin.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/severityscores/apsiii.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/severityscores/apsiii.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/severityscores/lods.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/severityscores/lods.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/severityscores/mlods.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/severityscores/mlods.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/severityscores/oasis.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/severityscores/oasis.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/severityscores/qsofa.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/severityscores/qsofa.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/severityscores/saps.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/severityscores/saps.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/severityscores/sapsii.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/severityscores/sapsii.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/severityscores/sirs.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/severityscores/sirs.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/severityscores/sofa.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/severityscores/sofa.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/treatment/abx_prescriptions_list.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/treatment/abx_prescriptions_list.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iii/treatment/suspicion_of_infection.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iii/treatment/suspicion_of_infection.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/comorbidity/charlson.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/comorbidity/charlson.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/comorbidity/first_day_lab.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/comorbidity/first_day_lab.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/demographics/age.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/demographics/age.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/demographics/icustay_detail.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/demographics/icustay_detail.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/demographics/icustay_hourly.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/demographics/icustay_hourly.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/demographics/icustay_times.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/demographics/icustay_times.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/demographics/weight_durations.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/demographics/weight_durations.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/firstday/first_day_bg.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/firstday/first_day_bg.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/firstday/first_day_bg_art.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/firstday/first_day_bg_art.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/firstday/first_day_gcs.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/firstday/first_day_gcs.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/firstday/first_day_height.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/firstday/first_day_height.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/firstday/first_day_lab.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/firstday/first_day_lab.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/firstday/first_day_rrt.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/firstday/first_day_rrt.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/firstday/first_day_sofa.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/firstday/first_day_sofa.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/firstday/first_day_urine_output.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/firstday/first_day_urine_output.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/firstday/first_day_vitalsign.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/firstday/first_day_vitalsign.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/firstday/first_day_weight.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/firstday/first_day_weight.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/bg.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/bg.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/blood_differential.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/blood_differential.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/cardiac_marker.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/cardiac_marker.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/chemistry.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/chemistry.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/coagulation.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/coagulation.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/complete_blood_count.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/complete_blood_count.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/creatinine_baseline.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/creatinine_baseline.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/enzyme.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/enzyme.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/gcs.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/gcs.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/height.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/height.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/icp.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/icp.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/inflammation.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/inflammation.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/oxygen_delivery.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/oxygen_delivery.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/rhythm.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/rhythm.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/urine_output.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/urine_output.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/urine_output_rate.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/urine_output_rate.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/ventilator_setting.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/ventilator_setting.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/measurement/vitalsign.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/measurement/vitalsign.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/medication/antibiotic.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/medication/antibiotic.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/medication/neuroblock.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/medication/neuroblock.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/medication/norepinephrine.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/medication/norepinephrine.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/medication/norepinephrine_equivalent_dose.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/medication/norepinephrine_equivalent_dose.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/medication/phenylephrine.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/medication/phenylephrine.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/medication/vasoactive_agent.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/medication/vasoactive_agent.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/medication/vasopressin.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/medication/vasopressin.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/organfailure/kdigo_creatinine.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/organfailure/kdigo_creatinine.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/organfailure/kdigo_stages.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/organfailure/kdigo_stages.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/organfailure/kdigo_uo.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/organfailure/kdigo_uo.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/organfailure/meld.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/organfailure/meld.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/README.md` & `lineagex-0.0.7/lineagex/examples/mimic-iv/README.md`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/score/apsiii.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/score/apsiii.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/score/lods.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/score/lods.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/score/oasis.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/score/oasis.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/score/sapsii.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/score/sapsii.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/score/sirs.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/score/sirs.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/score/sofa.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/score/sofa.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/sepsis/sepsis3.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/sepsis/sepsis3.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/sepsis/suspicion_of_infection.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/sepsis/suspicion_of_infection.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/treatment/crrt.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/treatment/crrt.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/treatment/invasive_line.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/treatment/invasive_line.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/treatment/rrt.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/treatment/rrt.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/examples/mimic-iv/treatment/ventilation.sql` & `lineagex-0.0.7/lineagex/examples/mimic-iv/treatment/ventilation.sql`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/LineageXNoConn.py` & `lineagex-0.0.7/lineagex/LineageXNoConn.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/LineageXWithConn.py` & `lineagex-0.0.7/lineagex/LineageXWithConn.py`

 * *Files 6% similar despite different names*

```diff
@@ -196,41 +196,52 @@
         """
         try:
             print(name + " processing")
             if name in self.creation_list:
                 self._create_view(name=name, sql=sql)
                 self.new_view_list.append(self.schema + "." + name)
                 self.creation_list.pop(self.creation_list.index(name))
+                table_name = self.schema + "." + name
+            elif name.isnumeric():
+                table_name = "lineagex_temp_{}".format(name)
+                self._create_view(name=table_name, sql=sql)
+                self.new_view_list.append(self.schema + "." + table_name)
+            elif name.find("_DELETION_") or name.find("_INSERTION_"):
+                table_name = name.replace(".", "_")
+                self._create_view(name=table_name, sql=sql)
+                self.new_view_list.append(self.schema + "." + table_name)
             else:
                 cur = self.conn.cursor()
                 cur.execute("""SET search_path TO {};""".format(self.search_schema))
                 cur.execute(
                     """SELECT CONCAT (schemaname,'.', tablename) from pg_tables WHERE schemaname = '{0}' and tablename = '{1}'""".format(
                         self.schema, name
                     )
                 )
                 table_result = cur.fetchone()
                 cur.close()
                 if not table_result:
                     self._create_view(name=name, sql=sql)
                     self.new_view_list.append(self.schema + "." + name)
-            table_name = self.schema + "." + name
+                table_name = self.schema + "." + name
             cols = find_column(
                 table_name=table_name,
                 engine=self.conn,
                 search_schema=self.search_schema,
             )
             col_lineage = ColumnLineage(
                 plan=self._get_plan(sql=sql),
                 sql=sql,
                 columns=cols,
                 conn=self.conn,
                 part_tables=self.part_tables,
                 search_schema=self.search_schema,
             )
+            if name.isnumeric() or name.find("_DELETION_") or name.find("_INSERTION_"):
+                table_name = name
             self.output_dict[table_name] = {
                 "tables": col_lineage.table_list,
                 "columns": col_lineage.column_dict,
                 "table_name": table_name,
             }
             self.finished_list.append(name)
             while not self.s.isEmpty():
```

### Comparing `lineagex-0.0.6/lineagex/SqlToDict.py` & `lineagex-0.0.7/lineagex/SqlToDict.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/stack.py` & `lineagex-0.0.7/lineagex/stack.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/utils.py` & `lineagex-0.0.7/lineagex/utils.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.6/lineagex/vendor.js` & `lineagex-0.0.7/lineagex/vendor.js`

 * *Files identical despite different names*

