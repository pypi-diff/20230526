# Comparing `tmp/aegea-4.4.0.tar.gz` & `tmp/aegea-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aegea-4.4.0.tar", last modified: Sat Apr 22 02:28:03 2023, max compression
+gzip compressed data, was "aegea-4.4.1.tar", last modified: Fri May 26 02:41:50 2023, max compression
```

## Comparing `aegea-4.4.0.tar` & `aegea-4.4.1.tar`

### file list

```diff
@@ -1,301 +1,301 @@
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.206467 aegea-4.4.0/
--rw-r--r--   0 kislyuk    (501) staff       (20)       44 2022-07-01 05:40:57.000000 aegea-4.4.0/.coveragerc
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.160079 aegea-4.4.0/.github/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.173805 aegea-4.4.0/.github/workflows/
--rw-r--r--   0 kislyuk    (501) staff       (20)     1251 2023-03-27 05:42:23.000000 aegea-4.4.0/.github/workflows/ci.yml
--rw-r--r--   0 kislyuk    (501) staff       (20)      518 2022-07-01 05:40:57.000000 aegea-4.4.0/.gitignore
--rw-r--r--   0 kislyuk    (501) staff       (20)    36433 2023-04-22 02:27:44.000000 aegea-4.4.0/Changes.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)    11357 2016-06-14 14:20:08.000000 aegea-4.4.0/LICENSE.md
--rw-r--r--   0 kislyuk    (501) staff       (20)      188 2022-07-01 05:40:57.000000 aegea-4.4.0/MANIFEST.in
--rw-r--r--   0 kislyuk    (501) staff       (20)     1311 2023-03-27 05:42:23.000000 aegea-4.4.0/Makefile
--rw-r--r--   0 kislyuk    (501) staff       (20)    11797 2023-04-22 02:28:03.206552 aegea-4.4.0/PKG-INFO
--rw-r--r--   0 kislyuk    (501) staff       (20)    11487 2023-04-02 15:14:35.000000 aegea-4.4.0/README.rst
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.180224 aegea-4.4.0/aegea/
--rw-r--r--   0 kislyuk    (501) staff       (20)     8094 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2048 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/aegea_config.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     1771 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/alarms.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    19424 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/audit.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    16677 2023-04-22 01:58:54.000000 aegea-4.4.0/aegea/base_config.yml
--rw-r--r--   0 kislyuk    (501) staff       (20)    27543 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/batch.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     5204 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/billing.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     5174 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/build_ami.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     6148 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/build_docker_image.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2044 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/cloudtrail.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     6915 2017-03-19 18:47:27.000000 aegea-4.4.0/aegea/constants.json
--rw-r--r--   0 kislyuk    (501) staff       (20)     5722 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/cost.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    11223 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/ebs.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     3202 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/ecr.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    14413 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/ecs.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     3560 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/efs.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    11720 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/elb.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2806 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/flow_logs.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     5587 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/iam.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2035 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/instance_ctl.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     3158 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/lambda.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    20335 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/launch.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     7654 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/logs.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     9585 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/ls.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.180933 aegea-4.4.0/aegea/missions/
--rw-r--r--   0 kislyuk    (501) staff       (20)       13 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/.gitignore
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.181806 aegea-4.4.0/aegea/missions/arvados/
--rw-r--r--   0 kislyuk    (501) staff       (20)      289 2017-01-13 19:39:20.000000 aegea-4.4.0/aegea/missions/arvados/Makefile
--rw-r--r--   0 kislyuk    (501) staff       (20)     1446 2017-01-19 22:26:48.000000 aegea-4.4.0/aegea/missions/arvados/config.yml
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     6026 2017-01-23 18:07:36.000000 aegea-4.4.0/aegea/missions/arvados/deploy-arvados.sh
--rw-r--r--   0 kislyuk    (501) staff       (20)     1641 2017-01-19 20:51:49.000000 aegea-4.4.0/aegea/missions/arvados/environment
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.166937 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.183486 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.165809 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.183769 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/api/
--rw-r--r--   0 kislyuk    (501) staff       (20)      407 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/api/application.yml
--rw-r--r--   0 kislyuk    (501) staff       (20)      783 2017-01-19 19:35:43.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/api/database.yml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.183905 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/crunch-dispatch-slurm/
--rw-r--r--   0 kislyuk    (501) staff       (20)       94 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/crunch-dispatch-slurm/crunch-dispatch-slurm.yml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.184069 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/docker-cleaner/
--rw-r--r--   0 kislyuk    (501) staff       (20)       77 2016-11-01 22:37:46.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/docker-cleaner/docker-cleaner.json
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.184221 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/keep-web/
--rw-r--r--   0 kislyuk    (501) staff       (20)      259 2016-11-01 22:37:46.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/keep-web/keep-web.yml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.184360 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/keepproxy/
--rw-r--r--   0 kislyuk    (501) staff       (20)      278 2016-12-13 22:13:26.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/keepproxy/keepproxy.yml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.184490 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/nodemanager/
--rw-r--r--   0 kislyuk    (501) staff       (20)     1230 2017-01-19 20:48:50.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/nodemanager/ec2.cfg
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.189367 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/sso/
--rw-r--r--   0 kislyuk    (501) staff       (20)      421 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/sso/application.yml
--rw-r--r--   0 kislyuk    (501) staff       (20)      795 2017-01-19 19:35:58.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/sso/database.yml
--rw-r--r--   0 kislyuk    (501) staff       (20)      461 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/sso/production.rb
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.189506 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/workbench/
--rw-r--r--   0 kislyuk    (501) staff       (20)      291 2016-10-17 17:18:05.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/workbench/application.yml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.189633 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/default/
--rw-r--r--   0 kislyuk    (501) staff       (20)       19 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/default/munge
--rw-r--r--   0 kislyuk    (501) staff       (20)       17 2016-11-01 22:37:46.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/fuse.conf
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.191177 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/
--rw-r--r--   0 kislyuk    (501) staff       (20)      210 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/arvados-api.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)      238 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/arvados-keep.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)       88 2016-11-01 22:37:46.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/arvados-keepproxy.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)       92 2016-11-01 22:37:46.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/arvados-keepweb.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)      155 2017-01-19 16:44:26.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/arvados-nodemanager.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)      230 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/awslogs.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)      165 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/crunch-dispatch-slurm.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)        7 2017-01-23 17:03:52.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/crunch-dispatch-slurm.override
--rw-r--r--   0 kislyuk    (501) staff       (20)        7 2017-01-23 17:37:49.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/munge.override
--rw-r--r--   0 kislyuk    (501) staff       (20)        7 2017-01-23 17:37:38.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/slurm-llnl.override
--rw-r--r--   0 kislyuk    (501) staff       (20)        7 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/squid-deb-proxy.override
--rw-r--r--   0 kislyuk    (501) staff       (20)        7 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/init/squid3.override
--rw-r--r--   0 kislyuk    (501) staff       (20)      317 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/keep.conf.json
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.191308 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/keepstore/
--rw-r--r--   0 kislyuk    (501) staff       (20)       26 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/keepstore/blob-signing.key
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.191428 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/munge/
--rw-r--r--   0 kislyuk    (501) staff       (20)     1024 2016-11-01 22:37:46.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/munge/munge.key
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.166255 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.191530 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/conf.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)       34 2016-10-17 16:42:52.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/conf.d/arvados
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.191653 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-available/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2016-11-01 22:37:46.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-available/default
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.191978 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/
--rw-r--r--   0 kislyuk    (501) staff       (20)     1479 2017-01-19 19:31:32.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-api
--rw-r--r--   0 kislyuk    (501) staff       (20)      708 2017-01-19 19:32:24.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-sso
--rw-r--r--   0 kislyuk    (501) staff       (20)      638 2017-01-19 19:32:06.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-workbench
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.192096 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/profile.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)       93 2016-11-01 22:37:46.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/profile.d/arvados.sh
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.166420 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/resolvconf/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.192238 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/resolvconf/resolv.conf.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)       33 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/resolvconf/resolv.conf.d/tail
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.192450 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/slurm-llnl/
--rw-r--r--   0 kislyuk    (501) staff       (20)       80 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/slurm-llnl/nodes.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)      882 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/slurm-llnl/slurm.conf
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.166578 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/systemd/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.166678 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.192550 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/docker.service.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2016-11-01 22:37:46.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/docker.service.d/arvados.conf
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.192639 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/multi-user.target.wants/
--rw-r--r--   0 kislyuk    (501) staff       (20)      730 2016-11-01 22:37:46.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/multi-user.target.wants/arvados-docker-cleaner.service
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.166778 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/mnt/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.192777 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/mnt/keep/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/mnt/keep/.keep
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.166875 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/usr/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.192950 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/usr/bin/
--rwxr-xr-x   0 kislyuk    (501) staff       (20)      778 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/usr/bin/aegea-set-slurm-nodes
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     1666 2017-01-19 20:26:41.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/usr/bin/init-arvados
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.167162 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/var/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.167017 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/var/lib/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.167057 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/var/lib/arvados/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.167101 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/var/lib/arvados/git/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.193076 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/var/lib/arvados/git/repositories/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/var/lib/arvados/git/repositories/.keep
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.167205 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/var/log/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.193162 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/var/log/arvados/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2017-01-19 16:47:27.000000 aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/var/log/arvados/.keep
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.182376 aegea-4.4.0/aegea/missions/arvados-worker/
--rw-r--r--   0 kislyuk    (501) staff       (20)      289 2017-01-13 19:39:17.000000 aegea-4.4.0/aegea/missions/arvados-worker/Makefile
--rw-r--r--   0 kislyuk    (501) staff       (20)      877 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados-worker/config.yml
--rw-r--r--   0 kislyuk    (501) staff       (20)     1641 2017-01-19 20:51:49.000000 aegea-4.4.0/aegea/missions/arvados-worker/environment
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.160682 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.160626 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/etc/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.182483 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/etc/default/
--rw-r--r--   0 kislyuk    (501) staff       (20)       19 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/etc/default/munge
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.182613 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/etc/munge/
--rw-r--r--   0 kislyuk    (501) staff       (20)     1024 2016-11-01 22:37:46.000000 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/etc/munge/munge.key
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.182994 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/etc/slurm-llnl/
--rw-r--r--   0 kislyuk    (501) staff       (20)       80 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/etc/slurm-llnl/nodes.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)      882 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/etc/slurm-llnl/slurm.conf
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.160721 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/usr/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.183191 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/usr/bin/
--rwxr-xr-x   0 kislyuk    (501) staff       (20)      778 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/usr/bin/aegea-set-slurm-nodes
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.193247 aegea-4.4.0/aegea/missions/docker-example/
--rw-r--r--   0 kislyuk    (501) staff       (20)      224 2017-01-12 00:44:16.000000 aegea-4.4.0/aegea/missions/docker-example/config.yml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.167366 aegea-4.4.0/aegea/missions/docker-example/rootfs.skel/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.167407 aegea-4.4.0/aegea/missions/docker-example/rootfs.skel/etc/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.193459 aegea-4.4.0/aegea/missions/docker-example/rootfs.skel/etc/update-motd.d/
--rwxr-xr-x   0 kislyuk    (501) staff       (20)      214 2017-01-10 17:44:55.000000 aegea-4.4.0/aegea/missions/docker-example/rootfs.skel/etc/update-motd.d/aegea-motd
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.193951 aegea-4.4.0/aegea/missions/ecs-container-instance/
--rw-r--r--   0 kislyuk    (501) staff       (20)      437 2019-10-14 14:47:55.000000 aegea-4.4.0/aegea/missions/ecs-container-instance/Makefile
--rw-r--r--   0 kislyuk    (501) staff       (20)      632 2019-10-14 14:47:55.000000 aegea-4.4.0/aegea/missions/ecs-container-instance/config.yml
--rw-r--r--   0 kislyuk    (501) staff       (20)      355 2019-10-14 14:47:55.000000 aegea-4.4.0/aegea/missions/ecs-container-instance/environment
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.167575 aegea-4.4.0/aegea/missions/ecs-container-instance/rootfs.skel.in/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.167619 aegea-4.4.0/aegea/missions/ecs-container-instance/rootfs.skel.in/etc/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.194077 aegea-4.4.0/aegea/missions/ecs-container-instance/rootfs.skel.in/etc/ecs/
--rw-r--r--   0 kislyuk    (501) staff       (20)       55 2019-10-14 14:47:55.000000 aegea-4.4.0/aegea/missions/ecs-container-instance/rootfs.skel.in/etc/ecs/ecs.config
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.194519 aegea-4.4.0/aegea/missions/fog-dog/
--rw-r--r--   0 kislyuk    (501) staff       (20)      285 2017-01-13 19:38:03.000000 aegea-4.4.0/aegea/missions/fog-dog/Makefile
--rw-r--r--   0 kislyuk    (501) staff       (20)     1365 2017-02-02 23:31:30.000000 aegea-4.4.0/aegea/missions/fog-dog/config.yml
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/fog-dog/environment
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.167807 aegea-4.4.0/aegea/missions/fog-dog/rootfs.skel.in/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.167860 aegea-4.4.0/aegea/missions/fog-dog/rootfs.skel.in/etc/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.194612 aegea-4.4.0/aegea/missions/fog-dog/rootfs.skel.in/etc/update-motd.d/
--rwxr-xr-x   0 kislyuk    (501) staff       (20)      219 2016-12-13 22:14:13.000000 aegea-4.4.0/aegea/missions/fog-dog/rootfs.skel.in/etc/update-motd.d/fogdog-motd
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.194736 aegea-4.4.0/aegea/missions/ubuntu-14.04/
--rw-r--r--   0 kislyuk    (501) staff       (20)      112 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/ubuntu-14.04/config.yml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.168041 aegea-4.4.0/aegea/missions/ubuntu-14.04/rootfs.skel/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.168085 aegea-4.4.0/aegea/missions/ubuntu-14.04/rootfs.skel/etc/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.194858 aegea-4.4.0/aegea/missions/ubuntu-14.04/rootfs.skel/etc/init/
--rw-r--r--   0 kislyuk    (501) staff       (20)      230 2016-10-14 16:17:29.000000 aegea-4.4.0/aegea/missions/ubuntu-14.04/rootfs.skel/etc/init/awslogs.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)     3221 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/pricing.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     5642 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/rds.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     8036 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/rm.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.170179 aegea-4.4.0/aegea/rootfs.skel.build_ami/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.195392 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.195510 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/R/
--rw-r--r--   0 kislyuk    (501) staff       (20)      100 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/R/Rprofile.site
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.168348 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/apt/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.195660 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/apt/apt.conf.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)      127 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/apt/apt.conf.d/99aegea
--rw-r--r--   0 kislyuk    (501) staff       (20)       71 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/aws.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)      449 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/awslogs.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)      672 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/awslogs.logging.conf
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.168448 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/cloud/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.196011 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/cloud/cloud.cfg.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)       25 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/cloud/cloud.cfg.d/90_dpkg.cfg
--rw-r--r--   0 kislyuk    (501) staff       (20)      546 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/cloud/cloud.cfg.d/99_aegea.cfg
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.196328 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/default/
--rw-r--r--   0 kislyuk    (501) staff       (20)       10 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/default/apport
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.196494 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/default/grub.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)      127 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/default/grub.d/99aegea.cfg
--rw-r--r--   0 kislyuk    (501) staff       (20)       35 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/default/mdadm
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.197528 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/ecs/
--rw-r--r--   0 kislyuk    (501) staff       (20)      101 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/ecs/ecs.config
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.168801 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/fail2ban/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.197713 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/fail2ban/jail.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)       21 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/fail2ban/jail.d/aegea.conf
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.198001 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/logrotate.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)      216 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/logrotate.d/awslogs
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.198163 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/profile.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)      174 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/profile.d/aegea.sh
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.169132 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/security/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.198319 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/security/limits.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)       56 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/security/limits.d/aegea.conf
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.198484 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/ssh/
--rw-r--r--   0 kislyuk    (501) staff       (20)      392 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/ssh/ssh_known_hosts
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.198631 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/sudoers.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)       68 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/sudoers.d/99-aegea
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.198921 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/sysctl.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)      558 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/sysctl.d/90-netflix-tunables.conf
--rw-r--r--   0 kislyuk    (501) staff       (20)       37 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/sysctl.d/91-aegea.conf
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.169526 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/systemd/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.169579 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/systemd/system/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.199064 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/systemd/system/docker.service.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)      383 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/systemd/system/docker.service.d/xb.conf
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.169708 aegea-4.4.0/aegea/rootfs.skel.build_ami/lib/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.169781 aegea-4.4.0/aegea/rootfs.skel.build_ami/lib/systemd/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.199962 aegea-4.4.0/aegea/rootfs.skel.build_ami/lib/systemd/system/
--rw-r--r--   0 kislyuk    (501) staff       (20)      301 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/lib/systemd/system/aegea-deploy@.service
--rw-r--r--   0 kislyuk    (501) staff       (20)      257 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/lib/systemd/system/awslogs.service
--rw-r--r--   0 kislyuk    (501) staff       (20)      236 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/lib/systemd/system/docker-event-relay.service
--rw-r--r--   0 kislyuk    (501) staff       (20)     1183 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/lib/systemd/system/ecs.service
--rw-r--r--   0 kislyuk    (501) staff       (20)      221 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/lib/systemd/system/efs.service
--rw-r--r--   0 kislyuk    (501) staff       (20)      190 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/lib/systemd/system/format-ephemeral-storage.service
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.169944 aegea-4.4.0/aegea/rootfs.skel.build_ami/root/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.200105 aegea-4.4.0/aegea/rootfs.skel.build_ami/root/.aws/
--rw-r--r--   0 kislyuk    (501) staff       (20)       71 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/root/.aws/config
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.170081 aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.200903 aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     8010 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/aegea-deploy-pilot
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     2476 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/aegea-docker-event-relay
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     3002 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/aegea-efs-mount
--rwxr-xr-x   0 kislyuk    (501) staff       (20)      803 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/aegea-format-ephemeral-storage
--rwxr-xr-x   0 kislyuk    (501) staff       (20)      927 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/aegea-git-ssh-helper
--rwxr-xr-x   0 kislyuk    (501) staff       (20)      432 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/aegea-imds
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.170415 aegea-4.4.0/aegea/rootfs.skel.build_ami/var/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.170338 aegea-4.4.0/aegea/rootfs.skel.build_ami/var/awslogs/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.201083 aegea-4.4.0/aegea/rootfs.skel.build_ami/var/awslogs/state/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/var/awslogs/state/.keep
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.170473 aegea-4.4.0/aegea/rootfs.skel.build_ami/var/lib/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.201172 aegea-4.4.0/aegea/rootfs.skel.build_ami/var/lib/docker/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.build_ami/var/lib/docker/.keep
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.170658 aegea-4.4.0/aegea/rootfs.skel.launch/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.170908 aegea-4.4.0/aegea/rootfs.skel.launch/var/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.170967 aegea-4.4.0/aegea/rootfs.skel.launch/var/lib/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.201274 aegea-4.4.0/aegea/rootfs.skel.launch/var/lib/aegea/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/rootfs.skel.launch/var/lib/aegea/.keep
--rw-r--r--   0 kislyuk    (501) staff       (20)     7747 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/s3.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     6134 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/secrets.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     7737 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/sfn.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    15928 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/ssh.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     1390 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/top.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      370 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/user_config.yml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.202390 aegea-4.4.0/aegea/util/
--rw-r--r--   0 kislyuk    (501) staff       (20)     5804 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/__init__.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.204066 aegea-4.4.0/aegea/util/aws/
--rw-r--r--   0 kislyuk    (501) staff       (20)    25319 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/aws/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     1201 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/aws/_boto3_loader.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    14524 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/aws/batch.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.204512 aegea-4.4.0/aegea/util/aws/batch_events_lambda/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.204861 aegea-4.4.0/aegea/util/aws/batch_events_lambda/.chalice/
--rw-r--r--   0 kislyuk    (501) staff       (20)      286 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/util/aws/batch_events_lambda/.chalice/config.json
--rw-r--r--   0 kislyuk    (501) staff       (20)      486 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/util/aws/batch_events_lambda/.chalice/policy-dev.json
--rw-r--r--   0 kislyuk    (501) staff       (20)       37 2022-07-01 05:40:57.000000 aegea-4.4.0/aegea/util/aws/batch_events_lambda/.gitignore
--rw-r--r--   0 kislyuk    (501) staff       (20)      984 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/aws/batch_events_lambda/app.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      172 2023-01-09 03:46:45.000000 aegea-4.4.0/aegea/util/aws/clients.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     3608 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/aws/dns.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     7268 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/aws/iam.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     7986 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/aws/logs.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      176 2023-01-09 03:46:45.000000 aegea-4.4.0/aegea/util/aws/resources.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     4389 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/aws/spot.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     6385 2023-04-22 02:17:51.000000 aegea-4.4.0/aegea/util/aws/ssm.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     7568 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/cloudinit.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     1079 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/constants.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2851 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/crypto.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      143 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/exceptions.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    10911 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/util/printing.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      799 2023-01-09 03:46:45.000000 aegea-4.4.0/aegea/util/ssh.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      160 2023-04-22 02:28:03.000000 aegea-4.4.0/aegea/version.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2241 2023-04-22 02:20:18.000000 aegea-4.4.0/aegea/zones.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.180829 aegea-4.4.0/aegea.egg-info/
--rw-r--r--   0 kislyuk    (501) staff       (20)    11797 2023-04-22 02:28:03.000000 aegea-4.4.0/aegea.egg-info/PKG-INFO
--rw-r--r--   0 kislyuk    (501) staff       (20)     7972 2023-04-22 02:28:03.000000 aegea-4.4.0/aegea.egg-info/SOURCES.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)        1 2023-04-22 02:28:03.000000 aegea-4.4.0/aegea.egg-info/dependency_links.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)      295 2023-04-22 02:28:03.000000 aegea-4.4.0/aegea.egg-info/requires.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)        6 2023-04-22 02:28:03.000000 aegea-4.4.0/aegea.egg-info/top_level.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)     1899 2023-03-27 05:22:54.000000 aegea-4.4.0/common.mk
--rw-r--r--   0 kislyuk    (501) staff       (20)      431 2022-07-01 05:40:57.000000 aegea-4.4.0/mypy.ini
--rw-r--r--   0 kislyuk    (501) staff       (20)      328 2023-03-27 05:42:23.000000 aegea-4.4.0/pyproject.toml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.205616 aegea-4.4.0/scripts/
--rwxr-xr-x   0 kislyuk    (501) staff       (20)      535 2022-07-01 05:40:57.000000 aegea-4.4.0/scripts/aegea
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     1603 2022-07-01 05:40:57.000000 aegea-4.4.0/scripts/aegea-build-image-for-mission
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     2971 2022-07-01 05:40:57.000000 aegea-4.4.0/scripts/aegea-rebuild-public-elb-sg
--rw-r--r--   0 kislyuk    (501) staff       (20)      529 2022-07-01 05:40:57.000000 aegea-4.4.0/scripts/aegea-ssh
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     2058 2022-07-01 05:40:57.000000 aegea-4.4.0/scripts/pypi-apt-freeze
--rw-r--r--   0 kislyuk    (501) staff       (20)       38 2023-04-22 02:28:03.206806 aegea-4.4.0/setup.cfg
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     1317 2023-04-22 01:48:30.000000 aegea-4.4.0/setup.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 02:28:03.206259 aegea-4.4.0/test/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2016-06-14 14:20:19.000000 aegea-4.4.0/test/__init__.py
--rwxr-xr-x   0 kislyuk    (501) staff       (20)    19641 2023-04-22 01:48:30.000000 aegea-4.4.0/test/test.py
--rw-r--r--   0 kislyuk    (501) staff       (20)       71 2022-07-01 05:40:57.000000 aegea-4.4.0/test/test.wdl
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.843110 aegea-4.4.1/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       44 2021-06-20 21:22:13.000000 aegea-4.4.1/.coveragerc
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.484796 aegea-4.4.1/.github/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.625045 aegea-4.4.1/.github/workflows/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1251 2023-05-25 21:11:10.000000 aegea-4.4.1/.github/workflows/ci.yml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      518 2021-12-23 22:52:43.000000 aegea-4.4.1/.gitignore
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    36559 2023-05-26 02:41:06.000000 aegea-4.4.1/Changes.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    11357 2021-06-20 21:22:13.000000 aegea-4.4.1/LICENSE.md
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      188 2021-06-20 21:22:13.000000 aegea-4.4.1/MANIFEST.in
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1311 2023-05-25 21:11:10.000000 aegea-4.4.1/Makefile
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    11797 2023-05-26 02:41:50.843630 aegea-4.4.1/PKG-INFO
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    11487 2023-05-25 21:11:10.000000 aegea-4.4.1/README.rst
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.660156 aegea-4.4.1/aegea/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8094 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2048 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/aegea_config.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1771 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/alarms.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    19424 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/audit.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    16948 2023-05-25 22:29:36.000000 aegea-4.4.1/aegea/base_config.yml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    27543 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/batch.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     5204 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/billing.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     5174 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/build_ami.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     6148 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/build_docker_image.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2044 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/cloudtrail.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     6915 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/constants.json
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     5722 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/cost.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    11223 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/ebs.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3202 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/ecr.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    14413 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/ecs.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3560 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/efs.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    11720 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/elb.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2806 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/flow_logs.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     5587 2022-12-16 21:36:51.000000 aegea-4.4.1/aegea/iam.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2035 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/instance_ctl.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3158 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/lambda.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    20335 2023-05-25 21:11:10.000000 aegea-4.4.1/aegea/launch.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     7654 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/logs.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     9590 2023-05-25 21:11:10.000000 aegea-4.4.1/aegea/ls.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.662944 aegea-4.4.1/aegea/missions/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       13 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/.gitignore
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.665703 aegea-4.4.1/aegea/missions/arvados/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      289 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/Makefile
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1446 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/config.yml
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     6026 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/deploy-arvados.sh
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1641 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/environment
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.529651 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.674024 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.522018 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/arvados/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.676062 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/arvados/api/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      407 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/arvados/api/application.yml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      783 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/arvados/api/database.yml
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.677142 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/arvados/crunch-dispatch-slurm/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       94 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/arvados/crunch-dispatch-slurm/crunch-dispatch-slurm.yml
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.677952 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/arvados/docker-cleaner/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       77 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/arvados/docker-cleaner/docker-cleaner.json
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.678797 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/arvados/keep-web/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      259 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/arvados/keep-web/keep-web.yml
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.679657 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/arvados/keepproxy/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      278 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/arvados/keepproxy/keepproxy.yml
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.680586 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/arvados/nodemanager/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1230 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/arvados/nodemanager/ec2.cfg
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.682690 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/arvados/sso/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      421 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/arvados/sso/application.yml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      795 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/arvados/sso/database.yml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      461 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/arvados/sso/production.rb
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.683385 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/arvados/workbench/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      291 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/arvados/workbench/application.yml
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.684088 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/default/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       19 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/default/munge
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       17 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/fuse.conf
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.692942 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/init/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      210 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/init/arvados-api.conf
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      238 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/init/arvados-keep.conf
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       88 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/init/arvados-keepproxy.conf
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       92 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/init/arvados-keepweb.conf
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      155 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/init/arvados-nodemanager.conf
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      230 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/init/awslogs.conf
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      165 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/init/crunch-dispatch-slurm.conf
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        7 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/init/crunch-dispatch-slurm.override
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        7 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/init/munge.override
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        7 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/init/slurm-llnl.override
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        7 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/init/squid-deb-proxy.override
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        7 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/init/squid3.override
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      317 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/keep.conf.json
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.693748 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/keepstore/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       26 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/keepstore/blob-signing.key
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.694673 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/munge/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1024 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/munge/munge.key
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.524385 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/nginx/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.696444 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/nginx/conf.d/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       34 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/nginx/conf.d/arvados
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.698145 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-available/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-available/default
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.702595 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1479 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-api
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      708 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-sso
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      638 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-workbench
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.704968 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/profile.d/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       93 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/profile.d/arvados.sh
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.525591 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/resolvconf/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.706328 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/resolvconf/resolv.conf.d/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       33 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/resolvconf/resolv.conf.d/tail
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.707841 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/slurm-llnl/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       80 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/slurm-llnl/nodes.conf
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      882 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/slurm-llnl/slurm.conf
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.526735 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/systemd/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.527314 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.708426 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/docker.service.d/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/docker.service.d/arvados.conf
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.725220 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/multi-user.target.wants/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      730 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/multi-user.target.wants/arvados-docker-cleaner.service
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.528167 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/mnt/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.726210 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/mnt/keep/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/mnt/keep/.keep
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.529104 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/usr/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.727591 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/usr/bin/
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)      778 2022-12-16 21:25:59.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/usr/bin/aegea-set-slurm-nodes
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1666 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/usr/bin/init-arvados
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.535176 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/var/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.533699 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/var/lib/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.534318 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/var/lib/arvados/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.534698 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/var/lib/arvados/git/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.728669 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/var/lib/arvados/git/repositories/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/var/lib/arvados/git/repositories/.keep
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.535482 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/var/log/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.729419 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/var/log/arvados/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/var/log/arvados/.keep
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.667578 aegea-4.4.1/aegea/missions/arvados-worker/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      289 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados-worker/Makefile
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      877 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados-worker/config.yml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1641 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados-worker/environment
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.487313 aegea-4.4.1/aegea/missions/arvados-worker/rootfs.skel.in/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.487059 aegea-4.4.1/aegea/missions/arvados-worker/rootfs.skel.in/etc/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.668078 aegea-4.4.1/aegea/missions/arvados-worker/rootfs.skel.in/etc/default/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       19 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados-worker/rootfs.skel.in/etc/default/munge
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.668784 aegea-4.4.1/aegea/missions/arvados-worker/rootfs.skel.in/etc/munge/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1024 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados-worker/rootfs.skel.in/etc/munge/munge.key
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.670904 aegea-4.4.1/aegea/missions/arvados-worker/rootfs.skel.in/etc/slurm-llnl/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       80 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados-worker/rootfs.skel.in/etc/slurm-llnl/nodes.conf
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      882 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/arvados-worker/rootfs.skel.in/etc/slurm-llnl/slurm.conf
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.487485 aegea-4.4.1/aegea/missions/arvados-worker/rootfs.skel.in/usr/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.671938 aegea-4.4.1/aegea/missions/arvados-worker/rootfs.skel.in/usr/bin/
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)      778 2022-12-16 21:25:59.000000 aegea-4.4.1/aegea/missions/arvados-worker/rootfs.skel.in/usr/bin/aegea-set-slurm-nodes
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.730068 aegea-4.4.1/aegea/missions/docker-example/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      224 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/docker-example/config.yml
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.536563 aegea-4.4.1/aegea/missions/docker-example/rootfs.skel/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.536756 aegea-4.4.1/aegea/missions/docker-example/rootfs.skel/etc/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.731082 aegea-4.4.1/aegea/missions/docker-example/rootfs.skel/etc/update-motd.d/
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)      214 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/docker-example/rootfs.skel/etc/update-motd.d/aegea-motd
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.734361 aegea-4.4.1/aegea/missions/ecs-container-instance/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      437 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/ecs-container-instance/Makefile
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      632 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/ecs-container-instance/config.yml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      355 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/ecs-container-instance/environment
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.560833 aegea-4.4.1/aegea/missions/ecs-container-instance/rootfs.skel.in/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.561061 aegea-4.4.1/aegea/missions/ecs-container-instance/rootfs.skel.in/etc/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.735402 aegea-4.4.1/aegea/missions/ecs-container-instance/rootfs.skel.in/etc/ecs/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       55 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/ecs-container-instance/rootfs.skel.in/etc/ecs/ecs.config
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.737996 aegea-4.4.1/aegea/missions/fog-dog/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      285 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/fog-dog/Makefile
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1365 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/fog-dog/config.yml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/fog-dog/environment
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.561926 aegea-4.4.1/aegea/missions/fog-dog/rootfs.skel.in/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.562112 aegea-4.4.1/aegea/missions/fog-dog/rootfs.skel.in/etc/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.738717 aegea-4.4.1/aegea/missions/fog-dog/rootfs.skel.in/etc/update-motd.d/
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)      219 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/fog-dog/rootfs.skel.in/etc/update-motd.d/fogdog-motd
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.740064 aegea-4.4.1/aegea/missions/ubuntu-14.04/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      112 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/ubuntu-14.04/config.yml
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.562914 aegea-4.4.1/aegea/missions/ubuntu-14.04/rootfs.skel/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.563093 aegea-4.4.1/aegea/missions/ubuntu-14.04/rootfs.skel/etc/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.741580 aegea-4.4.1/aegea/missions/ubuntu-14.04/rootfs.skel/etc/init/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      230 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/missions/ubuntu-14.04/rootfs.skel/etc/init/awslogs.conf
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3221 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/pricing.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     5642 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/rds.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8036 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/rm.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.610566 aegea-4.4.1/aegea/rootfs.skel.build_ami/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.747276 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.749269 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/R/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      100 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/R/Rprofile.site
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.564665 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/apt/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.752391 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/apt/apt.conf.d/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      127 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/apt/apt.conf.d/99aegea
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       71 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/aws.conf
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      449 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/awslogs.conf
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      672 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/awslogs.logging.conf
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.565247 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/cloud/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.756921 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/cloud/cloud.cfg.d/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       25 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/cloud/cloud.cfg.d/90_dpkg.cfg
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      546 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/cloud/cloud.cfg.d/99_aegea.cfg
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.760195 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/default/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       10 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/default/apport
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.761865 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/default/grub.d/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      127 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/default/grub.d/99aegea.cfg
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       35 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/default/mdadm
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.763412 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/ecs/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      101 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/ecs/ecs.config
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.604185 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/fail2ban/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.764612 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/fail2ban/jail.d/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       21 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/fail2ban/jail.d/aegea.conf
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.766011 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/logrotate.d/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      216 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/logrotate.d/awslogs
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.767584 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/profile.d/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      174 2022-01-14 05:36:28.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/profile.d/aegea.sh
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.605306 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/security/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.768954 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/security/limits.d/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       56 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/security/limits.d/aegea.conf
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.770286 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/ssh/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      392 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/ssh/ssh_known_hosts
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.771504 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/sudoers.d/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       68 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/sudoers.d/99-aegea
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.774475 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/sysctl.d/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      558 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/sysctl.d/90-netflix-tunables.conf
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       37 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/sysctl.d/91-aegea.conf
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.606707 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/systemd/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.606905 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/systemd/system/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.775919 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/systemd/system/docker.service.d/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      383 2022-01-14 05:36:28.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/systemd/system/docker.service.d/xb.conf
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.607734 aegea-4.4.1/aegea/rootfs.skel.build_ami/lib/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.608126 aegea-4.4.1/aegea/rootfs.skel.build_ami/lib/systemd/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.794794 aegea-4.4.1/aegea/rootfs.skel.build_ami/lib/systemd/system/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      301 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/lib/systemd/system/aegea-deploy@.service
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      257 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/lib/systemd/system/awslogs.service
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      236 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/lib/systemd/system/docker-event-relay.service
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1183 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/lib/systemd/system/ecs.service
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      221 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/lib/systemd/system/efs.service
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      190 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/lib/systemd/system/format-ephemeral-storage.service
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.609281 aegea-4.4.1/aegea/rootfs.skel.build_ami/root/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.795962 aegea-4.4.1/aegea/rootfs.skel.build_ami/root/.aws/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       71 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/root/.aws/config
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.610239 aegea-4.4.1/aegea/rootfs.skel.build_ami/usr/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.803019 aegea-4.4.1/aegea/rootfs.skel.build_ami/usr/bin/
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     8010 2022-12-16 21:25:59.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/usr/bin/aegea-deploy-pilot
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     2476 2022-12-16 21:25:59.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/usr/bin/aegea-docker-event-relay
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     3002 2022-12-16 21:25:59.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/usr/bin/aegea-efs-mount
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)      803 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/usr/bin/aegea-format-ephemeral-storage
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)      927 2022-12-16 21:25:59.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/usr/bin/aegea-git-ssh-helper
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)      432 2022-01-14 05:36:28.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/usr/bin/aegea-imds
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.611261 aegea-4.4.1/aegea/rootfs.skel.build_ami/var/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.610966 aegea-4.4.1/aegea/rootfs.skel.build_ami/var/awslogs/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.804213 aegea-4.4.1/aegea/rootfs.skel.build_ami/var/awslogs/state/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/var/awslogs/state/.keep
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.611454 aegea-4.4.1/aegea/rootfs.skel.build_ami/var/lib/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.805104 aegea-4.4.1/aegea/rootfs.skel.build_ami/var/lib/docker/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/rootfs.skel.build_ami/var/lib/docker/.keep
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.612043 aegea-4.4.1/aegea/rootfs.skel.launch/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.612390 aegea-4.4.1/aegea/rootfs.skel.launch/var/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.612738 aegea-4.4.1/aegea/rootfs.skel.launch/var/lib/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.806091 aegea-4.4.1/aegea/rootfs.skel.launch/var/lib/aegea/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2021-07-19 15:50:38.000000 aegea-4.4.1/aegea/rootfs.skel.launch/var/lib/aegea/.keep
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8070 2023-05-26 02:21:16.000000 aegea-4.4.1/aegea/s3.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     6134 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/secrets.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     7737 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/sfn.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    15928 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/ssh.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1390 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/top.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      370 2021-07-16 21:48:39.000000 aegea-4.4.1/aegea/user_config.yml
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.814169 aegea-4.4.1/aegea/util/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     5804 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/util/__init__.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.825568 aegea-4.4.1/aegea/util/aws/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    25319 2023-05-25 21:11:10.000000 aegea-4.4.1/aegea/util/aws/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1201 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/util/aws/_boto3_loader.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    14524 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/util/aws/batch.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.828272 aegea-4.4.1/aegea/util/aws/batch_events_lambda/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.830909 aegea-4.4.1/aegea/util/aws/batch_events_lambda/.chalice/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      286 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/util/aws/batch_events_lambda/.chalice/config.json
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      486 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/util/aws/batch_events_lambda/.chalice/policy-dev.json
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       37 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/util/aws/batch_events_lambda/.gitignore
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      984 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/util/aws/batch_events_lambda/app.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      172 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/util/aws/clients.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3608 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/util/aws/dns.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     7268 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/util/aws/iam.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     7986 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/util/aws/logs.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      176 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/util/aws/resources.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     4389 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/util/aws/spot.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     6385 2023-05-25 21:11:10.000000 aegea-4.4.1/aegea/util/aws/ssm.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     7568 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/util/cloudinit.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1079 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/util/constants.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2851 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/util/crypto.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      143 2021-06-20 21:22:13.000000 aegea-4.4.1/aegea/util/exceptions.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    10911 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/util/printing.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      799 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/util/ssh.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      160 2023-05-26 02:41:50.000000 aegea-4.4.1/aegea/version.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2241 2022-12-16 21:26:04.000000 aegea-4.4.1/aegea/zones.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.662511 aegea-4.4.1/aegea.egg-info/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    11797 2023-05-26 02:41:50.000000 aegea-4.4.1/aegea.egg-info/PKG-INFO
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     7972 2023-05-26 02:41:50.000000 aegea-4.4.1/aegea.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2023-05-26 02:41:50.000000 aegea-4.4.1/aegea.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      295 2023-05-26 02:41:50.000000 aegea-4.4.1/aegea.egg-info/requires.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        6 2023-05-26 02:41:50.000000 aegea-4.4.1/aegea.egg-info/top_level.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1899 2023-03-05 00:40:53.000000 aegea-4.4.1/common.mk
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      431 2021-06-20 21:22:13.000000 aegea-4.4.1/mypy.ini
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      328 2023-05-25 21:11:10.000000 aegea-4.4.1/pyproject.toml
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.837046 aegea-4.4.1/scripts/
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)      535 2021-12-23 21:58:16.000000 aegea-4.4.1/scripts/aegea
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1603 2021-12-23 21:58:19.000000 aegea-4.4.1/scripts/aegea-build-image-for-mission
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     2971 2021-12-23 21:58:05.000000 aegea-4.4.1/scripts/aegea-rebuild-public-elb-sg
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      529 2021-06-20 21:22:13.000000 aegea-4.4.1/scripts/aegea-ssh
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     2058 2021-12-23 21:57:59.000000 aegea-4.4.1/scripts/pypi-apt-freeze
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       38 2023-05-26 02:41:50.845344 aegea-4.4.1/setup.cfg
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1317 2023-05-25 21:11:10.000000 aegea-4.4.1/setup.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-05-26 02:41:50.841653 aegea-4.4.1/test/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2021-06-20 21:22:13.000000 aegea-4.4.1/test/__init__.py
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)    19641 2023-05-25 21:11:10.000000 aegea-4.4.1/test/test.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       71 2021-06-20 21:22:13.000000 aegea-4.4.1/test/test.wdl
```

### Comparing `aegea-4.4.0/.github/workflows/ci.yml` & `aegea-4.4.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/.gitignore` & `aegea-4.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/Changes.rst` & `aegea-4.4.1/Changes.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Changes for v4.4.1 (2023-05-25)
+===============================
+
+-  s3 buckets: Compute size metrics for all storage classes
+
 Changes for v4.4.0 (2023-04-21)
 ===============================
 
 -  aegea ssh: download correct SSM plugin
 
 -  aegea launch: use t3a.micro instance type by default
