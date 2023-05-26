# Comparing `tmp/multidecoder-0.0.9.tar.gz` & `tmp/multidecoder-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidecoder-0.0.9.tar", last modified: Tue May  3 17:13:01 2022, max compression
+gzip compressed data, was "multidecoder-0.1.0.tar", last modified: Fri May 26 13:38:58 2023, max compression
```

## Comparing `multidecoder-0.0.9.tar` & `multidecoder-0.1.0.tar`

### file list

```diff
@@ -1,189 +1,195 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-03 17:13:01.612146 multidecoder-0.0.9/
--rw-r--r--   0 vsts      (1001) docker     (121)     2126 2022-05-03 17:11:59.000000 multidecoder-0.0.9/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (121)     1390 2022-05-03 17:11:59.000000 multidecoder-0.0.9/LICENSE.md
--rw-r--r--   0 vsts      (1001) docker     (121)     2324 2022-05-03 17:13:01.612146 multidecoder-0.0.9/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1657 2022-05-03 17:11:59.000000 multidecoder-0.0.9/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-03 17:13:01.592146 multidecoder-0.0.9/multidecoder/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1379 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      142 2022-05-03 17:13:00.000000 multidecoder-0.0.9/multidecoder/_version.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-03 17:13:01.596146 multidecoder-0.0.9/multidecoder/analyzers/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1816 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/base64.py
--rw-r--r--   0 vsts      (1001) docker     (121)      724 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/concat.py
--rw-r--r--   0 vsts      (1001) docker     (121)      433 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/encoding.py
--rw-r--r--   0 vsts      (1001) docker     (121)      444 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/filename.py
--rw-r--r--   0 vsts      (1001) docker     (121)      414 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/hex.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3930 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/network.py
--rw-r--r--   0 vsts      (1001) docker     (121)      464 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/path.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1154 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/pe_file.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4396 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/shell.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1108 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/vba.py
--rw-r--r--   0 vsts      (1001) docker     (121)      637 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/xml.py
--rw-r--r--   0 vsts      (1001) docker     (121)    22373 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/domains.py
--rw-r--r--   0 vsts      (1001) docker     (121)      808 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/hit.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1987 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/json_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1067 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keyword.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-03 17:13:01.596146 multidecoder-0.0.9/multidecoder/keywords/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-03 17:13:01.612146 multidecoder-0.0.9/multidecoder/keywords/api/
--rw-r--r--   0 vsts      (1001) docker     (121)     4040 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.advapi32
--rw-r--r--   0 vsts      (1001) docker     (121)       23 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.apphelp
--rw-r--r--   0 vsts      (1001) docker     (121)     1212 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.atl
--rw-r--r--   0 vsts      (1001) docker     (121)      243 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.atl80
--rw-r--r--   0 vsts      (1001) docker     (121)      229 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.atl90
--rw-r--r--   0 vsts      (1001) docker     (121)      429 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.au3zip
--rw-r--r--   0 vsts      (1001) docker     (121)      162 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.avicap32
--rw-r--r--   0 vsts      (1001) docker     (121)      196 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.cabinet
--rw-r--r--   0 vsts      (1001) docker     (121)       16 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.clbcatq
--rw-r--r--   0 vsts      (1001) docker     (121)       56 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.cmdial32
--rw-r--r--   0 vsts      (1001) docker     (121)      177 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.comctl32
--rw-r--r--   0 vsts      (1001) docker     (121)       91 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.credui
--rw-r--r--   0 vsts      (1001) docker     (121)      197 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.cryptbase
--rw-r--r--   0 vsts      (1001) docker     (121)       26 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.cryptdll
--rw-r--r--   0 vsts      (1001) docker     (121)       24 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.cscapi
--rw-r--r--   0 vsts      (1001) docker     (121)      610 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.dbghelp
--rw-r--r--   0 vsts      (1001) docker     (121)       79 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.devmgr
--rw-r--r--   0 vsts      (1001) docker     (121)      406 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.dnsapi
--rw-r--r--   0 vsts      (1001) docker     (121)       16 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.drprov
--rw-r--r--   0 vsts      (1001) docker     (121)      225 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.dsound
--rw-r--r--   0 vsts      (1001) docker     (121)       32 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.dsuiext
--rw-r--r--   0 vsts      (1001) docker     (121)       13 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.esent
--rw-r--r--   0 vsts      (1001) docker     (121)       18 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.fveapi
--rw-r--r--   0 vsts      (1001) docker     (121)      127 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.fwpuclnt
--rw-r--r--   0 vsts      (1001) docker     (121)     1913 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.gdi32
--rw-r--r--   0 vsts      (1001) docker     (121)      388 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.gina
--rw-r--r--   0 vsts      (1001) docker     (121)      100 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.icmp
--rw-r--r--   0 vsts      (1001) docker     (121)     1254 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.imagehlp
--rw-r--r--   0 vsts      (1001) docker     (121)     1005 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.iphlpapi
--rw-r--r--   0 vsts      (1001) docker     (121)    19404 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.kernel32
--rw-r--r--   0 vsts      (1001) docker     (121)       21 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.kernelbase
--rw-r--r--   0 vsts      (1001) docker     (121)     2218 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.libeay32
--rw-r--r--   0 vsts      (1001) docker     (121)       22 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.lsasrv
--rw-r--r--   0 vsts      (1001) docker     (121)      265 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.mapi32
--rw-r--r--   0 vsts      (1001) docker     (121)     1968 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.mfc42
--rw-r--r--   0 vsts      (1001) docker     (121)      445 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.mpr
--rw-r--r--   0 vsts      (1001) docker     (121)      143 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.mprapi
--rw-r--r--   0 vsts      (1001) docker     (121)       54 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.msacm32
--rw-r--r--   0 vsts      (1001) docker     (121)       81 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.msasn1
--rw-r--r--   0 vsts      (1001) docker     (121)       53 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.mscoree
--rw-r--r--   0 vsts      (1001) docker     (121)     4043 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.msi
--rw-r--r--   0 vsts      (1001) docker     (121)       13 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.msimg32
--rw-r--r--   0 vsts      (1001) docker     (121)       16 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.mspdb80
--rw-r--r--   0 vsts      (1001) docker     (121)      520 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.mssign32
--rw-r--r--   0 vsts      (1001) docker     (121)       66 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.msutb
--rw-r--r--   0 vsts      (1001) docker     (121)     1527 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.msvbvm60
--rw-r--r--   0 vsts      (1001) docker     (121)     3448 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.msvcrt
--rw-r--r--   0 vsts      (1001) docker     (121)       22 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.msvfw32
--rw-r--r--   0 vsts      (1001) docker     (121)       16 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.mswsock
--rw-r--r--   0 vsts      (1001) docker     (121)       11 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.mydocs
--rw-r--r--   0 vsts      (1001) docker     (121)      525 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.nddeapi
--rw-r--r--   0 vsts      (1001) docker     (121)     1276 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.netapi32
--rw-r--r--   0 vsts      (1001) docker     (121)       20 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.netplwiz
--rw-r--r--   0 vsts      (1001) docker     (121)     4660 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.ntdll
--rw-r--r--   0 vsts      (1001) docker     (121)      197 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.ntdsapi
--rw-r--r--   0 vsts      (1001) docker     (121)     1137 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.ntoskrnl
--rw-r--r--   0 vsts      (1001) docker     (121)       43 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.ntshrui
--rw-r--r--   0 vsts      (1001) docker     (121)     1599 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.odbc32
--rw-r--r--   0 vsts      (1001) docker     (121)      970 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.odbccp32
--rw-r--r--   0 vsts      (1001) docker     (121)       55 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.odbctrac
--rw-r--r--   0 vsts      (1001) docker     (121)      829 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.ole32
--rw-r--r--   0 vsts      (1001) docker     (121)      641 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.oleaut32
--rw-r--r--   0 vsts      (1001) docker     (121)       58 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.oledlg
--rw-r--r--   0 vsts      (1001) docker     (121)      167 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.onex
--rw-r--r--   0 vsts      (1001) docker     (121)      587 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.packet
--rw-r--r--   0 vsts      (1001) docker     (121)      222 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.pdh
--rw-r--r--   0 vsts      (1001) docker     (121)     2236 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.powrprof
--rw-r--r--   0 vsts      (1001) docker     (121)      455 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.psapi
--rw-r--r--   0 vsts      (1001) docker     (121)       40 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.pstorec
--rw-r--r--   0 vsts      (1001) docker     (121)       15 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.query
--rw-r--r--   0 vsts      (1001) docker     (121)       29 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.rasapi32
--rw-r--r--   0 vsts      (1001) docker     (121)       22 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.rastapi
--rw-r--r--   0 vsts      (1001) docker     (121)       18 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.riched20
--rw-r--r--   0 vsts      (1001) docker     (121)     1207 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.rpcrt4
--rw-r--r--   0 vsts      (1001) docker     (121)       99 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.scarddlg
--rw-r--r--   0 vsts      (1001) docker     (121)     1561 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.scecli
--rw-r--r--   0 vsts      (1001) docker     (121)      729 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.se
--rw-r--r--   0 vsts      (1001) docker     (121)      166 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.secur32
--rw-r--r--   0 vsts      (1001) docker     (121)       14 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.sensapi
--rw-r--r--   0 vsts      (1001) docker     (121)      239 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.setupapi
--rw-r--r--   0 vsts      (1001) docker     (121)      123 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.sfc
--rw-r--r--   0 vsts      (1001) docker     (121)     3672 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.shell32
--rw-r--r--   0 vsts      (1001) docker     (121)       15 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.shimgvw
--rw-r--r--   0 vsts      (1001) docker     (121)      544 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.shlwapi
--rw-r--r--   0 vsts      (1001) docker     (121)       26 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.shsvcs
--rw-r--r--   0 vsts      (1001) docker     (121)     1328 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.ssleay32
--rw-r--r--   0 vsts      (1001) docker     (121)       86 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.unknown
--rw-r--r--   0 vsts      (1001) docker     (121)     1068 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.urlmon
--rw-r--r--   0 vsts      (1001) docker     (121)     1564 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.user32
--rw-r--r--   0 vsts      (1001) docker     (121)      309 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.userenv
--rw-r--r--   0 vsts      (1001) docker     (121)      114 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.usp10
--rw-r--r--   0 vsts      (1001) docker     (121)       60 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.version
--rw-r--r--   0 vsts      (1001) docker     (121)      312 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.winhttp
--rw-r--r--   0 vsts      (1001) docker     (121)      928 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.wininet
--rw-r--r--   0 vsts      (1001) docker     (121)       11 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.winmm
--rw-r--r--   0 vsts      (1001) docker     (121)      219 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.winscard
--rw-r--r--   0 vsts      (1001) docker     (121)       21 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.winshfhc
--rw-r--r--   0 vsts      (1001) docker     (121)     1994 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.winsock
--rw-r--r--   0 vsts      (1001) docker     (121)      254 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.winspool
--rw-r--r--   0 vsts      (1001) docker     (121)     3887 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.winsta
--rw-r--r--   0 vsts      (1001) docker     (121)       14 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.wintrust
--rw-r--r--   0 vsts      (1001) docker     (121)       55 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.wlanapi
--rw-r--r--   0 vsts      (1001) docker     (121)      249 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.wldap32
--rw-r--r--   0 vsts      (1001) docker     (121)      266 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.wship6
--rw-r--r--   0 vsts      (1001) docker     (121)      754 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.wsnmp32
--rw-r--r--   0 vsts      (1001) docker     (121)      490 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.wtsapi32
--rw-r--r--   0 vsts      (1001) docker     (121)       13 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/archive
--rw-r--r--   0 vsts      (1001) docker     (121)       13 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/av.name
--rw-r--r--   0 vsts      (1001) docker     (121)      503 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/cryptography
--rw-r--r--   0 vsts      (1001) docker     (121)       70 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/debugger.device.name
--rw-r--r--   0 vsts      (1001) docker     (121)      168 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/enable_content
--rw-r--r--   0 vsts      (1001) docker     (121)       27 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/environment.windows
--rw-r--r--   0 vsts      (1001) docker     (121)      634 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/event
--rw-r--r--   0 vsts      (1001) docker     (121)      517 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/guid
--rw-r--r--   0 vsts      (1001) docker     (121)     1091 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/key
--rw-r--r--   0 vsts      (1001) docker     (121)       41 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/network.protocol
--rw-r--r--   0 vsts      (1001) docker     (121)      532 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/network.string
--rw-r--r--   0 vsts      (1001) docker     (121)     1812 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/oid
--rw-r--r--   0 vsts      (1001) docker     (121)     2674 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/os_name
--rw-r--r--   0 vsts      (1001) docker     (121)     1476 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/powershell.cmdlet
--rw-r--r--   0 vsts      (1001) docker     (121)      873 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/privilege
--rw-r--r--   0 vsts      (1001) docker     (121)     1038 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/ransomware.string
--rw-r--r--   0 vsts      (1001) docker     (121)      263 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/sandbox.id
--rw-r--r--   0 vsts      (1001) docker     (121)      902 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/security_identifier
--rw-r--r--   0 vsts      (1001) docker     (121)      151 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/user_agent
--rw-r--r--   0 vsts      (1001) docker     (121)       53 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/vba.name
--rw-r--r--   0 vsts      (1001) docker     (121)     2164 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/windows.registry
--rw-r--r--   0 vsts      (1001) docker     (121)    22786 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords_to_review.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     2634 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/multidecoder.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1410 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/query.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2277 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/registry.py
--rw-r--r--   0 vsts      (1001) docker     (121)      472 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/string_helper.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-03 17:13:01.592146 multidecoder-0.0.9/multidecoder.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     2324 2022-05-03 17:13:01.000000 multidecoder-0.0.9/multidecoder.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     6193 2022-05-03 17:13:01.000000 multidecoder-0.0.9/multidecoder.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-05-03 17:13:01.000000 multidecoder-0.0.9/multidecoder.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       60 2022-05-03 17:13:01.000000 multidecoder-0.0.9/multidecoder.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-05-03 17:12:09.000000 multidecoder-0.0.9/multidecoder.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (121)       34 2022-05-03 17:13:01.000000 multidecoder-0.0.9/multidecoder.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       13 2022-05-03 17:13:01.000000 multidecoder-0.0.9/multidecoder.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-03 17:13:01.612146 multidecoder-0.0.9/pipelines/
--rw-r--r--   0 vsts      (1001) docker     (121)     1252 2022-05-03 17:11:59.000000 multidecoder-0.0.9/pipelines/publish.yaml
--rw-r--r--   0 vsts      (1001) docker     (121)      239 2022-05-03 17:11:59.000000 multidecoder-0.0.9/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (121)      994 2022-05-03 17:13:01.612146 multidecoder-0.0.9/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)       69 2022-05-03 17:11:59.000000 multidecoder-0.0.9/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-03 17:13:01.612146 multidecoder-0.0.9/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-03 17:13:01.612146 multidecoder-0.0.9/tests/test_analyzers/
--rw-r--r--   0 vsts      (1001) docker     (121)     1215 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_analyzers/test_base64.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1927 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_analyzers/test_concat.py
--rw-r--r--   0 vsts      (1001) docker     (121)      567 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_analyzers/test_encoding.py
--rw-r--r--   0 vsts      (1001) docker     (121)      334 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_analyzers/test_filename.py
--rw-r--r--   0 vsts      (1001) docker     (121)      449 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_analyzers/test_hex.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4661 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_analyzers/test_network.py
--rw-r--r--   0 vsts      (1001) docker     (121)      995 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_analyzers/test_path.py
--rw-r--r--   0 vsts      (1001) docker     (121)      382 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_analyzers/test_pe_file.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4561 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_analyzers/test_shell.py
--rw-r--r--   0 vsts      (1001) docker     (121)      473 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_analyzers/test_vba.py
--rw-r--r--   0 vsts      (1001) docker     (121)      708 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_analyzers/test_xml.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1170 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_multidecoder.py
--rw-r--r--   0 vsts      (1001) docker     (121)      111 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tox.ini
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 13:38:58.716854 multidecoder-0.1.0/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2126 2023-05-26 13:38:23.000000 multidecoder-0.1.0/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (122)     1390 2023-05-26 13:38:23.000000 multidecoder-0.1.0/LICENSE.md
+-rw-r--r--   0 vsts      (1001) docker     (122)     2547 2023-05-26 13:38:58.716854 multidecoder-0.1.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1900 2023-05-26 13:38:23.000000 multidecoder-0.1.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 13:38:58.648854 multidecoder-0.1.0/multidecoder/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1617 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      160 2023-05-26 13:38:58.000000 multidecoder-0.1.0/multidecoder/_version.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 13:38:58.652854 multidecoder-0.1.0/multidecoder/analyzers/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/analyzers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2982 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/analyzers/base64.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      370 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/analyzers/chr.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      887 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/analyzers/concat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/analyzers/encoding.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      455 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/analyzers/filename.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      414 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/analyzers/hex.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      435 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/analyzers/javascript.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3931 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/analyzers/network.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      464 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/analyzers/path.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1154 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/analyzers/pe_file.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1752 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/analyzers/replace.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4835 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/analyzers/shell.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1416 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/analyzers/vba.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      637 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/analyzers/xml.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    22373 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/domains.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      875 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/hit.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1987 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/json_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1067 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keyword.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 13:38:58.660854 multidecoder-0.1.0/multidecoder/keywords/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 13:38:58.708854 multidecoder-0.1.0/multidecoder/keywords/api/
+-rw-r--r--   0 vsts      (1001) docker     (122)     4040 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.advapi32
+-rw-r--r--   0 vsts      (1001) docker     (122)       23 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.apphelp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1212 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.atl
+-rw-r--r--   0 vsts      (1001) docker     (122)      243 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.atl80
+-rw-r--r--   0 vsts      (1001) docker     (122)      229 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.atl90
+-rw-r--r--   0 vsts      (1001) docker     (122)      429 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.au3zip
+-rw-r--r--   0 vsts      (1001) docker     (122)      162 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.avicap32
+-rw-r--r--   0 vsts      (1001) docker     (122)      196 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.cabinet
+-rw-r--r--   0 vsts      (1001) docker     (122)       16 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.clbcatq
+-rw-r--r--   0 vsts      (1001) docker     (122)       56 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.cmdial32
+-rw-r--r--   0 vsts      (1001) docker     (122)      177 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.comctl32
+-rw-r--r--   0 vsts      (1001) docker     (122)       91 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.credui
+-rw-r--r--   0 vsts      (1001) docker     (122)      197 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.cryptbase
+-rw-r--r--   0 vsts      (1001) docker     (122)       26 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.cryptdll
+-rw-r--r--   0 vsts      (1001) docker     (122)       24 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.cscapi
+-rw-r--r--   0 vsts      (1001) docker     (122)      610 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.dbghelp
+-rw-r--r--   0 vsts      (1001) docker     (122)       79 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.devmgr
+-rw-r--r--   0 vsts      (1001) docker     (122)      406 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.dnsapi
+-rw-r--r--   0 vsts      (1001) docker     (122)       16 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.drprov
+-rw-r--r--   0 vsts      (1001) docker     (122)      225 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.dsound
+-rw-r--r--   0 vsts      (1001) docker     (122)       32 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.dsuiext
+-rw-r--r--   0 vsts      (1001) docker     (122)       13 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.esent
+-rw-r--r--   0 vsts      (1001) docker     (122)       18 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.fveapi
+-rw-r--r--   0 vsts      (1001) docker     (122)      127 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.fwpuclnt
+-rw-r--r--   0 vsts      (1001) docker     (122)     1913 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.gdi32
+-rw-r--r--   0 vsts      (1001) docker     (122)      388 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.gina
+-rw-r--r--   0 vsts      (1001) docker     (122)      100 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.icmp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1254 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.imagehlp
+-rw-r--r--   0 vsts      (1001) docker     (122)     1005 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.iphlpapi
+-rw-r--r--   0 vsts      (1001) docker     (122)    19404 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.kernel32
+-rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.kernelbase
+-rw-r--r--   0 vsts      (1001) docker     (122)     2218 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.libeay32
+-rw-r--r--   0 vsts      (1001) docker     (122)       22 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.lsasrv
+-rw-r--r--   0 vsts      (1001) docker     (122)      265 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.mapi32
+-rw-r--r--   0 vsts      (1001) docker     (122)     1968 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.mfc42
+-rw-r--r--   0 vsts      (1001) docker     (122)      445 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.mpr
+-rw-r--r--   0 vsts      (1001) docker     (122)      143 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.mprapi
+-rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.msacm32
+-rw-r--r--   0 vsts      (1001) docker     (122)       81 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.msasn1
+-rw-r--r--   0 vsts      (1001) docker     (122)       53 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.mscoree
+-rw-r--r--   0 vsts      (1001) docker     (122)     4043 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.msi
+-rw-r--r--   0 vsts      (1001) docker     (122)       13 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.msimg32
+-rw-r--r--   0 vsts      (1001) docker     (122)       16 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.mspdb80
+-rw-r--r--   0 vsts      (1001) docker     (122)      520 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.mssign32
+-rw-r--r--   0 vsts      (1001) docker     (122)       66 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.msutb
+-rw-r--r--   0 vsts      (1001) docker     (122)     1527 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.msvbvm60
+-rw-r--r--   0 vsts      (1001) docker     (122)     3448 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.msvcrt
+-rw-r--r--   0 vsts      (1001) docker     (122)       22 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.msvfw32
+-rw-r--r--   0 vsts      (1001) docker     (122)       16 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.mswsock
+-rw-r--r--   0 vsts      (1001) docker     (122)       11 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.mydocs
+-rw-r--r--   0 vsts      (1001) docker     (122)      525 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.nddeapi
+-rw-r--r--   0 vsts      (1001) docker     (122)     1276 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.netapi32
+-rw-r--r--   0 vsts      (1001) docker     (122)       20 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.netplwiz
+-rw-r--r--   0 vsts      (1001) docker     (122)     4660 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.ntdll
+-rw-r--r--   0 vsts      (1001) docker     (122)      197 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.ntdsapi
+-rw-r--r--   0 vsts      (1001) docker     (122)     1137 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.ntoskrnl
+-rw-r--r--   0 vsts      (1001) docker     (122)       43 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.ntshrui
+-rw-r--r--   0 vsts      (1001) docker     (122)     1599 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.odbc32
+-rw-r--r--   0 vsts      (1001) docker     (122)      970 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.odbccp32
+-rw-r--r--   0 vsts      (1001) docker     (122)       55 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.odbctrac
+-rw-r--r--   0 vsts      (1001) docker     (122)      829 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.ole32
+-rw-r--r--   0 vsts      (1001) docker     (122)      641 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.oleaut32
+-rw-r--r--   0 vsts      (1001) docker     (122)       58 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.oledlg
+-rw-r--r--   0 vsts      (1001) docker     (122)      167 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.onex
+-rw-r--r--   0 vsts      (1001) docker     (122)      587 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.packet
+-rw-r--r--   0 vsts      (1001) docker     (122)      222 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.pdh
+-rw-r--r--   0 vsts      (1001) docker     (122)     2236 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.powrprof
+-rw-r--r--   0 vsts      (1001) docker     (122)      455 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.psapi
+-rw-r--r--   0 vsts      (1001) docker     (122)       40 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.pstorec
+-rw-r--r--   0 vsts      (1001) docker     (122)       15 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.query
+-rw-r--r--   0 vsts      (1001) docker     (122)       29 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.rasapi32
+-rw-r--r--   0 vsts      (1001) docker     (122)       22 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.rastapi
+-rw-r--r--   0 vsts      (1001) docker     (122)       18 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.riched20
+-rw-r--r--   0 vsts      (1001) docker     (122)     1207 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.rpcrt4
+-rw-r--r--   0 vsts      (1001) docker     (122)       99 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.scarddlg
+-rw-r--r--   0 vsts      (1001) docker     (122)     1561 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.scecli
+-rw-r--r--   0 vsts      (1001) docker     (122)      729 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.se
+-rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.secur32
+-rw-r--r--   0 vsts      (1001) docker     (122)       14 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.sensapi
+-rw-r--r--   0 vsts      (1001) docker     (122)      239 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.setupapi
+-rw-r--r--   0 vsts      (1001) docker     (122)      123 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.sfc
+-rw-r--r--   0 vsts      (1001) docker     (122)     3672 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.shell32
+-rw-r--r--   0 vsts      (1001) docker     (122)       15 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.shimgvw
+-rw-r--r--   0 vsts      (1001) docker     (122)      544 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.shlwapi
+-rw-r--r--   0 vsts      (1001) docker     (122)       26 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.shsvcs
+-rw-r--r--   0 vsts      (1001) docker     (122)     1328 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.ssleay32
+-rw-r--r--   0 vsts      (1001) docker     (122)       86 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.unknown
+-rw-r--r--   0 vsts      (1001) docker     (122)     1068 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.urlmon
+-rw-r--r--   0 vsts      (1001) docker     (122)     1564 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.user32
+-rw-r--r--   0 vsts      (1001) docker     (122)      309 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.userenv
+-rw-r--r--   0 vsts      (1001) docker     (122)      114 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.usp10
+-rw-r--r--   0 vsts      (1001) docker     (122)       60 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.version
+-rw-r--r--   0 vsts      (1001) docker     (122)      312 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.winhttp
+-rw-r--r--   0 vsts      (1001) docker     (122)      928 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.wininet
+-rw-r--r--   0 vsts      (1001) docker     (122)       11 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.winmm
+-rw-r--r--   0 vsts      (1001) docker     (122)      219 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.winscard
+-rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.winshfhc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1994 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.winsock
+-rw-r--r--   0 vsts      (1001) docker     (122)      254 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.winspool
+-rw-r--r--   0 vsts      (1001) docker     (122)     3887 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.winsta
+-rw-r--r--   0 vsts      (1001) docker     (122)       14 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.wintrust
+-rw-r--r--   0 vsts      (1001) docker     (122)       55 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.wlanapi
+-rw-r--r--   0 vsts      (1001) docker     (122)      249 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.wldap32
+-rw-r--r--   0 vsts      (1001) docker     (122)      266 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.wship6
+-rw-r--r--   0 vsts      (1001) docker     (122)      754 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.wsnmp32
+-rw-r--r--   0 vsts      (1001) docker     (122)      490 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/api/api.wtsapi32
+-rw-r--r--   0 vsts      (1001) docker     (122)       13 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/archive
+-rw-r--r--   0 vsts      (1001) docker     (122)       13 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/av.name
+-rw-r--r--   0 vsts      (1001) docker     (122)      503 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/cryptography
+-rw-r--r--   0 vsts      (1001) docker     (122)       70 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/debugger.device.name
+-rw-r--r--   0 vsts      (1001) docker     (122)      168 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/enable_content
+-rw-r--r--   0 vsts      (1001) docker     (122)       27 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/environment.windows
+-rw-r--r--   0 vsts      (1001) docker     (122)      634 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/event
+-rw-r--r--   0 vsts      (1001) docker     (122)      517 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/guid
+-rw-r--r--   0 vsts      (1001) docker     (122)     1091 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/key
+-rw-r--r--   0 vsts      (1001) docker     (122)       41 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/network.protocol
+-rw-r--r--   0 vsts      (1001) docker     (122)      532 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/network.string
+-rw-r--r--   0 vsts      (1001) docker     (122)     1812 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/oid
+-rw-r--r--   0 vsts      (1001) docker     (122)     2674 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/os_name
+-rw-r--r--   0 vsts      (1001) docker     (122)     1476 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/powershell.cmdlet
+-rw-r--r--   0 vsts      (1001) docker     (122)      873 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/privilege
+-rw-r--r--   0 vsts      (1001) docker     (122)     1038 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/ransomware.string
+-rw-r--r--   0 vsts      (1001) docker     (122)      263 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/sandbox.id
+-rw-r--r--   0 vsts      (1001) docker     (122)      902 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/security_identifier
+-rw-r--r--   0 vsts      (1001) docker     (122)      151 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/user_agent
+-rw-r--r--   0 vsts      (1001) docker     (122)       53 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/vba.name
+-rw-r--r--   0 vsts      (1001) docker     (122)     2164 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords/windows.registry
+-rw-r--r--   0 vsts      (1001) docker     (122)    22786 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/keywords_to_review.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     2634 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/multidecoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2275 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/query.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2277 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      472 2023-05-26 13:38:23.000000 multidecoder-0.1.0/multidecoder/string_helper.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 13:38:58.648854 multidecoder-0.1.0/multidecoder.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2547 2023-05-26 13:38:58.000000 multidecoder-0.1.0/multidecoder.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     6404 2023-05-26 13:38:58.000000 multidecoder-0.1.0/multidecoder.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-26 13:38:58.000000 multidecoder-0.1.0/multidecoder.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       60 2023-05-26 13:38:58.000000 multidecoder-0.1.0/multidecoder.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-26 13:38:33.000000 multidecoder-0.1.0/multidecoder.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)       34 2023-05-26 13:38:58.000000 multidecoder-0.1.0/multidecoder.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       13 2023-05-26 13:38:58.000000 multidecoder-0.1.0/multidecoder.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 13:38:58.708854 multidecoder-0.1.0/pipelines/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1252 2023-05-26 13:38:23.000000 multidecoder-0.1.0/pipelines/publish.yaml
+-rw-r--r--   0 vsts      (1001) docker     (122)      239 2023-05-26 13:38:23.000000 multidecoder-0.1.0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)      994 2023-05-26 13:38:58.716854 multidecoder-0.1.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)       69 2023-05-26 13:38:23.000000 multidecoder-0.1.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 13:38:58.708854 multidecoder-0.1.0/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-26 13:38:23.000000 multidecoder-0.1.0/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-26 13:38:58.716854 multidecoder-0.1.0/tests/test_analyzers/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1928 2023-05-26 13:38:23.000000 multidecoder-0.1.0/tests/test_analyzers/test_base64.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      365 2023-05-26 13:38:23.000000 multidecoder-0.1.0/tests/test_analyzers/test_chr.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1928 2023-05-26 13:38:23.000000 multidecoder-0.1.0/tests/test_analyzers/test_concat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      567 2023-05-26 13:38:23.000000 multidecoder-0.1.0/tests/test_analyzers/test_encoding.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      334 2023-05-26 13:38:23.000000 multidecoder-0.1.0/tests/test_analyzers/test_filename.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      449 2023-05-26 13:38:23.000000 multidecoder-0.1.0/tests/test_analyzers/test_hex.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      293 2023-05-26 13:38:23.000000 multidecoder-0.1.0/tests/test_analyzers/test_javascript.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4661 2023-05-26 13:38:23.000000 multidecoder-0.1.0/tests/test_analyzers/test_network.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      995 2023-05-26 13:38:23.000000 multidecoder-0.1.0/tests/test_analyzers/test_path.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      382 2023-05-26 13:38:23.000000 multidecoder-0.1.0/tests/test_analyzers/test_pe_file.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      965 2023-05-26 13:38:23.000000 multidecoder-0.1.0/tests/test_analyzers/test_replace.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5429 2023-05-26 13:38:23.000000 multidecoder-0.1.0/tests/test_analyzers/test_shell.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      834 2023-05-26 13:38:23.000000 multidecoder-0.1.0/tests/test_analyzers/test_vba.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      708 2023-05-26 13:38:23.000000 multidecoder-0.1.0/tests/test_analyzers/test_xml.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1323 2023-05-26 13:38:23.000000 multidecoder-0.1.0/tests/test_multidecoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-05-26 13:38:23.000000 multidecoder-0.1.0/tox.ini
```

### Comparing `multidecoder-0.0.9/.gitignore` & `multidecoder-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/LICENSE.md` & `multidecoder-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/PKG-INFO` & `multidecoder-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: multidecoder
-Version: 0.0.9
+Version: 0.1.0
 Summary: A context preserving IOC extraction library
 Home-page: https://github.com/CybercentreCanada/Multidecoder
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CybercentreCanada/Multidecoder/issues
 Keywords: malware,analysis,gc,canada,cse-cst,cse,cst,cyber,cccs
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
@@ -33,19 +32,29 @@
 - base64 encoding
 - hexadecimal encoding
 - string concatenation
 - powershell escape characters
 
 ## Installing
 
