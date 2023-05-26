# Comparing `tmp/dwiqc-0.2.1-py2.py3-none-any.whl.zip` & `tmp/dwiqc-0.2.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 22654 bytes, number of entries: 21
+Zip file size: 22458 bytes, number of entries: 21
 -rw-r--r--  2.0 unx      225 b- defN 23-May-19 16:11 dwiqc/__init__.py
--rw-r--r--  2.0 unx      247 b- defN 23-May-26 11:38 dwiqc/__version__.py
+-rw-r--r--  2.0 unx      247 b- defN 23-May-26 13:38 dwiqc/__version__.py
 -rw-r--r--  2.0 unx      283 b- defN 23-May-25 14:54 dwiqc/browser/__init__.py
 -rw-r--r--  2.0 unx       62 b- defN 23-May-19 16:11 dwiqc/cli/__init__.py
 -rw-r--r--  2.0 unx     6651 b- defN 23-May-25 14:45 dwiqc/cli/get.py
--rw-r--r--  2.0 unx     5805 b- defN 23-May-25 14:56 dwiqc/cli/process.py
+-rw-r--r--  2.0 unx     5731 b- defN 23-May-26 13:28 dwiqc/cli/process.py
 -rw-r--r--  2.0 unx      160 b- defN 23-May-19 16:11 dwiqc/config/__init__.py
 -rw-r--r--  2.0 unx      274 b- defN 23-May-19 16:11 dwiqc/config/dwiqc.yaml
 -rw-r--r--  2.0 unx       98 b- defN 23-May-19 16:11 dwiqc/state/__init__.py
 -rw-r--r--  2.0 unx     1892 b- defN 23-May-19 16:11 dwiqc/tasks/__init__.py
 -rw-r--r--  2.0 unx     8664 b- defN 23-May-23 14:22 dwiqc/tasks/prequal.py
 -rw-r--r--  2.0 unx     4209 b- defN 23-May-22 17:12 dwiqc/tasks/prequal_EQ.py
--rw-r--r--  2.0 unx     6193 b- defN 23-May-23 11:24 dwiqc/tasks/qsiprep.py
+-rw-r--r--  2.0 unx     6064 b- defN 23-May-26 13:26 dwiqc/tasks/qsiprep.py
 -rw-r--r--  2.0 unx     3782 b- defN 23-May-19 16:11 dwiqc/tasks/qsiprep_EQ.py
 -rw-r--r--  2.0 unx    16212 b- defN 23-May-26 11:38 dwiqc/xnat/__init__.py
--rwxr-xr-x  2.0 unx     3889 b- defN 23-May-26 11:42 dwiqc-0.2.1.data/scripts/dwiQC.py
--rw-r--r--  2.0 unx     1541 b- defN 23-May-26 11:42 dwiqc-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      457 b- defN 23-May-26 11:42 dwiqc-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-26 11:42 dwiqc-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-May-26 11:42 dwiqc-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1640 b- defN 23-May-26 11:42 dwiqc-0.2.1.dist-info/RECORD
-21 files, 62400 bytes uncompressed, 20016 bytes compressed:  67.9%
+-rwxr-xr-x  2.0 unx     3889 b- defN 23-May-26 13:39 dwiqc-0.2.2.data/scripts/dwiQC.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-May-26 13:39 dwiqc-0.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      432 b- defN 23-May-26 13:39 dwiqc-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-26 13:39 dwiqc-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-May-26 13:39 dwiqc-0.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1640 b- defN 23-May-26 13:39 dwiqc-0.2.2.dist-info/RECORD
+21 files, 62172 bytes uncompressed, 19820 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -39,26 +39,26 @@
 
 Filename: dwiqc/tasks/qsiprep_EQ.py
 Comment: 
 
 Filename: dwiqc/xnat/__init__.py
 Comment: 
 
-Filename: dwiqc-0.2.1.data/scripts/dwiQC.py
+Filename: dwiqc-0.2.2.data/scripts/dwiQC.py
 Comment: 
 