```

### Comparing `aegea-4.4.0/LICENSE.md` & `aegea-4.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/Makefile` & `aegea-4.4.1/Makefile`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/PKG-INFO` & `aegea-4.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegea
-Version: 4.4.0
+Version: 4.4.1
 Summary: Amazon Web Services Operator Interface
 Home-page: https://github.com/kislyuk/aegea
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Platform: MacOS X
 Platform: Posix
```

### Comparing `aegea-4.4.0/README.rst` & `aegea-4.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/__init__.py` & `aegea-4.4.1/aegea/__init__.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/aegea_config.py` & `aegea-4.4.1/aegea/aegea_config.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/alarms.py` & `aegea-4.4.1/aegea/alarms.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/audit.py` & `aegea-4.4.1/aegea/audit.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/base_config.yml` & `aegea-4.4.1/aegea/base_config.yml`

 * *Files 3% similar despite different names*

```diff
@@ -272,16 +272,28 @@
   resource: s3
   subresource: Bucket
   columns:
     - name
     - creation_date
     - LocationConstraint
     - NumberOfObjects
-    - BucketSizeBytes
     - Encryption
+    - BucketSizeBytes
+    - Standard
+    - StandardIA
+    - OneZoneIA
+    - ReducedRedundancy
+    - GlacierInstantRetrieval
+    - Glacier
+    - DeepArchive
+    - IntelligentTieringFA
+    - IntelligentTieringIA
+    - IntelligentTieringAA
+    - IntelligentTieringAIA
+    - IntelligentTieringDAA
 
 s3_versions:
   columns:
     - key
     - is_latest
     - last_modified
     - size
```

