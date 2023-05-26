# Comparing `tmp/pilk-0.2.3.tar.gz` & `tmp/pilk-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilk-0.2.3.tar", last modified: Wed Dec 21 01:55:08 2022, max compression
+gzip compressed data, was "pilk-0.2.4.tar", last modified: Fri May 26 03:28:30 2023, max compression
```

## Comparing `pilk-0.2.3.tar` & `pilk-0.2.4.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxrwxrwx   0        0        0        0 2022-12-21 01:55:08.038974 pilk-0.2.3/
--rw-rw-rw-   0        0        0    35823 2022-01-04 03:32:55.000000 pilk-0.2.3/LICENSE
--rw-rw-rw-   0        0        0       77 2022-05-18 14:04:57.000000 pilk-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     8887 2022-12-21 01:55:08.038974 pilk-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     7631 2022-03-27 06:13:15.000000 pilk-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2022-12-21 01:55:07.929086 pilk-0.2.3/pilk/
--rw-rw-rw-   0        0        0      649 2022-08-06 06:58:57.000000 pilk-0.2.3/pilk/SilkDecoder.py
--rw-rw-rw-   0        0        0     1727 2022-08-06 06:58:57.000000 pilk-0.2.3/pilk/SilkEncoder.py
--rw-rw-rw-   0        0        0     1596 2022-12-03 10:31:36.000000 pilk-0.2.3/pilk/__init__.py
--rw-rw-rw-   0        0        0     1851 2022-05-17 13:53:41.000000 pilk-0.2.3/pilk/_pilk.pyi
-drwxrwxrwx   0        0        0        0 2022-12-21 01:55:07.941591 pilk-0.2.3/pilk.egg-info/
--rw-rw-rw-   0        0        0     8887 2022-12-21 01:55:07.000000 pilk-0.2.3/pilk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11156 2022-12-21 01:55:07.000000 pilk-0.2.3/pilk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-21 01:55:07.000000 pilk-0.2.3/pilk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-08-06 10:40:14.000000 pilk-0.2.3/pilk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2022-12-21 01:55:07.000000 pilk-0.2.3/pilk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-12-21 01:55:07.000000 pilk-0.2.3/pilk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2021-12-31 06:14:52.000000 pilk-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-21 01:55:08.038974 pilk-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     2125 2022-12-21 01:47:46.000000 pilk-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-21 01:55:07.941591 pilk-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2022-12-21 01:55:08.038974 pilk-0.2.3/src/SKP_SILK_SRC/
--rw-rw-rw-   0        0        0    12147 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_A2NLSF.c
--rw-rw-rw-   0        0        0     4228 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_AsmHelper.h
--rw-rw-rw-   0        0        0     6402 2021-12-21 05:00:19.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_AsmPreproc.h
--rw-rw-rw-   0        0        0     7016 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_CNG.c
--rw-rw-rw-   0        0        0     6610 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_HP_variable_cutoff_FIX.c
--rw-rw-rw-   0        0        0    10724 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_Inlines.h
--rw-rw-rw-   0        0        0     2175 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_LBRR_reset.c
--rw-rw-rw-   0        0        0     7125 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_LPC_inv_pred_gain.c
--rw-rw-rw-   0        0        0     5760 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_LPC_synthesis_filter.c
--rw-rw-rw-   0        0        0     8900 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_LPC_synthesis_order16.c
--rw-rw-rw-   0        0        0     9742 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_LP_variable_cutoff.c
--rw-rw-rw-   0        0        0     4462 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_LSF_cos_table.c
--rw-rw-rw-   0        0        0     4234 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_LTP_analysis_filter_FIX.c
--rw-rw-rw-   0        0        0     4007 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_LTP_scale_ctrl_FIX.c
--rw-rw-rw-   0        0        0     5623 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_MA.c
--rw-rw-rw-   0        0        0     6581 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_NLSF2A.c
--rw-rw-rw-   0        0        0     2950 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_NLSF2A_stable.c
--rw-rw-rw-   0        0        0     4723 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_NLSF_MSVQ_decode.c
--rw-rw-rw-   0        0        0    12279 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_NLSF_MSVQ_encode_FIX.c
--rw-rw-rw-   0        0        0     3792 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_NLSF_VQ_rate_distortion_FIX.c
--rw-rw-rw-   0        0        0     4381 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_NLSF_VQ_sum_error_FIX.c
--rw-rw-rw-   0        0        0     4127 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_NLSF_VQ_weights_laroia.c
--rw-rw-rw-   0        0        0     6634 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_NLSF_stabilize.c
--rw-rw-rw-   0        0        0    24962 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_NSQ.c
--rw-rw-rw-   0        0        0    41591 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_NSQ_del_dec.c
--rw-rw-rw-   0        0        0    20697 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_PLC.c
--rw-rw-rw-   0        0        0     4318 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_PLC.h
--rw-rw-rw-   0        0        0    35908 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_SigProc_FIX.h
--rw-rw-rw-   0        0        0    14235 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_VAD.c
--rw-rw-rw-   0        0        0     8474 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_VQ_nearest_neighbor_FIX.c
--rw-rw-rw-   0        0        0     4460 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_ana_filt_bank_1.c
--rw-rw-rw-   0        0        0     6093 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_apply_sine_window.c
--rw-rw-rw-   0        0        0     3604 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_array_maxabs.c
--rw-rw-rw-   0        0        0     4460 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_autocorr.c
--rw-rw-rw-   0        0        0     3776 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_biquad.c
--rw-rw-rw-   0        0        0     4128 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_biquad_alt.c
--rw-rw-rw-   0        0        0    14193 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_burg_modified.c
--rw-rw-rw-   0        0        0     2841 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_bwexpander.c
--rw-rw-rw-   0        0        0     2532 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_bwexpander_32.c
--rw-rw-rw-   0        0        0     4620 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_code_signs.c
--rw-rw-rw-   0        0        0     4018 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_common_pitch_est_defines.h
--rw-rw-rw-   0        0        0     7222 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_control_audio_bandwidth.c
--rw-rw-rw-   0        0        0    19231 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_control_codec_FIX.c
--rw-rw-rw-   0        0        0     8021 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_corrMatrix_FIX.c
--rw-rw-rw-   0        0        0     2535 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_create_init_destroy.c
--rw-rw-rw-   0        0        0    12568 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_dec_API.c
--rw-rw-rw-   0        0        0    16449 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_decode_core.c
--rw-rw-rw-   0        0        0     7150 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_decode_frame.c
--rw-rw-rw-   0        0        0    11872 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_decode_parameters.c
--rw-rw-rw-   0        0        0     3013 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_decode_pitch.c
--rw-rw-rw-   0        0        0     5343 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_decode_pulses.c
--rw-rw-rw-   0        0        0     4031 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_decoder_set_fs.c
--rw-rw-rw-   0        0        0    14448 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_define.h
--rw-rw-rw-   0        0        0     4027 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_detect_SWB_input.c
--rw-rw-rw-   0        0        0     1965 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_div_oabi.c
--rw-rw-rw-   0        0        0     9765 2022-05-17 12:28:31.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_enc_API.c
--rw-rw-rw-   0        0        0    20676 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_encode_frame_FIX.c
--rw-rw-rw-   0        0        0     7182 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_encode_parameters.c
--rw-rw-rw-   0        0        0     8338 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_encode_pulses.c
--rw-rw-rw-   0        0        0     7620 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_find_LPC_FIX.c
--rw-rw-rw-   0        0        0    13040 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_find_LTP_FIX.c
--rw-rw-rw-   0        0        0     6883 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_find_pitch_lags_FIX.c
--rw-rw-rw-   0        0        0     6731 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_find_pred_coefs_FIX.c
--rw-rw-rw-   0        0        0     4921 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_gain_quant.c
--rw-rw-rw-   0        0        0     2792 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_init_encoder_FIX.c
--rw-rw-rw-   0        0        0     3774 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_inner_prod_aligned.c
--rw-rw-rw-   0        0        0     2749 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_interpolate.c
--rw-rw-rw-   0        0        0     3367 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_k2a.c
--rw-rw-rw-   0        0        0     3343 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_k2a_Q16.c
--rw-rw-rw-   0        0        0     3000 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_lin2log.c
--rw-rw-rw-   0        0        0     3370 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_log2lin.c
--rw-rw-rw-   0        0        0     5782 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_macros.h
--rw-rw-rw-   0        0        0     9732 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_macros_arm.h
--rw-rw-rw-   0        0        0    23449 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_main.h
--rw-rw-rw-   0        0        0    22891 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_main_FIX.h
--rw-rw-rw-   0        0        0    26006 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_noise_shape_analysis_FIX.c
--rw-rw-rw-   0        0        0    35387 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_pitch_analysis_core.c
--rw-rw-rw-   0        0        0     2338 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_pitch_est_defines.h
--rw-rw-rw-   0        0        0     3865 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_pitch_est_tables.c
--rw-rw-rw-   0        0        0    12561 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_prefilter_FIX.c
--rw-rw-rw-   0        0        0     6881 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_process_NLSFs_FIX.c
--rw-rw-rw-   0        0        0     6196 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_process_gains_FIX.c
--rw-rw-rw-   0        0        0     5276 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_quant_LTP_gains_FIX.c
--rw-rw-rw-   0        0        0    14752 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_range_coder.c
--rw-rw-rw-   0        0        0     2560 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_regularize_correlations_FIX.c
--rw-rw-rw-   0        0        0    14588 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler.c
--rw-rw-rw-   0        0        0     4127 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_down2.c
--rw-rw-rw-   0        0        0     5163 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_down2_3.c
--rw-rw-rw-   0        0        0     4661 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_down3.c
--rw-rw-rw-   0        0        0     6577 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_private.h
--rw-rw-rw-   0        0        0     3111 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_private_AR2.c
--rw-rw-rw-   0        0        0     4205 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_private_ARMA4.c
--rw-rw-rw-   0        0        0     5795 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_private_IIR_FIR.c
--rw-rw-rw-   0        0        0     2737 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_private_copy.c
--rw-rw-rw-   0        0        0     4273 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_private_down4.c
--rw-rw-rw-   0        0        0     8270 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_private_down_FIR.c
--rw-rw-rw-   0        0        0     6419 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_private_up2_HQ.c
--rw-rw-rw-   0        0        0     4252 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_private_up4.c
--rw-rw-rw-   0        0        0     9546 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_rom.c
--rw-rw-rw-   0        0        0     4983 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_rom.h
--rw-rw-rw-   0        0        0     3850 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_structs.h
--rw-rw-rw-   0        0        0     4044 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_up2.c
--rw-rw-rw-   0        0        0     4700 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_residual_energy16_FIX.c
--rw-rw-rw-   0        0        0     4686 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_residual_energy_FIX.c
--rw-rw-rw-   0        0        0     2383 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_scale_copy_vector16.c
--rw-rw-rw-   0        0        0     2373 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_scale_vector.c
--rw-rw-rw-   0        0        0     4644 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_schur.c
--rw-rw-rw-   0        0        0     4280 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_schur64.c
--rw-rw-rw-   0        0        0     5799 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_setup_complexity.h
--rw-rw-rw-   0        0        0     7989 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_shell_coder.c
--rw-rw-rw-   0        0        0     3915 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_sigm_Q15.c
--rw-rw-rw-   0        0        0    10610 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_solve_LS_FIX.c
--rw-rw-rw-   0        0        0     6133 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_sort.c
--rw-rw-rw-   0        0        0    20927 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_structs.h
--rw-rw-rw-   0        0        0     7490 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_structs_FIX.h
--rw-rw-rw-   0        0        0     4756 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_sum_sqr_shift.c
--rw-rw-rw-   0        0        0     9974 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables.h
--rw-rw-rw-   0        0        0     8153 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_LTP.c
--rw-rw-rw-   0        0        0    31448 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB0_10.c
--rw-rw-rw-   0        0        0     2500 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB0_10.h
--rw-rw-rw-   0        0        0    76776 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB0_16.c
--rw-rw-rw-   0        0        0     2501 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB0_16.h
--rw-rw-rw-   0        0        0    20648 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB1_10.c
--rw-rw-rw-   0        0        0     2499 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB1_10.h
--rw-rw-rw-   0        0        0    39704 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB1_16.c
--rw-rw-rw-   0        0        0     2501 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB1_16.h
--rw-rw-rw-   0        0        0     3681 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_gain.c
--rw-rw-rw-   0        0        0     7126 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_other.c
--rw-rw-rw-   0        0        0    11851 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_pitch_lag.c
--rw-rw-rw-   0        0        0    10102 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_pulses_per_block.c
--rw-rw-rw-   0        0        0     2270 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_sign.c
--rw-rw-rw-   0        0        0     2279 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_type_offset.c
--rw-rw-rw-   0        0        0     8097 2021-12-20 02:11:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tuning_parameters.h
--rw-rw-rw-   0        0        0     4469 2022-05-17 10:05:06.000000 pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_warped_autocorrelation_FIX.c
-drwxrwxrwx   0        0        0        0 2022-12-21 01:55:08.038974 pilk-0.2.3/src/interface/
--rw-rw-rw-   0        0        0     7971 2021-12-20 02:11:06.000000 pilk-0.2.3/src/interface/SKP_Silk_SDK_API.h
--rw-rw-rw-   0        0        0     4166 2021-12-20 02:11:06.000000 pilk-0.2.3/src/interface/SKP_Silk_control.h
--rw-rw-rw-   0        0        0     3648 2021-12-20 02:11:06.000000 pilk-0.2.3/src/interface/SKP_Silk_errors.h
--rw-rw-rw-   0        0        0     4304 2022-05-17 10:05:06.000000 pilk-0.2.3/src/interface/SKP_Silk_typedef.h
--rw-rw-rw-   0        0        0     3340 2022-05-18 14:16:24.000000 pilk-0.2.3/src/pilkmodule.c
-drwxrwxrwx   0        0        0        0 2022-12-21 01:55:08.038974 pilk-0.2.3/src/silk/
--rw-rw-rw-   0        0        0    12070 2022-12-21 01:49:26.000000 pilk-0.2.3/src/silk/pilk_decode.c
--rw-rw-rw-   0        0        0      272 2022-05-18 14:10:21.000000 pilk-0.2.3/src/silk/pilk_decode.h
--rw-rw-rw-   0        0        0     8745 2022-12-21 01:47:46.000000 pilk-0.2.3/src/silk/pilk_encode.c
--rw-rw-rw-   0        0        0      272 2022-05-18 14:10:21.000000 pilk-0.2.3/src/silk/pilk_encode.h
+drwxrwxrwx   0        0        0        0 2023-05-26 03:28:30.786177 pilk-0.2.4/
+-rw-rw-rw-   0        0        0    35823 2022-01-04 03:32:55.000000 pilk-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0       77 2022-05-18 14:04:57.000000 pilk-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     8887 2023-05-26 03:28:30.786177 pilk-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7631 2022-03-27 06:13:15.000000 pilk-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 03:28:30.665282 pilk-0.2.4/pilk/
+-rw-rw-rw-   0        0        0      649 2022-08-06 06:58:57.000000 pilk-0.2.4/pilk/SilkDecoder.py
+-rw-rw-rw-   0        0        0     1727 2022-08-06 06:58:57.000000 pilk-0.2.4/pilk/SilkEncoder.py
+-rw-rw-rw-   0        0        0     1528 2023-05-26 03:21:03.000000 pilk-0.2.4/pilk/__init__.py
+-rw-rw-rw-   0        0        0     1851 2022-05-17 13:53:41.000000 pilk-0.2.4/pilk/_pilk.pyi
+drwxrwxrwx   0        0        0        0 2023-05-26 03:28:30.665282 pilk-0.2.4/pilk.egg-info/
+-rw-rw-rw-   0        0        0     8887 2023-05-26 03:28:30.000000 pilk-0.2.4/pilk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11156 2023-05-26 03:28:30.000000 pilk-0.2.4/pilk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 03:28:30.000000 pilk-0.2.4/pilk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-08-06 10:40:14.000000 pilk-0.2.4/pilk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2023-05-26 03:28:30.000000 pilk-0.2.4/pilk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-26 03:28:30.000000 pilk-0.2.4/pilk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2021-12-31 06:14:52.000000 pilk-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 03:28:30.786177 pilk-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     2125 2023-05-26 03:21:03.000000 pilk-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 03:28:30.665282 pilk-0.2.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-26 03:28:30.770557 pilk-0.2.4/src/SKP_SILK_SRC/
+-rw-rw-rw-   0        0        0    12147 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_A2NLSF.c
+-rw-rw-rw-   0        0        0     4228 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_AsmHelper.h
+-rw-rw-rw-   0        0        0     6402 2021-12-21 05:00:19.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_AsmPreproc.h
+-rw-rw-rw-   0        0        0     7016 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_CNG.c
+-rw-rw-rw-   0        0        0     6610 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_HP_variable_cutoff_FIX.c
+-rw-rw-rw-   0        0        0    10724 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_Inlines.h
+-rw-rw-rw-   0        0        0     2175 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_LBRR_reset.c
+-rw-rw-rw-   0        0        0     7125 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_LPC_inv_pred_gain.c
+-rw-rw-rw-   0        0        0     5760 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_LPC_synthesis_filter.c
+-rw-rw-rw-   0        0        0     8900 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_LPC_synthesis_order16.c
+-rw-rw-rw-   0        0        0     9742 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_LP_variable_cutoff.c
+-rw-rw-rw-   0        0        0     4462 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_LSF_cos_table.c
+-rw-rw-rw-   0        0        0     4234 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_LTP_analysis_filter_FIX.c
+-rw-rw-rw-   0        0        0     4007 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_LTP_scale_ctrl_FIX.c
+-rw-rw-rw-   0        0        0     5623 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_MA.c
+-rw-rw-rw-   0        0        0     6581 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_NLSF2A.c
+-rw-rw-rw-   0        0        0     2950 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_NLSF2A_stable.c
+-rw-rw-rw-   0        0        0     4723 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_NLSF_MSVQ_decode.c
+-rw-rw-rw-   0        0        0    12279 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_NLSF_MSVQ_encode_FIX.c
+-rw-rw-rw-   0        0        0     3792 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_NLSF_VQ_rate_distortion_FIX.c
+-rw-rw-rw-   0        0        0     4381 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_NLSF_VQ_sum_error_FIX.c
+-rw-rw-rw-   0        0        0     4127 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_NLSF_VQ_weights_laroia.c
+-rw-rw-rw-   0        0        0     6634 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_NLSF_stabilize.c
+-rw-rw-rw-   0        0        0    24962 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_NSQ.c
+-rw-rw-rw-   0        0        0    41591 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_NSQ_del_dec.c
+-rw-rw-rw-   0        0        0    20697 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_PLC.c
+-rw-rw-rw-   0        0        0     4318 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_PLC.h
+-rw-rw-rw-   0        0        0    35908 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_SigProc_FIX.h
+-rw-rw-rw-   0        0        0    14235 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_VAD.c
+-rw-rw-rw-   0        0        0     8474 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_VQ_nearest_neighbor_FIX.c
+-rw-rw-rw-   0        0        0     4460 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_ana_filt_bank_1.c
+-rw-rw-rw-   0        0        0     6093 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_apply_sine_window.c
+-rw-rw-rw-   0        0        0     3604 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_array_maxabs.c
+-rw-rw-rw-   0        0        0     4460 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_autocorr.c
+-rw-rw-rw-   0        0        0     3776 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_biquad.c
+-rw-rw-rw-   0        0        0     4128 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_biquad_alt.c
+-rw-rw-rw-   0        0        0    14193 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_burg_modified.c
+-rw-rw-rw-   0        0        0     2841 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_bwexpander.c
+-rw-rw-rw-   0        0        0     2532 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_bwexpander_32.c
+-rw-rw-rw-   0        0        0     4620 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_code_signs.c
+-rw-rw-rw-   0        0        0     4018 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_common_pitch_est_defines.h
+-rw-rw-rw-   0        0        0     7222 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_control_audio_bandwidth.c
+-rw-rw-rw-   0        0        0    19231 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_control_codec_FIX.c
+-rw-rw-rw-   0        0        0     8021 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_corrMatrix_FIX.c
+-rw-rw-rw-   0        0        0     2535 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_create_init_destroy.c
+-rw-rw-rw-   0        0        0    12568 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_dec_API.c
+-rw-rw-rw-   0        0        0    16449 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_decode_core.c
+-rw-rw-rw-   0        0        0     7150 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_decode_frame.c
+-rw-rw-rw-   0        0        0    11872 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_decode_parameters.c
+-rw-rw-rw-   0        0        0     3013 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_decode_pitch.c
+-rw-rw-rw-   0        0        0     5343 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_decode_pulses.c
+-rw-rw-rw-   0        0        0     4031 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_decoder_set_fs.c
+-rw-rw-rw-   0        0        0    14448 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_define.h
+-rw-rw-rw-   0        0        0     4027 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_detect_SWB_input.c
+-rw-rw-rw-   0        0        0     1965 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_div_oabi.c
+-rw-rw-rw-   0        0        0     9765 2022-05-17 12:28:31.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_enc_API.c
+-rw-rw-rw-   0        0        0    20676 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_encode_frame_FIX.c
+-rw-rw-rw-   0        0        0     7182 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_encode_parameters.c
+-rw-rw-rw-   0        0        0     8338 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_encode_pulses.c
+-rw-rw-rw-   0        0        0     7620 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_find_LPC_FIX.c
+-rw-rw-rw-   0        0        0    13040 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_find_LTP_FIX.c
+-rw-rw-rw-   0        0        0     6883 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_find_pitch_lags_FIX.c
+-rw-rw-rw-   0        0        0     6731 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_find_pred_coefs_FIX.c
+-rw-rw-rw-   0        0        0     4921 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_gain_quant.c
+-rw-rw-rw-   0        0        0     2792 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_init_encoder_FIX.c
+-rw-rw-rw-   0        0        0     3774 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_inner_prod_aligned.c
+-rw-rw-rw-   0        0        0     2749 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_interpolate.c
+-rw-rw-rw-   0        0        0     3367 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_k2a.c
+-rw-rw-rw-   0        0        0     3343 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_k2a_Q16.c
+-rw-rw-rw-   0        0        0     3000 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_lin2log.c
+-rw-rw-rw-   0        0        0     3370 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_log2lin.c
+-rw-rw-rw-   0        0        0     5782 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_macros.h
+-rw-rw-rw-   0        0        0     9732 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_macros_arm.h
+-rw-rw-rw-   0        0        0    23449 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_main.h
+-rw-rw-rw-   0        0        0    22891 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_main_FIX.h
+-rw-rw-rw-   0        0        0    26006 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_noise_shape_analysis_FIX.c
+-rw-rw-rw-   0        0        0    35387 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_pitch_analysis_core.c
+-rw-rw-rw-   0        0        0     2338 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_pitch_est_defines.h
+-rw-rw-rw-   0        0        0     3865 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_pitch_est_tables.c
+-rw-rw-rw-   0        0        0    12561 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_prefilter_FIX.c
+-rw-rw-rw-   0        0        0     6881 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_process_NLSFs_FIX.c
+-rw-rw-rw-   0        0        0     6196 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_process_gains_FIX.c
+-rw-rw-rw-   0        0        0     5276 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_quant_LTP_gains_FIX.c
+-rw-rw-rw-   0        0        0    14752 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_range_coder.c
+-rw-rw-rw-   0        0        0     2560 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_regularize_correlations_FIX.c
+-rw-rw-rw-   0        0        0    14588 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler.c
+-rw-rw-rw-   0        0        0     4127 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_down2.c
+-rw-rw-rw-   0        0        0     5163 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_down2_3.c
+-rw-rw-rw-   0        0        0     4661 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_down3.c
+-rw-rw-rw-   0        0        0     6577 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_private.h
+-rw-rw-rw-   0        0        0     3111 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_private_AR2.c
+-rw-rw-rw-   0        0        0     4205 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_private_ARMA4.c
+-rw-rw-rw-   0        0        0     5795 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_private_IIR_FIR.c
+-rw-rw-rw-   0        0        0     2737 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_private_copy.c
+-rw-rw-rw-   0        0        0     4273 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_private_down4.c
+-rw-rw-rw-   0        0        0     8270 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_private_down_FIR.c
+-rw-rw-rw-   0        0        0     6419 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_private_up2_HQ.c
+-rw-rw-rw-   0        0        0     4252 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_private_up4.c
+-rw-rw-rw-   0        0        0     9546 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_rom.c
+-rw-rw-rw-   0        0        0     4983 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_rom.h
+-rw-rw-rw-   0        0        0     3850 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_structs.h
+-rw-rw-rw-   0        0        0     4044 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_up2.c
+-rw-rw-rw-   0        0        0     4700 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_residual_energy16_FIX.c
+-rw-rw-rw-   0        0        0     4686 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_residual_energy_FIX.c
+-rw-rw-rw-   0        0        0     2383 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_scale_copy_vector16.c
+-rw-rw-rw-   0        0        0     2373 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_scale_vector.c
+-rw-rw-rw-   0        0        0     4644 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_schur.c
+-rw-rw-rw-   0        0        0     4280 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_schur64.c
+-rw-rw-rw-   0        0        0     5799 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_setup_complexity.h
+-rw-rw-rw-   0        0        0     7989 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_shell_coder.c
+-rw-rw-rw-   0        0        0     3915 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_sigm_Q15.c
+-rw-rw-rw-   0        0        0    10610 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_solve_LS_FIX.c
+-rw-rw-rw-   0        0        0     6133 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_sort.c
+-rw-rw-rw-   0        0        0    20927 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_structs.h
+-rw-rw-rw-   0        0        0     7490 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_structs_FIX.h
+-rw-rw-rw-   0        0        0     4756 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_sum_sqr_shift.c
+-rw-rw-rw-   0        0        0     9974 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables.h
+-rw-rw-rw-   0        0        0     8153 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_LTP.c
+-rw-rw-rw-   0        0        0    31448 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB0_10.c
+-rw-rw-rw-   0        0        0     2500 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB0_10.h
+-rw-rw-rw-   0        0        0    76776 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB0_16.c
+-rw-rw-rw-   0        0        0     2501 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB0_16.h
+-rw-rw-rw-   0        0        0    20648 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB1_10.c
+-rw-rw-rw-   0        0        0     2499 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB1_10.h
+-rw-rw-rw-   0        0        0    39704 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB1_16.c
+-rw-rw-rw-   0        0        0     2501 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB1_16.h
+-rw-rw-rw-   0        0        0     3681 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_gain.c
+-rw-rw-rw-   0        0        0     7126 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_other.c
+-rw-rw-rw-   0        0        0    11851 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_pitch_lag.c
+-rw-rw-rw-   0        0        0    10102 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_pulses_per_block.c
+-rw-rw-rw-   0        0        0     2270 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_sign.c
+-rw-rw-rw-   0        0        0     2279 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_type_offset.c
+-rw-rw-rw-   0        0        0     8097 2021-12-20 02:11:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tuning_parameters.h
+-rw-rw-rw-   0        0        0     4469 2022-05-17 10:05:06.000000 pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_warped_autocorrelation_FIX.c
+drwxrwxrwx   0        0        0        0 2023-05-26 03:28:30.770557 pilk-0.2.4/src/interface/
+-rw-rw-rw-   0        0        0     7971 2021-12-20 02:11:06.000000 pilk-0.2.4/src/interface/SKP_Silk_SDK_API.h
+-rw-rw-rw-   0        0        0     4166 2021-12-20 02:11:06.000000 pilk-0.2.4/src/interface/SKP_Silk_control.h
+-rw-rw-rw-   0        0        0     3648 2021-12-20 02:11:06.000000 pilk-0.2.4/src/interface/SKP_Silk_errors.h
+-rw-rw-rw-   0        0        0     4304 2022-05-17 10:05:06.000000 pilk-0.2.4/src/interface/SKP_Silk_typedef.h
+-rw-rw-rw-   0        0        0     3340 2022-05-18 14:16:24.000000 pilk-0.2.4/src/pilkmodule.c
+drwxrwxrwx   0        0        0        0 2023-05-26 03:28:30.786177 pilk-0.2.4/src/silk/
+-rw-rw-rw-   0        0        0    12070 2022-12-21 01:49:26.000000 pilk-0.2.4/src/silk/pilk_decode.c
+-rw-rw-rw-   0        0        0      272 2022-05-18 14:10:21.000000 pilk-0.2.4/src/silk/pilk_decode.h
+-rw-rw-rw-   0        0        0     8745 2022-12-21 01:47:46.000000 pilk-0.2.4/src/silk/pilk_encode.c
+-rw-rw-rw-   0        0        0      272 2022-05-18 14:10:21.000000 pilk-0.2.4/src/silk/pilk_encode.h
```

### Comparing `pilk-0.2.3/LICENSE` & `pilk-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/PKG-INFO` & `pilk-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilk
-Version: 0.2.3
+Version: 0.2.4
 Summary: python silk voice library
 Home-page: https://github.com/foyoux/pilk
 Download-URL: https://github.com/foyoux/pilk/releases
 Author: foyou
 Author-email: yimi.0822@qq.com
 Maintainer: foyou
 Maintainer-email: yimi.0822@qq.com