-The latest Multidecoder can be installed from the repository:
+Multidecoder can be installed from pypi using pip:
+```
+pip install -U multidecoder
+```
+
+Alternatly, it can also be installed from the repository:
 ```
 pip install -U https://github.com/CybercentreCanada/Multidecoder/archive/main.zip
 ```
 
+To test the latest development version, install from the dev branch:
+```
+pip install -U https://github.com/CybercenterCanada/Multidecoder/archive/dev.zip
+```
+
 ## Command Line
 
 After being installed Multidecoder can be run on a file from the command-line
 ```
 > multidecoder file
 ```
 which will output a list of indicators found.
@@ -64,9 +73,7 @@
 which can scan data to give a dictionary tree similar to the command-line json output.
 ```
 from multidecoder.multidecoder import Multidecoder
 
 md = Multidecoder()
 context_tree = md.scan(data)
 ```
-
-
```

### Comparing `multidecoder-0.0.9/README.md` & `multidecoder-0.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -15,19 +15,29 @@
 - base64 encoding
 - hexadecimal encoding
 - string concatenation
 - powershell escape characters
 
 ## Installing
 
-The latest Multidecoder can be installed from the repository:
+Multidecoder can be installed from pypi using pip:
+```
+pip install -U multidecoder
+```
+
+Alternatly, it can also be installed from the repository:
 ```
 pip install -U https://github.com/CybercentreCanada/Multidecoder/archive/main.zip
 ```
 