### Comparing `aegea-4.4.0/aegea/batch.py` & `aegea-4.4.1/aegea/batch.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/billing.py` & `aegea-4.4.1/aegea/billing.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/build_ami.py` & `aegea-4.4.1/aegea/build_ami.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/build_docker_image.py` & `aegea-4.4.1/aegea/build_docker_image.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/cloudtrail.py` & `aegea-4.4.1/aegea/cloudtrail.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/constants.json` & `aegea-4.4.1/aegea/constants.json`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/cost.py` & `aegea-4.4.1/aegea/cost.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/ebs.py` & `aegea-4.4.1/aegea/ebs.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/ecr.py` & `aegea-4.4.1/aegea/ecr.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/ecs.py` & `aegea-4.4.1/aegea/ecs.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/efs.py` & `aegea-4.4.1/aegea/efs.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/elb.py` & `aegea-4.4.1/aegea/elb.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/flow_logs.py` & `aegea-4.4.1/aegea/flow_logs.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/iam.py` & `aegea-4.4.1/aegea/iam.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/instance_ctl.py` & `aegea-4.4.1/aegea/instance_ctl.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/lambda.py` & `aegea-4.4.1/aegea/lambda.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/launch.py` & `aegea-4.4.1/aegea/launch.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/logs.py` & `aegea-4.4.1/aegea/logs.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/ls.py` & `aegea-4.4.1/aegea/ls.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,17 @@
     page_output(tabulate(paginate(clients.sns.get_paginator("list_subscriptions")), args))
 
 parser = register_listing_parser(subscriptions, help="List SNS subscriptions",
                                  column_defaults=["SubscriptionArn", "Protocol", "Endpoint"])
 
 def limits(args):
     """
-    Describe limits in effect on your AWS account. See also https://console.aws.amazon.com/ec2/v2/home#Limits:
+    Describe limits in effect on your AWS account.
+
+    See also https://console.aws.amazon.com/ec2/v2/home#Limits:
     """
     # https://aws.amazon.com/about-aws/whats-new/2014/06/19/amazon-ec2-service-limits-report-now-available/
     # Console-only APIs: getInstanceLimits, getAccountLimits, getAutoscalingLimits, getHostLimits
     # http://boto3.readthedocs.io/en/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_limits
     attrs = ["max-instances", "vpc-max-security-groups-per-interface", "vpc-max-elastic-ips"]
     table = clients.ec2.describe_account_attributes(AttributeNames=attrs)["AccountAttributes"]
     page_output(tabulate(table, args))
