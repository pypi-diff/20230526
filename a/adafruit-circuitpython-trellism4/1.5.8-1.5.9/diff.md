# Comparing `tmp/adafruit-circuitpython-trellism4-1.5.8.tar.gz` & `tmp/adafruit-circuitpython-trellism4-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-trellism4-1.5.8.tar", last modified: Fri Feb  4 20:35:43 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-trellism4-1.5.9.tar", last modified: Tue Jun  7 16:56:51 2022, max compression
```

## Comparing `adafruit-circuitpython-trellism4-1.5.8.tar` & `adafruit-circuitpython-trellism4-1.5.9.tar`

### file list

```diff
@@ -1,223 +1,223 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:43.895810 adafruit-circuitpython-trellism4-1.5.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:43.875812 adafruit-circuitpython-trellism4-1.5.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:43.875812 adafruit-circuitpython-trellism4-1.5.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:43.875812 adafruit-circuitpython-trellism4-1.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:43.875812 adafruit-circuitpython-trellism4-1.5.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3581 2022-02-04 20:35:43.895810 adafruit-circuitpython-trellism4-1.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2874 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:43.879811 adafruit-circuitpython-trellism4-1.5.8/adafruit_circuitpython_trellism4.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3581 2022-02-04 20:35:43.000000 adafruit-circuitpython-trellism4-1.5.8/adafruit_circuitpython_trellism4.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10918 2022-02-04 20:35:43.000000 adafruit-circuitpython-trellism4-1.5.8/adafruit_circuitpython_trellism4.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 20:35:43.000000 adafruit-circuitpython-trellism4-1.5.8/adafruit_circuitpython_trellism4.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-04 20:35:43.000000 adafruit-circuitpython-trellism4-1.5.8/adafruit_circuitpython_trellism4.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-02-04 20:35:43.000000 adafruit-circuitpython-trellism4-1.5.8/adafruit_circuitpython_trellism4.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10539 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/adafruit_trellism4.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:43.879811 adafruit-circuitpython-trellism4-1.5.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:43.879811 adafruit-circuitpython-trellism4-1.5.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5444 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      898 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:43.879811 adafruit-circuitpython-trellism4-1.5.8/examples/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1253 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_neopixel_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      906 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_neopixel_toggle.py
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_press_and_release.py
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:43.879811 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:43.875812 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:43.883811 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/A3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/A3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/A4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/A4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/A5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/A5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/B3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/B3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/B4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/B4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/B5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/B5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/C3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/C3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/C4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/C4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/C5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/C5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/D3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/D3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/D4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/D4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/D5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/D5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/E3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/E3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/E4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/E4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/E5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/E5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/F3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/F3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/F4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/F4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/F5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/F5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/G3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/G3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/G4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/G4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/G5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/G5.wav.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:43.887811 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/A3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/A3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/A4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/A4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/A5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/A5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/B3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/B3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/B4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/B4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/B5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/B5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/C3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/C3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/C4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/C4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/C5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/C5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/D3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/D3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/D4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/D4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/D5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/D5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/E3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/E3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/E4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/E4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/E5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/E5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/F3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/F3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/F4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/F4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/F5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/F5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/G3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/G3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/G4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/G4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/G5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/G5.wav.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:43.891811 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/A3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/A3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/A4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/A4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/A5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/A5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/B3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/B3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/B4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/B4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/B5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/B5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/C3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/C3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/C4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/C4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/C5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/C5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/D3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/D3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/D4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/D4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/D5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/D5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/E3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/E3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/E4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/E4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/E5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/E5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/F3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/F3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/F4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/F4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/F5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/F5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/G3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/G3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/G4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/G4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/G5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/G5.wav.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:43.891811 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/A3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/A3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/A4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/A4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/A5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/A5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/B3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/B3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/B4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/B4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/B5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/B5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/C3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/C3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/C4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/C4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/C5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/C5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/D3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/D3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/D4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/D4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/D5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/D5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/E3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/E3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/E4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/E4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/E5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/E5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/F3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/F3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/F4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/F4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/F5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/F5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/G3.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/G3.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/G4.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/G4.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/G5.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/G5.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     4352 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/trellism4_wavefile_synth.py
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 20:35:43.895810 adafruit-circuitpython-trellism4-1.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1791 2022-02-04 20:35:28.000000 adafruit-circuitpython-trellism4-1.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:56:51.715310 adafruit-circuitpython-trellism4-1.5.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:56:51.683310 adafruit-circuitpython-trellism4-1.5.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:56:51.687310 adafruit-circuitpython-trellism4-1.5.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:56:51.687310 adafruit-circuitpython-trellism4-1.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:56:51.687310 adafruit-circuitpython-trellism4-1.5.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3604 2022-06-07 16:56:51.715310 adafruit-circuitpython-trellism4-1.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2897 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:56:51.687310 adafruit-circuitpython-trellism4-1.5.9/adafruit_circuitpython_trellism4.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3604 2022-06-07 16:56:51.000000 adafruit-circuitpython-trellism4-1.5.9/adafruit_circuitpython_trellism4.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10918 2022-06-07 16:56:51.000000 adafruit-circuitpython-trellism4-1.5.9/adafruit_circuitpython_trellism4.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 16:56:51.000000 adafruit-circuitpython-trellism4-1.5.9/adafruit_circuitpython_trellism4.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-07 16:56:51.000000 adafruit-circuitpython-trellism4-1.5.9/adafruit_circuitpython_trellism4.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-06-07 16:56:51.000000 adafruit-circuitpython-trellism4-1.5.9/adafruit_circuitpython_trellism4.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10539 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/adafruit_trellism4.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:56:51.691310 adafruit-circuitpython-trellism4-1.5.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:56:51.691310 adafruit-circuitpython-trellism4-1.5.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5444 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      898 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:56:51.691310 adafruit-circuitpython-trellism4-1.5.9/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1253 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_neopixel_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      906 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_neopixel_toggle.py
+-rw-r--r--   0 runner    (1001) docker     (121)      461 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_press_and_release.py
+-rw-r--r--   0 runner    (1001) docker     (121)      269 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:56:51.691310 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:56:51.683310 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:56:51.699310 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/A3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/A3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/A4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/A4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/A5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/A5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/B3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/B3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/B4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/B4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/B5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/B5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/C3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/C3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/C4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/C4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/C5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/C5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/D3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/D3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/D4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/D4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/D5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/D5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/E3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/E3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/E4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/E4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/E5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/E5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/F3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/F3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/F4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/F4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/F5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/F5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/G3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/G3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/G4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/G4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/G5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/G5.wav.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:56:51.707310 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/A3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/A3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/A4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/A4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/A5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/A5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/B3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/B3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/B4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/B4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/B5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/B5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/C3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/C3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/C4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/C4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/C5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/C5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/D3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/D3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/D4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/D4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/D5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/D5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/E3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/E3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/E4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/E4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/E5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/E5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/F3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/F3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/F4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/F4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/F5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/F5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/G3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/G3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/G4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/G4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/G5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/G5.wav.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:56:51.711310 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/A3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/A3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/A4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/A4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/A5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/A5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/B3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/B3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/B4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/B4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/B5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/B5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/C3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/C3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/C4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/C4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/C5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/C5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/D3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/D3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/D4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/D4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/D5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/D5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/E3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/E3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/E4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/E4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/E5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/E5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/F3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/F3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/F4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/F4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/F5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/F5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/G3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/G3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/G4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/G4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/G5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/G5.wav.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:56:51.715310 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/A3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/A3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/A4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/A4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/A5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/A5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/B3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/B3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/B4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/B4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/B5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/B5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/C3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/C3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/C4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/C4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/C5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/C5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/D3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/D3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/D4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/D4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/D5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/D5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/E3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/E3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/E4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/E4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/E5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/E5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/F3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/F3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/F4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/F4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/F5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/F5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/G3.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/G3.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/G4.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/G4.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8044 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/G5.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/G5.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     4352 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/trellism4_wavefile_synth.py
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 16:56:51.715310 adafruit-circuitpython-trellism4-1.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1791 2022-06-07 16:56:38.000000 adafruit-circuitpython-trellism4-1.5.9/setup.py
```

### Comparing `adafruit-circuitpython-trellism4-1.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-trellism4-1.5.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/.github/workflows/build.yml` & `adafruit-circuitpython-trellism4-1.5.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/.github/workflows/release.yml` & `adafruit-circuitpython-trellism4-1.5.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/.pre-commit-config.yaml` & `adafruit-circuitpython-trellism4-1.5.9/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
--   repo: https://github.com/python/black
-    rev: 20.8b1
+  - repo: https://github.com/python/black
+    rev: 22.3.0
     hooks:
