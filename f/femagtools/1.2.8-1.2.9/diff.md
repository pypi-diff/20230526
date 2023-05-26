# Comparing `tmp/femagtools-1.2.8.tar.gz` & `tmp/femagtools-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "femagtools-1.2.8.tar", last modified: Wed May 17 15:20:50 2023, max compression
+gzip compressed data, was "femagtools-1.2.9.tar", last modified: Fri May 26 13:42:30 2023, max compression
```

## Comparing `femagtools-1.2.8.tar` & `femagtools-1.2.9.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-17 15:20:50.052667 femagtools-1.2.8/
--rw-r--r--   0 tar        (210) tar        (210)     1316 2023-02-15 20:03:56.000000 femagtools-1.2.8/LICENSE
--rw-r--r--   0 tar        (210) tar        (210)       35 2023-02-15 20:03:56.000000 femagtools-1.2.8/MANIFEST.in
--rw-r--r--   0 tar        (210) tar        (210)     5262 2023-05-17 15:20:50.051667 femagtools-1.2.8/PKG-INFO
--rw-r--r--   0 tar        (210) tar        (210)     3072 2023-02-14 18:11:00.000000 femagtools-1.2.8/README.md
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-17 15:20:50.030667 femagtools-1.2.8/femagtools/
--rw-r--r--   0 tar        (210) tar        (210)     1630 2023-05-17 15:13:04.000000 femagtools-1.2.8/femagtools/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     2250 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/airgap.py
--rw-r--r--   0 tar        (210) tar        (210)    12122 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/amazon.py
--rw-r--r--   0 tar        (210) tar        (210)     9741 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/amela.py
--rw-r--r--   0 tar        (210) tar        (210)     7706 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/asm.py
--rwxr-xr-x   0 tar        (210) tar        (210)    68684 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/bch.py
--rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/bchxml.py
--rw-r--r--   0 tar        (210) tar        (210)    10766 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/condor.py
--rw-r--r--   0 tar        (210) tar        (210)     1076 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/conductor.py
--rw-r--r--   0 tar        (210) tar        (210)     3087 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/config.py
--rw-r--r--   0 tar        (210) tar        (210)    23706 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/convert.py
--rw-r--r--   0 tar        (210) tar        (210)     7017 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dakota.py
--rwxr-xr-x   0 tar        (210) tar        (210)     4064 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dakota_femag.py
--rw-r--r--   0 tar        (210) tar        (210)     5573 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dakotaout.py
--rw-r--r--   0 tar        (210) tar        (210)     7460 2023-03-24 14:45:00.000000 femagtools-1.2.8/femagtools/docker.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-17 15:20:50.034667 femagtools-1.2.8/femagtools/dxfsl/
--rw-r--r--   0 tar        (210) tar        (210)        0 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)    52503 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/area.py
--rw-r--r--   0 tar        (210) tar        (210)     8990 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/conv.py
--rw-r--r--   0 tar        (210) tar        (210)    18787 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/converter.py
--rw-r--r--   0 tar        (210) tar        (210)     1266 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/corner.py
--rw-r--r--   0 tar        (210) tar        (210)     1861 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/dumprenderer.py
--rw-r--r--   0 tar        (210) tar        (210)    23233 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/fslrenderer.py
--rw-r--r--   0 tar        (210) tar        (210)     9835 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/functions.py
--rw-r--r--   0 tar        (210) tar        (210)   132506 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/geom.py
--rw-r--r--   0 tar        (210) tar        (210)    27661 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/machine.py
--rw-r--r--   0 tar        (210) tar        (210)    12311 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/plotrenderer.py
--rw-r--r--   0 tar        (210) tar        (210)    43088 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/shape.py
--rw-r--r--   0 tar        (210) tar        (210)     1224 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/erg.py
--rw-r--r--   0 tar        (210) tar        (210)    40619 2023-04-13 07:48:25.000000 femagtools-1.2.8/femagtools/femag.py
--rw-r--r--   0 tar        (210) tar        (210)     7415 2023-05-17 15:12:10.000000 femagtools-1.2.8/femagtools/forcedens.py
--rw-r--r--   0 tar        (210) tar        (210)    28180 2023-02-21 19:53:03.000000 femagtools-1.2.8/femagtools/fsl.py
--rw-r--r--   0 tar        (210) tar        (210)     3017 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/getset.py
--rw-r--r--   0 tar        (210) tar        (210)     3903 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/gmsh.py
--rw-r--r--   0 tar        (210) tar        (210)    17166 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/google.py
--rw-r--r--   0 tar        (210) tar        (210)     1561 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/grid.py
--rw-r--r--   0 tar        (210) tar        (210)    41556 2023-04-13 07:48:25.000000 femagtools-1.2.8/femagtools/isa7.py
--rw-r--r--   0 tar        (210) tar        (210)     2790 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/jcf2msh.py
--rw-r--r--   0 tar        (210) tar        (210)     1779 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/jhb.py
--rw-r--r--   0 tar        (210) tar        (210)    11320 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/job.py
--rw-r--r--   0 tar        (210) tar        (210)     2261 2022-08-24 07:36:25.000000 femagtools-1.2.8/femagtools/losscoeffs.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-17 15:20:50.035667 femagtools-1.2.8/femagtools/machine/
--rw-r--r--   0 tar        (210) tar        (210)     5613 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/machine/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     5466 2023-05-17 15:12:10.000000 femagtools-1.2.8/femagtools/machine/effloss.py
--rw-r--r--   0 tar        (210) tar        (210)    34847 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/machine/im.py
--rwxr-xr-x   0 tar        (210) tar        (210)    30815 2023-05-17 15:12:10.000000 femagtools-1.2.8/femagtools/machine/pm.py
--rw-r--r--   0 tar        (210) tar        (210)    21743 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/machine/sizing.py
--rw-r--r--   0 tar        (210) tar        (210)    14584 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/machine/sm.py
--rw-r--r--   0 tar        (210) tar        (210)    16143 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/machine/utils.py
--rw-r--r--   0 tar        (210) tar        (210)     1093 2023-02-15 20:03:56.000000 femagtools-1.2.8/femagtools/magnet.py
--rw-r--r--   0 tar        (210) tar        (210)    38043 2023-02-16 09:09:33.000000 femagtools-1.2.8/femagtools/mcv.py
--rw-r--r--   0 tar        (210) tar        (210)     1833 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/me.py
--rw-r--r--   0 tar        (210) tar        (210)    14106 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/model.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-17 15:20:50.036667 femagtools-1.2.8/femagtools/moo/
--rw-r--r--   0 tar        (210) tar        (210)      175 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/moo/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     5493 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/moo/algorithm.py
--rw-r--r--   0 tar        (210) tar        (210)    10100 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/moo/population.py
--rw-r--r--   0 tar        (210) tar        (210)     2391 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/moo/problem.py
--rw-r--r--   0 tar        (210) tar        (210)     2825 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/moproblem.py
--rw-r--r--   0 tar        (210) tar        (210)     8265 2023-04-05 06:37:05.000000 femagtools-1.2.8/femagtools/multiproc.py
--rw-r--r--   0 tar        (210) tar        (210)     1841 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/mxw2msh.py
--rw-r--r--   0 tar        (210) tar        (210)    12781 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/nc.py
--rw-r--r--   0 tar        (210) tar        (210)     2052 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/netlist.py
--rw-r--r--   0 tar        (210) tar        (210)     3099 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/ntib.py
--rw-r--r--   0 tar        (210) tar        (210)     8685 2023-02-21 19:53:03.000000 femagtools-1.2.8/femagtools/opt.py
--rw-r--r--   0 tar        (210) tar        (210)    18733 2023-04-05 06:37:05.000000 femagtools-1.2.8/femagtools/parstudy.py
--rw-r--r--   0 tar        (210) tar        (210)    58040 2023-05-17 15:12:10.000000 femagtools-1.2.8/femagtools/plot.py
--rw-r--r--   0 tar        (210) tar        (210)     6536 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/poc.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-17 15:20:50.045667 femagtools-1.2.8/femagtools/templates/
--rw-r--r--   0 tar        (210) tar        (210)      874 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/FE-losses.mako
--rw-r--r--   0 tar        (210) tar        (210)      242 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/airgapinduc.mako
--rw-r--r--   0 tar        (210) tar        (210)     2879 2022-09-28 06:51:55.000000 femagtools-1.2.8/femagtools/templates/asyn_motor.mako
--rw-r--r--   0 tar        (210) tar        (210)     2483 2022-09-28 06:51:55.000000 femagtools-1.2.8/femagtools/templates/basic_modpar.mako
--rw-r--r--   0 tar        (210) tar        (210)     1911 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/calc_field_ts.mako
--rw-r--r--   0 tar        (210) tar        (210)      997 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/cogg_calc.mako
--rw-r--r--   0 tar        (210) tar        (210)      400 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/colorgrad.mako
--rw-r--r--   0 tar        (210) tar        (210)     1264 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/com_motor_sim.mako
--rw-r--r--   0 tar        (210) tar        (210)      472 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/conduct-data.mako
--rw-r--r--   0 tar        (210) tar        (210)      437 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/connect_models.mako
--rw-r--r--   0 tar        (210) tar        (210)     1350 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/cu_losses.mako
--rw-r--r--   0 tar        (210) tar        (210)     1672 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/ec-rotorbar.mako
--rw-r--r--   0 tar        (210) tar        (210)     1983 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/fe-contr.mako
--rw-r--r--   0 tar        (210) tar        (210)     4289 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/gen_winding.mako
--rw-r--r--   0 tar        (210) tar        (210)      560 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/inductances.mako
--rw-r--r--   0 tar        (210) tar        (210)     1270 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/ld_lq_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      600 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/leak_dist_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)      770 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/leak_evol_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)      431 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/leak_tooth_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)     1271 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnet-data.mako
--rw-r--r--   0 tar        (210) tar        (210)      788 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnetFC2.mako
--rw-r--r--   0 tar        (210) tar        (210)     1372 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnetIron.mako
--rw-r--r--   0 tar        (210) tar        (210)     1426 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnetIron2.mako
--rw-r--r--   0 tar        (210) tar        (210)     2315 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnetIron3.mako
--rw-r--r--   0 tar        (210) tar        (210)     1413 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnetIron4.mako
--rw-r--r--   0 tar        (210) tar        (210)     1376 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnetIron5.mako
--rw-r--r--   0 tar        (210) tar        (210)     2208 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnetIronV.mako
--rw-r--r--   0 tar        (210) tar        (210)     2010 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnetSector.mako
--rw-r--r--   0 tar        (210) tar        (210)      727 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnetSectorLinear.mako
--rw-r--r--   0 tar        (210) tar        (210)     1295 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnetShell.mako
--rw-r--r--   0 tar        (210) tar        (210)     4080 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnetShell2.mako
--rw-r--r--   0 tar        (210) tar        (210)     1094 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/mesh-airgap.mako
--rw-r--r--   0 tar        (210) tar        (210)     2298 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/modal_analysis.mako
--rw-r--r--   0 tar        (210) tar        (210)     1202 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/mult_cal_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      345 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/new_model.mako
--rw-r--r--   0 tar        (210) tar        (210)     3209 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/noloadflux-rot.mako
--rw-r--r--   0 tar        (210) tar        (210)     4661 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/noloadflux.mako
--rw-r--r--   0 tar        (210) tar        (210)     3146 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/noloadfluxdc.mako
--rw-r--r--   0 tar        (210) tar        (210)      313 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/open.mako
--rw-r--r--   0 tar        (210) tar        (210)      630 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/plots.mako
--rw-r--r--   0 tar        (210) tar        (210)     1373 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/pm_sym_f_cur.mako
--rw-r--r--   0 tar        (210) tar        (210)     2319 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/pm_sym_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      925 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/pm_sym_loss.mako
--rw-r--r--   0 tar        (210) tar        (210)     1251 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/psd_psq_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      643 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/ring.mako
--rw-r--r--   0 tar        (210) tar        (210)      973 2022-09-28 06:51:55.000000 femagtools-1.2.8/femagtools/templates/rot_hsm.mako
--rw-r--r--   0 tar        (210) tar        (210)     2280 2022-09-28 06:51:55.000000 femagtools-1.2.8/femagtools/templates/rotorAsyn.mako
--rw-r--r--   0 tar        (210) tar        (210)     1908 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/rotorKs2.mako
--rw-r--r--   0 tar        (210) tar        (210)     1910 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/rotor_msh.mako
--rw-r--r--   0 tar        (210) tar        (210)      753 2022-09-28 06:51:55.000000 femagtools-1.2.8/femagtools/templates/rotor_winding.mako
--rw-r--r--   0 tar        (210) tar        (210)     1981 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/shortcircuit.mako
--rw-r--r--   0 tar        (210) tar        (210)     2077 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/srm.mako
--rw-r--r--   0 tar        (210) tar        (210)      761 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/stator1.mako
--rw-r--r--   0 tar        (210) tar        (210)      599 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/stator2.mako
--rw-r--r--   0 tar        (210) tar        (210)      724 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/stator3Linear.mako
--rw-r--r--   0 tar        (210) tar        (210)     1179 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/stator4.mako
--rw-r--r--   0 tar        (210) tar        (210)      893 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/statorBG.mako
--rw-r--r--   0 tar        (210) tar        (210)     2071 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/statorRing.mako
--rw-r--r--   0 tar        (210) tar        (210)     4073 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/statorRotor3.mako
--rw-r--r--   0 tar        (210) tar        (210)     1799 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/stator_msh.mako
--rw-r--r--   0 tar        (210) tar        (210)     1761 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/torq_calc.mako
--rw-r--r--   0 tar        (210) tar        (210)     5791 2022-08-24 07:36:25.000000 femagtools-1.2.8/femagtools/tks.py
--rw-r--r--   0 tar        (210) tar        (210)    47280 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/ts.py
--rw-r--r--   0 tar        (210) tar        (210)     2444 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/vbf.py
--rw-r--r--   0 tar        (210) tar        (210)     8595 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/vtu.py
--rw-r--r--   0 tar        (210) tar        (210)    22279 2023-03-24 14:45:00.000000 femagtools-1.2.8/femagtools/windings.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-17 15:20:50.031667 femagtools-1.2.8/femagtools.egg-info/
--rw-r--r--   0 tar        (210) tar        (210)     5262 2023-05-17 15:20:50.000000 femagtools-1.2.8/femagtools.egg-info/PKG-INFO
--rw-r--r--   0 tar        (210) tar        (210)     4861 2023-05-17 15:20:50.000000 femagtools-1.2.8/femagtools.egg-info/SOURCES.txt
--rw-r--r--   0 tar        (210) tar        (210)        1 2023-05-17 15:20:50.000000 femagtools-1.2.8/femagtools.egg-info/dependency_links.txt
--rw-r--r--   0 tar        (210) tar        (210)      191 2023-05-17 15:20:50.000000 femagtools-1.2.8/femagtools.egg-info/entry_points.txt
--rw-r--r--   0 tar        (210) tar        (210)      144 2023-05-17 15:20:50.000000 femagtools-1.2.8/femagtools.egg-info/requires.txt
--rw-r--r--   0 tar        (210) tar        (210)       11 2023-05-17 15:20:50.000000 femagtools-1.2.8/femagtools.egg-info/top_level.txt
--rw-r--r--   0 tar        (210) tar        (210)     1369 2023-02-15 20:03:56.000000 femagtools-1.2.8/pyproject.toml
--rw-r--r--   0 tar        (210) tar        (210)       38 2023-05-17 15:20:50.052667 femagtools-1.2.8/setup.cfg
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-17 15:20:50.051667 femagtools-1.2.8/tests/
--rw-r--r--   0 tar        (210) tar        (210)     1065 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_airgap_induction.py
--rw-r--r--   0 tar        (210) tar        (210)      646 2023-02-14 18:11:00.000000 femagtools-1.2.8/tests/test_amela.py
--rw-r--r--   0 tar        (210) tar        (210)     1398 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_asm.py
--rwxr-xr-x   0 tar        (210) tar        (210)    14755 2023-02-14 18:11:00.000000 femagtools-1.2.8/tests/test_bchreader.py
--rw-r--r--   0 tar        (210) tar        (210)      332 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_conductor.py
--rw-r--r--   0 tar        (210) tar        (210)     6171 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_convert.py
--rw-r--r--   0 tar        (210) tar        (210)     1138 2023-05-17 15:12:10.000000 femagtools-1.2.8/tests/test_effloss.py
--rw-r--r--   0 tar        (210) tar        (210)      523 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_erg.py
--rw-r--r--   0 tar        (210) tar        (210)     1934 2023-02-16 09:09:33.000000 femagtools-1.2.8/tests/test_femag.py
--rw-r--r--   0 tar        (210) tar        (210)      533 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_forcedens.py
--rwxr-xr-x   0 tar        (210) tar        (210)    16079 2023-02-14 18:11:00.000000 femagtools-1.2.8/tests/test_fsl.py
--rw-r--r--   0 tar        (210) tar        (210)      662 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_im.py
--rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_isa7.py
--rw-r--r--   0 tar        (210) tar        (210)      824 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_jhb.py
--rw-r--r--   0 tar        (210) tar        (210)      981 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_job.py
--rw-r--r--   0 tar        (210) tar        (210)     2012 2022-08-24 07:36:25.000000 femagtools-1.2.8/tests/test_losscoeffs.py
--rwxr-xr-x   0 tar        (210) tar        (210)    12906 2023-02-14 18:11:00.000000 femagtools-1.2.8/tests/test_machine.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2608 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_magncurv.py
--rw-r--r--   0 tar        (210) tar        (210)      276 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_magnet.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2118 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_mcvreader.py
--rwxr-xr-x   0 tar        (210) tar        (210)     3922 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_mcvwriter.py
--rw-r--r--   0 tar        (210) tar        (210)      192 2023-02-14 18:11:00.000000 femagtools-1.2.8/tests/test_me.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2372 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_model.py
--rw-r--r--   0 tar        (210) tar        (210)     3116 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_nc.py
--rw-r--r--   0 tar        (210) tar        (210)     1323 2023-02-14 18:11:00.000000 femagtools-1.2.8/tests/test_parident.py
--rw-r--r--   0 tar        (210) tar        (210)     3200 2023-03-02 15:44:17.000000 femagtools-1.2.8/tests/test_parstudy.py
--rwxr-xr-x   0 tar        (210) tar        (210)     5816 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_pocfile.py
--rw-r--r--   0 tar        (210) tar        (210)     1109 2023-02-14 18:11:00.000000 femagtools-1.2.8/tests/test_sizing.py
--rw-r--r--   0 tar        (210) tar        (210)    83510 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_sm.py
--rwxr-xr-x   0 tar        (210) tar        (210)      766 2022-08-24 07:36:25.000000 femagtools-1.2.8/tests/test_tksreader.py
--rw-r--r--   0 tar        (210) tar        (210)     1825 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_ts.py
--rwxr-xr-x   0 tar        (210) tar        (210)      832 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_vbfreader.py
--rw-r--r--   0 tar        (210) tar        (210)      868 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_vtu.py
--rw-r--r--   0 tar        (210) tar        (210)     4912 2023-03-24 14:45:00.000000 femagtools-1.2.8/tests/test_windings.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-26 13:42:30.290895 femagtools-1.2.9/
+-rw-r--r--   0 tar        (210) tar        (210)     1316 2023-02-15 20:03:56.000000 femagtools-1.2.9/LICENSE
+-rw-r--r--   0 tar        (210) tar        (210)       35 2023-02-15 20:03:56.000000 femagtools-1.2.9/MANIFEST.in
+-rw-r--r--   0 tar        (210) tar        (210)     5262 2023-05-26 13:42:30.289895 femagtools-1.2.9/PKG-INFO
+-rw-r--r--   0 tar        (210) tar        (210)     3072 2023-02-14 18:11:00.000000 femagtools-1.2.9/README.md
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-26 13:42:30.271895 femagtools-1.2.9/femagtools/
+-rw-r--r--   0 tar        (210) tar        (210)     1630 2023-05-26 13:39:54.000000 femagtools-1.2.9/femagtools/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     2250 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/airgap.py
+-rw-r--r--   0 tar        (210) tar        (210)    12122 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/amazon.py
+-rw-r--r--   0 tar        (210) tar        (210)     9741 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/amela.py
+-rw-r--r--   0 tar        (210) tar        (210)     7706 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/asm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    68684 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/bch.py
+-rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/bchxml.py
+-rw-r--r--   0 tar        (210) tar        (210)    10766 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/condor.py
+-rw-r--r--   0 tar        (210) tar        (210)     1076 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/conductor.py
+-rw-r--r--   0 tar        (210) tar        (210)     3087 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/config.py
+-rw-r--r--   0 tar        (210) tar        (210)    23706 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/convert.py
+-rw-r--r--   0 tar        (210) tar        (210)     7017 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dakota.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     4064 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dakota_femag.py
+-rw-r--r--   0 tar        (210) tar        (210)     5573 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dakotaout.py
+-rw-r--r--   0 tar        (210) tar        (210)     7460 2023-03-24 14:45:00.000000 femagtools-1.2.9/femagtools/docker.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-26 13:42:30.274895 femagtools-1.2.9/femagtools/dxfsl/
+-rw-r--r--   0 tar        (210) tar        (210)        0 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)    52503 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/area.py
+-rw-r--r--   0 tar        (210) tar        (210)     8990 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/conv.py
+-rw-r--r--   0 tar        (210) tar        (210)    18787 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/converter.py
+-rw-r--r--   0 tar        (210) tar        (210)     1266 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/corner.py
+-rw-r--r--   0 tar        (210) tar        (210)     1861 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/dumprenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)    23233 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/fslrenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)     9835 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/functions.py
+-rw-r--r--   0 tar        (210) tar        (210)   132506 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/geom.py
+-rw-r--r--   0 tar        (210) tar        (210)    27661 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/machine.py
+-rw-r--r--   0 tar        (210) tar        (210)    12311 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/plotrenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)    43088 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/shape.py
+-rw-r--r--   0 tar        (210) tar        (210)     1224 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/erg.py
+-rw-r--r--   0 tar        (210) tar        (210)    40675 2023-05-26 13:39:42.000000 femagtools-1.2.9/femagtools/femag.py
+-rw-r--r--   0 tar        (210) tar        (210)     7415 2023-05-17 15:12:10.000000 femagtools-1.2.9/femagtools/forcedens.py
+-rw-r--r--   0 tar        (210) tar        (210)    28180 2023-02-21 19:53:03.000000 femagtools-1.2.9/femagtools/fsl.py
+-rw-r--r--   0 tar        (210) tar        (210)     3017 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/getset.py
+-rw-r--r--   0 tar        (210) tar        (210)     3903 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/gmsh.py
+-rw-r--r--   0 tar        (210) tar        (210)    17166 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/google.py
+-rw-r--r--   0 tar        (210) tar        (210)     1561 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/grid.py
+-rw-r--r--   0 tar        (210) tar        (210)    41556 2023-04-13 07:48:25.000000 femagtools-1.2.9/femagtools/isa7.py
+-rw-r--r--   0 tar        (210) tar        (210)     2790 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/jcf2msh.py
+-rw-r--r--   0 tar        (210) tar        (210)     1779 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/jhb.py
+-rw-r--r--   0 tar        (210) tar        (210)    11320 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/job.py
+-rw-r--r--   0 tar        (210) tar        (210)     2261 2022-08-24 07:36:25.000000 femagtools-1.2.9/femagtools/losscoeffs.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-26 13:42:30.275895 femagtools-1.2.9/femagtools/machine/
+-rw-r--r--   0 tar        (210) tar        (210)     7392 2023-05-26 13:39:42.000000 femagtools-1.2.9/femagtools/machine/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     5680 2023-05-26 13:39:42.000000 femagtools-1.2.9/femagtools/machine/effloss.py
+-rw-r--r--   0 tar        (210) tar        (210)    34847 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/machine/im.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    30721 2023-05-26 13:39:42.000000 femagtools-1.2.9/femagtools/machine/pm.py
+-rw-r--r--   0 tar        (210) tar        (210)    21743 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/machine/sizing.py
+-rw-r--r--   0 tar        (210) tar        (210)    26367 2023-05-26 13:39:42.000000 femagtools-1.2.9/femagtools/machine/sm.py
+-rw-r--r--   0 tar        (210) tar        (210)    16188 2023-05-26 13:39:42.000000 femagtools-1.2.9/femagtools/machine/utils.py
+-rw-r--r--   0 tar        (210) tar        (210)     1093 2023-02-15 20:03:56.000000 femagtools-1.2.9/femagtools/magnet.py
+-rw-r--r--   0 tar        (210) tar        (210)    38043 2023-02-16 09:09:33.000000 femagtools-1.2.9/femagtools/mcv.py
+-rw-r--r--   0 tar        (210) tar        (210)     1833 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/me.py
+-rw-r--r--   0 tar        (210) tar        (210)    14106 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/model.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-26 13:42:30.276895 femagtools-1.2.9/femagtools/moo/
+-rw-r--r--   0 tar        (210) tar        (210)      175 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/moo/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     5493 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/moo/algorithm.py
+-rw-r--r--   0 tar        (210) tar        (210)    10100 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/moo/population.py
+-rw-r--r--   0 tar        (210) tar        (210)     2391 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/moo/problem.py
+-rw-r--r--   0 tar        (210) tar        (210)     2825 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/moproblem.py
+-rw-r--r--   0 tar        (210) tar        (210)     8265 2023-04-05 06:37:05.000000 femagtools-1.2.9/femagtools/multiproc.py
+-rw-r--r--   0 tar        (210) tar        (210)     1841 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/mxw2msh.py
+-rw-r--r--   0 tar        (210) tar        (210)    12781 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/nc.py
+-rw-r--r--   0 tar        (210) tar        (210)     2052 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/netlist.py
+-rw-r--r--   0 tar        (210) tar        (210)     3099 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/ntib.py
+-rw-r--r--   0 tar        (210) tar        (210)     8685 2023-02-21 19:53:03.000000 femagtools-1.2.9/femagtools/opt.py
+-rw-r--r--   0 tar        (210) tar        (210)    18733 2023-04-05 06:37:05.000000 femagtools-1.2.9/femagtools/parstudy.py
+-rw-r--r--   0 tar        (210) tar        (210)    58201 2023-05-26 13:39:42.000000 femagtools-1.2.9/femagtools/plot.py
+-rw-r--r--   0 tar        (210) tar        (210)     6536 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/poc.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-26 13:42:30.283895 femagtools-1.2.9/femagtools/templates/
+-rw-r--r--   0 tar        (210) tar        (210)      874 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/FE-losses.mako
+-rw-r--r--   0 tar        (210) tar        (210)      242 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/airgapinduc.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2879 2022-09-28 06:51:55.000000 femagtools-1.2.9/femagtools/templates/asyn_motor.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2483 2022-09-28 06:51:55.000000 femagtools-1.2.9/femagtools/templates/basic_modpar.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1911 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/calc_field_ts.mako
+-rw-r--r--   0 tar        (210) tar        (210)      997 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/cogg_calc.mako
+-rw-r--r--   0 tar        (210) tar        (210)      400 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/colorgrad.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1264 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/com_motor_sim.mako
+-rw-r--r--   0 tar        (210) tar        (210)      472 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/conduct-data.mako
+-rw-r--r--   0 tar        (210) tar        (210)      437 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/connect_models.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1350 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/cu_losses.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1672 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/ec-rotorbar.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1983 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/fe-contr.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4289 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/gen_winding.mako
+-rw-r--r--   0 tar        (210) tar        (210)      560 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/inductances.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1270 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/ld_lq_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      600 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/leak_dist_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)      770 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/leak_evol_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)      431 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/leak_tooth_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1271 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnet-data.mako
+-rw-r--r--   0 tar        (210) tar        (210)      788 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnetFC2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1372 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnetIron.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1426 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnetIron2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2315 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnetIron3.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1413 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnetIron4.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1376 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnetIron5.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2208 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnetIronV.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2010 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnetSector.mako
+-rw-r--r--   0 tar        (210) tar        (210)      727 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnetSectorLinear.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1295 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnetShell.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4080 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnetShell2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1094 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/mesh-airgap.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2298 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/modal_analysis.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1202 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/mult_cal_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      345 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/new_model.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3209 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/noloadflux-rot.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4661 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/noloadflux.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3146 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/noloadfluxdc.mako
+-rw-r--r--   0 tar        (210) tar        (210)      313 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/open.mako
+-rw-r--r--   0 tar        (210) tar        (210)      630 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/plots.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1373 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/pm_sym_f_cur.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2319 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/pm_sym_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      925 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/pm_sym_loss.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1251 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/psd_psq_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      643 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/ring.mako
+-rw-r--r--   0 tar        (210) tar        (210)      973 2022-09-28 06:51:55.000000 femagtools-1.2.9/femagtools/templates/rot_hsm.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2280 2022-09-28 06:51:55.000000 femagtools-1.2.9/femagtools/templates/rotorAsyn.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1908 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/rotorKs2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1910 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/rotor_msh.mako
+-rw-r--r--   0 tar        (210) tar        (210)      753 2022-09-28 06:51:55.000000 femagtools-1.2.9/femagtools/templates/rotor_winding.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1981 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/shortcircuit.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2077 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/srm.mako
+-rw-r--r--   0 tar        (210) tar        (210)      761 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/stator1.mako
+-rw-r--r--   0 tar        (210) tar        (210)      599 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/stator2.mako
+-rw-r--r--   0 tar        (210) tar        (210)      724 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/stator3Linear.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1179 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/stator4.mako
+-rw-r--r--   0 tar        (210) tar        (210)      893 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/statorBG.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2071 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/statorRing.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4073 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/statorRotor3.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1799 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/stator_msh.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1716 2023-05-26 13:39:42.000000 femagtools-1.2.9/femagtools/templates/torq_calc.mako
+-rw-r--r--   0 tar        (210) tar        (210)     5791 2022-08-24 07:36:25.000000 femagtools-1.2.9/femagtools/tks.py
+-rw-r--r--   0 tar        (210) tar        (210)    47280 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/ts.py
+-rw-r--r--   0 tar        (210) tar        (210)     2444 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/vbf.py
+-rw-r--r--   0 tar        (210) tar        (210)     8595 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/vtu.py
+-rw-r--r--   0 tar        (210) tar        (210)    22279 2023-03-24 14:45:00.000000 femagtools-1.2.9/femagtools/windings.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-26 13:42:30.272895 femagtools-1.2.9/femagtools.egg-info/
+-rw-r--r--   0 tar        (210) tar        (210)     5262 2023-05-26 13:42:30.000000 femagtools-1.2.9/femagtools.egg-info/PKG-INFO
+-rw-r--r--   0 tar        (210) tar        (210)     4861 2023-05-26 13:42:30.000000 femagtools-1.2.9/femagtools.egg-info/SOURCES.txt
+-rw-r--r--   0 tar        (210) tar        (210)        1 2023-05-26 13:42:30.000000 femagtools-1.2.9/femagtools.egg-info/dependency_links.txt
+-rw-r--r--   0 tar        (210) tar        (210)      191 2023-05-26 13:42:30.000000 femagtools-1.2.9/femagtools.egg-info/entry_points.txt
+-rw-r--r--   0 tar        (210) tar        (210)      144 2023-05-26 13:42:30.000000 femagtools-1.2.9/femagtools.egg-info/requires.txt
+-rw-r--r--   0 tar        (210) tar        (210)       11 2023-05-26 13:42:30.000000 femagtools-1.2.9/femagtools.egg-info/top_level.txt
+-rw-r--r--   0 tar        (210) tar        (210)     1369 2023-02-15 20:03:56.000000 femagtools-1.2.9/pyproject.toml
+-rw-r--r--   0 tar        (210) tar        (210)       38 2023-05-26 13:42:30.290895 femagtools-1.2.9/setup.cfg
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-26 13:42:30.289895 femagtools-1.2.9/tests/
+-rw-r--r--   0 tar        (210) tar        (210)     1065 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_airgap_induction.py
+-rw-r--r--   0 tar        (210) tar        (210)      646 2023-02-14 18:11:00.000000 femagtools-1.2.9/tests/test_amela.py
+-rw-r--r--   0 tar        (210) tar        (210)     1398 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_asm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    14755 2023-02-14 18:11:00.000000 femagtools-1.2.9/tests/test_bchreader.py
+-rw-r--r--   0 tar        (210) tar        (210)      332 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_conductor.py
+-rw-r--r--   0 tar        (210) tar        (210)     6171 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_convert.py
+-rw-r--r--   0 tar        (210) tar        (210)     1142 2023-05-26 13:39:42.000000 femagtools-1.2.9/tests/test_effloss.py
+-rw-r--r--   0 tar        (210) tar        (210)      523 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_erg.py
+-rw-r--r--   0 tar        (210) tar        (210)     1934 2023-02-16 09:09:33.000000 femagtools-1.2.9/tests/test_femag.py
+-rw-r--r--   0 tar        (210) tar        (210)      533 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_forcedens.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    16079 2023-02-14 18:11:00.000000 femagtools-1.2.9/tests/test_fsl.py
+-rw-r--r--   0 tar        (210) tar        (210)      662 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_im.py
+-rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_isa7.py
+-rw-r--r--   0 tar        (210) tar        (210)      824 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_jhb.py
+-rw-r--r--   0 tar        (210) tar        (210)      981 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_job.py
+-rw-r--r--   0 tar        (210) tar        (210)     2012 2022-08-24 07:36:25.000000 femagtools-1.2.9/tests/test_losscoeffs.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    12906 2023-02-14 18:11:00.000000 femagtools-1.2.9/tests/test_machine.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2608 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_magncurv.py
+-rw-r--r--   0 tar        (210) tar        (210)      276 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_magnet.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2118 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_mcvreader.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     3922 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_mcvwriter.py
+-rw-r--r--   0 tar        (210) tar        (210)      192 2023-02-14 18:11:00.000000 femagtools-1.2.9/tests/test_me.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2372 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_model.py
+-rw-r--r--   0 tar        (210) tar        (210)     3116 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_nc.py
+-rw-r--r--   0 tar        (210) tar        (210)     1323 2023-02-14 18:11:00.000000 femagtools-1.2.9/tests/test_parident.py
+-rw-r--r--   0 tar        (210) tar        (210)     3200 2023-03-02 15:44:17.000000 femagtools-1.2.9/tests/test_parstudy.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     5816 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_pocfile.py
+-rw-r--r--   0 tar        (210) tar        (210)     1109 2023-02-14 18:11:00.000000 femagtools-1.2.9/tests/test_sizing.py
+-rw-r--r--   0 tar        (210) tar        (210)    83524 2023-05-26 13:39:42.000000 femagtools-1.2.9/tests/test_sm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)      766 2022-08-24 07:36:25.000000 femagtools-1.2.9/tests/test_tksreader.py
+-rw-r--r--   0 tar        (210) tar        (210)     1825 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_ts.py
+-rwxr-xr-x   0 tar        (210) tar        (210)      832 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_vbfreader.py
+-rw-r--r--   0 tar        (210) tar        (210)      868 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_vtu.py
+-rw-r--r--   0 tar        (210) tar        (210)     4912 2023-03-24 14:45:00.000000 femagtools-1.2.9/tests/test_windings.py
```

### Comparing `femagtools-1.2.8/LICENSE` & `femagtools-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/PKG-INFO` & `femagtools-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femagtools
-Version: 1.2.8
+Version: 1.2.9
 Summary: Python API for FEMAG
 Author-email: Ronald Tanner <tar@semafor.ch>, Dapu Zhang <d.zhan@gtisoft.com>, Beat Holm <hob@semafor.ch>, Günther Amsler <amg@semafor.ch>, Nicolas Mauchle <mau@semafor.ch>
 License: Copyright (c) 2016-2023, Semafor Informatik & Energie AG, Basel
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions
```

### Comparing `femagtools-1.2.8/README.md` & `femagtools-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/__init__.py` & `femagtools-1.2.9/femagtools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
     Python bindings for FEMAG
 
 
 
 """
 __title__ = 'femagtools'
-__version__ = '1.2.8'
+__version__ = '1.2.9'
 __author__ = 'Ronald Tanner'
 __license__ = 'BSD'
 __copyright__ = 'Copyright 2016-2022 SEMAFOR Informatik & Energie AG'
 
 from .asm import read
 from .bch import Reader
 from .model import MachineModel
```

### Comparing `femagtools-1.2.8/femagtools/airgap.py` & `femagtools-1.2.9/femagtools/airgap.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/amazon.py` & `femagtools-1.2.9/femagtools/amazon.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/amela.py` & `femagtools-1.2.9/femagtools/amela.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/asm.py` & `femagtools-1.2.9/femagtools/asm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/bch.py` & `femagtools-1.2.9/femagtools/bch.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/bchxml.py` & `femagtools-1.2.9/femagtools/bchxml.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/condor.py` & `femagtools-1.2.9/femagtools/condor.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/conductor.py` & `femagtools-1.2.9/femagtools/conductor.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/config.py` & `femagtools-1.2.9/femagtools/config.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/convert.py` & `femagtools-1.2.9/femagtools/convert.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/dakota.py` & `femagtools-1.2.9/femagtools/dakota.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/dakota_femag.py` & `femagtools-1.2.9/femagtools/dakota_femag.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/dakotaout.py` & `femagtools-1.2.9/femagtools/dakotaout.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/docker.py` & `femagtools-1.2.9/femagtools/docker.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/dxfsl/area.py` & `femagtools-1.2.9/femagtools/dxfsl/area.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/dxfsl/conv.py` & `femagtools-1.2.9/femagtools/dxfsl/conv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/dxfsl/converter.py` & `femagtools-1.2.9/femagtools/dxfsl/converter.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/dxfsl/corner.py` & `femagtools-1.2.9/femagtools/dxfsl/corner.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/dxfsl/dumprenderer.py` & `femagtools-1.2.9/femagtools/dxfsl/dumprenderer.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/dxfsl/fslrenderer.py` & `femagtools-1.2.9/femagtools/dxfsl/fslrenderer.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/dxfsl/functions.py` & `femagtools-1.2.9/femagtools/dxfsl/functions.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/dxfsl/geom.py` & `femagtools-1.2.9/femagtools/dxfsl/geom.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/dxfsl/machine.py` & `femagtools-1.2.9/femagtools/dxfsl/machine.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/dxfsl/plotrenderer.py` & `femagtools-1.2.9/femagtools/dxfsl/plotrenderer.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/dxfsl/shape.py` & `femagtools-1.2.9/femagtools/dxfsl/shape.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/erg.py` & `femagtools-1.2.9/femagtools/erg.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/femag.py` & `femagtools-1.2.9/femagtools/femag.py`

 * *Files 1% similar despite different names*

```diff
@@ -523,14 +523,15 @@
 
 
 class FemagTask(threading.Thread):
     def __init__(self, port, args, workdir, logdir):
         threading.Thread.__init__(self)
         self.port = port
         self.args = args + [str(self.port)]
+        self.proc = None
         self.returncode = None
         self.workdir = workdir
         self.logdir = logdir
 
     def run(self):
         logger.info("femag is ready on port %d workdir %s",
                     self.port, self.workdir)
@@ -797,24 +798,24 @@
         args = [cmd] + options
         self.femagTask = FemagTask(self.port, args, self.workdir, self.logdir)
         self.femagTask.start()
         if not self.request_socket:
             self.request_socket = self.__req_socket()
 
         # check if mq is ready for listening
-        lcount = 10
+        lcount = 300
         for t in range(lcount):
             time.sleep(0.1)
             if self.__is_running():
                 if self.femagTask.proc:
                     logger.info("femag (pid: '{}') is listening".format(
                         self.femagTask.proc.pid))
                 break
 
-        return self.femagTask.proc.pid
+        return self.femagTask.proc.pid if self.femagTask.proc else 0
 
     def quit(self, save_model=False):
         """terminates femag"""
 
         if not self.__is_running():
             logger.info("Femag already stopped")
             return
```

### Comparing `femagtools-1.2.8/femagtools/forcedens.py` & `femagtools-1.2.9/femagtools/forcedens.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/fsl.py` & `femagtools-1.2.9/femagtools/fsl.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/getset.py` & `femagtools-1.2.9/femagtools/getset.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/gmsh.py` & `femagtools-1.2.9/femagtools/gmsh.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/google.py` & `femagtools-1.2.9/femagtools/google.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/grid.py` & `femagtools-1.2.9/femagtools/grid.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/isa7.py` & `femagtools-1.2.9/femagtools/isa7.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/jcf2msh.py` & `femagtools-1.2.9/femagtools/jcf2msh.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/jhb.py` & `femagtools-1.2.9/femagtools/jhb.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/job.py` & `femagtools-1.2.9/femagtools/job.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/losscoeffs.py` & `femagtools-1.2.9/femagtools/losscoeffs.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/machine/__init__.py` & `femagtools-1.2.9/femagtools/machine/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
     Analytical machine models
 
 """
 import numpy as np
 from femagtools.bch import Reader
 from .pm import PmRelMachineLdq, PmRelMachinePsidq