```

### Comparing `aegea-4.4.0/aegea/missions/arvados/config.yml` & `aegea-4.4.1/aegea/missions/arvados/config.yml`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/missions/arvados/deploy-arvados.sh` & `aegea-4.4.1/aegea/missions/arvados/deploy-arvados.sh`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/missions/arvados/environment` & `aegea-4.4.1/aegea/missions/arvados/environment`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/api/database.yml` & `aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/arvados/api/database.yml`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/nodemanager/ec2.cfg` & `aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/arvados/nodemanager/ec2.cfg`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/arvados/sso/database.yml` & `aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/arvados/sso/database.yml`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/munge/munge.key` & `aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/munge/munge.key`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-api` & `aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-api`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-sso` & `aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-sso`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-workbench` & `aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/nginx/sites-enabled/arvados-workbench`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/slurm-llnl/slurm.conf` & `aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/slurm-llnl/slurm.conf`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/multi-user.target.wants/arvados-docker-cleaner.service` & `aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/etc/systemd/system/multi-user.target.wants/arvados-docker-cleaner.service`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/usr/bin/aegea-set-slurm-nodes` & `aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/usr/bin/aegea-set-slurm-nodes`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/missions/arvados/rootfs.skel.in/usr/bin/init-arvados` & `aegea-4.4.1/aegea/missions/arvados/rootfs.skel.in/usr/bin/init-arvados`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/missions/arvados-worker/config.yml` & `aegea-4.4.1/aegea/missions/arvados-worker/config.yml`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/missions/arvados-worker/environment` & `aegea-4.4.1/aegea/missions/arvados-worker/environment`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/etc/munge/munge.key` & `aegea-4.4.1/aegea/missions/arvados-worker/rootfs.skel.in/etc/munge/munge.key`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/etc/slurm-llnl/slurm.conf` & `aegea-4.4.1/aegea/missions/arvados-worker/rootfs.skel.in/etc/slurm-llnl/slurm.conf`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/missions/arvados-worker/rootfs.skel.in/usr/bin/aegea-set-slurm-nodes` & `aegea-4.4.1/aegea/missions/arvados-worker/rootfs.skel.in/usr/bin/aegea-set-slurm-nodes`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/missions/ecs-container-instance/config.yml` & `aegea-4.4.1/aegea/missions/ecs-container-instance/config.yml`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/missions/fog-dog/config.yml` & `aegea-4.4.1/aegea/missions/fog-dog/config.yml`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/pricing.py` & `aegea-4.4.1/aegea/pricing.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/rds.py` & `aegea-4.4.1/aegea/rds.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/rm.py` & `aegea-4.4.1/aegea/rm.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/awslogs.logging.conf` & `aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/awslogs.logging.conf`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/cloud/cloud.cfg.d/99_aegea.cfg` & `aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/cloud/cloud.cfg.d/99_aegea.cfg`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/rootfs.skel.build_ami/etc/sysctl.d/90-netflix-tunables.conf` & `aegea-4.4.1/aegea/rootfs.skel.build_ami/etc/sysctl.d/90-netflix-tunables.conf`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/rootfs.skel.build_ami/lib/systemd/system/ecs.service` & `aegea-4.4.1/aegea/rootfs.skel.build_ami/lib/systemd/system/ecs.service`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/aegea-deploy-pilot` & `aegea-4.4.1/aegea/rootfs.skel.build_ami/usr/bin/aegea-deploy-pilot`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/aegea-docker-event-relay` & `aegea-4.4.1/aegea/rootfs.skel.build_ami/usr/bin/aegea-docker-event-relay`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/aegea-efs-mount` & `aegea-4.4.1/aegea/rootfs.skel.build_ami/usr/bin/aegea-efs-mount`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/aegea-format-ephemeral-storage` & `aegea-4.4.1/aegea/rootfs.skel.build_ami/usr/bin/aegea-format-ephemeral-storage`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/rootfs.skel.build_ami/usr/bin/aegea-git-ssh-helper` & `aegea-4.4.1/aegea/rootfs.skel.build_ami/usr/bin/aegea-git-ssh-helper`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/s3.py` & `aegea-4.4.1/aegea/s3.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,88 +16,128 @@
 from .util.exceptions import AegeaException
 from .util.printing import format_number, page_output, tabulate
 
 
 def s3(args):
     s3_parser.print_help()
 