```

### Comparing `pilk-0.2.3/README.md` & `pilk-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/pilk/SilkDecoder.py` & `pilk-0.2.4/pilk/SilkDecoder.py`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/pilk/SilkEncoder.py` & `pilk-0.2.4/pilk/SilkEncoder.py`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/pilk/__init__.py` & `pilk-0.2.4/pilk/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from .SilkDecoder import SilkDecoder
 from .SilkEncoder import SilkEncoder
 from ._pilk import *
 
 __title__ = 'pilk'
 __description__ = 'python silk codec binding'
 __url__ = 'https://github.com/foyoux/pilk'
-__version__ = '0.0.2'
+__version__ = '0.2.4'
 # noinspection SpellCheckingInspection
 __author__ = 'foyou'
 __author_email__ = 'yimi.0822@qq.com'
-__license__ = 'Apache 2.0'
-__copyright__ = f'Copyright 2022 {__author__}'
+__license__ = ' GPL-3.0'
+__copyright__ = f'Copyright 2022~2023 {__author__}'
 __ide__ = 'PyCharm - https://www.jetbrains.com/pycharm/'
 
 
 def get_duration(silk_path: str, frame_ms: int = 20) -> int:
     """获取 silk 文件持续时间，单位：ms"""
     with open(silk_path, 'rb') as silk:
         tencent = False