-Filename: dwiqc-0.2.1.dist-info/LICENSE
+Filename: dwiqc-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: dwiqc-0.2.1.dist-info/METADATA
+Filename: dwiqc-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: dwiqc-0.2.1.dist-info/WHEEL
+Filename: dwiqc-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: dwiqc-0.2.1.dist-info/top_level.txt
+Filename: dwiqc-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: dwiqc-0.2.1.dist-info/RECORD
+Filename: dwiqc-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dwiqc/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'dwiqc'
 __description__ = 'Quality Assurance Pipeline for Diffusion MR Data'
 __url__ = 'https://github.com/harvard-nrg/dwiqc'
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## dwiqc/cli/process.py

```diff
@@ -16,19 +16,14 @@
 from executors.models import Job, JobArray
 from bids import BIDSLayout
 from dwiqc.xnat import Report
 import dwiqc.tasks.prequal as prequal
 import dwiqc.tasks.qsiprep as qsiprep
 import dwiqc.tasks.prequal_EQ as prequal_EQ
 import dwiqc.tasks.qsiprep_EQ as qsiprep_EQ
-import dwiqc.broswer as browser
-sys.path.insert(0, os.path.join(os.environ['MODULESHOME'], "init"))
-from env_modules_python import module
-
-module('load', 'chromium.org/chromium/102.0.5005.115-ncf')
 
 
 logger = logging.getLogger(__name__)
 
 def do(args):
     if args.insecure:
         logger.warning('disabling ssl certificate verification')
@@ -80,23 +75,22 @@
         logger.info(json.dumps(prequal_task.command, indent=1))
         jarray.add(prequal_task.job)
 
     # qsiprep job
     qsiprep_outdir = None
     if 'qsiprep' in args.sub_tasks:
         qsiprep_outdir = os.path.join(args.bids_dir, 'derivatives', 'dwiqc-qsiprep', f'sub-{args.sub}', f'ses-{args.ses}', basename, 'qsiprep_output')
-        qsiprep_trick = tempfile.TemporaryDirectory(dir='/n/holyscratch01/LABS/nrg/Lab', suffix='.qsiprep')
-        os.makedirs(qsiprep_outdir, exist_ok=True)
-        os.symlink(qsiprep_outdir, f"{qsiprep_trick.name}/q")
+        qsiprep_trick = tempfile.TemporaryDirectory(dir='/tmp', suffix='.qsiprep')
+        #os.symlink(qsiprep_outdir, f"{qsiprep_trick}/q")
         qsiprep_task = qsiprep.Task(
             sub=args.sub,
             ses=args.ses,
             run=args.run,
             bids=args.bids_dir,
-            outdir=f"{qsiprep_trick.name}/q",
+            outdir=qsiprep_outdir,
             tempdir=tempfile.gettempdir(),
             pipenv='/sw/apps/qsiprep'
         )
         os.environ['OPENBLAS_NUM_THREADS'] = '1'
         logger.info(json.dumps(qsiprep_task.command, indent=1))
         #check_for_output(args, qsiprep_outdir)
         jarray.add(qsiprep_task.job)
@@ -108,15 +102,14 @@
         logger.info('waiting for all jobs to finish')
         jarray.wait()
         numjobs = len(jarray.array)
         failed = len(jarray.failed)
         complete = len(jarray.complete)
         prequal_eddy(args, prequal_outdir)
         qsiprep_eddy(args, qsiprep_outdir)
-        browser.snapshot(f"{qsiprep_outdir}/qsiprep/sub-{args.sub}.html", f"{qsiprep_outdir}/qsiprep/qsiprep.pdf") 
         if failed:
             logger.info('%s/%s jobs failed', failed, numjobs)
             for pid,job in iter(jarray.failed.items()):
                 logger.error('%s exited with returncode %s', job.name, job.returncode)
                 with open(job.output, 'r') as fp:
                     logger.error('standard output\n%s', fp.read())
                 with open(job.error, 'r') as fp:
@@ -136,14 +129,23 @@
 
 
     # build data to upload to xnat
     R = Report(args.bids_dir, args.sub, args.ses, args.run)
     logger.info('building xnat artifacts to %s', args.artifacts_dir)
     R.build_assessment(args.artifacts_dir)
 
+    # upload data to xnat over rest api
+    if args.xnat_upload:
+        logger.info('Uploading artifacts to XNAT')
+        #auth = yaxil.auth2(args.xnat_alias)
+        yaxil.CHECK_CERTIFICATE=False
+        auth = yaxil.auth2('ssbc_stage')
+        yaxil.storerest(auth, args.artifacts_dir, 'dwiqc-resource')
+
+
 
 
 def prequal_eddy(args, prequal_outdir):
     if 'prequal' in args.sub_tasks:
         eq_task = prequal_EQ.Task(
             sub=args.sub,
             ses=args.ses,
@@ -162,17 +164,15 @@
             ses=args.ses,
             run=args.run,
             bids=args.bids_dir,
             outdir=qsiprep_outdir,
             tempdir=tempfile.gettempdir(),
         )
 
-        eq_task.build()   
+        eq_task.build()
 
+def copy_qsiprep_output(args, qsiprep_outdir):
+    final_qsiprep_outdir = os.path.join(args.bids_dir, 'derivatives', 'dwiqc-qsiprep', f'sub-{args.sub}', f'ses-{args.ses}', basename, 'qsiprep_output')
+    shutil.copytree(qsiprep_outdir, final_qsiprep_outdir)
 
 
-#    # upload data to xnat over rest api
-#    if args.xnat_upload:
-#        logger.info('Uploading artifacts to XNAT')
-#        auth = yaxil.auth2(args.xnat_alias)
-#        yaxil.storerest(auth, args.artifacts_dir, 'anatqc-resource')
```