+
 s3_parser = register_parser(s3, help="Manage S3 buckets and query s3 objects", description=__doc__)
 
+
 def describe_bucket_worker(bucket):
     bucket.LocationConstraint = clients.s3.get_bucket_location(Bucket=bucket.name)["LocationConstraint"]
     cloudwatch = resources.cloudwatch
     bucket_region = bucket.LocationConstraint or "us-east-1"
     if bucket_region != cloudwatch.meta.client.meta.region_name:
         cloudwatch = boto3.Session(region_name=bucket_region).resource("cloudwatch")
-    data = get_cloudwatch_metric_stats("AWS/S3", "NumberOfObjects",
-                                       start_time=datetime.utcnow() - timedelta(days=2),
-                                       end_time=datetime.utcnow(), period=3600, BucketName=bucket.name,
-                                       StorageType="AllStorageTypes", resource=cloudwatch)
+    data = get_cloudwatch_metric_stats(
+        "AWS/S3",
+        "NumberOfObjects",
+        start_time=datetime.utcnow() - timedelta(days=2),
+        end_time=datetime.utcnow(),
+        period=3600,
+        BucketName=bucket.name,
+        StorageType="AllStorageTypes",
+        resource=cloudwatch,
+    )
     bucket.NumberOfObjects = int(data["Datapoints"][-1]["Average"]) if data["Datapoints"] else None