+from .sm import SynchronousMachine, SynchronousMachineLdq, SynchronousMachinePsidq
 from .im import InductionMachine
 from .utils import betai1, iqd, invpark, K, T, puconv, dqpar_interpol
 import copy
 import logging
 
 logger = logging.getLogger(__name__)
 
@@ -28,76 +29,106 @@
         return l
     return {}
 
 
 def create_from_eecpars(temp, eecpars, lfe=1, wdg=1):
     """create machine according to the eecpars:
     PM, EESM or IM"""
-    if 'ldq' in eecpars:  # this is a PM (or EESM)
-        if (isinstance(eecpars['ldq'], list) and
-            'ex_current' in eecpars['ldq'][0] or
-            isinstance(eecpars['ldq'], dict) and
-                'ex_current' in eecpars['ldq']):
-            pars = copy.deepcopy(eecpars)
-            pars['tcu1'] = temp[0]
-            pars['tcu2'] = temp[1]
-            return femagtools.machine.sm.SynchronousMachine(pars, lfe=lfe, wdg=wdg)
+    rlfe = lfe
+    rwdg = wdg
+    if 'ldq' in eecpars or 'psidq' in eecpars:  # this is a PM (or EESM)
+        try:
+            dqpars = eecpars['ldq']
+        except KeyError:
+            dqpars = eecpars['psidq']
+        if (isinstance(dqpars, list) and
+            'ex_current' in dqpars[0] or
+            isinstance(dqpars, dict) and
+                'ex_current' in dqpars):
+            smpars = copy.deepcopy(eecpars)
+            smpars['tcu1'] = temp[0]
+            smpars['tcu2'] = temp[1]
+            if 'ldq' in smpars:
+                machine = SynchronousMachineLdq(smpars, lfe=rlfe, wdg=rwdg)
+            else:
+                machine = SynchronousMachinePsidq(smpars, lfe=rlfe, wdg=rwdg)
+            try:
+                machine.rotor_mass = rlfe*eecpars['rotor_mass']
+            except KeyError:
+                pass
+            return machine
 