## dwiqc/tasks/qsiprep.py

```diff
@@ -199,21 +199,20 @@
 		with open(f"{self._bids}/eddy_params_s2v_mbs.json", "w") as f:
 			json.dump(params_file, f)
 
 	# create qsiprep command to be executed
 
 	def build(self):
 		self.create_eddy_params()
-		self.create_nipype()
+		#self.create_nipype()
 		self.check_output_resolution()
 		self._command = [
 			'selfie',
 			'--lock',
 			'--output-file', self._prov,
-			#'qsiprep',
 			'singularity',
 			'run',
 			'--nv',
 			'/n/sw/ncf/apps/qsiprep/0.14.0/qsiprep.sif',			
 			self._bids,
 			self._outdir,
 			'participant',
@@ -230,24 +229,15 @@
 			'--n_cpus',
 			'2',
 			'--mem_mb',
 			'40000',
 			'--fs-license-file',
 			'/n/helmod/apps/centos7/Core/freesurfer/6.0.0-fasrc01/license.txt',
 			'-w',
-			self._tempdir#,
-			#'&&',
-			#'cp',
-			#'-r',
-			#self._tempdir,
-			#self._bids,
-			#'&&',
-			#'rm',
-			#'-r',
-			#self._tempdir
+			self._tempdir
 		]
 
 		logdir = self.logdir()
 		logfile = os.path.join(logdir, 'dwiqc-qsiprep.log')
 		self.job = Job(
 			name='dwiqc-qsiprep',
 			time='2000',
```

## Comparing `dwiqc-0.2.1.data/scripts/dwiQC.py` & `dwiqc-0.2.2.data/scripts/dwiQC.py`

 * *Files identical despite different names*