-    data = get_cloudwatch_metric_stats("AWS/S3", "BucketSizeBytes",
-                                       start_time=datetime.utcnow() - timedelta(days=2),
-                                       end_time=datetime.utcnow(), period=3600, BucketName=bucket.name,
-                                       StorageType="StandardStorage", resource=cloudwatch)
-    bucket.BucketSizeBytes = format_number(data["Datapoints"][-1]["Average"]) if data["Datapoints"] else None
+    total_bytes = 0
+    cloudwatch_metric_stats_args = dict(
+        start_time=datetime.utcnow() - timedelta(days=2),
+        end_time=datetime.utcnow(),
+        period=3600,
+        resource=cloudwatch,
+        BucketName=bucket.name,
+    )
+    for storage_type in (
+        "Standard",
+        "StandardIA",
+        "OneZoneIA",
+        "ReducedRedundancy",
+        "GlacierInstantRetrieval",
+        "Glacier",
+        "DeepArchive",
+        "IntelligentTieringFA",
+        "IntelligentTieringIA",
+        "IntelligentTieringAA",
+        "IntelligentTieringAIA",
+        "IntelligentTieringDAA",
+    ):
+        data = get_cloudwatch_metric_stats(
+            "AWS/S3", "BucketSizeBytes", StorageType=f"{storage_type}Storage", **cloudwatch_metric_stats_args
+        )
+        size_bytes = data["Datapoints"][-1]["Average"] if data["Datapoints"] else 0
+        setattr(bucket, storage_type, format_number(size_bytes))
+        total_bytes += size_bytes
+    bucket.BucketSizeBytes = format_number(total_bytes)
     try:
         res = clients.s3.get_bucket_encryption(Bucket=bucket.name)
         enc = res["ServerSideEncryptionConfiguration"]["Rules"][0]["ApplyServerSideEncryptionByDefault"]["SSEAlgorithm"]
         bucket.Encryption = enc
     except ClientError as e:
         expect_error_codes(e, "ServerSideEncryptionConfigurationNotFoundError", "AccessDenied")
         bucket.Encryption = None
     return bucket
 