-        if isinstance(eecpars['ldq'], list) and len(eecpars['ldq']) > 1:
+        if isinstance(dqpars, list) and len(dqpars) > 1:
             x, dqp = dqpar_interpol(
-                temp[1], eecpars['ldq'], ipkey='temperature')
+                temp[1], dqpars, ipkey='temperature')
         else:
-            dqp = eecpars['ldq'][0]
+            dqp = dqpars[0]
             logger.warning(
                 "single temperature DQ parameters: unable to fit temperature %s", temp)
 
-        beta = dqp['beta']
-        i1 = np.array(dqp['i1'])/wdg
-        psid = wdg*lfe*dqp['psid']
-        psiq = wdg*lfe*dqp['psiq']
+        psid = rwdg*rlfe*dqp['psid']
+        psiq = rwdg*rlfe*dqp['psiq']
         try:
-            losses = __scale_losses(dqp['losses'], lfe)
-            losses['ef'] = eecpars['ldq'][-1]['losses']['ef']
-            losses['eh'] = eecpars['ldq'][-1]['losses']['ef']
+            losses = __scale_losses(dqp['losses'], rlfe)
+            losses['ef'] = dqpars[-1]['losses']['ef']
+            losses['eh'] = dqpars[-1]['losses']['ef']
         except KeyError as e:
             logger.warning(e)
             losses = {}