+To test the latest development version, install from the dev branch:
+```
+pip install -U https://github.com/CybercenterCanada/Multidecoder/archive/dev.zip
+```
+
 ## Command Line
 
 After being installed Multidecoder can be run on a file from the command-line
 ```
 > multidecoder file
 ```
 which will output a list of indicators found.
```

### Comparing `multidecoder-0.0.9/multidecoder/__main__.py` & `multidecoder-0.1.0/multidecoder/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 import argparse
 import os
 import sys
 
 from multidecoder._version import version
 from multidecoder.multidecoder import Multidecoder
 from multidecoder.json_conversion import tree_to_json
-from multidecoder.query import string_summary
+from multidecoder.query import string_summary, squash_replace
 from multidecoder.registry import build_map
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('filepath', nargs='?', metavar='FILE')
     parser.add_argument('--version', '-V', action='version', version="%(prog)s " + version)
-    parser.add_argument('--json', '-j', action='store_true')
     parser.add_argument('--keywords', '-k')
+    output_format = parser.add_mutually_exclusive_group()
+    output_format.add_argument('--json', '-j', action='store_true')
+    output_format.add_argument('--replace', '-r', action='store_true')
     args = parser.parse_args()
     if args.filepath:
         try:
             with open(args.filepath, 'rb') as f:
                 data = f.read()
         except Exception as e:
             print(e, file=sys.stderr)
