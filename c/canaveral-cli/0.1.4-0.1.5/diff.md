# Comparing `tmp/canaveral_cli-0.1.4.tar.gz` & `tmp/canaveral_cli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canaveral_cli-0.1.4.tar", max compression
+gzip compressed data, was "canaveral_cli-0.1.5.tar", max compression
```

## Comparing `canaveral_cli-0.1.4.tar` & `canaveral_cli-0.1.5.tar`

### file list

```diff
@@ -1,80 +1,81 @@
--rw-r--r--   0        0        0    11337 2023-04-20 10:01:17.537352 canaveral_cli-0.1.4/LICENSE
--rw-r--r--   0        0        0     1063 2023-05-14 19:06:08.041164 canaveral_cli-0.1.4/README.md
--rw-r--r--   0        0        0     1550 2023-05-22 17:50:50.943498 canaveral_cli-0.1.4/canaveral_cli/__init__.py
--rw-r--r--   0        0        0      204 2023-05-22 17:30:04.733480 canaveral_cli-0.1.4/canaveral_cli/__main__.py
--rw-r--r--   0        0        0     2491 2023-05-24 21:22:27.706256 canaveral_cli-0.1.4/canaveral_cli/cli.py
--rw-r--r--   0        0        0    14194 2023-05-24 20:18:10.656263 canaveral_cli-0.1.4/canaveral_cli/create_oam.py
--rw-r--r--   0        0        0     6868 2023-05-22 17:29:51.893478 canaveral_cli-0.1.4/canaveral_cli/cue_parser.py
--rw-r--r--   0        0        0     3523 2023-05-22 18:08:16.403481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/component/cron-task.json
--rw-r--r--   0        0        0     2183 2023-05-22 18:08:16.693481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/component/daemon.json
--rw-r--r--   0        0        0      202 2023-05-22 18:08:16.943481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/component/k8s-objects.json
--rw-r--r--   0        0        0     2025 2023-05-22 18:08:17.493481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/component/task.json
--rw-r--r--   0        0        0     2370 2023-05-22 18:08:17.763481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/component/webservice.json
--rw-r--r--   0        0        0      471 2023-05-22 18:08:25.673481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/policy/apply-once.json
--rw-r--r--   0        0        0     1026 2023-05-22 18:08:25.963481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/policy/garbage-collect.json
--rw-r--r--   0        0        0      487 2023-05-22 18:08:26.193481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/policy/override.json
--rw-r--r--   0        0        0      312 2023-05-22 18:08:26.433481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/policy/read-only.json
--rw-r--r--   0        0        0      488 2023-05-22 18:08:26.683481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/policy/replication.json
--rw-r--r--   0        0        0      293 2023-05-22 18:08:26.933481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/policy/resource-update.json
--rw-r--r--   0        0        0      313 2023-05-22 18:08:27.193481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/policy/shared-resource.json
--rw-r--r--   0        0        0      310 2023-05-22 18:08:27.473481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/policy/take-over.json
--rw-r--r--   0        0        0      553 2023-05-22 18:08:27.723481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/policy/topology.json
--rw-r--r--   0        0        0      221 2023-05-22 18:08:18.793481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/annotations.json
--rw-r--r--   0        0        0      213 2023-05-22 18:08:19.063481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/command.json
--rw-r--r--   0        0        0      160 2023-05-22 18:08:19.323481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/container-image.json
--rw-r--r--   0        0        0      830 2023-05-22 18:08:19.583481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/cpuscaler.json
--rw-r--r--   0        0        0      205 2023-05-22 18:08:19.843481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/env.json
--rw-r--r--   0        0        0      680 2023-05-22 18:08:20.133481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/expose.json
--rw-r--r--   0        0        0     1380 2023-05-22 18:08:20.393481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/gateway.json
--rw-r--r--   0        0        0      274 2023-05-22 18:08:20.673481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/hostalias.json
--rw-r--r--   0        0        0      941 2023-05-22 18:08:20.933481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/hpa.json
--rw-r--r--   0        0        0     1329 2023-05-22 18:08:21.213481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/init-container.json
--rw-r--r--   0        0        0      510 2023-05-22 18:08:21.993481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/k8s-update-strategy.json
--rw-r--r--   0        0        0      205 2023-05-22 18:08:22.253481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/labels.json
--rw-r--r--   0        0        0      333 2023-05-22 18:08:22.513481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/lifecycle.json
--rw-r--r--   0        0        0      405 2023-05-22 18:08:23.103481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/pure-ingress.json
--rw-r--r--   0        0        0      702 2023-05-22 18:08:23.373481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/resource.json
--rw-r--r--   0        0        0      266 2023-05-22 18:08:23.623481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/scaler.json
--rw-r--r--   0        0        0      595 2023-05-22 18:08:23.883481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/service-account.json
--rw-r--r--   0        0        0     1121 2023-05-22 18:08:24.383481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/sidecar.json
--rw-r--r--   0        0        0      267 2023-05-22 18:08:24.643481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/startup-probe.json
--rw-r--r--   0        0        0      660 2023-05-22 18:08:24.903481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/storage.json
--rw-r--r--   0        0        0      288 2023-05-22 18:08:25.173481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/topologyspreadconstraints.json
--rw-r--r--   0        0        0      363 2023-05-22 18:08:28.253481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/apply-component.json
--rw-r--r--   0        0        0      374 2023-05-22 18:08:28.513481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/apply-deployment.json
--rw-r--r--   0        0        0      429 2023-05-22 18:08:28.783481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/apply-object.json
--rw-r--r--   0        0        0     1251 2023-05-22 18:08:29.073481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/apply-terraform-config.json
--rw-r--r--   0        0        0      287 2023-05-22 18:08:29.333481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/apply-terraform-provider.json
--rw-r--r--   0        0        0     1288 2023-05-22 18:08:29.663481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/build-push-image.json
--rw-r--r--   0        0        0      939 2023-05-22 18:08:29.943481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/check-metrics.json
--rw-r--r--   0        0        0      277 2023-05-22 18:08:30.223481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/clean-jobs.json
--rw-r--r--   0        0        0      908 2023-05-22 18:08:30.503481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/collect-service-endpoints.json
--rw-r--r--   0        0        0      530 2023-05-22 18:08:30.763481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/create-config.json
--rw-r--r--   0        0        0      309 2023-05-22 18:08:31.033481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/delete-config.json
--rw-r--r--   0        0        0      369 2023-05-22 18:08:31.303481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/depends-on-app.json
--rw-r--r--   0        0        0      429 2023-05-22 18:08:31.563481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/deploy-cloud-resource.json
--rw-r--r--   0        0        0      836 2023-05-22 18:08:31.823481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/deploy.json
--rw-r--r--   0        0        0      685 2023-05-22 18:08:32.093481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/export-data.json
--rw-r--r--   0        0        0      766 2023-05-22 18:08:32.343481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/export-service.json
--rw-r--r--   0        0        0      579 2023-05-22 18:08:32.603481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/export2config.json
--rw-r--r--   0        0        0      872 2023-05-22 18:08:32.883481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/export2secret.json
--rw-r--r--   0        0        0      427 2023-05-22 18:08:33.133481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/generate-jdbc-connection.json
--rw-r--r--   0        0        0      316 2023-05-22 18:08:33.393481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/list-config.json
--rw-r--r--   0        0        0      699 2023-05-22 18:08:33.643481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/notification.json
--rw-r--r--   0        0        0      190 2023-05-22 18:08:33.893481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/print-message-in-status.json
--rw-r--r--   0        0        0      305 2023-05-22 18:08:34.143481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/read-config.json
--rw-r--r--   0        0        0      817 2023-05-22 18:08:34.423481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/read-object.json
--rw-r--r--   0        0        0      374 2023-05-22 18:08:34.673481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/request.json
--rw-r--r--   0        0        0      596 2023-05-22 18:08:34.933481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/share-cloud-resource.json
--rw-r--r--   0        0        0      281 2023-05-22 18:08:35.183481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/step-group.json
--rw-r--r--   0        0        0      421 2023-05-22 18:08:35.453481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/suspend.json
--rw-r--r--   0        0        0      627 2023-05-22 18:08:35.713481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/vela-cli.json
--rw-r--r--   0        0        0      407 2023-05-22 18:08:35.983481 canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/webhook.json
--rw-r--r--   0        0        0     2558 2023-05-24 20:11:52.786262 canaveral_cli-0.1.4/canaveral_cli/data/raw_data.yaml
--rw-r--r--   0        0        0     1091 2023-05-14 19:06:08.091164 canaveral_cli-0.1.4/canaveral_cli/data/templates/vela_default.yaml
--rw-r--r--   0        0        0     1364 2023-05-21 11:24:22.059044 canaveral_cli-0.1.4/canaveral_cli/data/templates/vela_template.yaml.jinja
--rw-r--r--   0        0        0     2523 2023-05-22 18:02:51.603482 canaveral_cli-0.1.4/canaveral_cli/definitions.py
--rw-r--r--   0        0        0     1061 2023-05-24 21:16:16.806257 canaveral_cli-0.1.4/canaveral_cli/merge_oam.py
--rw-r--r--   0        0        0      777 2023-05-24 21:41:29.426278 canaveral_cli-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2340 2023-05-24 21:41:33.536062 canaveral_cli-0.1.4/setup.py
--rw-r--r--   0        0        0     1843 2023-05-24 21:41:33.536431 canaveral_cli-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-04-20 10:01:17.537352 canaveral_cli-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1063 2023-05-14 19:06:08.041164 canaveral_cli-0.1.5/README.md
+-rw-r--r--   0        0        0     1688 2023-05-25 20:25:55.944540 canaveral_cli-0.1.5/canaveral_cli/__init__.py
+-rw-r--r--   0        0        0      204 2023-05-22 17:30:04.733480 canaveral_cli-0.1.5/canaveral_cli/__main__.py
+-rw-r--r--   0        0        0     3024 2023-05-25 20:39:57.634527 canaveral_cli-0.1.5/canaveral_cli/cli.py
+-rw-r--r--   0        0        0    14194 2023-05-24 20:18:10.656263 canaveral_cli-0.1.5/canaveral_cli/create_oam.py
+-rw-r--r--   0        0        0     6868 2023-05-22 17:29:51.893478 canaveral_cli-0.1.5/canaveral_cli/cue_parser.py
+-rw-r--r--   0        0        0     3523 2023-05-22 18:08:16.403481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/component/cron-task.json
+-rw-r--r--   0        0        0     2183 2023-05-22 18:08:16.693481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/component/daemon.json
+-rw-r--r--   0        0        0      202 2023-05-22 18:08:16.943481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/component/k8s-objects.json
+-rw-r--r--   0        0        0     2025 2023-05-22 18:08:17.493481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/component/task.json
+-rw-r--r--   0        0        0     2370 2023-05-22 18:08:17.763481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/component/webservice.json
+-rw-r--r--   0        0        0      471 2023-05-22 18:08:25.673481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/policy/apply-once.json
+-rw-r--r--   0        0        0     1026 2023-05-22 18:08:25.963481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/policy/garbage-collect.json
+-rw-r--r--   0        0        0      487 2023-05-22 18:08:26.193481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/policy/override.json
+-rw-r--r--   0        0        0      312 2023-05-22 18:08:26.433481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/policy/read-only.json
+-rw-r--r--   0        0        0      488 2023-05-22 18:08:26.683481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/policy/replication.json
+-rw-r--r--   0        0        0      293 2023-05-22 18:08:26.933481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/policy/resource-update.json
+-rw-r--r--   0        0        0      313 2023-05-22 18:08:27.193481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/policy/shared-resource.json
+-rw-r--r--   0        0        0      310 2023-05-22 18:08:27.473481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/policy/take-over.json
+-rw-r--r--   0        0        0      553 2023-05-22 18:08:27.723481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/policy/topology.json
+-rw-r--r--   0        0        0      221 2023-05-22 18:08:18.793481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/annotations.json
+-rw-r--r--   0        0        0      213 2023-05-22 18:08:19.063481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/command.json
+-rw-r--r--   0        0        0      160 2023-05-22 18:08:19.323481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/container-image.json
+-rw-r--r--   0        0        0      830 2023-05-22 18:08:19.583481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/cpuscaler.json
+-rw-r--r--   0        0        0      205 2023-05-22 18:08:19.843481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/env.json
+-rw-r--r--   0        0        0      680 2023-05-22 18:08:20.133481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/expose.json
+-rw-r--r--   0        0        0     1380 2023-05-22 18:08:20.393481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/gateway.json
+-rw-r--r--   0        0        0      274 2023-05-22 18:08:20.673481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/hostalias.json
+-rw-r--r--   0        0        0      941 2023-05-22 18:08:20.933481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/hpa.json
+-rw-r--r--   0        0        0     1329 2023-05-22 18:08:21.213481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/init-container.json
+-rw-r--r--   0        0        0      510 2023-05-22 18:08:21.993481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/k8s-update-strategy.json
+-rw-r--r--   0        0        0      205 2023-05-22 18:08:22.253481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/labels.json
+-rw-r--r--   0        0        0      333 2023-05-22 18:08:22.513481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/lifecycle.json
+-rw-r--r--   0        0        0      405 2023-05-22 18:08:23.103481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/pure-ingress.json
+-rw-r--r--   0        0        0      702 2023-05-22 18:08:23.373481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/resource.json
+-rw-r--r--   0        0        0      266 2023-05-22 18:08:23.623481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/scaler.json
+-rw-r--r--   0        0        0      595 2023-05-22 18:08:23.883481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/service-account.json
+-rw-r--r--   0        0        0     1121 2023-05-22 18:08:24.383481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/sidecar.json
+-rw-r--r--   0        0        0      267 2023-05-22 18:08:24.643481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/startup-probe.json
+-rw-r--r--   0        0        0      660 2023-05-22 18:08:24.903481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/storage.json
+-rw-r--r--   0        0        0      288 2023-05-22 18:08:25.173481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/topologyspreadconstraints.json
+-rw-r--r--   0        0        0      363 2023-05-22 18:08:28.253481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/apply-component.json
+-rw-r--r--   0        0        0      374 2023-05-22 18:08:28.513481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/apply-deployment.json
+-rw-r--r--   0        0        0      429 2023-05-22 18:08:28.783481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/apply-object.json
+-rw-r--r--   0        0        0     1251 2023-05-22 18:08:29.073481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/apply-terraform-config.json
+-rw-r--r--   0        0        0      287 2023-05-22 18:08:29.333481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/apply-terraform-provider.json
+-rw-r--r--   0        0        0     1288 2023-05-22 18:08:29.663481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/build-push-image.json
+-rw-r--r--   0        0        0      939 2023-05-22 18:08:29.943481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/check-metrics.json
+-rw-r--r--   0        0        0      277 2023-05-22 18:08:30.223481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/clean-jobs.json
+-rw-r--r--   0        0        0      908 2023-05-22 18:08:30.503481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/collect-service-endpoints.json
+-rw-r--r--   0        0        0      530 2023-05-22 18:08:30.763481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/create-config.json
+-rw-r--r--   0        0        0      309 2023-05-22 18:08:31.033481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/delete-config.json
+-rw-r--r--   0        0        0      369 2023-05-22 18:08:31.303481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/depends-on-app.json
+-rw-r--r--   0        0        0      429 2023-05-22 18:08:31.563481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/deploy-cloud-resource.json
+-rw-r--r--   0        0        0      836 2023-05-22 18:08:31.823481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/deploy.json
+-rw-r--r--   0        0        0      685 2023-05-22 18:08:32.093481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/export-data.json
+-rw-r--r--   0        0        0      766 2023-05-22 18:08:32.343481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/export-service.json
+-rw-r--r--   0        0        0      579 2023-05-22 18:08:32.603481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/export2config.json
+-rw-r--r--   0        0        0      872 2023-05-22 18:08:32.883481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/export2secret.json
+-rw-r--r--   0        0        0      427 2023-05-22 18:08:33.133481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/generate-jdbc-connection.json
+-rw-r--r--   0        0        0      316 2023-05-22 18:08:33.393481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/list-config.json
+-rw-r--r--   0        0        0      699 2023-05-22 18:08:33.643481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/notification.json
+-rw-r--r--   0        0        0      190 2023-05-22 18:08:33.893481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/print-message-in-status.json
+-rw-r--r--   0        0        0      305 2023-05-22 18:08:34.143481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/read-config.json
+-rw-r--r--   0        0        0      817 2023-05-22 18:08:34.423481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/read-object.json
+-rw-r--r--   0        0        0      374 2023-05-22 18:08:34.673481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/request.json
+-rw-r--r--   0        0        0      596 2023-05-22 18:08:34.933481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/share-cloud-resource.json
+-rw-r--r--   0        0        0      281 2023-05-22 18:08:35.183481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/step-group.json
+-rw-r--r--   0        0        0      421 2023-05-22 18:08:35.453481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/suspend.json
+-rw-r--r--   0        0        0      627 2023-05-22 18:08:35.713481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/vela-cli.json
+-rw-r--r--   0        0        0      407 2023-05-22 18:08:35.983481 canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/webhook.json
+-rw-r--r--   0        0        0     2558 2023-05-24 20:11:52.786262 canaveral_cli-0.1.5/canaveral_cli/data/raw_data.yaml
+-rw-r--r--   0        0        0     1091 2023-05-14 19:06:08.091164 canaveral_cli-0.1.5/canaveral_cli/data/templates/vela_default.yaml
+-rw-r--r--   0        0        0     1364 2023-05-21 11:24:22.059044 canaveral_cli-0.1.5/canaveral_cli/data/templates/vela_template.yaml.jinja
+-rw-r--r--   0        0        0     2523 2023-05-22 18:02:51.603482 canaveral_cli-0.1.5/canaveral_cli/definitions.py
+-rw-r--r--   0        0        0      482 2023-05-25 20:40:27.404527 canaveral_cli-0.1.5/canaveral_cli/helper.py
+-rw-r--r--   0        0        0     1061 2023-05-24 21:16:16.806257 canaveral_cli-0.1.5/canaveral_cli/merge_oam.py
+-rw-r--r--   0        0        0      777 2023-05-26 08:13:32.548737 canaveral_cli-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2340 2023-05-26 08:14:08.524222 canaveral_cli-0.1.5/setup.py
+-rw-r--r--   0        0        0     1843 2023-05-26 08:14:08.524526 canaveral_cli-0.1.5/PKG-INFO
```

### Comparing `canaveral_cli-0.1.4/LICENSE` & `canaveral_cli-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/README.md` & `canaveral_cli-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/__init__.py` & `canaveral_cli-0.1.5/canaveral_cli/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Top-level package for Canaveral"""
 # canaveral_cli/__init__.py
 
 from dotenv import load_dotenv
 from pathlib import Path
+import logging
 
 load_dotenv()
 
 __app_name__ = "canaveral"
 __version__ = "0.1.0"
 PACKAGEDIR = Path(__file__).parent.absolute()
 
+logging.basicConfig(filename='canaveral.log', level=logging.INFO, format='%(asctime)s %(levelname)s %(name)s %(message)s')
 
 # COMPONENT_TYPES = ["webservice", "task", "cron-task", "daemon", "k8s-objects"]
 # TRAIT_TYPES = ["affinity", "annotations", "command", "container-image", "cpuscaler", "env", "expose", "gateway", "hostalias", "hpa", "init-container", "json-merge-patch", "json-patch",
 #                "k8s-update-strategy", "labels", "lifecycle", "nocalhost", "resource", "scaler", "service-account", "service-binding", "sidecar", "startup-probe", "storage", "topologyspreadconstraints"]
 # POLICY_TYPES = ["apply-once", "garbage-collect", "health", "override",
 #                 "read-only", "replication", "shared-resource", "take-over", "topology"]
 # WORKFLOWSTEP_TYPES = ["addon-operation", "apply-app", "apply-component", "apply-deployment", "apply-object", "apply-terraform-config", "apply-terraform-provider", "build-push-image", "clean-jobs", "collect-service-endpoints", "create-config", "delete-config", "depends-on-app", "deploy",
```

### Comparing `canaveral_cli-0.1.4/canaveral_cli/cli.py` & `canaveral_cli-0.1.5/canaveral_cli/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,66 @@
 """This module provides the Canaveral CLI"""
 # canaveral_cli/cli.py
 
+import logging
 from typing import Optional
 from pathlib import Path
 import typer
 import shutil
 import yaml
 from canaveral_cli import PACKAGEDIR, __app_name__, __version__
 from canaveral_cli.definitions import get_updated_type_data
+from canaveral_cli.helper import get_ammounts_oam_file
 from canaveral_cli.merge_oam import merge_oam
 from canaveral_cli.create_oam import oam_form, create_oam_file
 from rich import print
 
 app = typer.Typer()
 
 def _version_callback(value: bool):
     if value:
+        logging.info("version command")
         typer.echo(f"{__app_name__} v{__version__}")
         raise typer.Exit()
 
 @app.command()
 def definitions():
     """Retrieve OAM types from source and store them locally. Needed for creating OAM files"""
     get_updated_type_data()
 
 @app.command()
 def create():
     """Interactively Create a OAM file"""
+    logging.info("Start create command")
     oam_form_data = oam_form()
     # with open(PACKAGEDIR/"data/raw_data.yaml", "w") as f:
     #     yaml.dump(oam_form_data, f)
     #     f.close()
     # return
     # oam_form_data = yaml.load(open(PACKAGEDIR/"data/raw_data.yaml"), Loader=yaml.FullLoader)
+    
+    oam_numbers = get_ammounts_oam_file(oam_form_data)
+
+    # log the number of components, traits, policies, and workflowsteps
+    logging.info(f"create - comp: {oam_numbers[0]}, traits: {oam_numbers[1]}, policies: {oam_numbers[2]}, workflowsteps: {oam_numbers[3]}")
     create_oam_file(oam_form_data)
+    logging.info("End create command")
 
 @app.command()
 def default():
     """Create the default OAM file"""
+    logging.info("default command")
     shutil.copyfile(PACKAGEDIR/"data/templates/vela_default.yaml", "vela.yaml")
     print("✅ vela.yaml created successfully! ")
     
 @app.command()
 def merge(dev: Path = typer.Argument(..., exists=True, file_okay=True, dir_okay=False, readable=True, resolve_path=True),
           ops: Path = typer.Argument(..., exists=True, file_okay=True, dir_okay=False, readable=True, resolve_path=True)):
     """Merge Dev OAM file with Operations OAM file"""
+    logging.info("merge command")
     dev_yaml = yaml.load(dev.open(), Loader=yaml.FullLoader)
     ops_yaml = yaml.load(ops.open(), Loader=yaml.FullLoader)
 
     merged = merge_oam(dev_yaml, ops_yaml)
     
     with open("vela.yaml", "w") as f:
         yaml.dump(merged, f)
```

### Comparing `canaveral_cli-0.1.4/canaveral_cli/create_oam.py` & `canaveral_cli-0.1.5/canaveral_cli/create_oam.py`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/cue_parser.py` & `canaveral_cli-0.1.5/canaveral_cli/cue_parser.py`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/component/cron-task.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/component/cron-task.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/component/daemon.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/component/daemon.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/component/task.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/component/task.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/component/webservice.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/component/webservice.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/policy/garbage-collect.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/policy/garbage-collect.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/policy/topology.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/policy/topology.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/cpuscaler.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/cpuscaler.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/expose.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/expose.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/gateway.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/gateway.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/hpa.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/hpa.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/init-container.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/init-container.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/resource.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/resource.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/service-account.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/service-account.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/sidecar.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/sidecar.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/trait/storage.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/trait/storage.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/apply-terraform-config.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/apply-terraform-config.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/build-push-image.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/build-push-image.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/check-metrics.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/check-metrics.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/collect-service-endpoints.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/collect-service-endpoints.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/create-config.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/create-config.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/deploy.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/deploy.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/export-data.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/export-data.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/export-service.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/export-service.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/export2config.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/export2config.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/export2secret.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/export2secret.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/notification.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/notification.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/read-object.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/read-object.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/share-cloud-resource.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/share-cloud-resource.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/oam_types/workflowstep/vela-cli.json` & `canaveral_cli-0.1.5/canaveral_cli/data/oam_types/workflowstep/vela-cli.json`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/raw_data.yaml` & `canaveral_cli-0.1.5/canaveral_cli/data/raw_data.yaml`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/templates/vela_default.yaml` & `canaveral_cli-0.1.5/canaveral_cli/data/templates/vela_default.yaml`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/data/templates/vela_template.yaml.jinja` & `canaveral_cli-0.1.5/canaveral_cli/data/templates/vela_template.yaml.jinja`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/definitions.py` & `canaveral_cli-0.1.5/canaveral_cli/definitions.py`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/canaveral_cli/merge_oam.py` & `canaveral_cli-0.1.5/canaveral_cli/merge_oam.py`

 * *Files identical despite different names*

### Comparing `canaveral_cli-0.1.4/pyproject.toml` & `canaveral_cli-0.1.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "canaveral_cli"
-version = "0.1.4"
+version = "0.1.5"
 description = "Helper CLI to interact with Devscope's internal platform codename Canaveral"
 authors = ["André Gomes <andre.gomes@devscope.net>", "Hugo Sousa <hugo.sousa@devscope.net>", "Vitor Correia <vitor.correia@devscope.net>"]
 readme = "README.md"
 repository = "https://github.com/DevScope/canaveral-cli"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `canaveral_cli-0.1.4/setup.py` & `canaveral_cli-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'typer[all]>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['canaveral = canaveral_cli.cli:app']}
 
 setup_kwargs = {
     'name': 'canaveral-cli',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': "Helper CLI to interact with Devscope's internal platform codename Canaveral",
     'long_description': '# Canaveral CLI\n\nThis Project uses [Typer](https://typer.tiangolo.com/) for the CLI functionality and [InquirerPy](https://inquirerpy.readthedocs.io/en/latest/index.html#) for the parameter selection\n\n## Run it\nWorking with virtual envs in Python:\n- https://realpython.com/python-virtual-environments-a-primer\n- https://aaronlelevier.github.io/virtualenv-cheatsheet/\n\n```bash\n$ python3 -m venv venv --prompt="canaveral-env"\n$ source venv/bin/activate\n(canaveral-env) $ \n(canaveral-env) $ deactivate\n$ \n$ pip install -r requirements.txt\n$ OR\n$ python -m pip install -r requirements.txt\n```\n\n## How to contribuite\nProject layout to adhere to:\n- https://realpython.com/python-application-layouts/#command-line-application-layouts\n\n## Internal Notes\n\nDevscope Internal notes and documentation avaible at [Canaveral](https://devscope365.sharepoint.com/sites/academy/_layouts/OneNote.aspx?id=%2Fsites%2Facademy%2FSiteAssets%2FAcademy%20Notebook&wd=target%282023.one%7C1069493A-33E1-4F4C-8D77-28AA9AE54494%2FCanaveral%20CLI%7CF359B855-A8C4-4DB9-B416-CA0D700F2904%2F%29)\n',
     'author': 'André Gomes',
     'author_email': 'andre.gomes@devscope.net',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/DevScope/canaveral-cli',
```

### Comparing `canaveral_cli-0.1.4/PKG-INFO` & `canaveral_cli-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canaveral-cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: Helper CLI to interact with Devscope's internal platform codename Canaveral
 Home-page: https://github.com/DevScope/canaveral-cli
 Author: André Gomes
 Author-email: andre.gomes@devscope.net
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