@@ -29,18 +29,16 @@
         else:
             silk.seek(9)
         i = 0
         while True:
             size = silk.read(2)
             if len(size) != 2:
                 break
-            size = size[0] + size[1] << 8
-            if not tencent and size == 0xffff:
-                break
             i += 1
+            size = size[0] + size[1] * 16
             silk.seek(silk.tell() + size)
         return i * frame_ms
 
 
 def silk_to_wav(silk: str, wav: str, rate: int = 24000):
     """silk 文件转 wav"""
     pcm_path = tempfile.mktemp(suffix='.pcm')
```

### Comparing `pilk-0.2.3/pilk/_pilk.pyi` & `pilk-0.2.4/pilk/_pilk.pyi`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/pilk.egg-info/PKG-INFO` & `pilk-0.2.4/pilk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilk
-Version: 0.2.3
+Version: 0.2.4
 Summary: python silk voice library
 Home-page: https://github.com/foyoux/pilk
 Download-URL: https://github.com/foyoux/pilk/releases
 Author: foyou
 Author-email: yimi.0822@qq.com
 Maintainer: foyou
 Maintainer-email: yimi.0822@qq.com
```

### Comparing `pilk-0.2.3/pilk.egg-info/SOURCES.txt` & `pilk-0.2.4/pilk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/setup.py` & `pilk-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 with open('README.md', encoding='utf8') as f:
     long_description = f.read()
 
 # noinspection SpellCheckingInspection
 setup(
     name='pilk',
-    version='0.2.3',
+    version='0.2.4',
     description='python silk voice library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='foyou',
     author_email='yimi.0822@qq.com',
     maintainer='foyou',
     maintainer_email='yimi.0822@qq.com',
```

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_A2NLSF.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_A2NLSF.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_AsmHelper.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_AsmHelper.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_AsmPreproc.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_AsmPreproc.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_CNG.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_CNG.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_HP_variable_cutoff_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_HP_variable_cutoff_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_Inlines.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_Inlines.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_LBRR_reset.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_LBRR_reset.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_LPC_inv_pred_gain.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_LPC_inv_pred_gain.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_LPC_synthesis_filter.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_LPC_synthesis_filter.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_LPC_synthesis_order16.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_LPC_synthesis_order16.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_LP_variable_cutoff.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_LP_variable_cutoff.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_LSF_cos_table.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_LSF_cos_table.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_LTP_analysis_filter_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_LTP_analysis_filter_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_LTP_scale_ctrl_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_LTP_scale_ctrl_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_MA.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_MA.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_NLSF2A.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_NLSF2A.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_NLSF2A_stable.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_NLSF2A_stable.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_NLSF_MSVQ_decode.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_NLSF_MSVQ_decode.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_NLSF_MSVQ_encode_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_NLSF_MSVQ_encode_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_NLSF_VQ_rate_distortion_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_NLSF_VQ_rate_distortion_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_NLSF_VQ_sum_error_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_NLSF_VQ_sum_error_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_NLSF_VQ_weights_laroia.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_NLSF_VQ_weights_laroia.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_NLSF_stabilize.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_NLSF_stabilize.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_NSQ.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_NSQ.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_NSQ_del_dec.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_NSQ_del_dec.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_PLC.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_PLC.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_PLC.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_PLC.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_SigProc_FIX.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_SigProc_FIX.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_VAD.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_VAD.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_VQ_nearest_neighbor_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_VQ_nearest_neighbor_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_ana_filt_bank_1.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_ana_filt_bank_1.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_apply_sine_window.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_apply_sine_window.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_array_maxabs.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_array_maxabs.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_autocorr.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_autocorr.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_biquad.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_biquad.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_biquad_alt.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_biquad_alt.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_burg_modified.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_burg_modified.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_bwexpander.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_bwexpander.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_bwexpander_32.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_bwexpander_32.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_code_signs.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_code_signs.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_common_pitch_est_defines.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_common_pitch_est_defines.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_control_audio_bandwidth.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_control_audio_bandwidth.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_control_codec_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_control_codec_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_corrMatrix_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_corrMatrix_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_create_init_destroy.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_create_init_destroy.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_dec_API.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_dec_API.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_decode_core.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_decode_core.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_decode_frame.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_decode_frame.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_decode_parameters.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_decode_parameters.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_decode_pitch.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_decode_pitch.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_decode_pulses.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_decode_pulses.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_decoder_set_fs.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_decoder_set_fs.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_define.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_define.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_detect_SWB_input.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_detect_SWB_input.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_div_oabi.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_div_oabi.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_enc_API.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_enc_API.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_encode_frame_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_encode_frame_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_encode_parameters.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_encode_parameters.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_encode_pulses.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_encode_pulses.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_find_LPC_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_find_LPC_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_find_LTP_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_find_LTP_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_find_pitch_lags_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_find_pitch_lags_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_find_pred_coefs_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_find_pred_coefs_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_gain_quant.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_gain_quant.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_init_encoder_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_init_encoder_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_inner_prod_aligned.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_inner_prod_aligned.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_interpolate.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_interpolate.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_k2a.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_k2a.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_k2a_Q16.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_k2a_Q16.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_lin2log.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_lin2log.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_log2lin.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_log2lin.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_macros.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_macros.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_macros_arm.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_macros_arm.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_main.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_main.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_main_FIX.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_main_FIX.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_noise_shape_analysis_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_noise_shape_analysis_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_pitch_analysis_core.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_pitch_analysis_core.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_pitch_est_defines.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_pitch_est_defines.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_pitch_est_tables.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_pitch_est_tables.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_prefilter_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_prefilter_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_process_NLSFs_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_process_NLSFs_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_process_gains_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_process_gains_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_quant_LTP_gains_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_quant_LTP_gains_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_range_coder.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_range_coder.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_regularize_correlations_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_regularize_correlations_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_down2.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_down2.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_down2_3.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_down2_3.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_down3.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_down3.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_private.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_private.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_private_AR2.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_private_AR2.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_private_ARMA4.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_private_ARMA4.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_private_IIR_FIR.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_private_IIR_FIR.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_private_copy.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_private_copy.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_private_down4.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_private_down4.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_private_down_FIR.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_private_down_FIR.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_private_up2_HQ.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_private_up2_HQ.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_private_up4.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_private_up4.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_rom.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_rom.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_rom.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_rom.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_structs.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_structs.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_resampler_up2.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_resampler_up2.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_residual_energy16_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_residual_energy16_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_residual_energy_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_residual_energy_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_scale_copy_vector16.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_scale_copy_vector16.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_scale_vector.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_scale_vector.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_schur.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_schur.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_schur64.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_schur64.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_setup_complexity.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_setup_complexity.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_shell_coder.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_shell_coder.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_sigm_Q15.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_sigm_Q15.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_solve_LS_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_solve_LS_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_sort.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_sort.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_structs.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_structs.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_structs_FIX.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_structs_FIX.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_sum_sqr_shift.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_sum_sqr_shift.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_LTP.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_LTP.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB0_10.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB0_10.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB0_10.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB0_10.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB0_16.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB0_16.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB0_16.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB0_16.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB1_10.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB1_10.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB1_10.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB1_10.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB1_16.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB1_16.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB1_16.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_NLSF_CB1_16.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_gain.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_gain.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_other.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_other.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_pitch_lag.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_pitch_lag.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_pulses_per_block.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_pulses_per_block.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_sign.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_sign.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tables_type_offset.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tables_type_offset.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_tuning_parameters.h` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_tuning_parameters.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/SKP_SILK_SRC/SKP_Silk_warped_autocorrelation_FIX.c` & `pilk-0.2.4/src/SKP_SILK_SRC/SKP_Silk_warped_autocorrelation_FIX.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/interface/SKP_Silk_SDK_API.h` & `pilk-0.2.4/src/interface/SKP_Silk_SDK_API.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/interface/SKP_Silk_control.h` & `pilk-0.2.4/src/interface/SKP_Silk_control.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/interface/SKP_Silk_errors.h` & `pilk-0.2.4/src/interface/SKP_Silk_errors.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/interface/SKP_Silk_typedef.h` & `pilk-0.2.4/src/interface/SKP_Silk_typedef.h`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/pilkmodule.c` & `pilk-0.2.4/src/pilkmodule.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/silk/pilk_decode.c` & `pilk-0.2.4/src/silk/pilk_decode.c`

 * *Files identical despite different names*

### Comparing `pilk-0.2.3/src/silk/pilk_encode.c` & `pilk-0.2.4/src/silk/pilk_encode.c`

 * *Files identical despite different names*