-    - id: black
--   repo: https://github.com/fsfe/reuse-tool
-    rev: v0.12.1
+      - id: black
+  - repo: https://github.com/fsfe/reuse-tool
+    rev: v0.14.0
     hooks:
-    - id: reuse
--   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v2.3.0
+      - id: reuse
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.2.0
     hooks:
-    -   id: check-yaml
-    -   id: end-of-file-fixer
-    -   id: trailing-whitespace
--   repo: https://github.com/pycqa/pylint
+      - id: check-yaml
+      - id: end-of-file-fixer
+      - id: trailing-whitespace
+  - repo: https://github.com/pycqa/pylint
     rev: v2.11.1
     hooks:
-    -   id: pylint
+      - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
-    -   id: pylint
+      - id: pylint
         name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
         types: [python]
         files: "^examples/"
         args:
-        - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
-    -   id: pylint
+          - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
+      - id: pylint
         name: pylint (test code)
         description: Run pylint rules on "tests/*.py" files
         types: [python]
         files: "^tests/"
         args:
-        - --disable=missing-docstring,consider-using-f-string,duplicate-code
+          - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

### Comparing `adafruit-circuitpython-trellism4-1.5.8/.pylintrc` & `adafruit-circuitpython-trellism4-1.5.9/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code
 extension-pkg-whitelist=
 