+
 def buckets(args):
     """
     List S3 buckets. See also "aws s3 ls". Use "aws s3 ls NAME" to list bucket contents.
     """
     with ThreadPoolExecutor() as executor:
         table = executor.map(describe_bucket_worker, filter_collection(resources.s3.buckets, args))
     page_output(tabulate(table, args))
 
+
 buckets_parser = register_filtering_parser(buckets, parent=s3_parser)
 
+
 def lifecycle(args):
     if args.delete:
         return resources.s3.BucketLifecycle(args.bucket_name).delete()
     rule = defaultdict(list, Prefix=args.prefix, Status="Enabled")  # type: Dict[str, Any]
     if args.transition_to_infrequent_access is not None:
         rule["Transitions"].append(dict(StorageClass="STANDARD_IA", Days=args.transition_to_infrequent_access))
     if args.transition_to_glacier is not None:
         rule["Transitions"].append(dict(StorageClass="GLACIER", Days=args.transition_to_glacier))
     if args.expire is not None:
         rule["Expiration"] = dict(Days=args.expire)
     if args.abort_incomplete_multipart_upload is not None:
         rule["AbortIncompleteMultipartUpload"] = dict(DaysAfterInitiation=args.abort_incomplete_multipart_upload)
     if len(rule) > 2:
-        clients.s3.put_bucket_lifecycle_configuration(Bucket=args.bucket_name,
-                                                      LifecycleConfiguration=dict(Rules=[rule]))
+        clients.s3.put_bucket_lifecycle_configuration(
+            Bucket=args.bucket_name, LifecycleConfiguration=dict(Rules=[rule])
+        )
     try:
         for rule in resources.s3.BucketLifecycle(args.bucket_name).rules:
             print(json.dumps(rule))
     except ClientError as e:
         expect_error_codes(e, "NoSuchLifecycleConfiguration")
         logger.error("No lifecycle configuration for bucket %s", args.bucket_name)
 
+
 lifecycle_parser = register_parser(lifecycle, parent=s3_parser)
 lifecycle_parser.add_argument("bucket_name")
 lifecycle_parser.add_argument("--delete", action="store_true")
 lifecycle_parser.add_argument("--prefix", default="")
 lifecycle_parser.add_argument("--transition-to-infrequent-access", type=int, metavar="DAYS")
 lifecycle_parser.add_argument("--transition-to-glacier", type=int, metavar="DAYS")
 lifecycle_parser.add_argument("--expire", type=int, metavar="DAYS")
 lifecycle_parser.add_argument("--abort-incomplete-multipart-upload", type=int, metavar="DAYS")
 
+
 def cors(args):
     raise NotImplementedError()
 
+
 cors_parser = register_parser(cors, parent=s3_parser)
 cors_parser.add_argument("bucket_name")
 
+
 def select(args):
     """
     Select data from an S3 object using AWS S3 Select.
 
     See https://docs.aws.amazon.com/AmazonS3/latest/dev/selecting-content-from-objects.html.
 
     Example:
@@ -105,32 +145,36 @@
         aegea s3 select s3://my-bucket/data.json 'select * from S3Object[*].path'
     """
     _, _, bucket, key = args.s3_url.split("/", 3)
     input_serialization = {"JSON": {"Type": args.json_type.upper()}}
     if args.compression_type:
         input_serialization.update(CompressionType=args.compression_type)
 
-    res = clients.s3.select_object_content(Bucket=bucket,
-                                           Key=key,
-                                           Expression=args.expression,
-                                           ExpressionType="SQL",
-                                           InputSerialization=input_serialization,
-                                           OutputSerialization={"JSON": {"RecordDelimiter": "\n"}})
+    res = clients.s3.select_object_content(
+        Bucket=bucket,
+        Key=key,
+        Expression=args.expression,
+        ExpressionType="SQL",
+        InputSerialization=input_serialization,
+        OutputSerialization={"JSON": {"RecordDelimiter": "\n"}},
+    )
     for event in res["Payload"]:
         if "Records" in event:
             sys.stdout.buffer.write(event["Records"]["Payload"])
         elif "Stats" in event or "Progress" in event:
             logger.info(event)
 
+
 select_parser = register_parser(select, parent=s3_parser)
 select_parser.add_argument("s3_url")
 select_parser.add_argument("expression")
 select_parser.add_argument("--json-type", choices={"document", "lines"}, default="document")
 select_parser.add_argument("--compression-type", choices={"gzip", "bzip2"})
 
+
 def versions(args):
     """
     List versions of an object in a versioned S3 bucket.
 
     See https://docs.aws.amazon.com/AmazonS3/latest/dev/ObjectVersioning.html.
 
     Example:
@@ -141,14 +185,15 @@
     table = resources.s3.Bucket(bucket).object_versions.filter(Prefix=key)
     page_output(tabulate(table, args))
 
 
 versions_parser = register_listing_parser(versions, parent=s3_parser)
 versions_parser.add_argument("s3_url")
 
+
 def restore(args):
     """
     Restore a deleted object in a versioned S3 bucket.
 
     See https://docs.aws.amazon.com/AmazonS3/latest/dev/ObjectVersioning.html.
 
     Examples:
@@ -165,10 +210,11 @@
         elif version.is_latest and version.size is None:
             logger.critical("Deleting %s", version)
             version.delete()
             return
     else:
         raise AegeaException("No matching version found")
 
+
 restore_parser = register_parser(restore, parent=s3_parser)
 restore_parser.add_argument("s3_url")
 restore_parser.add_argument("version_id", nargs="?")
```

### Comparing `aegea-4.4.0/aegea/secrets.py` & `aegea-4.4.1/aegea/secrets.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/sfn.py` & `aegea-4.4.1/aegea/sfn.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/ssh.py` & `aegea-4.4.1/aegea/ssh.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/top.py` & `aegea-4.4.1/aegea/top.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/util/__init__.py` & `aegea-4.4.1/aegea/util/__init__.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/util/aws/__init__.py` & `aegea-4.4.1/aegea/util/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/util/aws/_boto3_loader.py` & `aegea-4.4.1/aegea/util/aws/_boto3_loader.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/util/aws/batch.py` & `aegea-4.4.1/aegea/util/aws/batch.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/util/aws/batch_events_lambda/app.py` & `aegea-4.4.1/aegea/util/aws/batch_events_lambda/app.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/util/aws/dns.py` & `aegea-4.4.1/aegea/util/aws/dns.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/util/aws/iam.py` & `aegea-4.4.1/aegea/util/aws/iam.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/util/aws/logs.py` & `aegea-4.4.1/aegea/util/aws/logs.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/util/aws/spot.py` & `aegea-4.4.1/aegea/util/aws/spot.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/util/aws/ssm.py` & `aegea-4.4.1/aegea/util/aws/ssm.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/util/cloudinit.py` & `aegea-4.4.1/aegea/util/cloudinit.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/util/constants.py` & `aegea-4.4.1/aegea/util/constants.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/util/crypto.py` & `aegea-4.4.1/aegea/util/crypto.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/util/printing.py` & `aegea-4.4.1/aegea/util/printing.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/util/ssh.py` & `aegea-4.4.1/aegea/util/ssh.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea/zones.py` & `aegea-4.4.1/aegea/zones.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/aegea.egg-info/PKG-INFO` & `aegea-4.4.1/aegea.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegea
-Version: 4.4.0
+Version: 4.4.1
 Summary: Amazon Web Services Operator Interface
 Home-page: https://github.com/kislyuk/aegea
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Platform: MacOS X
 Platform: Posix
```

### Comparing `aegea-4.4.0/aegea.egg-info/SOURCES.txt` & `aegea-4.4.1/aegea.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/common.mk` & `aegea-4.4.1/common.mk`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/scripts/aegea` & `aegea-4.4.1/scripts/aegea`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/scripts/aegea-build-image-for-mission` & `aegea-4.4.1/scripts/aegea-build-image-for-mission`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/scripts/aegea-rebuild-public-elb-sg` & `aegea-4.4.1/scripts/aegea-rebuild-public-elb-sg`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/scripts/aegea-ssh` & `aegea-4.4.1/scripts/aegea-ssh`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/scripts/pypi-apt-freeze` & `aegea-4.4.1/scripts/pypi-apt-freeze`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/setup.py` & `aegea-4.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `aegea-4.4.0/test/test.py` & `aegea-4.4.1/test/test.py`

 * *Files identical despite different names*