-
-        return PmRelMachineLdq(
-            eecpars['m'], eecpars['p'],
-            r1=eecpars['r1']*lfe*wdg**2,
-            ls=eecpars['ls1']*wdg**2,
-            psid=psid,
-            psiq=psiq,
-            losses=losses,
-            beta=beta,
-            i1=i1,
-            tcu1=temp[0])
-
-    else:  # must be an induction machine (TODO: check scaling)
-        pars = copy.deepcopy(eecpars)
-        pars['r1'] = lfe*wdg**2*pars['r1']
-        pars['lsigma1'] = lfe*pars['lsigma1']
-        pars['lsigma2'] = lfe*pars['lsigma2']
-        pars['psiref'] = wdg*lfe*pars['psiref']
-        pars['u1ref'] = wdg*lfe*pars['u1ref']
-        pars['rotor_mass'] = lfe*pars['rotor_mass']
-        pars['r2'] = lfe*pars['r2']
-        pars['fec'] = lfe*pars['fec']
-        pars['fee'] = lfe*pars['fee']
-        pars['im'] = [im/wdg for im in pars['im']]
-        pars['psi'] = [psi*wdg*lfe for psi in pars['psi']]
-        pars['tcu1'] = temp[0]
-        pars['tcu2'] = temp[1]
-        return InductionMachine(pars)
+        if 'psidq' in eecpars:
+            machine = PmRelMachinePsidq(
+                eecpars['m'], eecpars['p'],
+                r1=eecpars['r1']*rlfe*rwdg**2,
+                ls=eecpars['ls1']*rwdg**2,
+                psid=psid,
+                psiq=psiq,
+                losses=losses,
+                id=np.array(dqp['id'])/rwdg,
+                iq=np.array(dqp['iq'])/rwdg,
+                tcu1=temp[0])
+        else:
+            beta = dqp['beta']
+            i1 = np.array(dqp['i1'])/rwdg
+            machine = PmRelMachineLdq(
+                eecpars['m'], eecpars['p'],
+                r1=eecpars['r1']*rlfe*rwdg**2,
+                ls=eecpars['ls1']*rwdg**2,
+                psid=psid,
+                psiq=psiq,
+                losses=losses,
+                beta=beta,
+                i1=i1,
+                tcu1=temp[0])
+        try:
+            machine.rotor_mass = rlfe*eecpars['rotor_mass']
+        except KeyError:
+            pass
+        return machine
+
+    # must be an induction machine (TODO: check scaling)
+    pars = copy.deepcopy(eecpars)
+    pars['r1'] = rlfe*rwdg**2*pars['r1']
+    pars['lsigma1'] = rlfe*pars['lsigma1']
+    pars['lsigma2'] = rlfe*pars['lsigma2']
+    pars['psiref'] = rwdg*rlfe*pars['psiref']
+    pars['u1ref'] = rwdg*rlfe*pars['u1ref']
+    pars['rotor_mass'] = rlfe*pars['rotor_mass']
+    pars['r2'] = rlfe*pars['r2']
+    pars['fec'] = rlfe*pars['fec']
+    pars['fee'] = rlfe*pars['fee']
+    pars['im'] = [im/rwdg for im in pars['im']]
+    pars['psi'] = [psi*rwdg*rlfe for psi in pars['psi']]
+    pars['tcu1'] = temp[0]
+    pars['tcu2'] = temp[1]
+    return InductionMachine(pars)
 
 
-def __scale_losses(losses, lfe):
+def __scale_losses(losses, rlfe):
     if losses:
-        l = {k: lfe*np.array(losses[k]) for k in (
+        l = {k: rlfe*np.array(losses[k]) for k in (
             'styoke_hyst', 'styoke_eddy',
             'stteeth_hyst', 'stteeth_eddy',
             'rotor_hyst', 'rotor_eddy',
             'magnet')}
         l['speed'] = losses['speed']
         return l
     return {}
@@ -106,52 +137,76 @@
 def create(bch, r1, ls, lfe=1, wdg=1):
     """create PmRelMachine from BCH
 
     Arguments:
       bch: BchReader or Erg object
       r1: winding resistance
       ls: winding leakage
-      lfe: scale factor length
-      wdg: scale factor number of windings
+      rlfe: scale factor length
+      rwdg: scale factor number of windings
 """
+    rwdg = wdg
+    rlfe = lfe
     m = 3
     if isinstance(bch, Reader):
         p = bch.machine['p']
         if bch.type.lower().find('psid-psiq-identification') >= 0:
-            id = np.array(bch.psidq['id'])/wdg
-            iq = np.array(bch.psidq['iq'])/wdg
-            psid = wdg*lfe*np.array(bch.psidq['psid'])
-            psiq = wdg*lfe*np.array(bch.psidq['psiq'])
+            id = np.array(bch.psidq['id'])/rwdg
+            iq = np.array(bch.psidq['iq'])/rwdg
+            psid = rwdg*rlfe*np.array(bch.psidq['psid'])
+            psiq = rwdg*rlfe*np.array(bch.psidq['psiq'])
             try:
-                losses = __scale_losses(bch.psidq['losses'], lfe)
+                losses = __scale_losses(bch.psidq['losses'], rlfe)
                 losses['ef'] = bch.lossPar.get('ef', [2.0, 2.0])
                 losses['eh'] = bch.lossPar.get('eh', [1.0, 1.0])
             except KeyError:
                 losses = {}
-            return PmRelMachinePsidq(m, p, psid, psiq, r1*lfe*wdg**2,
-                                     id, iq, ls*wdg**2, losses=losses)
+            if 'ex_current' in bch.machine:
+                raise ValueError("not yet implemented for EESM")
+            machine = PmRelMachinePsidq(m, p, psid, psiq, r1*rlfe*rwdg**2,
+                                        id, iq, ls*rwdg**2, losses=losses)
+            try:
+                machine.rotor_mass = rlfe*np.sum(bch.weights[1])
+            except IndexError:
+                pass
+            return machine
+
 
         if bch.type.lower().find('ld-lq-identification') >= 0:
             beta = bch.ldq['beta']
-            i1 = np.array(bch.ldq['i1'])/wdg
-            psid = wdg*lfe*np.array(bch.ldq['psid'])
-            psiq = wdg*lfe*np.array(bch.ldq['psiq'])
+            i1 = np.array(bch.ldq['i1'])/rwdg
+            psid = rwdg*rlfe*np.array(bch.ldq['psid'])
+            psiq = rwdg*rlfe*np.array(bch.ldq['psiq'])
             try:
-                losses = __scale_losses(bch.ldq['losses'], lfe)
+                losses = __scale_losses(bch.ldq['losses'], rlfe)
                 losses['ef'] = bch.lossPar.get('ef', [2.0, 2.0])
                 losses['eh'] = bch.lossPar.get('eh', [1.0, 1.0])
             except KeyError:
                 losses = {}
-            return PmRelMachineLdq(m, p, psid=psid, psiq=psiq,
-                                   r1=r1*lfe*wdg**2,
-                                   i1=i1, beta=beta, ls=ls*wdg**2,
-                                   losses=losses)
+            if 'ex_current' in bch.machine:
+                raise ValueError("not yet implemented for EESM")
+
+            machine = PmRelMachineLdq(m, p, psid=psid, psiq=psiq,
+                                      r1=r1*rlfe*rwdg**2,
+                                      i1=i1, beta=beta, ls=ls*rwdg**2,
+                                      losses=losses)
+            try:
+                machine.rotor_mass = rlfe*np.sum(bch.weights[1])
+            except IndexError:
+                pass
+            return machine
+
         raise ValueError("Unsupported BCH type {}".format(bch.type))
     # must be ERG type:
     p = int(round(np.sqrt(2)*bch['M_sim'][-1][-1]/(
         m*bch['Psi_d'][-1][-1] * bch['i1'][-1])))
 
-    return PmRelMachineLdq(m, p, r1=r1*lfe*wdg**2,
-                           beta=bch['beta'], i1=np.array(bch['i1'])/wdg,
-                           psid=wdg*lfe*np.array(bch['Psi_d'])/np.sqrt(2),
-                           psiq=wdg*lfe*np.array(bch['Psi_q'])/np.sqrt(2),
-                           ls=ls*wdg**2)
+    machine = PmRelMachineLdq(m, p, r1=r1*rlfe*rwdg**2,
+                              beta=bch['beta'], i1=np.array(bch['i1'])/rwdg,
+                              psid=rwdg*rlfe*np.array(bch['Psi_d'])/np.sqrt(2),
+                              psiq=rwdg*rlfe*np.array(bch['Psi_q'])/np.sqrt(2),
+                              ls=ls*rwdg**2)
+    try:
+        machine.rotor_mass = rlfe*np.sum(bch.weights[1])
+    except IndexError:
+        pass
+    return machine
```

### Comparing `femagtools-1.2.8/femagtools/machine/effloss.py` & `femagtools-1.2.9/femagtools/machine/effloss.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import scipy.interpolate as ip
 import logging
 from .utils import betai1
 from .pm import PmRelMachineLdq, PmRelMachinePsidq, PmRelMachine
+from .sm import SynchronousMachine
 from . import create_from_eecpars
 
 logger = logging.getLogger("femagtools.effloss")
 
 
 def _generate_mesh(n, T, nb, Tb, npoints):
     """return speed and torque list for driving/braking speed range
@@ -64,15 +65,15 @@
             xtemp = [temp, temp]
         m = create_from_eecpars(xtemp, eecpars)
     else:  # must be an instance of Machine
         m = eecpars
     if isinstance(T, list):
         r = {'T': T, 'n': n}
         rb = {'T': [], 'n': []}
-    else:  # calculate speed,torque charactersics
+    else:  # calculate speed,torque characteristics
         nmax = n
         rb = {}
         r = m.characteristics(T, nmax, u1)  # driving mode
         if isinstance(m, PmRelMachineLdq):
             if min(m.betarange) >= -np.pi/2:  # driving mode only
                 rb['n'] = None
                 rb['T'] = None
@@ -81,15 +82,15 @@
                 rb['n'] = None
                 rb['T'] = None
         if 'n' not in rb:
             rb = m.characteristics(-T, max(r['n']), u1)  # braking mode
     ntmesh = _generate_mesh(r['n'], r['T'],
                             rb['n'], rb['T'], npoints)
 
-    if isinstance(m, PmRelMachine):
+    if isinstance(m, PmRelMachine) or isinstance(m, SynchronousMachine):
         iqd = np.array([
             m.iqd_torque_umax(
                 nt[1],
                 2*np.pi*nt[0]*m.p,
                 u1)[:-1]
             for nt in ntmesh.T]).T
         beta, i1 = betai1(iqd[0], iqd[1])
@@ -111,34 +112,37 @@
             r['i1'].append(np.abs(i1))
             r['plfe1'].append(m.m*np.abs(u1)**2/m.rfe(w1, m.psi))
             i2 = m.i2(w1, m.psi, wm)
             r['plcu1'].append(m.m*np.abs(i1)**2*m.rstat(w1))
             r['plcu2'].append(m.m*np.abs(i2)**2*m.rrot(w1-m.p*wm))
 
 
-    if isinstance(m, PmRelMachine):
+    if isinstance(m, PmRelMachine) or isinstance(m, SynchronousMachine):
         plfe1 = m.iqd_plfe1(*iqd, f1)
         plfe2 = m.iqd_plfe2(iqd[0], iqd[1], f1)
         plmag = m.iqd_plmag(iqd[0], iqd[1], f1)
         plcu1 = m.iqd_plcu1(iqd[0], iqd[1], 2*np.pi*f1)
         plcu2 = m.iqd_plcu2(*iqd)
         try:
-            tfric = eecpars['kfric_b']*eecpars['rotor_mass']*30e-3/np.pi
-        except:
+            tfric = m.kfric_b*m.rotor_mass*30e-3/np.pi
+        except AttributeError:
             tfric = 0
     else:
         plfe1 = np.array(r['plfe1'])
         plfe2 = np.zeros(ntmesh.shape[1])
         plmag = np.zeros(ntmesh.shape[1])
         plcu1 = np.array(r['plcu1'])
         plcu2 = np.array(r['plcu2'])
         iqd = np.zeros(ntmesh.shape)
         u1 = np.array(r['u1'])
         i1 = np.array(r['i1'])
-        tfric = 0
+        try:
+            tfric = eecpars['kfric_b']*eecpars['rotor_mass']*30e-3/np.pi
+        except:
+            tfric = 0
 
     plfric = 2*np.pi*ntmesh[0]*tfric
     ntmesh[1] -= tfric
     pmech = np.array(
         [2*np.pi*nt[0]*nt[1]
          for nt in ntmesh.T])
     ploss = plfe1+plfe2+plmag+plcu1+plcu2+plfric
```

### Comparing `femagtools-1.2.8/femagtools/machine/im.py` & `femagtools-1.2.9/femagtools/machine/im.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/machine/pm.py` & `femagtools-1.2.9/femagtools/machine/pm.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         self.ls = ls
         self.io = (1, -1)
         self.fo = 50.0
         self.tcu1 = 20
         self.zeta1 = 0.2
         self.gam = 0.7
         self.kh = 2
+        self.kfric_b = 1
         for k in kwargs.keys():
             setattr(self, k, kwargs[k])
 
         self.plexp = {'styoke_hyst': 1.0,
                       'stteeth_hyst': 1.0,
                       'styoke_eddy': 2.0,
                       'stteeth_eddy': 2.0,
@@ -79,15 +80,15 @@
                           constraints=({'type': 'eq',
                                         'fun': lambda iqd:
                                         self.torque_iqd(*iqd) - torque}))
         if not res.success:
             raise ValueError(f'Torque {torque} out of current range')
         return res.x
 
-    def tmech_iqd(iq, id, n, kpfe, pfw):
+    def tmech_iqd(self, iq, id, n, kpfe, pfw):
         """return shaft torque with given d-q current, iron loss correction factor
           and friction windage losses"""
         f1 = self.p*n
         plfe1 = self.iqd_plfe1(iq, id, f1)
         plfe2 = self.iqd_plfe2(iq, id, f1)
         plfe = kpfe * (plfe1 + plfe2)
         pmag = self.iqd_plmag(iq, id, f1)
@@ -175,32 +176,28 @@
             return i1
         raise ValueError("{} for w1 {}, u1 {}, beta {}".format(
             mesg, w1, u1, beta))
 
     def id_torque(self, torque, iq):
         "return d current with given torque and d-current"
         id0 = min(self.io[1]/4, iq/np.tan(self.betarange[0]))
-        return so.fsolve(lambda id: self.torque_iqd(np.array([iq]), id)-torque, id0)[0]
+        return so.fsolve(
+            lambda id: self.torque_iqd(np.array([iq]), id)-torque, id0)[0]
 
     def iqd_torque_umax(self, torque, w1, u1max):
         "return d-q current and torque at stator frequency and max voltage"
-        iq, id = self.iqd_torque(torque)
-        # check voltage
-        if la.norm(self.uqd(w1, iq, id)) <= u1max*np.sqrt(2):
-            return (iq, id, torque)
-        # decrease psi (flux weakening mode), let i1 == i1max
-        iqd, info, ier, mesg = so.fsolve(
-            lambda iqd: (la.norm(self.uqd(w1, *iqd)) - u1max*np.sqrt(2),
-                         self.torque_iqd(*iqd) - torque),
-            (iq, id),
-            full_output=True)
-        if ier != 1:  # didn't converge
-            return self.mtpv(w1, u1max, betai1(iq, id)[1],
-                             maxtorque=torque > 0)
-        return iqd[0], iqd[1], self.torque_iqd(iq, id)
+        res = so.minimize(lambda iqd: la.norm(iqd), self.io, method='SLSQP',
+                          constraints=(
+                              {'type': 'eq',
+                               'fun': lambda iqd:
+                               self.torque_iqd(*iqd) - torque},
+                              {'type': 'ineq',
+                               'fun': lambda iqd:
+                               np.sqrt(2)*u1max - la.norm(self.uqd(w1, *iqd))}))
+        return res.x[0], res.x[1], self.torque_iqd(*res.x)
 
     def iqd_torque_imax_umax(self, torque, n, umax):
         """return iq, id, torque for constant torque or field weakening"""
         iq, id = self.iqd_torque(torque)
         w1 = 2*np.pi*n*self.p
         # Constant torque range
         if np.linalg.norm(self.uqd(w1, iq, id)) <= umax*np.sqrt(2):
@@ -218,17 +215,17 @@
             btab = np.linspace(max(-np.pi/2, self.betarange[0]), 0)
         else:
             btab = np.linspace(min(-np.pi/2, self.betarange[1]),
                                self.betarange[0])
         u1b = [np.linalg.norm(self.uqd(w1, *iqd(b, i1max)))
                for b in btab]
         if np.max(u1b) > np.sqrt(2)*u1max:
-            beta0=btab[0]
+            beta0 = btab[0]
             for bx, ux in zip(btab, u1b):
-                if ux/np.sqrt(2)>u1max:
+                if ux/np.sqrt(2) > u1max:
                     break
                 beta0 = bx
             beta, info, ier, mesg = so.fsolve(
                 lambda b: la.norm(
                     self.uqd(w1, *iqd(b, i1max))) - u1max*np.sqrt(2),
                 beta0,
                 full_output=True)
```

### Comparing `femagtools-1.2.8/femagtools/machine/sizing.py` & `femagtools-1.2.9/femagtools/machine/sizing.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/machine/utils.py` & `femagtools-1.2.9/femagtools/machine/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,16 @@
     """return winding resistance per phase in Ohm
     Arguments:
     wdg: (Winding) winding
     n: (int) number of wires per coil side
     g: (int) number of parallel coil groups
     lfe: length of stator lamination stack in m
     aw: wire cross section area m2
+    da1: bore diameter m
+    hs: slot height
     sigma: (float) conductivity of wire material 1/Ohm m
     """
     # mean length of one turn
     lt = 2.8*(da1+hs)/2*wdg.yd*2*np.pi/wdg.Q + 16e-3 + 2*lfe
     return wdg.turns_per_phase(n, g)*lt/sigma/aw/g
```

### Comparing `femagtools-1.2.8/femagtools/magnet.py` & `femagtools-1.2.9/femagtools/magnet.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/mcv.py` & `femagtools-1.2.9/femagtools/mcv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/me.py` & `femagtools-1.2.9/femagtools/me.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/model.py` & `femagtools-1.2.9/femagtools/model.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/moo/algorithm.py` & `femagtools-1.2.9/femagtools/moo/algorithm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/moo/population.py` & `femagtools-1.2.9/femagtools/moo/population.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/moo/problem.py` & `femagtools-1.2.9/femagtools/moo/problem.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/moproblem.py` & `femagtools-1.2.9/femagtools/moproblem.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/multiproc.py` & `femagtools-1.2.9/femagtools/multiproc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/mxw2msh.py` & `femagtools-1.2.9/femagtools/mxw2msh.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/nc.py` & `femagtools-1.2.9/femagtools/nc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/netlist.py` & `femagtools-1.2.9/femagtools/netlist.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/ntib.py` & `femagtools-1.2.9/femagtools/ntib.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/opt.py` & `femagtools-1.2.9/femagtools/opt.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/parstudy.py` & `femagtools-1.2.9/femagtools/parstudy.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/plot.py` & `femagtools-1.2.9/femagtools/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1728,16 +1728,21 @@
 def plot_contour(speed, torque, z, ax, title='', levels=[], clabel=True):
     from matplotlib.path import Path
     from matplotlib.patches import PathPatch
     x = [60*n for n in speed]
     y = torque
     if not levels:
         if max(z) <= 1:
-            levels = [0.25, 0.5, 0.75, 0.8, 0.84,
-                      0.88, 0.9, 0.92, 0.94, 0.96]
+            if max(z) > 0.96:
+                levels = [0.5, 0.75, 0.8, 0.84,
+                          0.88, 0.91, 0.93, 0.95, 0.97]
+            else:
+                levels = [0.25, 0.5, 0.75, 0.8, 0.84,
+                          0.88, 0.9, 0.92, 0.94, 0.96]
+
             if max(z) > levels[-1]:
                 levels.append(np.ceil(max(z)*100)/100)
         else:
             levels = 14
     cont = ax.tricontour(x, y, z,
                          linewidths=0.4, levels=levels, colors='k')
     if clabel:
```

### Comparing `femagtools-1.2.8/femagtools/poc.py` & `femagtools-1.2.9/femagtools/poc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/FE-losses.mako` & `femagtools-1.2.9/femagtools/templates/FE-losses.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/asyn_motor.mako` & `femagtools-1.2.9/femagtools/templates/asyn_motor.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/basic_modpar.mako` & `femagtools-1.2.9/femagtools/templates/basic_modpar.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/calc_field_ts.mako` & `femagtools-1.2.9/femagtools/templates/calc_field_ts.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/cogg_calc.mako` & `femagtools-1.2.9/femagtools/templates/cogg_calc.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/com_motor_sim.mako` & `femagtools-1.2.9/femagtools/templates/com_motor_sim.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/cu_losses.mako` & `femagtools-1.2.9/femagtools/templates/cu_losses.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/ec-rotorbar.mako` & `femagtools-1.2.9/femagtools/templates/ec-rotorbar.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/fe-contr.mako` & `femagtools-1.2.9/femagtools/templates/fe-contr.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/gen_winding.mako` & `femagtools-1.2.9/femagtools/templates/gen_winding.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/inductances.mako` & `femagtools-1.2.9/femagtools/templates/inductances.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/ld_lq_fast.mako` & `femagtools-1.2.9/femagtools/templates/ld_lq_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/leak_dist_wind.mako` & `femagtools-1.2.9/femagtools/templates/leak_dist_wind.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/leak_evol_wind.mako` & `femagtools-1.2.9/femagtools/templates/leak_evol_wind.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/magnet-data.mako` & `femagtools-1.2.9/femagtools/templates/magnet-data.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/magnetFC2.mako` & `femagtools-1.2.9/femagtools/templates/magnetFC2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/magnetIron.mako` & `femagtools-1.2.9/femagtools/templates/magnetIron.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/magnetIron2.mako` & `femagtools-1.2.9/femagtools/templates/magnetIron2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/magnetIron3.mako` & `femagtools-1.2.9/femagtools/templates/magnetIron3.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/magnetIron4.mako` & `femagtools-1.2.9/femagtools/templates/magnetIron4.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/magnetIron5.mako` & `femagtools-1.2.9/femagtools/templates/magnetIron5.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/magnetIronV.mako` & `femagtools-1.2.9/femagtools/templates/magnetIronV.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/magnetSector.mako` & `femagtools-1.2.9/femagtools/templates/magnetSector.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/magnetSectorLinear.mako` & `femagtools-1.2.9/femagtools/templates/magnetSectorLinear.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/magnetShell.mako` & `femagtools-1.2.9/femagtools/templates/magnetShell.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/magnetShell2.mako` & `femagtools-1.2.9/femagtools/templates/magnetShell2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/mesh-airgap.mako` & `femagtools-1.2.9/femagtools/templates/mesh-airgap.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/modal_analysis.mako` & `femagtools-1.2.9/femagtools/templates/modal_analysis.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/mult_cal_fast.mako` & `femagtools-1.2.9/femagtools/templates/mult_cal_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/noloadflux-rot.mako` & `femagtools-1.2.9/femagtools/templates/noloadflux-rot.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/noloadflux.mako` & `femagtools-1.2.9/femagtools/templates/noloadflux.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/noloadfluxdc.mako` & `femagtools-1.2.9/femagtools/templates/noloadfluxdc.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/plots.mako` & `femagtools-1.2.9/femagtools/templates/plots.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/pm_sym_f_cur.mako` & `femagtools-1.2.9/femagtools/templates/pm_sym_f_cur.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/pm_sym_fast.mako` & `femagtools-1.2.9/femagtools/templates/pm_sym_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/pm_sym_loss.mako` & `femagtools-1.2.9/femagtools/templates/pm_sym_loss.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/psd_psq_fast.mako` & `femagtools-1.2.9/femagtools/templates/psd_psq_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/ring.mako` & `femagtools-1.2.9/femagtools/templates/ring.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/rot_hsm.mako` & `femagtools-1.2.9/femagtools/templates/rot_hsm.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/rotorAsyn.mako` & `femagtools-1.2.9/femagtools/templates/rotorAsyn.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/rotorKs2.mako` & `femagtools-1.2.9/femagtools/templates/rotorKs2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/rotor_msh.mako` & `femagtools-1.2.9/femagtools/templates/rotor_msh.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/rotor_winding.mako` & `femagtools-1.2.9/femagtools/templates/rotor_winding.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/shortcircuit.mako` & `femagtools-1.2.9/femagtools/templates/shortcircuit.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/srm.mako` & `femagtools-1.2.9/femagtools/templates/srm.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/stator1.mako` & `femagtools-1.2.9/femagtools/templates/stator1.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/stator2.mako` & `femagtools-1.2.9/femagtools/templates/stator2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/stator3Linear.mako` & `femagtools-1.2.9/femagtools/templates/stator3Linear.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/stator4.mako` & `femagtools-1.2.9/femagtools/templates/stator4.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/statorBG.mako` & `femagtools-1.2.9/femagtools/templates/statorBG.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/statorRing.mako` & `femagtools-1.2.9/femagtools/templates/statorRing.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/statorRotor3.mako` & `femagtools-1.2.9/femagtools/templates/statorRotor3.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/stator_msh.mako` & `femagtools-1.2.9/femagtools/templates/stator_msh.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/templates/torq_calc.mako` & `femagtools-1.2.9/femagtools/templates/torq_calc.mako`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 --
 -- Torque/Force calculation
 --
 m.move_action     =    ${model.get('move_action', 0)}
-% if 'lfe' in model:
+% if model.get('lfe',0):
 m.arm_length      =    ${model.get('lfe')*1e3}
 % endif
 % if model.get('move_action', 0) == 0:
 m.speed           =    ${model.get('speed')*60}
 m.skew_angle      =    ${model.get('skew_angle',0)}
 m.fc_radius2      =    0.0
 m.phi_start       =    ${model.get('phi_start', 0)}
 m.range_phi       =    ${model.get('range_phi', 0)}
-m.nu_force_pat    =    0.0
 % else:
 m.speed_linear    =    ${model.get('speed')}
 m.skew_linear     =    ${model.get('skew_displ',0)}
 m.line            =    0
 m.two_pole_wi     =    2*m.pole_width
 m.range_x         =    m.two_pole_wi
-m.range_y         =    0.0 
+m.range_y         =    0.0
 
-m.fc_force_points =  5                                                
+m.fc_force_points =  5
 m.fcpx_mm1        =   m.npols_gen*m.pole_width +1.0
 m.fcpy_mm1        =   -3*ag/4
 m.fcpx_mm2        =   -1.0
 m.fcpy_mm2        =   m.fcpy_mm1
 m.fcpx_mm3        =   m.fcpx_mm2
 m.fcpy_mm3        =   -m.magn_height -m.yoke_height -m.gap_ma_yoke -4
 m.fcpx_mm4        =   m.fcpx_mm1
 m.fcpy_mm4        =   m.fcpy_mm3
 m.fcpx_mm5        =   m.fcpx_mm1
 m.fcpy_mm5        =   m.fcpy_mm1
 
 m.npols_gen       =  1 -- number of sectors simulated
 
 % endif
+m.nu_force_pat    =    0.0
 m.nu_skew_steps   =    ${model.get('num_skew_steps',0)}
 m.magn_temp       =    ${model.get('magn_temp',20.0)}
 m.winding_temp    =    ${model.get('wind_temp', 20.0)}
 m.fc_mult_move_type =  1.0 --  Type of move path in air gap
 m.nu_move_steps   =    ${model.get('num_move_steps', 49)}
 
 m.num_par_wdgs    =    ${model.get('num_par_wdgs',1)}
```

### Comparing `femagtools-1.2.8/femagtools/tks.py` & `femagtools-1.2.9/femagtools/tks.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/ts.py` & `femagtools-1.2.9/femagtools/ts.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/vbf.py` & `femagtools-1.2.9/femagtools/vbf.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/vtu.py` & `femagtools-1.2.9/femagtools/vtu.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools/windings.py` & `femagtools-1.2.9/femagtools/windings.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/femagtools.egg-info/PKG-INFO` & `femagtools-1.2.9/femagtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femagtools
-Version: 1.2.8
+Version: 1.2.9
 Summary: Python API for FEMAG
 Author-email: Ronald Tanner <tar@semafor.ch>, Dapu Zhang <d.zhan@gtisoft.com>, Beat Holm <hob@semafor.ch>, Günther Amsler <amg@semafor.ch>, Nicolas Mauchle <mau@semafor.ch>
 License: Copyright (c) 2016-2023, Semafor Informatik & Energie AG, Basel
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions
```

### Comparing `femagtools-1.2.8/femagtools.egg-info/SOURCES.txt` & `femagtools-1.2.9/femagtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/pyproject.toml` & `femagtools-1.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_airgap_induction.py` & `femagtools-1.2.9/tests/test_airgap_induction.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_amela.py` & `femagtools-1.2.9/tests/test_amela.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_asm.py` & `femagtools-1.2.9/tests/test_asm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_bchreader.py` & `femagtools-1.2.9/tests/test_bchreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_convert.py` & `femagtools-1.2.9/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_effloss.py` & `femagtools-1.2.9/tests/test_effloss.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,12 +22,12 @@
     T = 32.9
     u1 = 230
     temp = (120, 120)
 
     r = femagtools.machine.effloss.efficiency_losses_map(
         impars, u1, T, temp, nmax, npoints=(5, 4))
     assert r['T'] == pytest.approx(
-        [-33, -0.5, 0.5, 32.8,
-         -25, -0.5, 0.5, 23.2,
-         -12.8, -0.5, 0.5, 11.7,
-         -8.6, -0.5, 0.5, 7.8,
-         -6.5, -0.5, 0.5, 5.8], abs=1e-1)
+        [-33.1, -0.6, 0.4, 32.7,
+         -25.2, -0.6, 0.4, 23.2,
+         -12.8, -0.6, 0.4, 11.6,
+         -8.7, -0.6, 0.4, 7.7,
+         -6.6, -0.6, 0.4, 5.8], abs=1e-1)
```

### Comparing `femagtools-1.2.8/tests/test_erg.py` & `femagtools-1.2.9/tests/test_erg.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_femag.py` & `femagtools-1.2.9/tests/test_femag.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_forcedens.py` & `femagtools-1.2.9/tests/test_forcedens.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_fsl.py` & `femagtools-1.2.9/tests/test_fsl.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_im.py` & `femagtools-1.2.9/tests/test_im.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_isa7.py` & `femagtools-1.2.9/tests/test_isa7.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_jhb.py` & `femagtools-1.2.9/tests/test_jhb.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_job.py` & `femagtools-1.2.9/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_losscoeffs.py` & `femagtools-1.2.9/tests/test_losscoeffs.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_machine.py` & `femagtools-1.2.9/tests/test_machine.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_magncurv.py` & `femagtools-1.2.9/tests/test_magncurv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_mcvreader.py` & `femagtools-1.2.9/tests/test_mcvreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_mcvwriter.py` & `femagtools-1.2.9/tests/test_mcvwriter.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_model.py` & `femagtools-1.2.9/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_nc.py` & `femagtools-1.2.9/tests/test_nc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_parident.py` & `femagtools-1.2.9/tests/test_parident.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_parstudy.py` & `femagtools-1.2.9/tests/test_parstudy.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_pocfile.py` & `femagtools-1.2.9/tests/test_pocfile.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_sizing.py` & `femagtools-1.2.9/tests/test_sizing.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_sm.py` & `femagtools-1.2.9/tests/test_sm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1127,15 +1127,16 @@
                                              [10.68, 10.61, 12.58,
                                                  16.6, 21.58, 28.23],
                                              [10.68, 11.52, 13.67,
                                                  16.88, 20.49, 25.0],
                                              [10.68, 12.06, 14.5,
                                                  17.56, 19.53, 21.85],
                                              [10.68, 12.57, 15.18, 17.33, 18.99, 20.43]]}}]}
-    return femagtools.machine.sm.SynchronousMachine(smpars)
+    return femagtools.machine.sm.SynchronousMachineLdq(smpars)
 
 
 def test_sm(sm):
     u1 = 230
     f1 = 50
     iqdf = sm.iqd_torque(120)
-    assert pytest.approx(iqdf, rel=0.01) == [271.5, -45.31, 5.4]
+
+    assert pytest.approx(iqdf, rel=0.1) == np.array([276.9, -26.5,   5.3])
```

### Comparing `femagtools-1.2.8/tests/test_tksreader.py` & `femagtools-1.2.9/tests/test_tksreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_ts.py` & `femagtools-1.2.9/tests/test_ts.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_vbfreader.py` & `femagtools-1.2.9/tests/test_vbfreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_vtu.py` & `femagtools-1.2.9/tests/test_vtu.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.8/tests/test_windings.py` & `femagtools-1.2.9/tests/test_windings.py`

 * *Files identical despite different names*