-# Add files or directories to the blacklist. They should be base names, not
+# Add files or directories to the ignore-list. They should be base names, not
 # paths.
 ignore=CVS
 
-# Add files or directories matching the regex patterns to the blacklist. The
+# Add files or directories matching the regex patterns to the ignore-list. The
 # regex matches against base names, not paths.
 ignore-patterns=
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
 #init-hook=
 
@@ -248,15 +248,15 @@
 # Ignore docstrings when computing similarities.
 ignore-docstrings=yes
 
 # Ignore imports when computing similarities.
 ignore-imports=yes
 
 # Minimum lines number of a similarity.
-min-similarity-lines=4
+min-similarity-lines=12
 
 
 [BASIC]
 
 # Naming hint for argument names
 argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
```

### Comparing `adafruit-circuitpython-trellism4-1.5.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-trellism4-1.5.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/LICENSE` & `adafruit-circuitpython-trellism4-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-trellism4-1.5.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/LICENSES/MIT.txt` & `adafruit-circuitpython-trellism4-1.5.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-trellism4-1.5.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/PKG-INFO` & `adafruit-circuitpython-trellism4-1.5.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-trellism4
-Version: 1.5.8
+Version: 1.5.9
 Summary: CircuitPython library Trellis M4 Express.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_TrellisM4
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit trellism4 hardware micropython circuitpython
 Platform: UNKNOWN
@@ -20,15 +20,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-trellism4/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/trellism4/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_TrellisM4/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_TrellisM4/actions/
     :alt: Build Status
 
@@ -92,20 +92,17 @@
          current_press = pressed
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/trellism4/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_TrellisM4/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
```

### Comparing `adafruit-circuitpython-trellism4-1.5.8/README.rst` & `adafruit-circuitpython-trellism4-1.5.9/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-trellism4/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/trellism4/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_TrellisM4/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_TrellisM4/actions/
     :alt: Build Status
 