@@ -34,14 +36,16 @@
         analyzers = build_map(args.keywords)
     else:
         analyzers = None
     md = Multidecoder(analyzers)
     tree = md.scan(data)
     if args.json:
         print(tree_to_json(tree))
-        return
-    for string in string_summary(tree):
-        print(string)
+    elif args.replace:
+        sys.stdout.buffer.write(squash_replace(data, tree))
+    else:
+        for string in string_summary(tree):
+            print(string)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `multidecoder-0.0.9/multidecoder/analyzers/base64.py` & `multidecoder-0.1.0/multidecoder/analyzers/base64.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 from multidecoder.hit import Hit
 from multidecoder.registry import analyzer
 
 HTML_ESCAPE_RE = rb'&#(?:x[a-fA-F0-9]{1,4}|\d{1,4});'
 BASE64_RE = rb'(?:[A-Za-z0-9+/]{4,}(?:<\x00  \x00)?(?:&#13;|&#xD;)?(?:&#10;|&#xA)?\r?\n?){5,}' \
             rb'[A-Za-z0-9+/]{2,}=?=?'
+BASE64DECODE_RE = rb'(?i)Base64Decode\("([a-z0-9/+]+=?=?)"\)'
+FROMB64STRING_RE = rb"(?i)(\[System.Convert\]::)?FromBase64String\('([a-z0-9+/]+=?=?)'\)"
 
 CAMEL_RE = rb'(?i)[a-z]+'
 HEX_RE = rb'(?i)[a-f0-9]+'
 MIN_B64_CHARS = 6
 
 
 @analyzer('')
@@ -50,7 +52,38 @@
             continue
         try:
             b64_result = binascii.a2b_base64(b64_string)
             b64_matches.append(Hit(b64_result, 'decoded.base64', b64_match.start(), b64_match.end()))
         except binascii.Error:
             pass
     return b64_matches
+
+
+@analyzer('vba.string')
+def find_Base64Decode(data: bytes) -> list[Hit]:
+    out: list[Hit] = []
+    for match in re.finditer(BASE64DECODE_RE, data):
+        try:
+            b64 = binascii.a2b_base64(match.group(1))
+            out.append(Hit(b64, 'decode.base64', *match.span()))
+        except binascii.Error:
+            continue
+    return out
+
+
+@analyzer('powershell.bytes')
+def find_FromBase64String(data: bytes) -> list[Hit]:
+    out: list[Hit] = []
+    for match in re.finditer(FROMB64STRING_RE, data):
+        try:
+            b64 = binascii.a2b_base64(match.group(2))
+            xorkey = re.search(rb'(?i)-b?xor\s*(\d{1,3})', data)
+            if xorkey:
+                key = int(xorkey.group(1))
+                b64 = bytes(b ^ key for b in b64)
+                obfuscation = 'decode.base64/>xor'+str(key)
+            else:
+                obfuscation = 'decode.base64'
+            out.append(Hit(b64, obfuscation, *match.span()))
+        except binascii.Error:
+            continue
+    return out
```