## Comparing `dwiqc-0.2.1.dist-info/LICENSE` & `dwiqc-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dwiqc-0.2.1.dist-info/RECORD` & `dwiqc-0.2.2.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 dwiqc/__init__.py,sha256=MZJhUZKhHHoZ2w_GeoFCITk1m_0ASdRw_ZaeDixFEPU,225
-dwiqc/__version__.py,sha256=Sgnrt606IOFHQvDt3B-tbrw3bBwq7FFpW8OP__0X9LE,247
+dwiqc/__version__.py,sha256=JG0S942mJGhbQCQIJBp9bR8VWELpRCcBPOGM97kE3SY,247
 dwiqc/browser/__init__.py,sha256=MlUOz0v7bA_dtQyXX27WF0dzyGGo4xkEEt2PT2B0_aQ,283
 dwiqc/cli/__init__.py,sha256=zGIm7lrjh3wA191D-VjQBZNjSlspFUx148VwDNQGaTk,62
 dwiqc/cli/get.py,sha256=6ixaBdwEgY_GXh8L-_3QDY4MEsNqSJgXle_mxW99mlk,6651
-dwiqc/cli/process.py,sha256=bRZ4tOIyJM3xLB1XVN5035YdkQRma_1NcZ4nDIxzZMs,5805
+dwiqc/cli/process.py,sha256=WlCWyY-zd3lnOwbgeZ6wPPGNv5ZAetn_X4Id2QieEJs,5731
 dwiqc/config/__init__.py,sha256=k_w5JzoJN_7R7eI_sIJxHA4FQQHs0_KGf-6jsbG4Xs8,160
 dwiqc/config/dwiqc.yaml,sha256=x8gKMFZyChdzvNX3GthRe0eWvyKDDL5itXo0kLWVfd0,274
 dwiqc/state/__init__.py,sha256=NaRifw26bI3F1J9BqeLa-KLSzEPq2m_UNhMbXdmPdh4,98
 dwiqc/tasks/__init__.py,sha256=LnlN7iYjpqiBic2ihFrM-_h7m8FD_N7Beh7UIwKyGZ8,1892
 dwiqc/tasks/prequal.py,sha256=GagoXzYhHaWV2uEfcadsc-85ij71hxP3YnZDANMO2UY,8664
 dwiqc/tasks/prequal_EQ.py,sha256=PWmlo8u_D5qM1lyXdmT7iq865JL6xoPM0JHGEwzRnes,4209
-dwiqc/tasks/qsiprep.py,sha256=2HAmLSSXyKRUuYmok9EEmoPaSo8_7LoCAU-JGfudeiY,6193
+dwiqc/tasks/qsiprep.py,sha256=h4xFJ3dPYPCkelHAtrpGZx47P938dQDOmSeT5JEC__0,6064
 dwiqc/tasks/qsiprep_EQ.py,sha256=JWildptHsuyJVj7ZYMFlWWYvsAIszJpWk1a0m05JM-Q,3782
 dwiqc/xnat/__init__.py,sha256=4-tJIvDSzSiek-aNwRwvKTQ19_xhEwsF-7ty9czWwec,16212
-dwiqc-0.2.1.data/scripts/dwiQC.py,sha256=D6ZRhtwJAl0gYODeWhrT4fl7tZtnul0iXrMRyrHxIfE,3889
-dwiqc-0.2.1.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-dwiqc-0.2.1.dist-info/METADATA,sha256=NUBxWlJeEXYsyAnhAmYA9ZDDJJHkcx21VlKIe6TXYqc,457
-dwiqc-0.2.1.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-dwiqc-0.2.1.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
-dwiqc-0.2.1.dist-info/RECORD,,
+dwiqc-0.2.2.data/scripts/dwiQC.py,sha256=D6ZRhtwJAl0gYODeWhrT4fl7tZtnul0iXrMRyrHxIfE,3889
+dwiqc-0.2.2.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+dwiqc-0.2.2.dist-info/METADATA,sha256=0u518gvez7WYjpQV8nqj2Kok481T8p3De0wlHECj2lI,432
+dwiqc-0.2.2.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+dwiqc-0.2.2.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
+dwiqc-0.2.2.dist-info/RECORD,,
```