@@ -73,18 +73,15 @@
          current_press = pressed
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/trellism4/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_TrellisM4/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-trellism4-1.5.8/adafruit_circuitpython_trellism4.egg-info/PKG-INFO` & `adafruit-circuitpython-trellism4-1.5.9/adafruit_circuitpython_trellism4.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-trellism4
-Version: 1.5.8
+Version: 1.5.9
 Summary: CircuitPython library Trellis M4 Express.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_TrellisM4
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit trellism4 hardware micropython circuitpython
 Platform: UNKNOWN
@@ -20,15 +20,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-trellism4/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/trellism4/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_TrellisM4/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_TrellisM4/actions/
     :alt: Build Status
 
@@ -92,20 +92,17 @@
          current_press = pressed
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/trellism4/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_TrellisM4/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
```

### Comparing `adafruit-circuitpython-trellism4-1.5.8/adafruit_circuitpython_trellism4.egg-info/SOURCES.txt` & `adafruit-circuitpython-trellism4-1.5.9/adafruit_circuitpython_trellism4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/adafruit_trellism4.py` & `adafruit-circuitpython-trellism4-1.5.9/adafruit_trellism4.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/docs/_static/favicon.ico` & `adafruit-circuitpython-trellism4-1.5.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/docs/conf.py` & `adafruit-circuitpython-trellism4-1.5.9/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 release = "1.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".env", "CODE_OF_CONDUCT.md"]
 
 # The reST default role (used for this markup: `text`) to use for all
```

### Comparing `adafruit-circuitpython-trellism4-1.5.8/docs/index.rst` & `adafruit-circuitpython-trellism4-1.5.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_neopixel_simpletest.py` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_neopixel_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_neopixel_toggle.py` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_neopixel_toggle.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/A3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/A3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/A4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/A4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/A5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/A5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/B3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/B3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/B4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/B4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/B5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/B5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/C3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/C3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/C4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/C4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/C5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/C5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/D3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/D3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/D4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/D4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/D5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/D5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/E3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/E3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/E4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/E4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/E5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/E5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/F3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/F3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/F4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/F4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/F5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/F5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/G3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/G3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/G4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/G4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sawtooth/G5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sawtooth/G5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/A3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/A3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/A4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/A4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/A5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/A5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/B3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/B3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/B4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/B4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/B5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/B5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/C3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/C3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/C4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/C4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/C5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/C5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/D3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/D3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/D4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/D4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/D5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/D5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/E3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/E3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/E4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/E4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/E5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/E5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/F3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/F3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/F4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/F4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/F5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/F5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/G3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/G3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/G4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/G4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/sine/G5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/sine/G5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/A3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/A3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/A4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/A4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/A5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/A5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/B3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/B3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/B4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/B4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/B5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/B5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/C3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/C3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/C4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/C4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/C5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/C5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/D3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/D3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/D4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/D4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/D5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/D5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/E3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/E3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/E4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/E4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/E5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/E5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/F3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/F3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/F4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/F4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/F5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/F5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/G3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/G3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/G4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/G4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/square/G5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/square/G5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/A3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/A3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/A4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/A4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/A5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/A5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/B3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/B3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/B4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/B4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/B5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/B5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/C3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/C3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/C4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/C4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/C5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/C5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/D3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/D3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/D4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/D4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/D5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/D5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/E3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/E3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/E4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/E4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/E5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/E5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/F3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/F3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/F4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/F4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/F5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/F5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/G3.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/G3.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/G4.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/G4.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/notes/triangle/G5.wav` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/notes/triangle/G5.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/examples/trellism4_wavefile_synth/trellism4_wavefile_synth.py` & `adafruit-circuitpython-trellism4-1.5.9/examples/trellism4_wavefile_synth/trellism4_wavefile_synth.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-trellism4-1.5.8/setup.py` & `adafruit-circuitpython-trellism4-1.5.9/setup.py`

 * *Files identical despite different names*