### Comparing `multidecoder-0.0.9/multidecoder/analyzers/concat.py` & `multidecoder-0.1.0/multidecoder/analyzers/concat.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 
 from multidecoder.hit import Hit
 
 from multidecoder.registry import analyzer
 
 DOUBLE_QUOTE_ESCAPES = rb'\\""|""|\\"|`"'
 # Single or double quoted strings with various possible escapes for ' or "
-STRING_RE = rb'(?:"(?:' + DOUBLE_QUOTE_ESCAPES + rb'|[^"])*"|\'(?:[^\']|\'\')*\')'
-CONCAT_RE = rb'(?:' + STRING_RE + rb'\s*(?:&|\+|&amp;)\s*)+' + STRING_RE
+DOUBLE_QUOTE_STRING_RE = rb'"(?:' + DOUBLE_QUOTE_ESCAPES + rb'|[^"])*"'
+SINGLE_QUOTE_STRING_RE = rb"'(?:[^']|'')*'"
+STRING_RE = rb'(?:' + DOUBLE_QUOTE_STRING_RE + rb'|' + SINGLE_QUOTE_STRING_RE + rb')'
+# _ is VB line continuation character
+CONCAT_RE = rb'(?:' + STRING_RE + rb'[\s_]*(?:&|\+|&amp;)[\s_]*)+' + STRING_RE
 
 
 @analyzer('string')
 def find_concat(data: bytes) -> list[Hit]:
     return [
         Hit(
             b''.join(string[1:-1] for string in re.findall(STRING_RE, match.group())),
```

### Comparing `multidecoder-0.0.9/multidecoder/analyzers/network.py` & `multidecoder-0.1.0/multidecoder/analyzers/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 from multidecoder.string_helper import make_bytes
 from multidecoder.registry import analyzer
 
 _OCTET_RE = rb'(?:0x0*[a-f0-9]{1,2}|0*\d{1,3})'
 IP_RE = rb'(?i)\b(?:' + _OCTET_RE + rb'[.]){3}' + _OCTET_RE + rb'\b'
 DOMAIN_RE = rb'(?i)\b(?:[a-z0-9-]+\.)+(?:xn--[a-z0-9]{4,18}|[a-z]{2,12})\b'
 EMAIL_RE = rb'(?i)\b[a-z0-9._%+-]{3,}@(' + DOMAIN_RE[4:] + rb')\b'
-URL_RE = rb'(?i)(?:ftp|https?)://[a-z0-9-%.]+(?::[0-9]{1,5})?' \
-         rb'(?:/[a-z0-9/\-.&%$#=~?_+]{3,200})?'
+URL_RE = rb'(?i)(?:ftp|https?)://[a-z0-9-%.]+(?::[0-9]{1,5})?/?' \
+         rb'(?:[a-z0-9/\-.&%$#=~?_+]{3,200})?'
 
 
 @analyzer('network.domain')
 def find_domains(data: bytes) -> List[Hit]:
     """ Find domains in data """
     return [match_to_hit(match) for match in re.finditer(DOMAIN_RE, data)
             if is_valid_domain(match.group())]
```

### Comparing `multidecoder-0.0.9/multidecoder/analyzers/pe_file.py` & `multidecoder-0.1.0/multidecoder/analyzers/pe_file.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/analyzers/shell.py` & `multidecoder-0.1.0/multidecoder/analyzers/shell.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from __future__ import annotations
 
-import regex as re
 import binascii
 
+import regex as re
 from multidecoder.analyzers.concat import DOUBLE_QUOTE_ESCAPES
-from multidecoder.hit import Hit, find_and_deobfuscate
+from multidecoder.hit import Hit
 from multidecoder.registry import analyzer
 
-
-CMD_RE = rb'(?i)\bc\^?m\^?d(?:' + DOUBLE_QUOTE_ESCAPES + rb'|[^)"])+'
-POWERSHELL_INDICATOR_RE = rb'(?i)(?:^|/c|/k|[\s;,=\'"])(\^?p\^?(?:o\^?w\^?e\^?r\^?s\^?h\^?e\^?l\^?l|w\^?s\^?h))\b'
+CMD_RE = b'(?i)\\bc\\^?m\\^?d(?:' + DOUBLE_QUOTE_ESCAPES + rb'|[^)"\x00])*'
+POWERSHELL_INDICATOR_RE = rb'(?i)(?:^|/c|/k|/r|[\s;,=&\'"])(\^?p\^?(?:o\^?w\^?e\^?r\^?s\^?h\^?e\^?l\^?l|w\^?s\^?h))\b'
 SH_RE = rb'"(\s*(?:sh|bash|zsh|csh)[^"]+)"'
 ENC_RE = rb'(?i)\s\^?(?:-|/)\^?e\^?(?:c|n\^?(?:c\^?(?:o\^?(?:d\^?(?:e\^?(?:d\^?(?:c\^?(?:o\^?(?:m' \
-         rb'\^?(?:m\^?(?:a\^?(?:n\^?d?)?)?)?)?)?)?)?)?)?)?)?)?[\s^]+([a-z0-9+/^]{4,}=?\^?=?\^?)'
+         rb'\^?(?:m\^?(?:a\^?(?:n\^?d?)?)?)?)?)?)?)?)?)?)?)?)?[\s^]+[\"\']?([a-z0-9+/^]{4,}=?\^?=?\^?[\'\"]?)'
 POWERSHELL_ARGS_RE = rb'\s*(powershell|pwsh)?(.exe)?\s*((-|/)[^\s]+\s+)*'
 
 
 def strip_carets(cmd: bytes) -> bytes:
     in_string = False
     out = []
     i = 0
@@ -43,29 +42,38 @@
 def deobfuscate_cmd(cmd: bytes):
     stripped = strip_carets(cmd)
     return stripped, 'unescape.shell.carets' if stripped != cmd else ''
 
 
 @analyzer('shell.cmd')
 def find_cmd_strings(data: bytes) -> list[Hit]:
-    return find_and_deobfuscate(CMD_RE, data, deobfuscate_cmd)
+    return [
+        Hit(*deobfuscate_cmd(match.group()), *match.span())
+        for match in re.finditer(CMD_RE, data)
+        if match.group().lower().strip() not in (b'cmd', b'cmd.exe')
+    ]
 
 
 @analyzer('shell.powershell')
 def find_powershell_strings(data: bytes) -> list[Hit]:
     out = []
     # Find the string PowerShell, possibly obfuscated or shortened to pwsh
     for indicator in re.finditer(POWERSHELL_INDICATOR_RE, data):
         # Check for encoded parameter
         start = indicator.start(1)
         enc = re.search(ENC_RE, data, pos=start)
         if enc:
             powershell = data[start:enc.end()]
             deobfuscated, ob = deobfuscate_cmd(powershell)
             split = re.split(rb'\s+', deobfuscated)
+
+            # Remove quotation symbols
+            if (split[-1].startswith(b'\"') and split[-1].endswith(b'\"')) or split[-1].startswith(b"\'") and split[-1].endswith(b"\'"):
+                split[-1] = split[-1][1:-1]
+
             b64 = (binascii.a2b_base64(_pad(split[-1]))
                            .decode('utf-16', errors='ignore')
                            .encode())
             deobfuscated = b' '.join(split[:-2]) + b' -Command ' + b64
             obfuscation = ob + ('/>' if ob else '') + 'powershell.base64'
             out.append(Hit(deobfuscated, obfuscation, start, enc.end()))
             continue
@@ -99,31 +107,31 @@
         return b64[:-1]  # Corrupted end, just keep the valid part
     elif padding:
         return b64 + b'='*padding
     else:
         return b64
 
 
-def get_cmd_command(cmd: bytes):
+def get_cmd_command(cmd: bytes) -> bytes:
     # Find end of argument string
-    lcmd = cmd.lower()
-    arg_end = len(cmd)
-    c = lcmd.find(b'/c')
-    if c > 0:
-        arg_end = min(arg_end, c+2)
-    k = lcmd.find(b'/k')
-    if k > 0:
-        arg_end = min(arg_end, k+2)
-    amp = lcmd.find(b'&')
-    if amp > 0:
-        arg_end = min(arg_end, amp+1)
+    end = re.search(rb'(?i)&|/(c|k|r)', cmd)
+    if end is None:
+        return b''
+    arg = cmd[end.end():].strip()
+    if end.group() != b'"' and arg.startswith(b'"'):
+        # strip leading and final quote
+        index = arg.rfind(b'"')
+        if index > 0:
+            arg = arg[1:index] + arg[index+1:]
+        else:
+            arg = arg[1:]
 
     # return everything after the arguments
-    return cmd[arg_end:]
+    return arg
 
 
-def get_powershell_command(powershell: bytes):
+def get_powershell_command(powershell: bytes) -> bytes:
     match = re.match(POWERSHELL_ARGS_RE, powershell)
     if match:
         return powershell[match.end():]
     else:
         return powershell
```

### Comparing `multidecoder-0.0.9/multidecoder/analyzers/vba.py` & `multidecoder-0.1.0/multidecoder/analyzers/vba.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 
 import regex as re
 
-from multidecoder.hit import Hit
+from multidecoder.analyzers.concat import STRING_RE
+from multidecoder.hit import Hit, find_and_deobfuscate
 from multidecoder.registry import analyzer
 
 CREATE_OBJECT_RE = rb'(?i)createobject\('
+STRREVERSE_RE = rb'(?i)StrReverse\(\s*(' + STRING_RE + rb')\s*\)'
 
 OPEN_TO_CLOSE_MAP = {
     ord('('): ord(')'),
     ord('{'): ord('}'),
     ord('['): ord(']'),
     ord('<'): ord('>')
 }
@@ -35,7 +37,12 @@
 def find_createobject(data: bytes) -> list[Hit]:
     out = []
     for match in re.finditer(CREATE_OBJECT_RE, data):
         index = get_closing_brace(data, match.end())
         if index > 0:
             out.append(Hit(data[match.start():index], '', match.start(), index))
     return out
+
+
+@analyzer('vba.string')
+def find_strreverse(data: bytes) -> list[Hit]:
+    return find_and_deobfuscate(STRREVERSE_RE, data, lambda s: (s[-2:0:-1], 'vba.reverse'), 1)
```

### Comparing `multidecoder-0.0.9/multidecoder/analyzers/xml.py` & `multidecoder-0.1.0/multidecoder/analyzers/xml.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/domains.py` & `multidecoder-0.1.0/multidecoder/domains.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/hit.py` & `multidecoder-0.1.0/multidecoder/hit.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,11 +14,12 @@
 def regex_hits(regex: bytes, data: bytes, group: int = 0) -> list[Hit]:
     return [match_to_hit(match, group) for match in re.finditer(regex, data)]
 
 
 def find_and_deobfuscate(regex: bytes,
                          data: bytes,
                          deobfuscation: Callable[[bytes], tuple[bytes, str]],
-                         group: int = 0) -> list[Hit]:
+                         deob_group: int = 0,
+                         context_group: int = 0) -> list[Hit]:
     return [
-        Hit(*deobfuscation(match.group(group)), *match.span(group)) for match in re.finditer(regex, data)
+        Hit(*deobfuscation(match.group(deob_group)), *match.span(context_group)) for match in re.finditer(regex, data)
     ]
```

### Comparing `multidecoder-0.0.9/multidecoder/json_conversion.py` & `multidecoder-0.1.0/multidecoder/json_conversion.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keyword.py` & `multidecoder-0.1.0/multidecoder/keyword.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.advapi32` & `multidecoder-0.1.0/multidecoder/keywords/api/api.advapi32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.atl` & `multidecoder-0.1.0/multidecoder/keywords/api/api.atl`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.dbghelp` & `multidecoder-0.1.0/multidecoder/keywords/api/api.dbghelp`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.gdi32` & `multidecoder-0.1.0/multidecoder/keywords/api/api.gdi32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.imagehlp` & `multidecoder-0.1.0/multidecoder/keywords/api/api.imagehlp`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.iphlpapi` & `multidecoder-0.1.0/multidecoder/keywords/api/api.iphlpapi`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.kernel32` & `multidecoder-0.1.0/multidecoder/keywords/api/api.kernel32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.libeay32` & `multidecoder-0.1.0/multidecoder/keywords/api/api.libeay32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.mfc42` & `multidecoder-0.1.0/multidecoder/keywords/api/api.mfc42`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.msi` & `multidecoder-0.1.0/multidecoder/keywords/api/api.msi`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.mssign32` & `multidecoder-0.1.0/multidecoder/keywords/api/api.mssign32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.msvbvm60` & `multidecoder-0.1.0/multidecoder/keywords/api/api.msvbvm60`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.msvcrt` & `multidecoder-0.1.0/multidecoder/keywords/api/api.msvcrt`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.nddeapi` & `multidecoder-0.1.0/multidecoder/keywords/api/api.nddeapi`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.netapi32` & `multidecoder-0.1.0/multidecoder/keywords/api/api.netapi32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.ntdll` & `multidecoder-0.1.0/multidecoder/keywords/api/api.ntdll`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.ntoskrnl` & `multidecoder-0.1.0/multidecoder/keywords/api/api.ntoskrnl`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.odbc32` & `multidecoder-0.1.0/multidecoder/keywords/api/api.odbc32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.odbccp32` & `multidecoder-0.1.0/multidecoder/keywords/api/api.odbccp32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.ole32` & `multidecoder-0.1.0/multidecoder/keywords/api/api.ole32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.oleaut32` & `multidecoder-0.1.0/multidecoder/keywords/api/api.oleaut32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.packet` & `multidecoder-0.1.0/multidecoder/keywords/api/api.packet`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.powrprof` & `multidecoder-0.1.0/multidecoder/keywords/api/api.powrprof`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.rpcrt4` & `multidecoder-0.1.0/multidecoder/keywords/api/api.rpcrt4`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.scecli` & `multidecoder-0.1.0/multidecoder/keywords/api/api.scecli`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.se` & `multidecoder-0.1.0/multidecoder/keywords/api/api.se`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.shell32` & `multidecoder-0.1.0/multidecoder/keywords/api/api.shell32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.shlwapi` & `multidecoder-0.1.0/multidecoder/keywords/api/api.shlwapi`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.ssleay32` & `multidecoder-0.1.0/multidecoder/keywords/api/api.ssleay32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.urlmon` & `multidecoder-0.1.0/multidecoder/keywords/api/api.urlmon`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.user32` & `multidecoder-0.1.0/multidecoder/keywords/api/api.user32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.wininet` & `multidecoder-0.1.0/multidecoder/keywords/api/api.wininet`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.winsock` & `multidecoder-0.1.0/multidecoder/keywords/api/api.winsock`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.winsta` & `multidecoder-0.1.0/multidecoder/keywords/api/api.winsta`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/api/api.wsnmp32` & `multidecoder-0.1.0/multidecoder/keywords/api/api.wsnmp32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/event` & `multidecoder-0.1.0/multidecoder/keywords/event`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/guid` & `multidecoder-0.1.0/multidecoder/keywords/guid`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/key` & `multidecoder-0.1.0/multidecoder/keywords/key`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/network.string` & `multidecoder-0.1.0/multidecoder/keywords/network.string`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/oid` & `multidecoder-0.1.0/multidecoder/keywords/oid`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/os_name` & `multidecoder-0.1.0/multidecoder/keywords/os_name`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/powershell.cmdlet` & `multidecoder-0.1.0/multidecoder/keywords/powershell.cmdlet`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/privilege` & `multidecoder-0.1.0/multidecoder/keywords/privilege`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/ransomware.string` & `multidecoder-0.1.0/multidecoder/keywords/ransomware.string`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/security_identifier` & `multidecoder-0.1.0/multidecoder/keywords/security_identifier`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/keywords/windows.registry` & `multidecoder-0.1.0/multidecoder/keywords/windows.registry`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 \Device\KeyboardClass0
 Software\Skype\Phone
 \registry\machine\system\CurrentControlSet\Services\Tcpip\Parameters\Interfaces\
-Software\Microsoft
+SOFTWARE\Microsoft
 System\WPA\
 HARDWARE\DEVICEMAP\SERIALCOMM
 HARDWARE\DEVICEMAP\PARALLEL PORTS
 Software\Microsoft\Windows\CurrentVersion\Run
 .DEFAULT\Software\Microsoft\Windows\CurrentVersion\RunServices
 .DEFAULT\Software\Microsoft\Windows\CurrentVersion\Runonce
 .DEFAULT\Software\Microsoft\Windows\CurrentVersion\Run
```

### Comparing `multidecoder-0.0.9/multidecoder/keywords_to_review.txt` & `multidecoder-0.1.0/multidecoder/keywords_to_review.txt`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/multidecoder.py` & `multidecoder-0.1.0/multidecoder/multidecoder.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder/query.py` & `multidecoder-0.1.0/multidecoder/query.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from collections import Counter
 from typing import Any, Optional
 
 
 class Node():
     def __init__(self,
                  type: str,
                  value: bytes,
@@ -42,7 +43,31 @@
     return '/'.join(label_list[::-1]) + ' ' + repr(value)[2:-1]
 
 
 def string_summary(tree: list[dict[str, Any]]) -> list[str]:
     return [
         make_label(node) for node in invert_tree(tree)
     ]
+
+
+def squash_replace(data: bytes, tree: list[dict[str, Any]]) -> bytes:
+    offset = 0
+    output = []
+    for node in tree:
+        node_data = squash_replace(node['value'], node['children'])
+        if node_data != data[node['start']:node['end']]:
+            output.append(data[offset:node['start']])
+            if node['type'].endswith('string'):
+                node_data = b'"' + node_data + b'"'
+            output.append(node_data)
+            offset = node['end']
+    output.append(data[offset:])
+    return b''.join(output)
+
+
+def obfuscation_counts(tree: list[dict[str, Any]]) -> Counter[str]:
+    counts: Counter[str] = Counter()
+    for node in tree:
+        if node['obfuscation']:
+            counts.update(node['obfuscation'].split('/>'))
+        counts.update(obfuscation_counts(node['children']))
+    return counts
```

### Comparing `multidecoder-0.0.9/multidecoder/registry.py` & `multidecoder-0.1.0/multidecoder/registry.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/multidecoder.egg-info/PKG-INFO` & `multidecoder-0.1.0/multidecoder.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: multidecoder
-Version: 0.0.9
+Version: 0.1.0
 Summary: A context preserving IOC extraction library
 Home-page: https://github.com/CybercentreCanada/Multidecoder
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CybercentreCanada/Multidecoder/issues
 Keywords: malware,analysis,gc,canada,cse-cst,cse,cst,cyber,cccs
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
@@ -33,19 +32,29 @@
 - base64 encoding
 - hexadecimal encoding
 - string concatenation
 - powershell escape characters
 
 ## Installing
 
-The latest Multidecoder can be installed from the repository:
+Multidecoder can be installed from pypi using pip:
+```
+pip install -U multidecoder
+```
+
+Alternatly, it can also be installed from the repository:
 ```
 pip install -U https://github.com/CybercentreCanada/Multidecoder/archive/main.zip
 ```
 
+To test the latest development version, install from the dev branch:
+```
+pip install -U https://github.com/CybercenterCanada/Multidecoder/archive/dev.zip
+```
+
 ## Command Line
 
 After being installed Multidecoder can be run on a file from the command-line
 ```
 > multidecoder file
 ```
 which will output a list of indicators found.
@@ -64,9 +73,7 @@
 which can scan data to give a dictionary tree similar to the command-line json output.
 ```
 from multidecoder.multidecoder import Multidecoder
 
 md = Multidecoder()
 context_tree = md.scan(data)
 ```
-
-
```

### Comparing `multidecoder-0.0.9/multidecoder.egg-info/SOURCES.txt` & `multidecoder-0.1.0/multidecoder.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,21 +22,24 @@
 multidecoder.egg-info/dependency_links.txt
 multidecoder.egg-info/entry_points.txt
 multidecoder.egg-info/not-zip-safe
 multidecoder.egg-info/requires.txt
 multidecoder.egg-info/top_level.txt
 multidecoder/analyzers/__init__.py
 multidecoder/analyzers/base64.py
+multidecoder/analyzers/chr.py
 multidecoder/analyzers/concat.py
 multidecoder/analyzers/encoding.py
 multidecoder/analyzers/filename.py
 multidecoder/analyzers/hex.py
+multidecoder/analyzers/javascript.py
 multidecoder/analyzers/network.py
 multidecoder/analyzers/path.py
 multidecoder/analyzers/pe_file.py
+multidecoder/analyzers/replace.py
 multidecoder/analyzers/shell.py
 multidecoder/analyzers/vba.py
 multidecoder/analyzers/xml.py
 multidecoder/keywords/archive
 multidecoder/keywords/av.name
 multidecoder/keywords/cryptography
 multidecoder/keywords/debugger.device.name
@@ -163,17 +166,20 @@
 multidecoder/keywords/api/api.wship6
 multidecoder/keywords/api/api.wsnmp32
 multidecoder/keywords/api/api.wtsapi32
 pipelines/publish.yaml
 tests/__init__.py
 tests/test_multidecoder.py
 tests/test_analyzers/test_base64.py
+tests/test_analyzers/test_chr.py
 tests/test_analyzers/test_concat.py
 tests/test_analyzers/test_encoding.py
 tests/test_analyzers/test_filename.py
 tests/test_analyzers/test_hex.py
+tests/test_analyzers/test_javascript.py
 tests/test_analyzers/test_network.py
 tests/test_analyzers/test_path.py
 tests/test_analyzers/test_pe_file.py
+tests/test_analyzers/test_replace.py
 tests/test_analyzers/test_shell.py
 tests/test_analyzers/test_vba.py
 tests/test_analyzers/test_xml.py
```

### Comparing `multidecoder-0.0.9/pipelines/publish.yaml` & `multidecoder-0.1.0/pipelines/publish.yaml`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/setup.cfg` & `multidecoder-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/tests/test_analyzers/test_base64.py` & `multidecoder-0.1.0/tests/test_analyzers/test_base64.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import binascii
 import regex as re
 
-from multidecoder.analyzers.base64 import find_base64, BASE64_RE
+from multidecoder.analyzers.base64 import find_FromBase64String, find_base64, BASE64_RE
+from multidecoder.hit import Hit
 
 
 def test_empty():
     assert find_base64(b'') == []
 
 
 def test_hex():
@@ -37,7 +38,27 @@
 }
 
 
 def test_base64_search_texts():
     for data, expected in TEST_STRINGS.items():
         response = find_base64(data)
         assert response == expected, f'{data} Failed'
+
+
+# -- FromBase64String --
+
+def test_fromb64string_no_xor():
+    test = b"FromBase64String('ZHVjaw==')"
+    test2 = b"[System.Convert]::FromBase64String('ZHVjaw==')"
+    assert find_FromBase64String(test) == [
+        Hit(value=b'duck', obfuscation='decode.base64', start=0, end=len(test))
+    ]
+    assert find_FromBase64String(test2) == [
+        Hit(value=b'duck', obfuscation='decode.base64', start=0, end=len(test2))
+    ]
+
+
+def test_fromb64string_xor():
+    test = b"FromBase64String('R1ZASA==')\n-bxor 35"
+    assert find_FromBase64String(test) == [
+        Hit(value=b'duck', obfuscation='decode.base64/>xor35', start=0, end=test.find(b'\n'))
+    ]
```

### Comparing `multidecoder-0.0.9/tests/test_analyzers/test_concat.py` & `multidecoder-0.1.0/tests/test_analyzers/test_concat.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -56,8 +56,8 @@
 def test_concat_mixed_multiple():
     test = b'"double" & \'single\' & "double" & \'single\''
     assert find_concat(test) == [Hit(b'doublesingledoublesingle', 'concatenation', 0, len(test))]
 
 
 def test_concat_xml():
     test = b'<t>"a"&amp;"pp"&amp;"lesauce"&amp;" is "&amp;"a"&amp;" del"&amp;"icio"&amp;"us foo"&amp;"d","</t>'
-    assert find_concat(test) == [Hit(b'applesauce is a delicious food', 'concatenation', 3, len(test)-6)]
+    assert find_concat(test) == [Hit(b'applesauce is a delicious food', 'concatenation', 3, len(test)-6)]
```

### Comparing `multidecoder-0.0.9/tests/test_analyzers/test_encoding.py` & `multidecoder-0.1.0/tests/test_analyzers/test_encoding.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/tests/test_analyzers/test_network.py` & `multidecoder-0.1.0/tests/test_analyzers/test_network.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/tests/test_analyzers/test_path.py` & `multidecoder-0.1.0/tests/test_analyzers/test_path.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/tests/test_analyzers/test_shell.py` & `multidecoder-0.1.0/tests/test_analyzers/test_shell.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 import regex as re
-
-from multidecoder.analyzers.shell import CMD_RE
-from multidecoder.analyzers.shell import find_cmd_strings, find_powershell_strings
-from multidecoder.analyzers.shell import get_cmd_command, get_powershell_command, strip_carets
+from multidecoder.analyzers.shell import (
+    CMD_RE,
+    find_cmd_strings,
+    find_powershell_strings,
+    get_cmd_command,
+    get_powershell_command,
+    strip_carets,
+)
 from multidecoder.hit import Hit
 
 test = b'SET.NAME(a , cmd /c m^sh^t^a h^tt^p^:/^/some.url/x.html)'
 
 
 # CMD_RE
 def test_cmd_re_empty():
     assert not re.search(CMD_RE, b'')
 
 
 def test_cmd_re_command():
-    assert re.match(CMD_RE, b'cmd command')
+    assert re.match(CMD_RE, b'cmd arguments')
 
 
 def test_cmd_re_mixed_case():
-    assert re.match(CMD_RE, b'CmD CoMMaNd')
+    assert re.match(CMD_RE, b'CmD ArgUmenTs')
 
 
 def test_cmd_re_carets():
     assert re.match(CMD_RE, b'c^m^d c^omman^d')
 
 
 def test_cmd_re_quotes():
     assert re.match(CMD_RE, b'cmd /c ""echo bee""')
 
 
+def test_cmd_re_null():
+    match = re.match(CMD_RE, b'cmd.exe\x00somethingelse')
+    assert match
+    assert match.span() == (0, 7)
+
+
 def test_cmd_re_ex1():
     match = re.search(CMD_RE, test)
     assert match and test[match.start(): match.end()] == b'cmd /c m^sh^t^a h^tt^p^:/^/some.url/x.html'
 
 
 # strip_carets
 def test_strip_carets_empty():
@@ -83,14 +93,23 @@
     assert find_powershell_strings(ex) == [
         Hit(value=b'powershell -Command echo bee',
             obfuscation='unescape.shell.carets/>powershell.base64',
             start=0,
             end=len(ex))
     ]
 
+def test_find_powershell_strings_enc_with_quotes():
+    ex = b'powershell /e "ZQBjAGgAbwAgAGIAZQBlAA=="'
+    assert find_powershell_strings(ex) == [
+        Hit(value=b'powershell -Command echo bee',
+            obfuscation='powershell.base64',
+            start=0,
+            end=len(ex))
+    ]
+
 
 def test_find_powershell_for_loop():
     ex = b"for /f \"tokens=*\" %%a in ('powershell -Command \"hostname " \
          b"| %%{$_ -replace '[^a-zA-Z0-9]+', '_'}\"') do echo prx.%%a"
     assert find_powershell_strings(ex) == [
         Hit(value=b"powershell -Command \"hostname | %%{$_ -replace '[^a-zA-Z0-9]+', '_'}\"",
             obfuscation='',
@@ -120,28 +139,45 @@
 
 
 def test_get_cmd_command_k():
     assert get_cmd_command(b'cmd/kcommand') == b'command'
     assert get_cmd_command(b'cmd.exe/kcommand') == b'command'
 
 
+def test_get_cmd_command_r():
+    assert get_cmd_command(b'cmd/rcommand') == b'command'
+    assert get_cmd_command(b'cmd.exe/rcommand') == b'command'
+
+
 def test_get_cmd_command_amp():
     assert get_cmd_command(b'cmd&command&command2&command3') == b'command&command2&command3'
 
 
 def test_get_cmd_command_upper():
     assert get_cmd_command(b'CMD/CCOMMAND') == b'COMMAND'
     assert get_cmd_command(b'CMD/KCOMMAND') == b'COMMAND'
 
 
 def test_get_cmd_command_nested():
-    assert get_cmd_command(b'cmd /c cmd /c command') == b' cmd /c command'
-    assert get_cmd_command(b'cmd /c cmd /k command') == b' cmd /k command'
-    assert get_cmd_command(b'cmd /k cmd /c command') == b' cmd /c command'
-    assert get_cmd_command(b'cmd /k cmd /k command') == b' cmd /k command'
+    assert get_cmd_command(b'cmd /c cmd /c command') == b'cmd /c command'
+    assert get_cmd_command(b'cmd /c cmd /k command') == b'cmd /k command'
+    assert get_cmd_command(b'cmd /k cmd /c command') == b'cmd /c command'
+    assert get_cmd_command(b'cmd /k cmd /k command') == b'cmd /k command'
+
+
+def test_get_cmd_command_strip_quotes():
+    assert get_cmd_command(b'cmd /c   "command"') == b'command'
+
+
+def test_get_cmd_command_last_quote_only():
+    assert get_cmd_command(b'cmd /c "comm"an"d') == b'comm"and'
+
+
+def test_get_cmd_command_strip_only_if_first_quote():
+    assert get_cmd_command(b'cmd /c command"') == b'command"'
 
 
 # get_powershell_command
 def test_get_powershell_command_empty():
     assert get_powershell_command(b'') == b''
```

### Comparing `multidecoder-0.0.9/tests/test_analyzers/test_xml.py` & `multidecoder-0.1.0/tests/test_analyzers/test_xml.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.9/tests/test_multidecoder.py` & `multidecoder-0.1.0/tests/test_multidecoder.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,24 +9,29 @@
 
 
 def test_scan_empty(md):
     assert md.scan(b'') == []
 
 
 def test_analyze_data_url(md):
-    assert md.scan(b'https://some.domain.com') == [
-        {
+    assert md.scan(b'https://some.domain.com') == [{
+        'obfuscation': '',
+        'type': 'network.url',
+        'value': b'https://some.domain.com/',
+        'start': 0,
+        'end': 23,
+        'children': [{
             'obfuscation': '',
-            'type': 'network.url',
-            'value': b'https://some.domain.com/',
-            'start': 0,
+            'type': 'network.domain',
+            'value': b'some.domain.com',
+            'start': 8,
             'end': 23,
             'children': []
-        }
-    ]
+        }]
+    }]
 
 
 def test_scan_no_overlap(md):
     assert md.scan(b'google.com, amazon.com, 8.8.8.8') == [
         {
             'obfuscation': '',
             'type': 'network.domain',
```

