# Comparing `tmp/kcli-99.0.202305260939-py3-none-any.whl.zip` & `tmp/kcli-99.0.202305261953-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,603 +1,598 @@
-Zip file size: 1475828 bytes, number of entries: 601
--rw-r--r--  2.0 unx       15 b- defN 23-May-26 09:36 kvirt/__init__.py
--rw-r--r--  2.0 unx   100178 b- defN 23-May-26 09:36 kvirt/baseconfig.py
--rw-r--r--  2.0 unx   171487 b- defN 23-May-26 09:36 kvirt/bottle.py
--rw-r--r--  2.0 unx   249965 b- defN 23-May-26 09:36 kvirt/cli.py
--rw-r--r--  2.0 unx   185831 b- defN 23-May-26 09:36 kvirt/config.py
--rw-r--r--  2.0 unx     2851 b- defN 23-May-26 09:36 kvirt/containerconfig.py
--rw-r--r--  2.0 unx    11522 b- defN 23-May-26 09:36 kvirt/defaults.py
--rw-r--r--  2.0 unx    18835 b- defN 23-May-26 09:36 kvirt/examples.py
--rw-r--r--  2.0 unx     4333 b- defN 23-May-26 09:36 kvirt/ignitionmerger.py
--rw-r--r--  2.0 unx    10074 b- defN 23-May-26 09:36 kvirt/keywords.yaml
--rw-r--r--  2.0 unx     3487 b- defN 23-May-26 09:36 kvirt/klist.py
--rw-r--r--  2.0 unx     6009 b- defN 23-May-26 09:36 kvirt/ansibleutils/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-26 09:36 kvirt/cluster/__init__.py
--rw-r--r--  2.0 unx      931 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/99-apps.yaml
--rw-r--r--  2.0 unx      694 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/99-forcedns
--rw-r--r--  2.0 unx     1480 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/99-notifications.yaml
--rw-r--r--  2.0 unx      653 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/Corefile
--rw-r--r--  2.0 unx    42181 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/__init__.py
--rw-r--r--  2.0 unx     1121 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/assisted_infra.yml
--rw-r--r--  2.0 unx     1269 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/assisted_ingress.yml
--rw-r--r--  2.0 unx     1417 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/autoapprovercron.yml
--rw-r--r--  2.0 unx     1106 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/bmc.yml.j2
--rw-r--r--  2.0 unx      511 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/calico.sh.j2
--rw-r--r--  2.0 unx      200 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/cloud_lb_apps.yml
--rw-r--r--  2.0 unx      184 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/extras.service
--rw-r--r--  2.0 unx      839 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/extras.sh
--rw-r--r--  2.0 unx     2770 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/hostedcluster.yaml
--rw-r--r--  2.0 unx     1174 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/httpd.yaml
--rw-r--r--  2.0 unx      889 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/ignition.sh
--rw-r--r--  2.0 unx     2307 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/kcli_plan.yml
--rw-r--r--  2.0 unx     2070 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/kcli_plan_default.yml
--rw-r--r--  2.0 unx      502 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/keepalived.conf
--rw-r--r--  2.0 unx     1587 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/nmstateconfig.yml.j2
--rw-r--r--  2.0 unx      752 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/nodepool.yaml
--rw-r--r--  2.0 unx       60 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/nonlocalbind.conf
--rw-r--r--  2.0 unx     1992 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/staticpods/coredns.yml
--rw-r--r--  2.0 unx     2244 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/staticpods/keepalived.yml
--rw-r--r--  2.0 unx     1721 b- defN 23-May-26 09:36 kvirt/cluster/hypershift/staticpods/mdns.yml
--rw-r--r--  2.0 unx    11453 b- defN 23-May-26 09:36 kvirt/cluster/k3s/__init__.py
--rw-r--r--  2.0 unx     1248 b- defN 23-May-26 09:36 kvirt/cluster/k3s/bootstrap.sh
--rw-r--r--  2.0 unx     1050 b- defN 23-May-26 09:36 kvirt/cluster/k3s/bootstrap.yml
--rw-r--r--  2.0 unx      409 b- defN 23-May-26 09:36 kvirt/cluster/k3s/cloud_lb_api.yml
--rw-r--r--  2.0 unx      568 b- defN 23-May-26 09:36 kvirt/cluster/k3s/ctlplanes.sh
--rw-r--r--  2.0 unx     1329 b- defN 23-May-26 09:36 kvirt/cluster/k3s/ctlplanes.yml
--rw-r--r--  2.0 unx      214 b- defN 23-May-26 09:36 kvirt/cluster/k3s/gcp-hack.service
--rw-r--r--  2.0 unx      424 b- defN 23-May-26 09:36 kvirt/cluster/k3s/gcp-hack.sh
--rw-r--r--  2.0 unx      338 b- defN 23-May-26 09:36 kvirt/cluster/k3s/join.sh
--rw-r--r--  2.0 unx     1245 b- defN 23-May-26 09:36 kvirt/cluster/k3s/kcli_default.yml
--rw-r--r--  2.0 unx      511 b- defN 23-May-26 09:36 kvirt/cluster/k3s/keepalived.conf
--rw-r--r--  2.0 unx      352 b- defN 23-May-26 09:36 kvirt/cluster/k3s/keepalived.sh
--rw-r--r--  2.0 unx      240 b- defN 23-May-26 09:36 kvirt/cluster/k3s/workers.sh
--rw-r--r--  2.0 unx      914 b- defN 23-May-26 09:36 kvirt/cluster/k3s/workers.yml
--rw-r--r--  2.0 unx    13543 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/__init__.py
--rwxr-xr-x  2.0 unx     2707 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/bootstrap.sh
--rw-r--r--  2.0 unx     1621 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/bootstrap.yml
--rw-r--r--  2.0 unx      325 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/cloud_lb_api.yml
--rw-r--r--  2.0 unx     1367 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/ctlplanes.yml
--rwxr-xr-x  2.0 unx      417 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/deploy.sh
--rw-r--r--  2.0 unx      214 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/gcp-hack.service
--rw-r--r--  2.0 unx      355 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/gcp-hack.sh
--rwxr-xr-x  2.0 unx      412 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/join.sh
--rw-r--r--  2.0 unx     1822 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/kcli_default.yml
--rw-r--r--  2.0 unx      563 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/keepalived.conf
--rw-r--r--  2.0 unx      424 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/keepalived.sh
--rw-r--r--  2.0 unx      140 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/kubernetes.repo
--rw-r--r--  2.0 unx      179 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/multus.sh
--rw-r--r--  2.0 unx      572 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/nfs.sh
--rw-r--r--  2.0 unx      226 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/nfs.yml
--rw-r--r--  2.0 unx     4021 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/pre_el.sh
--rw-r--r--  2.0 unx     3906 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/pre_ubuntu.sh
--rw-r--r--  2.0 unx     2127 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/registry.yml
--rw-r--r--  2.0 unx     1154 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/workers.yml
--rw-r--r--  2.0 unx      487 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/argocd/ingress.yml
--rw-r--r--  2.0 unx     2134 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/argocd/install.sh
--rw-r--r--  2.0 unx       71 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/argocd/kcli_default.yml
--rw-r--r--  2.0 unx      314 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/argocd/uninstall.sh
--rw-r--r--  2.0 unx       90 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/autolabeller/install.sh
--rw-r--r--  2.0 unx       91 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/autolabeller/uninstall.sh
--rw-r--r--  2.0 unx      380 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/certmanager/install.sh
--rw-r--r--  2.0 unx      317 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/dashboard/admin.yml
--rw-r--r--  2.0 unx      452 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/dashboard/ingress.yml
--rw-r--r--  2.0 unx     1433 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/dashboard/install.sh
--rw-r--r--  2.0 unx       23 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/dashboard/kcli_default.yml
--rw-r--r--  2.0 unx      373 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/dashboard/user.yml
--rw-r--r--  2.0 unx      157 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/falco/falco_advertisements.yml
--rw-r--r--  2.0 unx      185 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/falco/falco_ip.yml
--rw-r--r--  2.0 unx      839 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/falco/install.sh
--rw-r--r--  2.0 unx       57 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/falco/kcli_default.yml
--rw-r--r--  2.0 unx      133 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/falco/uninstall.sh
--rw-r--r--  2.0 unx      175 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/ingress/install.sh
--rw-r--r--  2.0 unx      176 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/ingress/uninstall.sh
--rw-r--r--  2.0 unx      112 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/istio/install.sh
--rw-r--r--  2.0 unx      910 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/istio/istio-minimal-operator.yaml
--rw-r--r--  2.0 unx      766 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/katacontainer/install.sh
--rw-r--r--  2.0 unx      913 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/katacontainer/uninstall.sh
--rw-r--r--  2.0 unx      198 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/knative/cr_eventing.yml
--rw-r--r--  2.0 unx      194 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/knative/cr_serving.yml
--rw-r--r--  2.0 unx      253 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/knative/install.sh
--rw-r--r--  2.0 unx      670 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/kubevirt/install.sh
--rw-r--r--  2.0 unx       30 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/kubevirt/kcli_default.yml
--rw-r--r--  2.0 unx      534 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/metallb/install.sh
--rw-r--r--  2.0 unx       47 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/metallb/kcli_default.yml
--rw-r--r--  2.0 unx      157 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/metallb/metallb_advertisements.yml
--rw-r--r--  2.0 unx      150 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/metallb/metallb_cr.yml
--rw-r--r--  2.0 unx      283 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/metallb/uninstall.sh
--rw-r--r--  2.0 unx      348 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/olm/install.sh
--rw-r--r--  2.0 unx      350 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/olm/uninstall.sh
--rw-r--r--  2.0 unx      320 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/policy_as_code/install.sh
--rw-r--r--  2.0 unx       34 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/policy_as_code/kcli_default.yml
--rw-r--r--  2.0 unx      322 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/policy_as_code/uninstall.sh
--rw-r--r--  2.0 unx     1662 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/rancher/install.sh
--rw-r--r--  2.0 unx      103 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/rancher/kcli_default.yml
--rw-r--r--  2.0 unx      161 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/rancher/rancher_advertisements.yml
--rw-r--r--  2.0 unx      191 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/rancher/rancher_ip.yml
--rw-r--r--  2.0 unx      151 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/rancher/uninstall.sh
--rw-r--r--  2.0 unx      572 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/rook/install.sh
--rw-r--r--  2.0 unx      190 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/submariner/install.sh
--rw-r--r--  2.0 unx       22 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/submariner/kcli_default.yml
--rw-r--r--  2.0 unx      277 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/tekton/install.sh
--rw-r--r--  2.0 unx      278 b- defN 23-May-26 09:36 kvirt/cluster/kubeadm/apps/tekton/uninstall.sh
--rw-r--r--  2.0 unx     2970 b- defN 23-May-26 09:36 kvirt/cluster/kubecommon/__init__.py
--rw-r--r--  2.0 unx     9395 b- defN 23-May-26 09:36 kvirt/cluster/kubernetes/__init__.py
--rw-r--r--  2.0 unx     4805 b- defN 23-May-26 09:36 kvirt/cluster/microshift/__init__.py
--rw-r--r--  2.0 unx      603 b- defN 23-May-26 09:36 kvirt/cluster/microshift/kcli_plan.yml
--rw-r--r--  2.0 unx      625 b- defN 23-May-26 09:36 kvirt/cluster/microshift/kcli_plan_default.yml
--rw-r--r--  2.0 unx      262 b- defN 23-May-26 09:36 kvirt/cluster/microshift/scripts/00_sslip.sh
--rw-r--r--  2.0 unx      799 b- defN 23-May-26 09:36 kvirt/cluster/microshift/scripts/01_clients.sh
--rw-r--r--  2.0 unx      183 b- defN 23-May-26 09:36 kvirt/cluster/microshift/scripts/02_crio.sh
--rw-r--r--  2.0 unx      538 b- defN 23-May-26 09:36 kvirt/cluster/microshift/scripts/03_microshift.sh
--rw-r--r--  2.0 unx      341 b- defN 23-May-26 09:36 kvirt/cluster/microshift/scripts/04_kubeconfig.sh
--rw-r--r--  2.0 unx     2252 b- defN 23-May-26 09:36 kvirt/cluster/microshift/scripts/05_acm.sh
--rw-r--r--  2.0 unx      696 b- defN 23-May-26 09:36 kvirt/cluster/microshift/scripts/deploy.sh
--rw-r--r--  2.0 unx      219 b- defN 23-May-26 09:36 kvirt/cluster/openshift/01-workload-partitioning
--rw-r--r--  2.0 unx      573 b- defN 23-May-26 09:36 kvirt/cluster/openshift/10-node-ip-hint.yaml
--rw-r--r--  2.0 unx     1005 b- defN 23-May-26 09:36 kvirt/cluster/openshift/99-apps.yaml
--rw-r--r--  2.0 unx      618 b- defN 23-May-26 09:36 kvirt/cluster/openshift/99-bootstrap-deletion-2.yaml
--rw-r--r--  2.0 unx     1239 b- defN 23-May-26 09:36 kvirt/cluster/openshift/99-bootstrap-deletion.yaml
--rw-r--r--  2.0 unx      529 b- defN 23-May-26 09:36 kvirt/cluster/openshift/99-chrony.yaml
--rw-r--r--  2.0 unx      646 b- defN 23-May-26 09:36 kvirt/cluster/openshift/99-forcedns
--rw-r--r--  2.0 unx      476 b- defN 23-May-26 09:36 kvirt/cluster/openshift/99-forcedns-ibm
--rw-r--r--  2.0 unx      854 b- defN 23-May-26 09:36 kvirt/cluster/openshift/99-kubevirt-fix.yaml
--rw-r--r--  2.0 unx     1127 b- defN 23-May-26 09:36 kvirt/cluster/openshift/99-localhost-fix.yaml
--rw-r--r--  2.0 unx      250 b- defN 23-May-26 09:36 kvirt/cluster/openshift/99-metal3-fake-machine.yaml
--rw-r--r--  2.0 unx      162 b- defN 23-May-26 09:36 kvirt/cluster/openshift/99-metal3-provisioning.yaml
--rw-r--r--  2.0 unx     1659 b- defN 23-May-26 09:36 kvirt/cluster/openshift/99-notifications.yaml
--rw-r--r--  2.0 unx      118 b- defN 23-May-26 09:36 kvirt/cluster/openshift/99-operatorhub.yaml
--rw-r--r--  2.0 unx      314 b- defN 23-May-26 09:36 kvirt/cluster/openshift/99-ovn.yaml
--rw-r--r--  2.0 unx      912 b- defN 23-May-26 09:36 kvirt/cluster/openshift/99-sno.yaml
--rw-r--r--  2.0 unx      762 b- defN 23-May-26 09:36 kvirt/cluster/openshift/Corefile
--rw-r--r--  2.0 unx    81595 b- defN 23-May-26 09:36 kvirt/cluster/openshift/__init__.py
--rw-r--r--  2.0 unx     1326 b- defN 23-May-26 09:36 kvirt/cluster/openshift/autoapprovercron.yml
--rw-r--r--  2.0 unx      987 b- defN 23-May-26 09:36 kvirt/cluster/openshift/autorules.yml
--rw-r--r--  2.0 unx     1630 b- defN 23-May-26 09:36 kvirt/cluster/openshift/bootstrap.yml
--rw-r--r--  2.0 unx      250 b- defN 23-May-26 09:36 kvirt/cluster/openshift/calico.sh.j2
--rw-r--r--  2.0 unx      107 b- defN 23-May-26 09:36 kvirt/cluster/openshift/chrony.conf
--rw-r--r--  2.0 unx      629 b- defN 23-May-26 09:36 kvirt/cluster/openshift/cloud_bootstrap.yml
--rw-r--r--  2.0 unx     1086 b- defN 23-May-26 09:36 kvirt/cluster/openshift/cloud_ctlplanes.yml
--rw-r--r--  2.0 unx      217 b- defN 23-May-26 09:36 kvirt/cluster/openshift/cloud_dns.yml
--rw-r--r--  2.0 unx      616 b- defN 23-May-26 09:36 kvirt/cluster/openshift/cloud_lb_api.yml
--rw-r--r--  2.0 unx      204 b- defN 23-May-26 09:36 kvirt/cluster/openshift/cloud_lb_apps.yml
--rw-r--r--  2.0 unx      703 b- defN 23-May-26 09:36 kvirt/cluster/openshift/cloud_workers.yml
--rw-r--r--  2.0 unx      123 b- defN 23-May-26 09:36 kvirt/cluster/openshift/cluster-ingress-02-config.yml
--rw-r--r--  2.0 unx      159 b- defN 23-May-26 09:36 kvirt/cluster/openshift/cluster-scheduler-02-config.yml
--rw-r--r--  2.0 unx      224 b- defN 23-May-26 09:36 kvirt/cluster/openshift/config.hcl.templ
--rw-r--r--  2.0 unx       98 b- defN 23-May-26 09:36 kvirt/cluster/openshift/contrail-ca-patch.service
--rw-r--r--  2.0 unx      486 b- defN 23-May-26 09:36 kvirt/cluster/openshift/contrail-ca-patch.sh
--rw-r--r--  2.0 unx       87 b- defN 23-May-26 09:36 kvirt/cluster/openshift/contrail.auth
--rw-r--r--  2.0 unx     1108 b- defN 23-May-26 09:36 kvirt/cluster/openshift/contrail.sh.j2
--rw-r--r--  2.0 unx     2278 b- defN 23-May-26 09:36 kvirt/cluster/openshift/ctlplanes.yml
--rw-r--r--  2.0 unx      326 b- defN 23-May-26 09:36 kvirt/cluster/openshift/dhcp.conf
--rw-r--r--  2.0 unx      106 b- defN 23-May-26 09:36 kvirt/cluster/openshift/dhcp.sh
--rw-r--r--  2.0 unx      536 b- defN 23-May-26 09:36 kvirt/cluster/openshift/dhcp.yml
--rw-r--r--  2.0 unx      836 b- defN 23-May-26 09:36 kvirt/cluster/openshift/disconnected.yml
--rw-r--r--  2.0 unx     8945 b- defN 23-May-26 09:36 kvirt/cluster/openshift/fake_kubeconfig.json
--rw-r--r--  2.0 unx       35 b- defN 23-May-26 09:36 kvirt/cluster/openshift/fake_pull.json
--rw-r--r--  2.0 unx       24 b- defN 23-May-26 09:36 kvirt/cluster/openshift/gcp-hack.preset
--rw-r--r--  2.0 unx      320 b- defN 23-May-26 09:36 kvirt/cluster/openshift/gcp-hack.service
--rw-r--r--  2.0 unx      355 b- defN 23-May-26 09:36 kvirt/cluster/openshift/gcp-hack.sh
--rw-r--r--  2.0 unx     1792 b- defN 23-May-26 09:36 kvirt/cluster/openshift/haproxy.cfg
--rw-r--r--  2.0 unx     2483 b- defN 23-May-26 09:36 kvirt/cluster/openshift/haproxy.cfg.kubevirt
--rw-r--r--  2.0 unx      902 b- defN 23-May-26 09:36 kvirt/cluster/openshift/httpd.yaml
--rw-r--r--  2.0 unx      524 b- defN 23-May-26 09:36 kvirt/cluster/openshift/ignition.j2
--rw-r--r--  2.0 unx     3562 b- defN 23-May-26 09:36 kvirt/cluster/openshift/install-config.yaml
--rw-r--r--  2.0 unx     2691 b- defN 23-May-26 09:36 kvirt/cluster/openshift/iso.sh
--rw-r--r--  2.0 unx      237 b- defN 23-May-26 09:36 kvirt/cluster/openshift/kcli-ipv6.conf.j2
--rw-r--r--  2.0 unx     4257 b- defN 23-May-26 09:36 kvirt/cluster/openshift/kcli_default.yml
--rw-r--r--  2.0 unx      982 b- defN 23-May-26 09:36 kvirt/cluster/openshift/keepalived.conf
--rw-r--r--  2.0 unx       60 b- defN 23-May-26 09:36 kvirt/cluster/openshift/nonlocalbind.conf
--rw-r--r--  2.0 unx       59 b- defN 23-May-26 09:36 kvirt/cluster/openshift/openshift-workload-pinning
--rw-r--r--  2.0 unx      157 b- defN 23-May-26 09:36 kvirt/cluster/openshift/relocate-ip-bootstrap.service
--rw-r--r--  2.0 unx      281 b- defN 23-May-26 09:36 kvirt/cluster/openshift/relocate-ip-bootstrap.sh
--rw-r--r--  2.0 unx      690 b- defN 23-May-26 09:36 kvirt/cluster/openshift/relocate-ip.sh
--rw-r--r--  2.0 unx      212 b- defN 23-May-26 09:36 kvirt/cluster/openshift/sno-finish.service
--rw-r--r--  2.0 unx     2085 b- defN 23-May-26 09:36 kvirt/cluster/openshift/sno-finish.sh
--rw-r--r--  2.0 unx      660 b- defN 23-May-26 09:36 kvirt/cluster/openshift/sno.yml
--rw-r--r--  2.0 unx     1615 b- defN 23-May-26 09:36 kvirt/cluster/openshift/workers.yml
--rw-r--r--  2.0 unx       40 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/cr.sh
--rw-r--r--  2.0 unx      768 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/install.yml.j2
--rw-r--r--  2.0 unx      162 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/advanced-cluster-management/99-metal3-provisioning.yaml
--rw-r--r--  2.0 unx     2754 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sample.yml
--rwxr-xr-x  2.0 unx     2838 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sh
--rw-r--r--  2.0 unx      418 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/advanced-cluster-management/cr.yml
--rw-r--r--  2.0 unx      625 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/advanced-cluster-management/gen_registries.py
--rw-r--r--  2.0 unx      259 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/advanced-cluster-management/kcli_default.yml
--rw-r--r--  2.0 unx     1219 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/advanced-cluster-management/post.sh
--rw-r--r--  2.0 unx      645 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/argocd/configmap.yml
--rw-r--r--  2.0 unx     2423 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/argocd/install.sh
--rw-r--r--  2.0 unx       49 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/argocd/kcli_default.yml
--rw-r--r--  2.0 unx     1093 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/autolabeller/cr.yml
--rw-r--r--  2.0 unx      142 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/autolabeller/install.sh
--rw-r--r--  2.0 unx     1093 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/autolabeller/install.yml
--rw-r--r--  2.0 unx      165 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/autolabeller/kcli_default.yml
--rw-r--r--  2.0 unx       25 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/autolabeller/uninstall.sh
--rw-r--r--  2.0 unx      873 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/cluster-logging/cr.yml
--rw-r--r--  2.0 unx       63 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/cluster-logging/kcli_default.yml
--rw-r--r--  2.0 unx      265 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/istio/install.sh
--rw-r--r--  2.0 unx      377 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/istio/istio-cni.yaml
--rw-r--r--  2.0 unx     1039 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/kubevirt-hyperconverged/cr.yml
--rw-r--r--  2.0 unx      154 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/kubevirt-hyperconverged/kcli_default.yml
--rw-r--r--  2.0 unx      775 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/local-storage-operator/cr.yml
--rw-r--r--  2.0 unx      227 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/local-storage-operator/kcli_default.yml
--rw-r--r--  2.0 unx      642 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/local-storage-operator/post.sh
--rw-r--r--  2.0 unx      349 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/lvms-operator/cr.yml
--rw-r--r--  2.0 unx      137 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/lvms-operator/kcli_default.yml
--rw-r--r--  2.0 unx      595 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/lvms-operator/post.sh
--rw-r--r--  2.0 unx      510 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/metallb-operator/cr.yml
--rw-r--r--  2.0 unx       94 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/metallb-operator/kcli_default.yml
--rw-r--r--  2.0 unx      162 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/multicluster-engine/99-metal3-provisioning.yaml
--rw-r--r--  2.0 unx     2754 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sample.yml
--rwxr-xr-x  2.0 unx     2845 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sh
--rw-r--r--  2.0 unx      245 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/multicluster-engine/cr.yml
--rw-r--r--  2.0 unx      625 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/multicluster-engine/gen_registries.py
--rw-r--r--  2.0 unx      118 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/multicluster-engine/kcli_default.yml
--rwxr-xr-x  2.0 unx       55 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/multicluster-engine/post.sh
--rwxr-xr-x  2.0 unx     2298 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/nfs/install.sh
--rw-r--r--  2.0 unx      117 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/nfs/kcli_default.yml
--rw-r--r--  2.0 unx      185 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/nfs/uninstall.sh
--rw-r--r--  2.0 unx      849 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/odf-operator/cr.yml
--rw-r--r--  2.0 unx      298 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/odf-operator/kcli_default.yml
--rw-r--r--  2.0 unx      364 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/odf-operator/nad_cluster.yml
--rw-r--r--  2.0 unx      362 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/odf-operator/nad_public.yml
--rw-r--r--  2.0 unx      745 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/odf-operator/post.sh
--rw-r--r--  2.0 unx      530 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/odf-operator/pre.sh
--rw-r--r--  2.0 unx      363 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/serverless-operator/cr.yml
--rw-r--r--  2.0 unx      157 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/serverless-operator/kcli_default.yml
--rw-r--r--  2.0 unx      278 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/serverless-operator/post.sh
--rw-r--r--  2.0 unx     1227 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/users/install.sh
--rw-r--r--  2.0 unx       84 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/users/kcli_default.yml
--rw-r--r--  2.0 unx      258 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/users/oauth.yml
--rw-r--r--  2.0 unx      249 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/users/oauth_hypershift.yml
--rw-r--r--  2.0 unx      422 b- defN 23-May-26 09:36 kvirt/cluster/openshift/apps/users/uninstall.sh
--rw-r--r--  2.0 unx       60 b- defN 23-May-26 09:36 kvirt/cluster/openshift/customisation/00-kcli-namespace.yaml
--rw-r--r--  2.0 unx       91 b- defN 23-May-26 09:36 kvirt/cluster/openshift/customisation/97-autoapprovercron-sa.yaml
--rw-r--r--  2.0 unx      264 b- defN 23-May-26 09:36 kvirt/cluster/openshift/customisation/98-autoapprovercron-binding.yaml
--rw-r--r--  2.0 unx      912 b- defN 23-May-26 09:36 kvirt/cluster/openshift/customisation/99-autoapprovercron-cronjob.yaml
--rw-r--r--  2.0 unx      389 b- defN 23-May-26 09:36 kvirt/cluster/openshift/customisation/99-ingress-controller.yaml
--rw-r--r--  2.0 unx      184 b- defN 23-May-26 09:36 kvirt/cluster/openshift/customisation/99-monitoring.yaml
--rw-r--r--  2.0 unx      289 b- defN 23-May-26 09:36 kvirt/cluster/openshift/customisation/99-registry.yaml
--rw-r--r--  2.0 unx     1685 b- defN 23-May-26 09:36 kvirt/cluster/openshift/disconnected/haproxy.cfg
--rw-r--r--  2.0 unx      211 b- defN 23-May-26 09:36 kvirt/cluster/openshift/disconnected/registry.service
--rwxr-xr-x  2.0 unx      328 b- defN 23-May-26 09:36 kvirt/cluster/openshift/disconnected/bin/sync_image.sh
--rwxr-xr-x  2.0 unx      201 b- defN 23-May-26 09:36 kvirt/cluster/openshift/disconnected/scripts/01_get_oc.sh
--rwxr-xr-x  2.0 unx     2484 b- defN 23-May-26 09:36 kvirt/cluster/openshift/disconnected/scripts/03_mirror.sh
--rwxr-xr-x  2.0 unx     2046 b- defN 23-May-26 09:36 kvirt/cluster/openshift/disconnected/scripts/03_registry.sh
--rwxr-xr-x  2.0 unx      337 b- defN 23-May-26 09:36 kvirt/cluster/openshift/disconnected/scripts/04_extras.sh
--rwxr-xr-x  2.0 unx     2390 b- defN 23-May-26 09:36 kvirt/cluster/openshift/disconnected/scripts/05_olm.sh
--rwxr-xr-x  2.0 unx      241 b- defN 23-May-26 09:36 kvirt/cluster/openshift/disconnected/scripts/06_web.sh
--rwxr-xr-x  2.0 unx      733 b- defN 23-May-26 09:36 kvirt/cluster/openshift/disconnected/scripts/deploy.sh
--rw-r--r--  2.0 unx     1768 b- defN 23-May-26 09:36 kvirt/cluster/openshift/disconnected/scripts/mirror-config.yaml.sample
--rw-r--r--  2.0 unx     2557 b- defN 23-May-26 09:36 kvirt/cluster/openshift/staticpods/coredns.yml
--rw-r--r--  2.0 unx      987 b- defN 23-May-26 09:36 kvirt/cluster/openshift/staticpods/haproxy.yml
--rw-r--r--  2.0 unx     2539 b- defN 23-May-26 09:36 kvirt/cluster/openshift/staticpods/keepalived.yml
--rw-r--r--  2.0 unx     1721 b- defN 23-May-26 09:36 kvirt/cluster/openshift/staticpods/mdns.yml
--rw-r--r--  2.0 unx      193 b- defN 23-May-26 09:36 kvirt/cluster/profiles/sample-kubeadm-default.yml
--rw-r--r--  2.0 unx      135 b- defN 23-May-26 09:36 kvirt/cluster/profiles/sample-openshift-compact.yml
--rw-r--r--  2.0 unx      213 b- defN 23-May-26 09:36 kvirt/cluster/profiles/sample-openshift-contrail.yml
--rw-r--r--  2.0 unx      157 b- defN 23-May-26 09:36 kvirt/cluster/profiles/sample-openshift-ipv6.yml
--rw-r--r--  2.0 unx       55 b- defN 23-May-26 09:36 kvirt/cluster/profiles/sample-openshift-sno-bm.yml
--rw-r--r--  2.0 unx      148 b- defN 23-May-26 09:36 kvirt/cluster/profiles/sample-openshift-sno.yml
--rw-r--r--  2.0 unx     3377 b- defN 23-May-26 09:36 kvirt/common/Jenkinsfile.j2
--rw-r--r--  2.0 unx    96428 b- defN 23-May-26 09:36 kvirt/common/__init__.py
--rw-r--r--  2.0 unx     1406 b- defN 23-May-26 09:36 kvirt/common/autoscale.yaml.j2
--rw-r--r--  2.0 unx     8945 b- defN 23-May-26 09:36 kvirt/common/fake_kubeconfig.json
--rw-r--r--  2.0 unx      669 b- defN 23-May-26 09:36 kvirt/common/ignition.j2
--rw-r--r--  2.0 unx      125 b- defN 23-May-26 09:36 kvirt/common/kubevirt_kcli_conf.j2
--rw-r--r--  2.0 unx       99 b- defN 23-May-26 09:36 kvirt/common/local_kcli_conf.j2
--rw-r--r--  2.0 unx     3068 b- defN 23-May-26 09:36 kvirt/common/pipeline.yml.j2
--rw-r--r--  2.0 unx     2377 b- defN 23-May-26 09:36 kvirt/common/pipeline_kube.yml.j2
--rw-r--r--  2.0 unx     1381 b- defN 23-May-26 09:36 kvirt/common/playbook.j2
--rw-r--r--  2.0 unx     1557 b- defN 23-May-26 09:36 kvirt/common/storage.sh.j2
--rw-r--r--  2.0 unx     4562 b- defN 23-May-26 09:36 kvirt/common/vm.ovf.j2
--rw-r--r--  2.0 unx     2241 b- defN 23-May-26 09:36 kvirt/common/workflow.yml.j2
--rw-r--r--  2.0 unx     2208 b- defN 23-May-26 09:36 kvirt/common/workflow_script.yml.j2
--rw-r--r--  2.0 unx    15041 b- defN 23-May-26 09:36 kvirt/container/__init__.py
--rw-r--r--  2.0 unx    11716 b- defN 23-May-26 09:36 kvirt/expose/__init__.py
--rw-r--r--  2.0 unx     4319 b- defN 23-May-26 09:36 kvirt/expose/swagger.yml
--rw-r--r--  2.0 unx      408 b- defN 23-May-26 09:36 kvirt/expose/static/css/bootstrap-notify.css
--rw-r--r--  2.0 unx   121125 b- defN 23-May-26 09:36 kvirt/expose/static/css/bootstrap.min.css
--rw-r--r--  2.0 unx      399 b- defN 23-May-26 09:36 kvirt/expose/static/css/dataTables.checkboxes.css
--rw-r--r--  2.0 unx    13587 b- defN 23-May-26 09:36 kvirt/expose/static/css/jquery.dataTables.min.css
--rw-r--r--  2.0 unx      868 b- defN 23-May-26 09:36 kvirt/expose/static/css/kcli.css
--rw-r--r--  2.0 unx      269 b- defN 23-May-26 09:36 kvirt/expose/static/css/wheel.css
--rw-r--r--  2.0 unx     1406 b- defN 23-May-26 09:36 kvirt/expose/static/images/favicon.ico
--rw-r--r--  2.0 unx      160 b- defN 23-May-26 09:36 kvirt/expose/static/images/sort_asc.png
--rw-r--r--  2.0 unx      201 b- defN 23-May-26 09:36 kvirt/expose/static/images/sort_both.png
--rw-r--r--  2.0 unx      158 b- defN 23-May-26 09:36 kvirt/expose/static/images/sort_desc.png
--rw-r--r--  2.0 unx    24772 b- defN 23-May-26 09:36 kvirt/expose/static/images/wheel.gif
--rw-r--r--  2.0 unx    12398 b- defN 23-May-26 09:36 kvirt/expose/static/js/dataTables.checkboxes.min.js
--rw-r--r--  2.0 unx      367 b- defN 23-May-26 09:36 kvirt/expose/static/js/exposeactions.js
--rw-r--r--  2.0 unx    83059 b- defN 23-May-26 09:36 kvirt/expose/static/js/jquery.dataTables.min.js
--rw-r--r--  2.0 unx    89795 b- defN 23-May-26 09:36 kvirt/expose/static/js/jquery.min.js
--rw-r--r--  2.0 unx      263 b- defN 23-May-26 09:36 kvirt/expose/static/js/list.js
--rw-r--r--  2.0 unx     1605 b- defN 23-May-26 09:36 kvirt/expose/templates/form.html
--rw-r--r--  2.0 unx     1035 b- defN 23-May-26 09:36 kvirt/expose/templates/head.html
--rw-r--r--  2.0 unx      406 b- defN 23-May-26 09:36 kvirt/expose/templates/index.html
--rw-r--r--  2.0 unx     1220 b- defN 23-May-26 09:36 kvirt/expose/templates/infoplan.html
--rw-r--r--  2.0 unx      574 b- defN 23-May-26 09:36 kvirt/expose/templates/planstable.html
--rw-r--r--  2.0 unx      550 b- defN 23-May-26 09:36 kvirt/expose/templates/result.html
--rw-r--r--  2.0 unx     1754 b- defN 23-May-26 09:36 kvirt/internalplans/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-26 09:36 kvirt/jinjafilters/__init__.py
--rw-r--r--  2.0 unx     5249 b- defN 23-May-26 09:36 kvirt/jinjafilters/jinjafilters.py
--rw-r--r--  2.0 unx     8477 b- defN 23-May-26 09:36 kvirt/kfish/__init__.py
--rw-r--r--  2.0 unx     9124 b- defN 23-May-26 09:36 kvirt/ksushy/__init__.py
--rw-r--r--  2.0 unx      121 b- defN 23-May-26 09:36 kvirt/ksushy/main.py
--rw-r--r--  2.0 unx     1028 b- defN 23-May-26 09:36 kvirt/ksushy/templates/bios.json
--rw-r--r--  2.0 unx      443 b- defN 23-May-26 09:36 kvirt/ksushy/templates/interface.json
--rw-r--r--  2.0 unx      418 b- defN 23-May-26 09:36 kvirt/ksushy/templates/interfaces.json
--rw-r--r--  2.0 unx     1050 b- defN 23-May-26 09:36 kvirt/ksushy/templates/manager.json
--rw-r--r--  2.0 unx      571 b- defN 23-May-26 09:36 kvirt/ksushy/templates/managers.json
--rw-r--r--  2.0 unx      535 b- defN 23-May-26 09:36 kvirt/ksushy/templates/root.json
--rw-r--r--  2.0 unx     2732 b- defN 23-May-26 09:36 kvirt/ksushy/templates/system.json
--rw-r--r--  2.0 unx      511 b- defN 23-May-26 09:36 kvirt/ksushy/templates/systems.json
--rw-r--r--  2.0 unx     1219 b- defN 23-May-26 09:36 kvirt/ksushy/templates/virtualmedia_cd.json
--rw-r--r--  2.0 unx      705 b- defN 23-May-26 09:36 kvirt/ksushy/templates/virtualmedias.json
--rw-r--r--  2.0 unx     2780 b- defN 23-May-26 09:36 kvirt/miniconsole/__init__.py
--rw-r--r--  2.0 unx     3488 b- defN 23-May-26 09:36 kvirt/nameutils/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-26 09:36 kvirt/providers/__init__.py
--rw-r--r--  2.0 unx     8935 b- defN 23-May-26 09:36 kvirt/providers/sampleprovider.py
--rw-r--r--  2.0 unx    65799 b- defN 23-May-26 09:36 kvirt/providers/aws/__init__.py
--rw-r--r--  2.0 unx      479 b- defN 23-May-26 09:36 kvirt/providers/fake/__init__.py
--rw-r--r--  2.0 unx    65306 b- defN 23-May-26 09:36 kvirt/providers/gcp/__init__.py
--rw-r--r--  2.0 unx    65035 b- defN 23-May-26 09:36 kvirt/providers/ibm/__init__.py
--rw-r--r--  2.0 unx    80949 b- defN 23-May-26 09:36 kvirt/providers/kubevirt/__init__.py
--rw-r--r--  2.0 unx   184146 b- defN 23-May-26 09:36 kvirt/providers/kvm/__init__.py
--rw-r--r--  2.0 unx     1965 b- defN 23-May-26 09:36 kvirt/providers/kvm/helpers.py
--rw-r--r--  2.0 unx    57063 b- defN 23-May-26 09:36 kvirt/providers/openstack/__init__.py
--rw-r--r--  2.0 unx    62531 b- defN 23-May-26 09:36 kvirt/providers/ovirt/__init__.py
--rw-r--r--  2.0 unx    31099 b- defN 23-May-26 09:36 kvirt/providers/packet/__init__.py
--rw-r--r--  2.0 unx    73086 b- defN 23-May-26 09:36 kvirt/providers/vsphere/__init__.py
--rw-r--r--  2.0 unx    13655 b- defN 23-May-26 09:36 kvirt/providers/vsphere/helpers.py
--rw-r--r--  2.0 unx     4893 b- defN 23-May-26 09:36 kvirt/providers/vsphere/tagging.py
--rw-r--r--  2.0 unx    21273 b- defN 23-May-26 09:36 kvirt/providers/web/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-26 09:36 kvirt/version/__init__.py
--rw-r--r--  2.0 unx       19 b- defN 23-May-26 09:39 kvirt/version/git
--rw-r--r--  2.0 unx    46592 b- defN 23-May-26 09:36 kvirt/web/__init__.py
--rw-r--r--  2.0 unx      261 b- defN 23-May-26 09:36 kvirt/web/main.py
--rw-r--r--  2.0 unx      408 b- defN 23-May-26 09:36 kvirt/web/static/css/bootstrap-notify.css
--rw-r--r--  2.0 unx    23409 b- defN 23-May-26 09:36 kvirt/web/static/css/bootstrap-theme.min.css
--rw-r--r--  2.0 unx   121125 b- defN 23-May-26 09:36 kvirt/web/static/css/bootstrap.min.css
--rw-r--r--  2.0 unx      399 b- defN 23-May-26 09:36 kvirt/web/static/css/dataTables.checkboxes.css
--rw-r--r--  2.0 unx    13587 b- defN 23-May-26 09:36 kvirt/web/static/css/jquery.dataTables.min.css
--rw-r--r--  2.0 unx      816 b- defN 23-May-26 09:36 kvirt/web/static/css/kcli.css
--rw-r--r--  2.0 unx     3033 b- defN 23-May-26 09:36 kvirt/web/static/css/navbar.css
--rw-r--r--  2.0 unx     2908 b- defN 23-May-26 09:36 kvirt/web/static/css/spice.css
--rw-r--r--  2.0 unx      271 b- defN 23-May-26 09:36 kvirt/web/static/css/wheel.css
--rw-r--r--  2.0 unx    18028 b- defN 23-May-26 09:36 kvirt/web/static/fonts/glyphicons-halflings-regular.woff2
--rw-r--r--  2.0 unx      715 b- defN 23-May-26 09:36 kvirt/web/static/images/Centos.png
--rw-r--r--  2.0 unx      294 b- defN 23-May-26 09:36 kvirt/web/static/images/Debian.png
--rw-r--r--  2.0 unx      987 b- defN 23-May-26 09:36 kvirt/web/static/images/Fedora.png
--rw-r--r--  2.0 unx      672 b- defN 23-May-26 09:36 kvirt/web/static/images/Redhat.png
--rw-r--r--  2.0 unx     1278 b- defN 23-May-26 09:36 kvirt/web/static/images/Suse.png
--rw-r--r--  2.0 unx     1782 b- defN 23-May-26 09:36 kvirt/web/static/images/Tux.png
--rw-r--r--  2.0 unx      544 b- defN 23-May-26 09:36 kvirt/web/static/images/Ubuntu.png
--rw-r--r--  2.0 unx     4213 b- defN 23-May-26 09:36 kvirt/web/static/images/delete.png
--rw-r--r--  2.0 unx     1406 b- defN 23-May-26 09:36 kvirt/web/static/images/favicon.ico
--rw-r--r--  2.0 unx    23320 b- defN 23-May-26 09:36 kvirt/web/static/images/kcli-small.png
--rw-r--r--  2.0 unx    27185 b- defN 23-May-26 09:36 kvirt/web/static/images/kcli.jpg
--rw-r--r--  2.0 unx   113928 b- defN 23-May-26 09:36 kvirt/web/static/images/kcli.png
--rw-r--r--  2.0 unx    48809 b- defN 23-May-26 09:36 kvirt/web/static/images/logo-header.svg
--rw-r--r--  2.0 unx    48809 b- defN 23-May-26 09:36 kvirt/web/static/images/logo-main.svg
--rw-r--r--  2.0 unx      160 b- defN 23-May-26 09:36 kvirt/web/static/images/sort_asc.png
--rw-r--r--  2.0 unx      201 b- defN 23-May-26 09:36 kvirt/web/static/images/sort_both.png
--rw-r--r--  2.0 unx      158 b- defN 23-May-26 09:36 kvirt/web/static/images/sort_desc.png
--rw-r--r--  2.0 unx     3927 b- defN 23-May-26 09:36 kvirt/web/static/images/start.png
--rw-r--r--  2.0 unx     3631 b- defN 23-May-26 09:36 kvirt/web/static/images/stop.png
--rw-r--r--  2.0 unx    24772 b- defN 23-May-26 09:36 kvirt/web/static/images/wheel.gif
--rw-r--r--  2.0 unx     2933 b- defN 23-May-26 09:36 kvirt/web/static/js/bootstrap-notify.js
--rw-r--r--  2.0 unx    37045 b- defN 23-May-26 09:36 kvirt/web/static/js/bootstrap.min.js
--rw-r--r--  2.0 unx     2523 b- defN 23-May-26 09:36 kvirt/web/static/js/containeraction.js
--rw-r--r--  2.0 unx    12398 b- defN 23-May-26 09:36 kvirt/web/static/js/dataTables.checkboxes.min.js
--rw-r--r--  2.0 unx     1642 b- defN 23-May-26 09:36 kvirt/web/static/js/hostaction.js
--rw-r--r--  2.0 unx     1187 b- defN 23-May-26 09:36 kvirt/web/static/js/imageaction.js
--rw-r--r--  2.0 unx    83059 b- defN 23-May-26 09:36 kvirt/web/static/js/jquery.dataTables.min.js
--rw-r--r--  2.0 unx    89795 b- defN 23-May-26 09:36 kvirt/web/static/js/jquery.min.js
--rw-r--r--  2.0 unx     2704 b- defN 23-May-26 09:36 kvirt/web/static/js/kcli.js
--rw-r--r--  2.0 unx     1594 b- defN 23-May-26 09:36 kvirt/web/static/js/kubeaction.js
--rw-r--r--  2.0 unx     3907 b- defN 23-May-26 09:36 kvirt/web/static/js/list.js
--rw-r--r--  2.0 unx     1376 b- defN 23-May-26 09:36 kvirt/web/static/js/networkaction.js
--rw-r--r--  2.0 unx     2457 b- defN 23-May-26 09:36 kvirt/web/static/js/planaction.js
--rw-r--r--  2.0 unx     1237 b- defN 23-May-26 09:36 kvirt/web/static/js/poolaction.js
--rw-r--r--  2.0 unx      846 b- defN 23-May-26 09:36 kvirt/web/static/js/productaction.js
--rw-r--r--  2.0 unx      270 b- defN 23-May-26 09:36 kvirt/web/static/js/refresh.js
--rw-r--r--  2.0 unx     1835 b- defN 23-May-26 09:36 kvirt/web/static/js/repoaction.js
--rw-r--r--  2.0 unx     3463 b- defN 23-May-26 09:36 kvirt/web/static/js/snapshotaction.js
--rw-r--r--  2.0 unx     2745 b- defN 23-May-26 09:36 kvirt/web/static/js/vmaction.js
--rw-r--r--  2.0 unx      123 b- defN 23-May-26 09:36 kvirt/web/static/js/wheel.js
--rw-r--r--  2.0 unx     9944 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/atKeynames.js
--rw-r--r--  2.0 unx     2335 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/bitmap.js
--rw-r--r--  2.0 unx     4795 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/cursor.js
--rw-r--r--  2.0 unx    49214 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/display.js
--rw-r--r--  2.0 unx    13253 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/enums.js
--rw-r--r--  2.0 unx     2847 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/filexfer.js
--rw-r--r--  2.0 unx     9535 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/inputs.js
--rw-r--r--  2.0 unx     6176 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/lz.js
--rw-r--r--  2.0 unx    18370 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/main.js
--rw-r--r--  2.0 unx    12677 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/playback.js
--rw-r--r--  2.0 unx     7036 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/png.js
--rw-r--r--  2.0 unx     3110 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/port.js
--rw-r--r--  2.0 unx    44531 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/quic.js
--rw-r--r--  2.0 unx     3030 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/resize.js
--rw-r--r--  2.0 unx     7282 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/simulatecursor.js
--rw-r--r--  2.0 unx     1895 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/spicearraybuffer.js
--rw-r--r--  2.0 unx    18202 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/spiceconn.js
--rw-r--r--  2.0 unx     3616 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/spicedataview.js
--rw-r--r--  2.0 unx    33015 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/spicemsg.js
--rw-r--r--  2.0 unx    12767 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/spicetype.js
--rw-r--r--  2.0 unx     6808 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/ticket.js
--rw-r--r--  2.0 unx    13628 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/utils.js
--rw-r--r--  2.0 unx    21577 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/webm.js
--rw-r--r--  2.0 unx     4131 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/wire.js
--rw-r--r--  2.0 unx    16580 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/thirdparty/jsbn.js
--rw-r--r--  2.0 unx     2529 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/thirdparty/prng4.js
--rw-r--r--  2.0 unx     3442 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/thirdparty/rng.js
--rw-r--r--  2.0 unx     4257 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/thirdparty/rsa.js
--rw-r--r--  2.0 unx    10671 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/thirdparty/sha1.js
--rw-r--r--  2.0 unx        0 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/.npmignore
--rw-r--r--  2.0 unx      419 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/README.md
--rw-r--r--  2.0 unx      359 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/rollup.config.js
--rw-r--r--  2.0 unx     1113 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/babel-worker.js
--rw-r--r--  2.0 unx     8601 b- defN 23-May-26 09:36 kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/browser-es-module-loader.js
--rw-r--r--  2.0 unx     2176 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/error-handler.js
--rw-r--r--  2.0 unx     5682 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/localization.js
--rw-r--r--  2.0 unx    56845 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/ui.js
--rw-r--r--  2.0 unx     6696 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/webutil.js
--rw-r--r--  2.0 unx     3553 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/alt.svg
--rw-r--r--  2.0 unx     3980 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/clipboard.svg
--rw-r--r--  2.0 unx     3430 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/connect.svg
--rw-r--r--  2.0 unx     4381 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/ctrl.svg
--rw-r--r--  2.0 unx     3237 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/ctrlaltdel.svg
--rw-r--r--  2.0 unx     5062 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/disconnect.svg
--rw-r--r--  2.0 unx     4684 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/drag.svg
--rw-r--r--  2.0 unx     3106 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/error.svg
--rw-r--r--  2.0 unx     4522 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/esc.svg
--rw-r--r--  2.0 unx     3066 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/expander.svg
--rw-r--r--  2.0 unx     3139 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/fullscreen.svg
--rw-r--r--  2.0 unx     2559 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/handle.svg
--rw-r--r--  2.0 unx     6386 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/handle_bg.svg
--rw-r--r--  2.0 unx     3204 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/info.svg
--rw-r--r--  2.0 unx     6404 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/keyboard.svg
--rw-r--r--  2.0 unx     7000 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/mouse_left.svg
--rw-r--r--  2.0 unx     7002 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/mouse_middle.svg
--rw-r--r--  2.0 unx     6993 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/mouse_none.svg
--rw-r--r--  2.0 unx     7001 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/mouse_right.svg
--rw-r--r--  2.0 unx     3985 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/power.svg
--rw-r--r--  2.0 unx     3082 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/settings.svg
--rw-r--r--  2.0 unx     2953 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/tab.svg
--rw-r--r--  2.0 unx     4441 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/toggleextrakeys.svg
--rw-r--r--  2.0 unx     3869 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/warning.svg
--rw-r--r--  2.0 unx     3178 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/windows.svg
--rw-r--r--  2.0 unx      871 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/icons/Makefile
--rw-r--r--  2.0 unx     4028 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/icons/novnc-120x120.png
--rw-r--r--  2.0 unx     4582 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/icons/novnc-144x144.png
--rw-r--r--  2.0 unx     5216 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/icons/novnc-152x152.png
--rw-r--r--  2.0 unx      675 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/icons/novnc-16x16.png
--rw-r--r--  2.0 unx     5787 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/icons/novnc-192x192.png
--rw-r--r--  2.0 unx     1000 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/icons/novnc-24x24.png
--rw-r--r--  2.0 unx     1064 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/icons/novnc-32x32.png
--rw-r--r--  2.0 unx     1397 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/icons/novnc-48x48.png
--rw-r--r--  2.0 unx     1932 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/icons/novnc-60x60.png
--rw-r--r--  2.0 unx     1946 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/icons/novnc-64x64.png
--rw-r--r--  2.0 unx     2699 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/icons/novnc-72x72.png
--rw-r--r--  2.0 unx     2874 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/icons/novnc-76x76.png
--rw-r--r--  2.0 unx     2351 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/icons/novnc-96x96.png
--rw-r--r--  2.0 unx    11685 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/icons/novnc-icon-sm.svg
--rw-r--r--  2.0 unx    11549 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/images/icons/novnc-icon.svg
--rw-r--r--  2.0 unx     2885 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/locale/cs.json
--rw-r--r--  2.0 unx     2854 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/locale/de.json
--rw-r--r--  2.0 unx     3906 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/locale/el.json
--rw-r--r--  2.0 unx     2671 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/locale/es.json
--rw-r--r--  2.0 unx     3354 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/locale/ja.json
--rw-r--r--  2.0 unx     2961 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/locale/ko.json
--rw-r--r--  2.0 unx     3035 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/locale/nl.json
--rw-r--r--  2.0 unx     2830 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/locale/pl.json
--rw-r--r--  2.0 unx     3825 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/locale/ru.json
--rw-r--r--  2.0 unx     2845 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/locale/sv.json
--rw-r--r--  2.0 unx     2811 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/locale/tr.json
--rw-r--r--  2.0 unx     2597 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/locale/zh_CN.json
--rw-r--r--  2.0 unx     2606 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/locale/zh_TW.json
--rw-r--r--  2.0 unx      157 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/sounds/CREDITS
--rw-r--r--  2.0 unx     4531 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/sounds/bell.mp3
--rw-r--r--  2.0 unx     8495 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/sounds/bell.oga
--rw-r--r--  2.0 unx    38580 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/styles/Orbitron700.ttf
--rw-r--r--  2.0 unx    17472 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/styles/Orbitron700.woff
--rw-r--r--  2.0 unx    18450 b- defN 23-May-26 09:36 kvirt/web/static/vnc/app/styles/base.css
--rw-r--r--  2.0 unx     4189 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/base64.js
--rw-r--r--  2.0 unx    11241 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/des.js
--rw-r--r--  2.0 unx    20381 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/display.js
--rw-r--r--  2.0 unx     1374 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/encodings.js
--rw-r--r--  2.0 unx     1170 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/inflator.js
--rw-r--r--  2.0 unx    74196 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/rfb.js
--rw-r--r--  2.0 unx     9130 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/websock.js
--rw-r--r--  2.0 unx      628 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/decoders/copyrect.js
--rw-r--r--  2.0 unx     4814 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/decoders/hextile.js
--rw-r--r--  2.0 unx     1739 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/decoders/raw.js
--rw-r--r--  2.0 unx     1210 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/decoders/rre.js
--rw-r--r--  2.0 unx     9662 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/decoders/tight.js
--rw-r--r--  2.0 unx      768 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/decoders/tightpng.js
--rw-r--r--  2.0 unx    11438 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/input/domkeytable.js
--rw-r--r--  2.0 unx     3804 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/input/fixedkeys.js
--rw-r--r--  2.0 unx    13090 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/input/keyboard.js
--rw-r--r--  2.0 unx    34609 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/input/keysym.js
--rw-r--r--  2.0 unx    25374 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/input/keysymdef.js
--rw-r--r--  2.0 unx     9995 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/input/mouse.js
--rw-r--r--  2.0 unx     5283 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/input/util.js
--rw-r--r--  2.0 unx     2580 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/input/vkeys.js
--rw-r--r--  2.0 unx    14256 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/input/xtscancodes.js
--rw-r--r--  2.0 unx     3155 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/util/browser.js
--rw-r--r--  2.0 unx     7556 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/util/cursor.js
--rw-r--r--  2.0 unx     4221 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/util/events.js
--rw-r--r--  2.0 unx      896 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/util/eventtarget.js
--rw-r--r--  2.0 unx     1358 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/util/logging.js
--rw-r--r--  2.0 unx     1866 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/util/polyfill.js
--rw-r--r--  2.0 unx      301 b- defN 23-May-26 09:36 kvirt/web/static/vnc/core/util/strings.js
--rw-r--r--  2.0 unx     7388 b- defN 23-May-26 09:36 kvirt/web/static/vnc/vendor/promise.js
--rw-r--r--  2.0 unx      419 b- defN 23-May-26 09:36 kvirt/web/static/vnc/vendor/browser-es-module-loader/README.md
--rw-r--r--  2.0 unx      295 b- defN 23-May-26 09:36 kvirt/web/static/vnc/vendor/browser-es-module-loader/rollup.config.js
--rw-r--r--  2.0 unx     1113 b- defN 23-May-26 09:36 kvirt/web/static/vnc/vendor/browser-es-module-loader/src/babel-worker.js
--rw-r--r--  2.0 unx     8498 b- defN 23-May-26 09:36 kvirt/web/static/vnc/vendor/browser-es-module-loader/src/browser-es-module-loader.js
--rw-r--r--  2.0 unx     1084 b- defN 23-May-26 09:36 kvirt/web/static/vnc/vendor/pako/LICENSE
--rw-r--r--  2.0 unx      301 b- defN 23-May-26 09:36 kvirt/web/static/vnc/vendor/pako/README.md
--rw-r--r--  2.0 unx     1062 b- defN 23-May-26 09:36 kvirt/web/static/vnc/vendor/pako/lib/utils/common.js
--rw-r--r--  2.0 unx      666 b- defN 23-May-26 09:36 kvirt/web/static/vnc/vendor/pako/lib/zlib/adler32.js
--rw-r--r--  2.0 unx     1334 b- defN 23-May-26 09:36 kvirt/web/static/vnc/vendor/pako/lib/zlib/constants.js
--rw-r--r--  2.0 unx      764 b- defN 23-May-26 09:36 kvirt/web/static/vnc/vendor/pako/lib/zlib/crc32.js
--rw-r--r--  2.0 unx    60016 b- defN 23-May-26 09:36 kvirt/web/static/vnc/vendor/pako/lib/zlib/deflate.js
--rw-r--r--  2.0 unx     1251 b- defN 23-May-26 09:36 kvirt/web/static/vnc/vendor/pako/lib/zlib/gzheader.js
--rw-r--r--  2.0 unx    11690 b- defN 23-May-26 09:36 kvirt/web/static/vnc/vendor/pako/lib/zlib/inffast.js
--rw-r--r--  2.0 unx    47128 b- defN 23-May-26 09:36 kvirt/web/static/vnc/vendor/pako/lib/zlib/inflate.js
--rw-r--r--  2.0 unx    11527 b- defN 23-May-26 09:36 kvirt/web/static/vnc/vendor/pako/lib/zlib/inftrees.js
--rw-r--r--  2.0 unx      560 b- defN 23-May-26 09:36 kvirt/web/static/vnc/vendor/pako/lib/zlib/messages.js
--rw-r--r--  2.0 unx    38767 b- defN 23-May-26 09:36 kvirt/web/static/vnc/vendor/pako/lib/zlib/trees.js
--rw-r--r--  2.0 unx      823 b- defN 23-May-26 09:36 kvirt/web/static/vnc/vendor/pako/lib/zlib/zstream.js
--rw-r--r--  2.0 unx     2509 b- defN 23-May-26 09:36 kvirt/web/templates/bootstrap.html
--rw-r--r--  2.0 unx    14595 b- defN 23-May-26 09:36 kvirt/web/templates/console.html
--rw-r--r--  2.0 unx      717 b- defN 23-May-26 09:36 kvirt/web/templates/containercreate.html
--rw-r--r--  2.0 unx      493 b- defN 23-May-26 09:36 kvirt/web/templates/containerprofiles.html
--rw-r--r--  2.0 unx     1050 b- defN 23-May-26 09:36 kvirt/web/templates/containerprofilestable.html
--rw-r--r--  2.0 unx      490 b- defN 23-May-26 09:36 kvirt/web/templates/containers.html
--rw-r--r--  2.0 unx     1746 b- defN 23-May-26 09:36 kvirt/web/templates/containerstable.html
--rw-r--r--  2.0 unx     2123 b- defN 23-May-26 09:36 kvirt/web/templates/head.html
--rw-r--r--  2.0 unx      473 b- defN 23-May-26 09:36 kvirt/web/templates/hosts.html
--rw-r--r--  2.0 unx     1705 b- defN 23-May-26 09:36 kvirt/web/templates/hoststable.html
--rw-r--r--  2.0 unx     1119 b- defN 23-May-26 09:36 kvirt/web/templates/imagecreate.html
--rw-r--r--  2.0 unx      478 b- defN 23-May-26 09:36 kvirt/web/templates/images.html
--rw-r--r--  2.0 unx      646 b- defN 23-May-26 09:36 kvirt/web/templates/imagestable.html
--rw-r--r--  2.0 unx      472 b- defN 23-May-26 09:36 kvirt/web/templates/isos.html
--rw-r--r--  2.0 unx      261 b- defN 23-May-26 09:36 kvirt/web/templates/isostable.html
--rw-r--r--  2.0 unx      609 b- defN 23-May-26 09:36 kvirt/web/templates/kubecreate.html
--rw-r--r--  2.0 unx      622 b- defN 23-May-26 09:36 kvirt/web/templates/kubeinfo.html
--rw-r--r--  2.0 unx      488 b- defN 23-May-26 09:36 kvirt/web/templates/kubeprofiles.html
--rw-r--r--  2.0 unx      845 b- defN 23-May-26 09:36 kvirt/web/templates/kubeprofilestable.html
--rw-r--r--  2.0 unx      475 b- defN 23-May-26 09:36 kvirt/web/templates/kubes.html
--rw-r--r--  2.0 unx     1850 b- defN 23-May-26 09:36 kvirt/web/templates/kubestable.html
--rw-r--r--  2.0 unx      151 b- defN 23-May-26 09:36 kvirt/web/templates/layout.html
--rw-r--r--  2.0 unx     5517 b- defN 23-May-26 09:36 kvirt/web/templates/navbar.html
--rw-r--r--  2.0 unx      882 b- defN 23-May-26 09:36 kvirt/web/templates/networkcreate.html
--rw-r--r--  2.0 unx      537 b- defN 23-May-26 09:36 kvirt/web/templates/networks.html
--rw-r--r--  2.0 unx      845 b- defN 23-May-26 09:36 kvirt/web/templates/networkstable.html
--rw-r--r--  2.0 unx      750 b- defN 23-May-26 09:36 kvirt/web/templates/plancreate.html
--rw-r--r--  2.0 unx      475 b- defN 23-May-26 09:36 kvirt/web/templates/plans.html
--rw-r--r--  2.0 unx     1525 b- defN 23-May-26 09:36 kvirt/web/templates/planstable.html
--rw-r--r--  2.0 unx      859 b- defN 23-May-26 09:36 kvirt/web/templates/poolcreate.html
--rw-r--r--  2.0 unx      475 b- defN 23-May-26 09:36 kvirt/web/templates/pools.html
--rw-r--r--  2.0 unx      554 b- defN 23-May-26 09:36 kvirt/web/templates/poolstable.html
--rw-r--r--  2.0 unx     1282 b- defN 23-May-26 09:36 kvirt/web/templates/productcreate.html
--rw-r--r--  2.0 unx      484 b- defN 23-May-26 09:36 kvirt/web/templates/products.html
--rw-r--r--  2.0 unx      895 b- defN 23-May-26 09:36 kvirt/web/templates/productstable.html
--rw-r--r--  2.0 unx      699 b- defN 23-May-26 09:36 kvirt/web/templates/repocreate.html
--rw-r--r--  2.0 unx      475 b- defN 23-May-26 09:36 kvirt/web/templates/repos.html
--rw-r--r--  2.0 unx     1203 b- defN 23-May-26 09:36 kvirt/web/templates/repostable.html
--rw-r--r--  2.0 unx      958 b- defN 23-May-26 09:36 kvirt/web/templates/vmcreate.html
--rw-r--r--  2.0 unx      486 b- defN 23-May-26 09:36 kvirt/web/templates/vmprofiles.html
--rw-r--r--  2.0 unx     1420 b- defN 23-May-26 09:36 kvirt/web/templates/vmprofilestable.html
--rw-r--r--  2.0 unx      470 b- defN 23-May-26 09:36 kvirt/web/templates/vms.html
--rw-r--r--  2.0 unx     4894 b- defN 23-May-26 09:36 kvirt/web/templates/vmstable.html
--rw-r--r--  2.0 unx    11358 b- defN 23-May-26 09:39 kcli-99.0.202305260939.dist-info/LICENSE
--rw-r--r--  2.0 unx     2914 b- defN 23-May-26 09:39 kcli-99.0.202305260939.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-26 09:39 kcli-99.0.202305260939.dist-info/WHEEL
--rw-r--r--  2.0 unx      209 b- defN 23-May-26 09:39 kcli-99.0.202305260939.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-May-26 09:39 kcli-99.0.202305260939.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    58990 b- defN 23-May-26 09:39 kcli-99.0.202305260939.dist-info/RECORD
-601 files, 4548391 bytes uncompressed, 1380070 bytes compressed:  69.7%
+Zip file size: 1473841 bytes, number of entries: 596
+-rw-r--r--  2.0 unx       15 b- defN 23-May-26 19:51 kvirt/__init__.py
+-rw-r--r--  2.0 unx   100178 b- defN 23-May-26 19:51 kvirt/baseconfig.py
+-rw-r--r--  2.0 unx   171487 b- defN 23-May-26 19:51 kvirt/bottle.py
+-rw-r--r--  2.0 unx   249965 b- defN 23-May-26 19:51 kvirt/cli.py
+-rw-r--r--  2.0 unx   185831 b- defN 23-May-26 19:51 kvirt/config.py
+-rw-r--r--  2.0 unx     2851 b- defN 23-May-26 19:51 kvirt/containerconfig.py
+-rw-r--r--  2.0 unx    11522 b- defN 23-May-26 19:51 kvirt/defaults.py
+-rw-r--r--  2.0 unx    18835 b- defN 23-May-26 19:51 kvirt/examples.py
+-rw-r--r--  2.0 unx     4333 b- defN 23-May-26 19:51 kvirt/ignitionmerger.py
+-rw-r--r--  2.0 unx    10074 b- defN 23-May-26 19:51 kvirt/keywords.yaml
+-rw-r--r--  2.0 unx     3487 b- defN 23-May-26 19:51 kvirt/klist.py
+-rw-r--r--  2.0 unx     6009 b- defN 23-May-26 19:51 kvirt/ansibleutils/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-26 19:51 kvirt/cluster/__init__.py
+-rw-r--r--  2.0 unx      931 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/99-apps.yaml
+-rw-r--r--  2.0 unx      694 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/99-forcedns
+-rw-r--r--  2.0 unx     1480 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/99-notifications.yaml
+-rw-r--r--  2.0 unx      653 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/Corefile
+-rw-r--r--  2.0 unx    42181 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/__init__.py
+-rw-r--r--  2.0 unx     1121 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/assisted_infra.yml
+-rw-r--r--  2.0 unx     1269 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/assisted_ingress.yml
+-rw-r--r--  2.0 unx     1417 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/autoapprovercron.yml
+-rw-r--r--  2.0 unx     1106 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/bmc.yml.j2
+-rw-r--r--  2.0 unx      511 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/calico.sh.j2
+-rw-r--r--  2.0 unx      200 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/cloud_lb_apps.yml
+-rw-r--r--  2.0 unx      184 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/extras.service
+-rw-r--r--  2.0 unx      839 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/extras.sh
+-rw-r--r--  2.0 unx     2770 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/hostedcluster.yaml
+-rw-r--r--  2.0 unx     1174 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/httpd.yaml
+-rw-r--r--  2.0 unx      889 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/ignition.sh
+-rw-r--r--  2.0 unx     2307 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/kcli_plan.yml
+-rw-r--r--  2.0 unx     2070 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/kcli_plan_default.yml
+-rw-r--r--  2.0 unx      502 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/keepalived.conf
+-rw-r--r--  2.0 unx     1587 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/nmstateconfig.yml.j2
+-rw-r--r--  2.0 unx      752 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/nodepool.yaml
+-rw-r--r--  2.0 unx       60 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/nonlocalbind.conf
+-rw-r--r--  2.0 unx     1992 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/staticpods/coredns.yml
+-rw-r--r--  2.0 unx     2244 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/staticpods/keepalived.yml
+-rw-r--r--  2.0 unx     1721 b- defN 23-May-26 19:51 kvirt/cluster/hypershift/staticpods/mdns.yml
+-rw-r--r--  2.0 unx    11453 b- defN 23-May-26 19:51 kvirt/cluster/k3s/__init__.py
+-rw-r--r--  2.0 unx     1117 b- defN 23-May-26 19:51 kvirt/cluster/k3s/bootstrap.sh
+-rw-r--r--  2.0 unx     1050 b- defN 23-May-26 19:51 kvirt/cluster/k3s/bootstrap.yml
+-rw-r--r--  2.0 unx      409 b- defN 23-May-26 19:51 kvirt/cluster/k3s/cloud_lb_api.yml
+-rw-r--r--  2.0 unx      438 b- defN 23-May-26 19:51 kvirt/cluster/k3s/ctlplanes.sh
+-rw-r--r--  2.0 unx     1068 b- defN 23-May-26 19:51 kvirt/cluster/k3s/ctlplanes.yml
+-rw-r--r--  2.0 unx      338 b- defN 23-May-26 19:51 kvirt/cluster/k3s/join.sh
+-rw-r--r--  2.0 unx     1245 b- defN 23-May-26 19:51 kvirt/cluster/k3s/kcli_default.yml
+-rw-r--r--  2.0 unx      511 b- defN 23-May-26 19:51 kvirt/cluster/k3s/keepalived.conf
+-rw-r--r--  2.0 unx      352 b- defN 23-May-26 19:51 kvirt/cluster/k3s/keepalived.sh
+-rw-r--r--  2.0 unx      166 b- defN 23-May-26 19:51 kvirt/cluster/k3s/workers.sh
+-rw-r--r--  2.0 unx      709 b- defN 23-May-26 19:51 kvirt/cluster/k3s/workers.yml
+-rw-r--r--  2.0 unx    13543 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/__init__.py
+-rwxr-xr-x  2.0 unx     2707 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/bootstrap.sh
+-rw-r--r--  2.0 unx     1621 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/bootstrap.yml
+-rw-r--r--  2.0 unx      325 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/cloud_lb_api.yml
+-rw-r--r--  2.0 unx     1172 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/ctlplanes.yml
+-rwxr-xr-x  2.0 unx      343 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/deploy.sh
+-rwxr-xr-x  2.0 unx      412 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/join.sh
+-rw-r--r--  2.0 unx     1822 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/kcli_default.yml
+-rw-r--r--  2.0 unx      563 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/keepalived.conf
+-rw-r--r--  2.0 unx      424 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/keepalived.sh
+-rw-r--r--  2.0 unx      140 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/kubernetes.repo
+-rw-r--r--  2.0 unx      179 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/multus.sh
+-rw-r--r--  2.0 unx      572 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/nfs.sh
+-rw-r--r--  2.0 unx      226 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/nfs.yml
+-rw-r--r--  2.0 unx     4021 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/pre_el.sh
+-rw-r--r--  2.0 unx     3906 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/pre_ubuntu.sh
+-rw-r--r--  2.0 unx     2127 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/registry.yml
+-rw-r--r--  2.0 unx      949 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/workers.yml
+-rw-r--r--  2.0 unx      487 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/argocd/ingress.yml
+-rw-r--r--  2.0 unx     2134 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/argocd/install.sh
+-rw-r--r--  2.0 unx       71 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/argocd/kcli_default.yml
+-rw-r--r--  2.0 unx      314 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/argocd/uninstall.sh
+-rw-r--r--  2.0 unx       90 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/autolabeller/install.sh
+-rw-r--r--  2.0 unx       91 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/autolabeller/uninstall.sh
+-rw-r--r--  2.0 unx      380 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/certmanager/install.sh
+-rw-r--r--  2.0 unx      317 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/dashboard/admin.yml
+-rw-r--r--  2.0 unx      452 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/dashboard/ingress.yml
+-rw-r--r--  2.0 unx     1433 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/dashboard/install.sh
+-rw-r--r--  2.0 unx       23 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/dashboard/kcli_default.yml
+-rw-r--r--  2.0 unx      373 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/dashboard/user.yml
+-rw-r--r--  2.0 unx      157 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/falco/falco_advertisements.yml
+-rw-r--r--  2.0 unx      185 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/falco/falco_ip.yml
+-rw-r--r--  2.0 unx      839 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/falco/install.sh
+-rw-r--r--  2.0 unx       57 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/falco/kcli_default.yml
+-rw-r--r--  2.0 unx      133 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/falco/uninstall.sh
+-rw-r--r--  2.0 unx      175 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/ingress/install.sh
+-rw-r--r--  2.0 unx      176 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/ingress/uninstall.sh
+-rw-r--r--  2.0 unx      112 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/istio/install.sh
+-rw-r--r--  2.0 unx      910 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/istio/istio-minimal-operator.yaml
+-rw-r--r--  2.0 unx      766 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/katacontainer/install.sh
+-rw-r--r--  2.0 unx      913 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/katacontainer/uninstall.sh
+-rw-r--r--  2.0 unx      198 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/knative/cr_eventing.yml
+-rw-r--r--  2.0 unx      194 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/knative/cr_serving.yml
+-rw-r--r--  2.0 unx      253 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/knative/install.sh
+-rw-r--r--  2.0 unx      670 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/kubevirt/install.sh
+-rw-r--r--  2.0 unx       30 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/kubevirt/kcli_default.yml
+-rw-r--r--  2.0 unx      534 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/metallb/install.sh
+-rw-r--r--  2.0 unx       47 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/metallb/kcli_default.yml
+-rw-r--r--  2.0 unx      157 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/metallb/metallb_advertisements.yml
+-rw-r--r--  2.0 unx      150 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/metallb/metallb_cr.yml
+-rw-r--r--  2.0 unx      283 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/metallb/uninstall.sh
+-rw-r--r--  2.0 unx      348 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/olm/install.sh
+-rw-r--r--  2.0 unx      350 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/olm/uninstall.sh
+-rw-r--r--  2.0 unx      320 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/policy_as_code/install.sh
+-rw-r--r--  2.0 unx       34 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/policy_as_code/kcli_default.yml
+-rw-r--r--  2.0 unx      322 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/policy_as_code/uninstall.sh
+-rw-r--r--  2.0 unx     1662 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/rancher/install.sh
+-rw-r--r--  2.0 unx      103 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/rancher/kcli_default.yml
+-rw-r--r--  2.0 unx      161 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/rancher/rancher_advertisements.yml
+-rw-r--r--  2.0 unx      191 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/rancher/rancher_ip.yml
+-rw-r--r--  2.0 unx      151 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/rancher/uninstall.sh
+-rw-r--r--  2.0 unx      572 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/rook/install.sh
+-rw-r--r--  2.0 unx      190 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/submariner/install.sh
+-rw-r--r--  2.0 unx       22 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/submariner/kcli_default.yml
+-rw-r--r--  2.0 unx      277 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/tekton/install.sh
+-rw-r--r--  2.0 unx      278 b- defN 23-May-26 19:51 kvirt/cluster/kubeadm/apps/tekton/uninstall.sh
+-rw-r--r--  2.0 unx     2970 b- defN 23-May-26 19:51 kvirt/cluster/kubecommon/__init__.py
+-rw-r--r--  2.0 unx     9395 b- defN 23-May-26 19:51 kvirt/cluster/kubernetes/__init__.py
+-rw-r--r--  2.0 unx     4805 b- defN 23-May-26 19:51 kvirt/cluster/microshift/__init__.py
+-rw-r--r--  2.0 unx      603 b- defN 23-May-26 19:51 kvirt/cluster/microshift/kcli_plan.yml
+-rw-r--r--  2.0 unx      625 b- defN 23-May-26 19:51 kvirt/cluster/microshift/kcli_plan_default.yml
+-rw-r--r--  2.0 unx      262 b- defN 23-May-26 19:51 kvirt/cluster/microshift/scripts/00_sslip.sh
+-rw-r--r--  2.0 unx      799 b- defN 23-May-26 19:51 kvirt/cluster/microshift/scripts/01_clients.sh
+-rw-r--r--  2.0 unx      183 b- defN 23-May-26 19:51 kvirt/cluster/microshift/scripts/02_crio.sh
+-rw-r--r--  2.0 unx      538 b- defN 23-May-26 19:51 kvirt/cluster/microshift/scripts/03_microshift.sh
+-rw-r--r--  2.0 unx      341 b- defN 23-May-26 19:51 kvirt/cluster/microshift/scripts/04_kubeconfig.sh
+-rw-r--r--  2.0 unx     2252 b- defN 23-May-26 19:51 kvirt/cluster/microshift/scripts/05_acm.sh
+-rw-r--r--  2.0 unx      696 b- defN 23-May-26 19:51 kvirt/cluster/microshift/scripts/deploy.sh
+-rw-r--r--  2.0 unx      219 b- defN 23-May-26 19:51 kvirt/cluster/openshift/01-workload-partitioning
+-rw-r--r--  2.0 unx      573 b- defN 23-May-26 19:51 kvirt/cluster/openshift/10-node-ip-hint.yaml
+-rw-r--r--  2.0 unx     1005 b- defN 23-May-26 19:51 kvirt/cluster/openshift/99-apps.yaml
+-rw-r--r--  2.0 unx      618 b- defN 23-May-26 19:51 kvirt/cluster/openshift/99-bootstrap-deletion-2.yaml
+-rw-r--r--  2.0 unx     1239 b- defN 23-May-26 19:51 kvirt/cluster/openshift/99-bootstrap-deletion.yaml
+-rw-r--r--  2.0 unx      529 b- defN 23-May-26 19:51 kvirt/cluster/openshift/99-chrony.yaml
+-rw-r--r--  2.0 unx      646 b- defN 23-May-26 19:51 kvirt/cluster/openshift/99-forcedns
+-rw-r--r--  2.0 unx      476 b- defN 23-May-26 19:51 kvirt/cluster/openshift/99-forcedns-ibm
+-rw-r--r--  2.0 unx      854 b- defN 23-May-26 19:51 kvirt/cluster/openshift/99-kubevirt-fix.yaml
+-rw-r--r--  2.0 unx     1127 b- defN 23-May-26 19:51 kvirt/cluster/openshift/99-localhost-fix.yaml
+-rw-r--r--  2.0 unx      250 b- defN 23-May-26 19:51 kvirt/cluster/openshift/99-metal3-fake-machine.yaml
+-rw-r--r--  2.0 unx      162 b- defN 23-May-26 19:51 kvirt/cluster/openshift/99-metal3-provisioning.yaml
+-rw-r--r--  2.0 unx     1659 b- defN 23-May-26 19:51 kvirt/cluster/openshift/99-notifications.yaml
+-rw-r--r--  2.0 unx      118 b- defN 23-May-26 19:51 kvirt/cluster/openshift/99-operatorhub.yaml
+-rw-r--r--  2.0 unx      314 b- defN 23-May-26 19:51 kvirt/cluster/openshift/99-ovn.yaml
+-rw-r--r--  2.0 unx      912 b- defN 23-May-26 19:51 kvirt/cluster/openshift/99-sno.yaml
+-rw-r--r--  2.0 unx      762 b- defN 23-May-26 19:51 kvirt/cluster/openshift/Corefile
+-rw-r--r--  2.0 unx    81595 b- defN 23-May-26 19:51 kvirt/cluster/openshift/__init__.py
+-rw-r--r--  2.0 unx     1326 b- defN 23-May-26 19:51 kvirt/cluster/openshift/autoapprovercron.yml
+-rw-r--r--  2.0 unx      987 b- defN 23-May-26 19:51 kvirt/cluster/openshift/autorules.yml
+-rw-r--r--  2.0 unx     1630 b- defN 23-May-26 19:51 kvirt/cluster/openshift/bootstrap.yml
+-rw-r--r--  2.0 unx      250 b- defN 23-May-26 19:51 kvirt/cluster/openshift/calico.sh.j2
+-rw-r--r--  2.0 unx      107 b- defN 23-May-26 19:51 kvirt/cluster/openshift/chrony.conf
+-rw-r--r--  2.0 unx      629 b- defN 23-May-26 19:51 kvirt/cluster/openshift/cloud_bootstrap.yml
+-rw-r--r--  2.0 unx      792 b- defN 23-May-26 19:51 kvirt/cluster/openshift/cloud_ctlplanes.yml
+-rw-r--r--  2.0 unx      217 b- defN 23-May-26 19:51 kvirt/cluster/openshift/cloud_dns.yml
+-rw-r--r--  2.0 unx      616 b- defN 23-May-26 19:51 kvirt/cluster/openshift/cloud_lb_api.yml
+-rw-r--r--  2.0 unx      204 b- defN 23-May-26 19:51 kvirt/cluster/openshift/cloud_lb_apps.yml
+-rw-r--r--  2.0 unx      703 b- defN 23-May-26 19:51 kvirt/cluster/openshift/cloud_workers.yml
+-rw-r--r--  2.0 unx      123 b- defN 23-May-26 19:51 kvirt/cluster/openshift/cluster-ingress-02-config.yml
+-rw-r--r--  2.0 unx      159 b- defN 23-May-26 19:51 kvirt/cluster/openshift/cluster-scheduler-02-config.yml
+-rw-r--r--  2.0 unx      224 b- defN 23-May-26 19:51 kvirt/cluster/openshift/config.hcl.templ
+-rw-r--r--  2.0 unx       98 b- defN 23-May-26 19:51 kvirt/cluster/openshift/contrail-ca-patch.service
+-rw-r--r--  2.0 unx      486 b- defN 23-May-26 19:51 kvirt/cluster/openshift/contrail-ca-patch.sh
+-rw-r--r--  2.0 unx       87 b- defN 23-May-26 19:51 kvirt/cluster/openshift/contrail.auth
+-rw-r--r--  2.0 unx     1108 b- defN 23-May-26 19:51 kvirt/cluster/openshift/contrail.sh.j2
+-rw-r--r--  2.0 unx     2278 b- defN 23-May-26 19:51 kvirt/cluster/openshift/ctlplanes.yml
+-rw-r--r--  2.0 unx      326 b- defN 23-May-26 19:51 kvirt/cluster/openshift/dhcp.conf
+-rw-r--r--  2.0 unx      106 b- defN 23-May-26 19:51 kvirt/cluster/openshift/dhcp.sh
+-rw-r--r--  2.0 unx      536 b- defN 23-May-26 19:51 kvirt/cluster/openshift/dhcp.yml
+-rw-r--r--  2.0 unx      836 b- defN 23-May-26 19:51 kvirt/cluster/openshift/disconnected.yml
+-rw-r--r--  2.0 unx     8945 b- defN 23-May-26 19:51 kvirt/cluster/openshift/fake_kubeconfig.json
+-rw-r--r--  2.0 unx       35 b- defN 23-May-26 19:51 kvirt/cluster/openshift/fake_pull.json
+-rw-r--r--  2.0 unx     1792 b- defN 23-May-26 19:51 kvirt/cluster/openshift/haproxy.cfg
+-rw-r--r--  2.0 unx     2483 b- defN 23-May-26 19:51 kvirt/cluster/openshift/haproxy.cfg.kubevirt
+-rw-r--r--  2.0 unx      902 b- defN 23-May-26 19:51 kvirt/cluster/openshift/httpd.yaml
+-rw-r--r--  2.0 unx      524 b- defN 23-May-26 19:51 kvirt/cluster/openshift/ignition.j2
+-rw-r--r--  2.0 unx     3562 b- defN 23-May-26 19:51 kvirt/cluster/openshift/install-config.yaml
+-rw-r--r--  2.0 unx     2691 b- defN 23-May-26 19:51 kvirt/cluster/openshift/iso.sh
+-rw-r--r--  2.0 unx      237 b- defN 23-May-26 19:51 kvirt/cluster/openshift/kcli-ipv6.conf.j2
+-rw-r--r--  2.0 unx     4257 b- defN 23-May-26 19:51 kvirt/cluster/openshift/kcli_default.yml
+-rw-r--r--  2.0 unx      982 b- defN 23-May-26 19:51 kvirt/cluster/openshift/keepalived.conf
+-rw-r--r--  2.0 unx       60 b- defN 23-May-26 19:51 kvirt/cluster/openshift/nonlocalbind.conf
+-rw-r--r--  2.0 unx       59 b- defN 23-May-26 19:51 kvirt/cluster/openshift/openshift-workload-pinning
+-rw-r--r--  2.0 unx      157 b- defN 23-May-26 19:51 kvirt/cluster/openshift/relocate-ip-bootstrap.service
+-rw-r--r--  2.0 unx      281 b- defN 23-May-26 19:51 kvirt/cluster/openshift/relocate-ip-bootstrap.sh
+-rw-r--r--  2.0 unx      690 b- defN 23-May-26 19:51 kvirt/cluster/openshift/relocate-ip.sh
+-rw-r--r--  2.0 unx      212 b- defN 23-May-26 19:51 kvirt/cluster/openshift/sno-finish.service
+-rw-r--r--  2.0 unx     2085 b- defN 23-May-26 19:51 kvirt/cluster/openshift/sno-finish.sh
+-rw-r--r--  2.0 unx      660 b- defN 23-May-26 19:51 kvirt/cluster/openshift/sno.yml
+-rw-r--r--  2.0 unx     1615 b- defN 23-May-26 19:51 kvirt/cluster/openshift/workers.yml
+-rw-r--r--  2.0 unx       40 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/cr.sh
+-rw-r--r--  2.0 unx      768 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/install.yml.j2
+-rw-r--r--  2.0 unx      162 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/advanced-cluster-management/99-metal3-provisioning.yaml
+-rw-r--r--  2.0 unx     2754 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sample.yml
+-rwxr-xr-x  2.0 unx     2838 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/advanced-cluster-management/assisted-service.sh
+-rw-r--r--  2.0 unx      418 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/advanced-cluster-management/cr.yml
+-rw-r--r--  2.0 unx      625 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/advanced-cluster-management/gen_registries.py
+-rw-r--r--  2.0 unx      259 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/advanced-cluster-management/kcli_default.yml
+-rw-r--r--  2.0 unx     1219 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/advanced-cluster-management/post.sh
+-rw-r--r--  2.0 unx      645 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/argocd/configmap.yml
+-rw-r--r--  2.0 unx     2423 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/argocd/install.sh
+-rw-r--r--  2.0 unx       49 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/argocd/kcli_default.yml
+-rw-r--r--  2.0 unx     1093 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/autolabeller/cr.yml
+-rw-r--r--  2.0 unx      142 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/autolabeller/install.sh
+-rw-r--r--  2.0 unx     1093 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/autolabeller/install.yml
+-rw-r--r--  2.0 unx      165 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/autolabeller/kcli_default.yml
+-rw-r--r--  2.0 unx       25 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/autolabeller/uninstall.sh
+-rw-r--r--  2.0 unx      873 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/cluster-logging/cr.yml
+-rw-r--r--  2.0 unx       63 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/cluster-logging/kcli_default.yml
+-rw-r--r--  2.0 unx      265 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/istio/install.sh
+-rw-r--r--  2.0 unx      377 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/istio/istio-cni.yaml
+-rw-r--r--  2.0 unx     1039 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/kubevirt-hyperconverged/cr.yml
+-rw-r--r--  2.0 unx      154 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/kubevirt-hyperconverged/kcli_default.yml
+-rw-r--r--  2.0 unx      775 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/local-storage-operator/cr.yml
+-rw-r--r--  2.0 unx      227 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/local-storage-operator/kcli_default.yml
+-rw-r--r--  2.0 unx      642 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/local-storage-operator/post.sh
+-rw-r--r--  2.0 unx      349 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/lvms-operator/cr.yml
+-rw-r--r--  2.0 unx      137 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/lvms-operator/kcli_default.yml
+-rw-r--r--  2.0 unx      595 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/lvms-operator/post.sh
+-rw-r--r--  2.0 unx      510 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/metallb-operator/cr.yml
+-rw-r--r--  2.0 unx       94 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/metallb-operator/kcli_default.yml
+-rw-r--r--  2.0 unx      162 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/multicluster-engine/99-metal3-provisioning.yaml
+-rw-r--r--  2.0 unx     2754 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sample.yml
+-rwxr-xr-x  2.0 unx     2845 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/multicluster-engine/assisted-service.sh
+-rw-r--r--  2.0 unx      245 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/multicluster-engine/cr.yml
+-rw-r--r--  2.0 unx      625 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/multicluster-engine/gen_registries.py
+-rw-r--r--  2.0 unx      118 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/multicluster-engine/kcli_default.yml
+-rwxr-xr-x  2.0 unx       55 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/multicluster-engine/post.sh
+-rwxr-xr-x  2.0 unx     2298 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/nfs/install.sh
+-rw-r--r--  2.0 unx      117 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/nfs/kcli_default.yml
+-rw-r--r--  2.0 unx      185 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/nfs/uninstall.sh
+-rw-r--r--  2.0 unx      849 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/odf-operator/cr.yml
+-rw-r--r--  2.0 unx      298 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/odf-operator/kcli_default.yml
+-rw-r--r--  2.0 unx      364 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/odf-operator/nad_cluster.yml
+-rw-r--r--  2.0 unx      362 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/odf-operator/nad_public.yml
+-rw-r--r--  2.0 unx      745 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/odf-operator/post.sh
+-rw-r--r--  2.0 unx      530 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/odf-operator/pre.sh
+-rw-r--r--  2.0 unx      363 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/serverless-operator/cr.yml
+-rw-r--r--  2.0 unx      157 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/serverless-operator/kcli_default.yml
+-rw-r--r--  2.0 unx      278 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/serverless-operator/post.sh
+-rw-r--r--  2.0 unx     1227 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/users/install.sh
+-rw-r--r--  2.0 unx       84 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/users/kcli_default.yml
+-rw-r--r--  2.0 unx      258 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/users/oauth.yml
+-rw-r--r--  2.0 unx      249 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/users/oauth_hypershift.yml
+-rw-r--r--  2.0 unx      422 b- defN 23-May-26 19:51 kvirt/cluster/openshift/apps/users/uninstall.sh
+-rw-r--r--  2.0 unx       60 b- defN 23-May-26 19:51 kvirt/cluster/openshift/customisation/00-kcli-namespace.yaml
+-rw-r--r--  2.0 unx       91 b- defN 23-May-26 19:51 kvirt/cluster/openshift/customisation/97-autoapprovercron-sa.yaml
+-rw-r--r--  2.0 unx      264 b- defN 23-May-26 19:51 kvirt/cluster/openshift/customisation/98-autoapprovercron-binding.yaml
+-rw-r--r--  2.0 unx      912 b- defN 23-May-26 19:51 kvirt/cluster/openshift/customisation/99-autoapprovercron-cronjob.yaml
+-rw-r--r--  2.0 unx      389 b- defN 23-May-26 19:51 kvirt/cluster/openshift/customisation/99-ingress-controller.yaml
+-rw-r--r--  2.0 unx      184 b- defN 23-May-26 19:51 kvirt/cluster/openshift/customisation/99-monitoring.yaml
+-rw-r--r--  2.0 unx      289 b- defN 23-May-26 19:51 kvirt/cluster/openshift/customisation/99-registry.yaml
+-rw-r--r--  2.0 unx     1685 b- defN 23-May-26 19:51 kvirt/cluster/openshift/disconnected/haproxy.cfg
+-rw-r--r--  2.0 unx      211 b- defN 23-May-26 19:51 kvirt/cluster/openshift/disconnected/registry.service
+-rwxr-xr-x  2.0 unx      328 b- defN 23-May-26 19:51 kvirt/cluster/openshift/disconnected/bin/sync_image.sh
+-rwxr-xr-x  2.0 unx      201 b- defN 23-May-26 19:51 kvirt/cluster/openshift/disconnected/scripts/01_get_oc.sh
+-rwxr-xr-x  2.0 unx     2484 b- defN 23-May-26 19:51 kvirt/cluster/openshift/disconnected/scripts/03_mirror.sh
+-rwxr-xr-x  2.0 unx     2046 b- defN 23-May-26 19:51 kvirt/cluster/openshift/disconnected/scripts/03_registry.sh
+-rwxr-xr-x  2.0 unx      337 b- defN 23-May-26 19:51 kvirt/cluster/openshift/disconnected/scripts/04_extras.sh
+-rwxr-xr-x  2.0 unx     2390 b- defN 23-May-26 19:51 kvirt/cluster/openshift/disconnected/scripts/05_olm.sh
+-rwxr-xr-x  2.0 unx      241 b- defN 23-May-26 19:51 kvirt/cluster/openshift/disconnected/scripts/06_web.sh
+-rwxr-xr-x  2.0 unx      733 b- defN 23-May-26 19:51 kvirt/cluster/openshift/disconnected/scripts/deploy.sh
+-rw-r--r--  2.0 unx     1768 b- defN 23-May-26 19:51 kvirt/cluster/openshift/disconnected/scripts/mirror-config.yaml.sample
+-rw-r--r--  2.0 unx     2557 b- defN 23-May-26 19:51 kvirt/cluster/openshift/staticpods/coredns.yml
+-rw-r--r--  2.0 unx      987 b- defN 23-May-26 19:51 kvirt/cluster/openshift/staticpods/haproxy.yml
+-rw-r--r--  2.0 unx     2539 b- defN 23-May-26 19:51 kvirt/cluster/openshift/staticpods/keepalived.yml
+-rw-r--r--  2.0 unx     1721 b- defN 23-May-26 19:51 kvirt/cluster/openshift/staticpods/mdns.yml
+-rw-r--r--  2.0 unx      193 b- defN 23-May-26 19:51 kvirt/cluster/profiles/sample-kubeadm-default.yml
+-rw-r--r--  2.0 unx      135 b- defN 23-May-26 19:51 kvirt/cluster/profiles/sample-openshift-compact.yml
+-rw-r--r--  2.0 unx      213 b- defN 23-May-26 19:51 kvirt/cluster/profiles/sample-openshift-contrail.yml
+-rw-r--r--  2.0 unx      157 b- defN 23-May-26 19:51 kvirt/cluster/profiles/sample-openshift-ipv6.yml
+-rw-r--r--  2.0 unx       55 b- defN 23-May-26 19:51 kvirt/cluster/profiles/sample-openshift-sno-bm.yml
+-rw-r--r--  2.0 unx      148 b- defN 23-May-26 19:51 kvirt/cluster/profiles/sample-openshift-sno.yml
+-rw-r--r--  2.0 unx     3377 b- defN 23-May-26 19:51 kvirt/common/Jenkinsfile.j2
+-rw-r--r--  2.0 unx    96428 b- defN 23-May-26 19:51 kvirt/common/__init__.py
+-rw-r--r--  2.0 unx     1406 b- defN 23-May-26 19:51 kvirt/common/autoscale.yaml.j2
+-rw-r--r--  2.0 unx     8945 b- defN 23-May-26 19:51 kvirt/common/fake_kubeconfig.json
+-rw-r--r--  2.0 unx      669 b- defN 23-May-26 19:51 kvirt/common/ignition.j2
+-rw-r--r--  2.0 unx      125 b- defN 23-May-26 19:51 kvirt/common/kubevirt_kcli_conf.j2
+-rw-r--r--  2.0 unx       99 b- defN 23-May-26 19:51 kvirt/common/local_kcli_conf.j2
+-rw-r--r--  2.0 unx     3068 b- defN 23-May-26 19:51 kvirt/common/pipeline.yml.j2
+-rw-r--r--  2.0 unx     2377 b- defN 23-May-26 19:51 kvirt/common/pipeline_kube.yml.j2
+-rw-r--r--  2.0 unx     1381 b- defN 23-May-26 19:51 kvirt/common/playbook.j2
+-rw-r--r--  2.0 unx     1557 b- defN 23-May-26 19:51 kvirt/common/storage.sh.j2
+-rw-r--r--  2.0 unx     4562 b- defN 23-May-26 19:51 kvirt/common/vm.ovf.j2
+-rw-r--r--  2.0 unx     2241 b- defN 23-May-26 19:51 kvirt/common/workflow.yml.j2
+-rw-r--r--  2.0 unx     2208 b- defN 23-May-26 19:51 kvirt/common/workflow_script.yml.j2
+-rw-r--r--  2.0 unx    15041 b- defN 23-May-26 19:51 kvirt/container/__init__.py
+-rw-r--r--  2.0 unx    11716 b- defN 23-May-26 19:51 kvirt/expose/__init__.py
+-rw-r--r--  2.0 unx     4319 b- defN 23-May-26 19:51 kvirt/expose/swagger.yml
+-rw-r--r--  2.0 unx      408 b- defN 23-May-26 19:51 kvirt/expose/static/css/bootstrap-notify.css
+-rw-r--r--  2.0 unx   121125 b- defN 23-May-26 19:51 kvirt/expose/static/css/bootstrap.min.css
+-rw-r--r--  2.0 unx      399 b- defN 23-May-26 19:51 kvirt/expose/static/css/dataTables.checkboxes.css
+-rw-r--r--  2.0 unx    13587 b- defN 23-May-26 19:51 kvirt/expose/static/css/jquery.dataTables.min.css
+-rw-r--r--  2.0 unx      868 b- defN 23-May-26 19:51 kvirt/expose/static/css/kcli.css
+-rw-r--r--  2.0 unx      269 b- defN 23-May-26 19:51 kvirt/expose/static/css/wheel.css
+-rw-r--r--  2.0 unx     1406 b- defN 23-May-26 19:51 kvirt/expose/static/images/favicon.ico
+-rw-r--r--  2.0 unx      160 b- defN 23-May-26 19:51 kvirt/expose/static/images/sort_asc.png
+-rw-r--r--  2.0 unx      201 b- defN 23-May-26 19:51 kvirt/expose/static/images/sort_both.png
+-rw-r--r--  2.0 unx      158 b- defN 23-May-26 19:51 kvirt/expose/static/images/sort_desc.png
+-rw-r--r--  2.0 unx    24772 b- defN 23-May-26 19:51 kvirt/expose/static/images/wheel.gif
+-rw-r--r--  2.0 unx    12398 b- defN 23-May-26 19:51 kvirt/expose/static/js/dataTables.checkboxes.min.js
+-rw-r--r--  2.0 unx      367 b- defN 23-May-26 19:51 kvirt/expose/static/js/exposeactions.js
+-rw-r--r--  2.0 unx    83059 b- defN 23-May-26 19:51 kvirt/expose/static/js/jquery.dataTables.min.js
+-rw-r--r--  2.0 unx    89795 b- defN 23-May-26 19:51 kvirt/expose/static/js/jquery.min.js
+-rw-r--r--  2.0 unx      263 b- defN 23-May-26 19:51 kvirt/expose/static/js/list.js
+-rw-r--r--  2.0 unx     1605 b- defN 23-May-26 19:51 kvirt/expose/templates/form.html
+-rw-r--r--  2.0 unx     1035 b- defN 23-May-26 19:51 kvirt/expose/templates/head.html
+-rw-r--r--  2.0 unx      406 b- defN 23-May-26 19:51 kvirt/expose/templates/index.html
+-rw-r--r--  2.0 unx     1220 b- defN 23-May-26 19:51 kvirt/expose/templates/infoplan.html
+-rw-r--r--  2.0 unx      574 b- defN 23-May-26 19:51 kvirt/expose/templates/planstable.html
+-rw-r--r--  2.0 unx      550 b- defN 23-May-26 19:51 kvirt/expose/templates/result.html
+-rw-r--r--  2.0 unx     1754 b- defN 23-May-26 19:51 kvirt/internalplans/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-26 19:51 kvirt/jinjafilters/__init__.py
+-rw-r--r--  2.0 unx     5249 b- defN 23-May-26 19:51 kvirt/jinjafilters/jinjafilters.py
+-rw-r--r--  2.0 unx     8477 b- defN 23-May-26 19:51 kvirt/kfish/__init__.py
+-rw-r--r--  2.0 unx     9124 b- defN 23-May-26 19:51 kvirt/ksushy/__init__.py
+-rw-r--r--  2.0 unx      121 b- defN 23-May-26 19:51 kvirt/ksushy/main.py
+-rw-r--r--  2.0 unx     1028 b- defN 23-May-26 19:51 kvirt/ksushy/templates/bios.json
+-rw-r--r--  2.0 unx      443 b- defN 23-May-26 19:51 kvirt/ksushy/templates/interface.json
+-rw-r--r--  2.0 unx      418 b- defN 23-May-26 19:51 kvirt/ksushy/templates/interfaces.json
+-rw-r--r--  2.0 unx     1050 b- defN 23-May-26 19:51 kvirt/ksushy/templates/manager.json
+-rw-r--r--  2.0 unx      571 b- defN 23-May-26 19:51 kvirt/ksushy/templates/managers.json
+-rw-r--r--  2.0 unx      535 b- defN 23-May-26 19:51 kvirt/ksushy/templates/root.json
+-rw-r--r--  2.0 unx     2732 b- defN 23-May-26 19:51 kvirt/ksushy/templates/system.json
+-rw-r--r--  2.0 unx      511 b- defN 23-May-26 19:51 kvirt/ksushy/templates/systems.json
+-rw-r--r--  2.0 unx     1219 b- defN 23-May-26 19:51 kvirt/ksushy/templates/virtualmedia_cd.json
+-rw-r--r--  2.0 unx      705 b- defN 23-May-26 19:51 kvirt/ksushy/templates/virtualmedias.json
+-rw-r--r--  2.0 unx     2780 b- defN 23-May-26 19:51 kvirt/miniconsole/__init__.py
+-rw-r--r--  2.0 unx     3488 b- defN 23-May-26 19:51 kvirt/nameutils/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-26 19:51 kvirt/providers/__init__.py
+-rw-r--r--  2.0 unx     8935 b- defN 23-May-26 19:51 kvirt/providers/sampleprovider.py
+-rw-r--r--  2.0 unx    65799 b- defN 23-May-26 19:51 kvirt/providers/aws/__init__.py
+-rw-r--r--  2.0 unx      479 b- defN 23-May-26 19:51 kvirt/providers/fake/__init__.py
+-rw-r--r--  2.0 unx    66344 b- defN 23-May-26 19:51 kvirt/providers/gcp/__init__.py
+-rw-r--r--  2.0 unx      175 b- defN 23-May-26 19:51 kvirt/providers/gcp/gcp-hack.service
+-rw-r--r--  2.0 unx      231 b- defN 23-May-26 19:51 kvirt/providers/gcp/gcp-hack.sh
+-rw-r--r--  2.0 unx    65035 b- defN 23-May-26 19:51 kvirt/providers/ibm/__init__.py
+-rw-r--r--  2.0 unx    80949 b- defN 23-May-26 19:51 kvirt/providers/kubevirt/__init__.py
+-rw-r--r--  2.0 unx   184146 b- defN 23-May-26 19:51 kvirt/providers/kvm/__init__.py
+-rw-r--r--  2.0 unx     1965 b- defN 23-May-26 19:51 kvirt/providers/kvm/helpers.py
+-rw-r--r--  2.0 unx    57063 b- defN 23-May-26 19:51 kvirt/providers/openstack/__init__.py
+-rw-r--r--  2.0 unx    62531 b- defN 23-May-26 19:51 kvirt/providers/ovirt/__init__.py
+-rw-r--r--  2.0 unx    31099 b- defN 23-May-26 19:51 kvirt/providers/packet/__init__.py
+-rw-r--r--  2.0 unx    73086 b- defN 23-May-26 19:51 kvirt/providers/vsphere/__init__.py
+-rw-r--r--  2.0 unx    13655 b- defN 23-May-26 19:51 kvirt/providers/vsphere/helpers.py
+-rw-r--r--  2.0 unx     4893 b- defN 23-May-26 19:51 kvirt/providers/vsphere/tagging.py
+-rw-r--r--  2.0 unx    21273 b- defN 23-May-26 19:51 kvirt/providers/web/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-26 19:51 kvirt/version/__init__.py
+-rw-r--r--  2.0 unx       19 b- defN 23-May-26 19:53 kvirt/version/git
+-rw-r--r--  2.0 unx    46592 b- defN 23-May-26 19:51 kvirt/web/__init__.py
+-rw-r--r--  2.0 unx      261 b- defN 23-May-26 19:51 kvirt/web/main.py
+-rw-r--r--  2.0 unx      408 b- defN 23-May-26 19:51 kvirt/web/static/css/bootstrap-notify.css
+-rw-r--r--  2.0 unx    23409 b- defN 23-May-26 19:51 kvirt/web/static/css/bootstrap-theme.min.css
+-rw-r--r--  2.0 unx   121125 b- defN 23-May-26 19:51 kvirt/web/static/css/bootstrap.min.css
+-rw-r--r--  2.0 unx      399 b- defN 23-May-26 19:51 kvirt/web/static/css/dataTables.checkboxes.css
+-rw-r--r--  2.0 unx    13587 b- defN 23-May-26 19:51 kvirt/web/static/css/jquery.dataTables.min.css
+-rw-r--r--  2.0 unx      816 b- defN 23-May-26 19:51 kvirt/web/static/css/kcli.css
+-rw-r--r--  2.0 unx     3033 b- defN 23-May-26 19:51 kvirt/web/static/css/navbar.css
+-rw-r--r--  2.0 unx     2908 b- defN 23-May-26 19:51 kvirt/web/static/css/spice.css
+-rw-r--r--  2.0 unx      271 b- defN 23-May-26 19:51 kvirt/web/static/css/wheel.css
+-rw-r--r--  2.0 unx    18028 b- defN 23-May-26 19:51 kvirt/web/static/fonts/glyphicons-halflings-regular.woff2
+-rw-r--r--  2.0 unx      715 b- defN 23-May-26 19:51 kvirt/web/static/images/Centos.png
+-rw-r--r--  2.0 unx      294 b- defN 23-May-26 19:51 kvirt/web/static/images/Debian.png
+-rw-r--r--  2.0 unx      987 b- defN 23-May-26 19:51 kvirt/web/static/images/Fedora.png
+-rw-r--r--  2.0 unx      672 b- defN 23-May-26 19:51 kvirt/web/static/images/Redhat.png
+-rw-r--r--  2.0 unx     1278 b- defN 23-May-26 19:51 kvirt/web/static/images/Suse.png
+-rw-r--r--  2.0 unx     1782 b- defN 23-May-26 19:51 kvirt/web/static/images/Tux.png
+-rw-r--r--  2.0 unx      544 b- defN 23-May-26 19:51 kvirt/web/static/images/Ubuntu.png
+-rw-r--r--  2.0 unx     4213 b- defN 23-May-26 19:51 kvirt/web/static/images/delete.png
+-rw-r--r--  2.0 unx     1406 b- defN 23-May-26 19:51 kvirt/web/static/images/favicon.ico
+-rw-r--r--  2.0 unx    23320 b- defN 23-May-26 19:51 kvirt/web/static/images/kcli-small.png
+-rw-r--r--  2.0 unx    27185 b- defN 23-May-26 19:51 kvirt/web/static/images/kcli.jpg
+-rw-r--r--  2.0 unx   113928 b- defN 23-May-26 19:51 kvirt/web/static/images/kcli.png
+-rw-r--r--  2.0 unx    48809 b- defN 23-May-26 19:51 kvirt/web/static/images/logo-header.svg
+-rw-r--r--  2.0 unx    48809 b- defN 23-May-26 19:51 kvirt/web/static/images/logo-main.svg
+-rw-r--r--  2.0 unx      160 b- defN 23-May-26 19:51 kvirt/web/static/images/sort_asc.png
+-rw-r--r--  2.0 unx      201 b- defN 23-May-26 19:51 kvirt/web/static/images/sort_both.png
+-rw-r--r--  2.0 unx      158 b- defN 23-May-26 19:51 kvirt/web/static/images/sort_desc.png
+-rw-r--r--  2.0 unx     3927 b- defN 23-May-26 19:51 kvirt/web/static/images/start.png
+-rw-r--r--  2.0 unx     3631 b- defN 23-May-26 19:51 kvirt/web/static/images/stop.png
+-rw-r--r--  2.0 unx    24772 b- defN 23-May-26 19:51 kvirt/web/static/images/wheel.gif
+-rw-r--r--  2.0 unx     2933 b- defN 23-May-26 19:51 kvirt/web/static/js/bootstrap-notify.js
+-rw-r--r--  2.0 unx    37045 b- defN 23-May-26 19:51 kvirt/web/static/js/bootstrap.min.js
+-rw-r--r--  2.0 unx     2523 b- defN 23-May-26 19:51 kvirt/web/static/js/containeraction.js
+-rw-r--r--  2.0 unx    12398 b- defN 23-May-26 19:51 kvirt/web/static/js/dataTables.checkboxes.min.js
+-rw-r--r--  2.0 unx     1642 b- defN 23-May-26 19:51 kvirt/web/static/js/hostaction.js
+-rw-r--r--  2.0 unx     1187 b- defN 23-May-26 19:51 kvirt/web/static/js/imageaction.js
+-rw-r--r--  2.0 unx    83059 b- defN 23-May-26 19:51 kvirt/web/static/js/jquery.dataTables.min.js
+-rw-r--r--  2.0 unx    89795 b- defN 23-May-26 19:51 kvirt/web/static/js/jquery.min.js
+-rw-r--r--  2.0 unx     2704 b- defN 23-May-26 19:51 kvirt/web/static/js/kcli.js
+-rw-r--r--  2.0 unx     1594 b- defN 23-May-26 19:51 kvirt/web/static/js/kubeaction.js
+-rw-r--r--  2.0 unx     3907 b- defN 23-May-26 19:51 kvirt/web/static/js/list.js
+-rw-r--r--  2.0 unx     1376 b- defN 23-May-26 19:51 kvirt/web/static/js/networkaction.js
+-rw-r--r--  2.0 unx     2457 b- defN 23-May-26 19:51 kvirt/web/static/js/planaction.js
+-rw-r--r--  2.0 unx     1237 b- defN 23-May-26 19:51 kvirt/web/static/js/poolaction.js
+-rw-r--r--  2.0 unx      846 b- defN 23-May-26 19:51 kvirt/web/static/js/productaction.js
+-rw-r--r--  2.0 unx      270 b- defN 23-May-26 19:51 kvirt/web/static/js/refresh.js
+-rw-r--r--  2.0 unx     1835 b- defN 23-May-26 19:51 kvirt/web/static/js/repoaction.js
+-rw-r--r--  2.0 unx     3463 b- defN 23-May-26 19:51 kvirt/web/static/js/snapshotaction.js
+-rw-r--r--  2.0 unx     2745 b- defN 23-May-26 19:51 kvirt/web/static/js/vmaction.js
+-rw-r--r--  2.0 unx      123 b- defN 23-May-26 19:51 kvirt/web/static/js/wheel.js
+-rw-r--r--  2.0 unx     9944 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/atKeynames.js
+-rw-r--r--  2.0 unx     2335 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/bitmap.js
+-rw-r--r--  2.0 unx     4795 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/cursor.js
+-rw-r--r--  2.0 unx    49214 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/display.js
+-rw-r--r--  2.0 unx    13253 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/enums.js
+-rw-r--r--  2.0 unx     2847 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/filexfer.js
+-rw-r--r--  2.0 unx     9535 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/inputs.js
+-rw-r--r--  2.0 unx     6176 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/lz.js
+-rw-r--r--  2.0 unx    18370 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/main.js
+-rw-r--r--  2.0 unx    12677 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/playback.js
+-rw-r--r--  2.0 unx     7036 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/png.js
+-rw-r--r--  2.0 unx     3110 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/port.js
+-rw-r--r--  2.0 unx    44531 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/quic.js
+-rw-r--r--  2.0 unx     3030 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/resize.js
+-rw-r--r--  2.0 unx     7282 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/simulatecursor.js
+-rw-r--r--  2.0 unx     1895 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/spicearraybuffer.js
+-rw-r--r--  2.0 unx    18202 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/spiceconn.js
+-rw-r--r--  2.0 unx     3616 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/spicedataview.js
+-rw-r--r--  2.0 unx    33015 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/spicemsg.js
+-rw-r--r--  2.0 unx    12767 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/spicetype.js
+-rw-r--r--  2.0 unx     6808 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/ticket.js
+-rw-r--r--  2.0 unx    13628 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/utils.js
+-rw-r--r--  2.0 unx    21577 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/webm.js
+-rw-r--r--  2.0 unx     4131 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/wire.js
+-rw-r--r--  2.0 unx    16580 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/thirdparty/jsbn.js
+-rw-r--r--  2.0 unx     2529 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/thirdparty/prng4.js
+-rw-r--r--  2.0 unx     3442 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/thirdparty/rng.js
+-rw-r--r--  2.0 unx     4257 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/thirdparty/rsa.js
+-rw-r--r--  2.0 unx    10671 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/thirdparty/sha1.js
+-rw-r--r--  2.0 unx        0 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/.npmignore
+-rw-r--r--  2.0 unx      419 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/README.md
+-rw-r--r--  2.0 unx      359 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/rollup.config.js
+-rw-r--r--  2.0 unx     1113 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/babel-worker.js
+-rw-r--r--  2.0 unx     8601 b- defN 23-May-26 19:51 kvirt/web/static/js/spice/thirdparty/browser-es-module-loader/src/browser-es-module-loader.js
+-rw-r--r--  2.0 unx     2176 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/error-handler.js
+-rw-r--r--  2.0 unx     5682 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/localization.js
+-rw-r--r--  2.0 unx    56845 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/ui.js
+-rw-r--r--  2.0 unx     6696 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/webutil.js
+-rw-r--r--  2.0 unx     3553 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/alt.svg
+-rw-r--r--  2.0 unx     3980 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/clipboard.svg
+-rw-r--r--  2.0 unx     3430 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/connect.svg
+-rw-r--r--  2.0 unx     4381 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/ctrl.svg
+-rw-r--r--  2.0 unx     3237 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/ctrlaltdel.svg
+-rw-r--r--  2.0 unx     5062 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/disconnect.svg
+-rw-r--r--  2.0 unx     4684 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/drag.svg
+-rw-r--r--  2.0 unx     3106 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/error.svg
+-rw-r--r--  2.0 unx     4522 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/esc.svg
+-rw-r--r--  2.0 unx     3066 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/expander.svg
+-rw-r--r--  2.0 unx     3139 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/fullscreen.svg
+-rw-r--r--  2.0 unx     2559 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/handle.svg
+-rw-r--r--  2.0 unx     6386 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/handle_bg.svg
+-rw-r--r--  2.0 unx     3204 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/info.svg
+-rw-r--r--  2.0 unx     6404 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/keyboard.svg
+-rw-r--r--  2.0 unx     7000 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/mouse_left.svg
+-rw-r--r--  2.0 unx     7002 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/mouse_middle.svg
+-rw-r--r--  2.0 unx     6993 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/mouse_none.svg
+-rw-r--r--  2.0 unx     7001 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/mouse_right.svg
+-rw-r--r--  2.0 unx     3985 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/power.svg
+-rw-r--r--  2.0 unx     3082 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/settings.svg
+-rw-r--r--  2.0 unx     2953 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/tab.svg
+-rw-r--r--  2.0 unx     4441 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/toggleextrakeys.svg
+-rw-r--r--  2.0 unx     3869 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/warning.svg
+-rw-r--r--  2.0 unx     3178 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/windows.svg
+-rw-r--r--  2.0 unx      871 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/icons/Makefile
+-rw-r--r--  2.0 unx     4028 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/icons/novnc-120x120.png
+-rw-r--r--  2.0 unx     4582 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/icons/novnc-144x144.png
+-rw-r--r--  2.0 unx     5216 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/icons/novnc-152x152.png
+-rw-r--r--  2.0 unx      675 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/icons/novnc-16x16.png
+-rw-r--r--  2.0 unx     5787 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/icons/novnc-192x192.png
+-rw-r--r--  2.0 unx     1000 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/icons/novnc-24x24.png
+-rw-r--r--  2.0 unx     1064 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/icons/novnc-32x32.png
+-rw-r--r--  2.0 unx     1397 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/icons/novnc-48x48.png
+-rw-r--r--  2.0 unx     1932 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/icons/novnc-60x60.png
+-rw-r--r--  2.0 unx     1946 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/icons/novnc-64x64.png
+-rw-r--r--  2.0 unx     2699 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/icons/novnc-72x72.png
+-rw-r--r--  2.0 unx     2874 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/icons/novnc-76x76.png
+-rw-r--r--  2.0 unx     2351 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/icons/novnc-96x96.png
+-rw-r--r--  2.0 unx    11685 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/icons/novnc-icon-sm.svg
+-rw-r--r--  2.0 unx    11549 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/images/icons/novnc-icon.svg
+-rw-r--r--  2.0 unx     2885 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/locale/cs.json
+-rw-r--r--  2.0 unx     2854 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/locale/de.json
+-rw-r--r--  2.0 unx     3906 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/locale/el.json
+-rw-r--r--  2.0 unx     2671 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/locale/es.json
+-rw-r--r--  2.0 unx     3354 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/locale/ja.json
+-rw-r--r--  2.0 unx     2961 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/locale/ko.json
+-rw-r--r--  2.0 unx     3035 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/locale/nl.json
+-rw-r--r--  2.0 unx     2830 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/locale/pl.json
+-rw-r--r--  2.0 unx     3825 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/locale/ru.json
+-rw-r--r--  2.0 unx     2845 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/locale/sv.json
+-rw-r--r--  2.0 unx     2811 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/locale/tr.json
+-rw-r--r--  2.0 unx     2597 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/locale/zh_CN.json
+-rw-r--r--  2.0 unx     2606 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/locale/zh_TW.json
+-rw-r--r--  2.0 unx      157 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/sounds/CREDITS
+-rw-r--r--  2.0 unx     4531 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/sounds/bell.mp3
+-rw-r--r--  2.0 unx     8495 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/sounds/bell.oga
+-rw-r--r--  2.0 unx    38580 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/styles/Orbitron700.ttf
+-rw-r--r--  2.0 unx    17472 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/styles/Orbitron700.woff
+-rw-r--r--  2.0 unx    18450 b- defN 23-May-26 19:51 kvirt/web/static/vnc/app/styles/base.css
+-rw-r--r--  2.0 unx     4189 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/base64.js
+-rw-r--r--  2.0 unx    11241 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/des.js
+-rw-r--r--  2.0 unx    20381 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/display.js
+-rw-r--r--  2.0 unx     1374 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/encodings.js
+-rw-r--r--  2.0 unx     1170 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/inflator.js
+-rw-r--r--  2.0 unx    74196 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/rfb.js
+-rw-r--r--  2.0 unx     9130 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/websock.js
+-rw-r--r--  2.0 unx      628 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/decoders/copyrect.js
+-rw-r--r--  2.0 unx     4814 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/decoders/hextile.js
+-rw-r--r--  2.0 unx     1739 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/decoders/raw.js
+-rw-r--r--  2.0 unx     1210 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/decoders/rre.js
+-rw-r--r--  2.0 unx     9662 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/decoders/tight.js
+-rw-r--r--  2.0 unx      768 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/decoders/tightpng.js
+-rw-r--r--  2.0 unx    11438 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/input/domkeytable.js
+-rw-r--r--  2.0 unx     3804 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/input/fixedkeys.js
+-rw-r--r--  2.0 unx    13090 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/input/keyboard.js
+-rw-r--r--  2.0 unx    34609 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/input/keysym.js
+-rw-r--r--  2.0 unx    25374 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/input/keysymdef.js
+-rw-r--r--  2.0 unx     9995 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/input/mouse.js
+-rw-r--r--  2.0 unx     5283 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/input/util.js
+-rw-r--r--  2.0 unx     2580 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/input/vkeys.js
+-rw-r--r--  2.0 unx    14256 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/input/xtscancodes.js
+-rw-r--r--  2.0 unx     3155 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/util/browser.js
+-rw-r--r--  2.0 unx     7556 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/util/cursor.js
+-rw-r--r--  2.0 unx     4221 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/util/events.js
+-rw-r--r--  2.0 unx      896 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/util/eventtarget.js
+-rw-r--r--  2.0 unx     1358 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/util/logging.js
+-rw-r--r--  2.0 unx     1866 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/util/polyfill.js
+-rw-r--r--  2.0 unx      301 b- defN 23-May-26 19:51 kvirt/web/static/vnc/core/util/strings.js
+-rw-r--r--  2.0 unx     7388 b- defN 23-May-26 19:51 kvirt/web/static/vnc/vendor/promise.js
+-rw-r--r--  2.0 unx      419 b- defN 23-May-26 19:51 kvirt/web/static/vnc/vendor/browser-es-module-loader/README.md
+-rw-r--r--  2.0 unx      295 b- defN 23-May-26 19:51 kvirt/web/static/vnc/vendor/browser-es-module-loader/rollup.config.js
+-rw-r--r--  2.0 unx     1113 b- defN 23-May-26 19:51 kvirt/web/static/vnc/vendor/browser-es-module-loader/src/babel-worker.js
+-rw-r--r--  2.0 unx     8498 b- defN 23-May-26 19:51 kvirt/web/static/vnc/vendor/browser-es-module-loader/src/browser-es-module-loader.js
+-rw-r--r--  2.0 unx     1084 b- defN 23-May-26 19:51 kvirt/web/static/vnc/vendor/pako/LICENSE
+-rw-r--r--  2.0 unx      301 b- defN 23-May-26 19:51 kvirt/web/static/vnc/vendor/pako/README.md
+-rw-r--r--  2.0 unx     1062 b- defN 23-May-26 19:51 kvirt/web/static/vnc/vendor/pako/lib/utils/common.js
+-rw-r--r--  2.0 unx      666 b- defN 23-May-26 19:51 kvirt/web/static/vnc/vendor/pako/lib/zlib/adler32.js
+-rw-r--r--  2.0 unx     1334 b- defN 23-May-26 19:51 kvirt/web/static/vnc/vendor/pako/lib/zlib/constants.js
+-rw-r--r--  2.0 unx      764 b- defN 23-May-26 19:51 kvirt/web/static/vnc/vendor/pako/lib/zlib/crc32.js
+-rw-r--r--  2.0 unx    60016 b- defN 23-May-26 19:51 kvirt/web/static/vnc/vendor/pako/lib/zlib/deflate.js
+-rw-r--r--  2.0 unx     1251 b- defN 23-May-26 19:51 kvirt/web/static/vnc/vendor/pako/lib/zlib/gzheader.js
+-rw-r--r--  2.0 unx    11690 b- defN 23-May-26 19:51 kvirt/web/static/vnc/vendor/pako/lib/zlib/inffast.js
+-rw-r--r--  2.0 unx    47128 b- defN 23-May-26 19:51 kvirt/web/static/vnc/vendor/pako/lib/zlib/inflate.js
+-rw-r--r--  2.0 unx    11527 b- defN 23-May-26 19:51 kvirt/web/static/vnc/vendor/pako/lib/zlib/inftrees.js
+-rw-r--r--  2.0 unx      560 b- defN 23-May-26 19:51 kvirt/web/static/vnc/vendor/pako/lib/zlib/messages.js
+-rw-r--r--  2.0 unx    38767 b- defN 23-May-26 19:51 kvirt/web/static/vnc/vendor/pako/lib/zlib/trees.js
+-rw-r--r--  2.0 unx      823 b- defN 23-May-26 19:51 kvirt/web/static/vnc/vendor/pako/lib/zlib/zstream.js
+-rw-r--r--  2.0 unx     2509 b- defN 23-May-26 19:51 kvirt/web/templates/bootstrap.html
+-rw-r--r--  2.0 unx    14595 b- defN 23-May-26 19:51 kvirt/web/templates/console.html
+-rw-r--r--  2.0 unx      717 b- defN 23-May-26 19:51 kvirt/web/templates/containercreate.html
+-rw-r--r--  2.0 unx      493 b- defN 23-May-26 19:51 kvirt/web/templates/containerprofiles.html
+-rw-r--r--  2.0 unx     1050 b- defN 23-May-26 19:51 kvirt/web/templates/containerprofilestable.html
+-rw-r--r--  2.0 unx      490 b- defN 23-May-26 19:51 kvirt/web/templates/containers.html
+-rw-r--r--  2.0 unx     1746 b- defN 23-May-26 19:51 kvirt/web/templates/containerstable.html
+-rw-r--r--  2.0 unx     2123 b- defN 23-May-26 19:51 kvirt/web/templates/head.html
+-rw-r--r--  2.0 unx      473 b- defN 23-May-26 19:51 kvirt/web/templates/hosts.html
+-rw-r--r--  2.0 unx     1705 b- defN 23-May-26 19:51 kvirt/web/templates/hoststable.html
+-rw-r--r--  2.0 unx     1119 b- defN 23-May-26 19:51 kvirt/web/templates/imagecreate.html
+-rw-r--r--  2.0 unx      478 b- defN 23-May-26 19:51 kvirt/web/templates/images.html
+-rw-r--r--  2.0 unx      646 b- defN 23-May-26 19:51 kvirt/web/templates/imagestable.html
+-rw-r--r--  2.0 unx      472 b- defN 23-May-26 19:51 kvirt/web/templates/isos.html
+-rw-r--r--  2.0 unx      261 b- defN 23-May-26 19:51 kvirt/web/templates/isostable.html
+-rw-r--r--  2.0 unx      609 b- defN 23-May-26 19:51 kvirt/web/templates/kubecreate.html
+-rw-r--r--  2.0 unx      622 b- defN 23-May-26 19:51 kvirt/web/templates/kubeinfo.html
+-rw-r--r--  2.0 unx      488 b- defN 23-May-26 19:51 kvirt/web/templates/kubeprofiles.html
+-rw-r--r--  2.0 unx      845 b- defN 23-May-26 19:51 kvirt/web/templates/kubeprofilestable.html
+-rw-r--r--  2.0 unx      475 b- defN 23-May-26 19:51 kvirt/web/templates/kubes.html
+-rw-r--r--  2.0 unx     1850 b- defN 23-May-26 19:51 kvirt/web/templates/kubestable.html
+-rw-r--r--  2.0 unx      151 b- defN 23-May-26 19:51 kvirt/web/templates/layout.html
+-rw-r--r--  2.0 unx     5517 b- defN 23-May-26 19:51 kvirt/web/templates/navbar.html
+-rw-r--r--  2.0 unx      882 b- defN 23-May-26 19:51 kvirt/web/templates/networkcreate.html
+-rw-r--r--  2.0 unx      537 b- defN 23-May-26 19:51 kvirt/web/templates/networks.html
+-rw-r--r--  2.0 unx      845 b- defN 23-May-26 19:51 kvirt/web/templates/networkstable.html
+-rw-r--r--  2.0 unx      750 b- defN 23-May-26 19:51 kvirt/web/templates/plancreate.html
+-rw-r--r--  2.0 unx      475 b- defN 23-May-26 19:51 kvirt/web/templates/plans.html
+-rw-r--r--  2.0 unx     1525 b- defN 23-May-26 19:51 kvirt/web/templates/planstable.html
+-rw-r--r--  2.0 unx      859 b- defN 23-May-26 19:51 kvirt/web/templates/poolcreate.html
+-rw-r--r--  2.0 unx      475 b- defN 23-May-26 19:51 kvirt/web/templates/pools.html
+-rw-r--r--  2.0 unx      554 b- defN 23-May-26 19:51 kvirt/web/templates/poolstable.html
+-rw-r--r--  2.0 unx     1282 b- defN 23-May-26 19:51 kvirt/web/templates/productcreate.html
+-rw-r--r--  2.0 unx      484 b- defN 23-May-26 19:51 kvirt/web/templates/products.html
+-rw-r--r--  2.0 unx      895 b- defN 23-May-26 19:51 kvirt/web/templates/productstable.html
+-rw-r--r--  2.0 unx      699 b- defN 23-May-26 19:51 kvirt/web/templates/repocreate.html
+-rw-r--r--  2.0 unx      475 b- defN 23-May-26 19:51 kvirt/web/templates/repos.html
+-rw-r--r--  2.0 unx     1203 b- defN 23-May-26 19:51 kvirt/web/templates/repostable.html
+-rw-r--r--  2.0 unx      958 b- defN 23-May-26 19:51 kvirt/web/templates/vmcreate.html
+-rw-r--r--  2.0 unx      486 b- defN 23-May-26 19:51 kvirt/web/templates/vmprofiles.html
+-rw-r--r--  2.0 unx     1420 b- defN 23-May-26 19:51 kvirt/web/templates/vmprofilestable.html
+-rw-r--r--  2.0 unx      470 b- defN 23-May-26 19:51 kvirt/web/templates/vms.html
+-rw-r--r--  2.0 unx     4894 b- defN 23-May-26 19:51 kvirt/web/templates/vmstable.html
+-rw-r--r--  2.0 unx    11358 b- defN 23-May-26 19:53 kcli-99.0.202305261953.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2914 b- defN 23-May-26 19:53 kcli-99.0.202305261953.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-26 19:53 kcli-99.0.202305261953.dist-info/WHEEL
+-rw-r--r--  2.0 unx      209 b- defN 23-May-26 19:53 kcli-99.0.202305261953.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-May-26 19:53 kcli-99.0.202305261953.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    58528 b- defN 23-May-26 19:53 kcli-99.0.202305261953.dist-info/RECORD
+596 files, 4545898 bytes uncompressed, 1378825 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -126,20 +126,14 @@
 
 Filename: kvirt/cluster/k3s/ctlplanes.sh
 Comment: 
 
 Filename: kvirt/cluster/k3s/ctlplanes.yml
 Comment: 
 
-Filename: kvirt/cluster/k3s/gcp-hack.service
-Comment: 
-
-Filename: kvirt/cluster/k3s/gcp-hack.sh
-Comment: 
-
 Filename: kvirt/cluster/k3s/join.sh
 Comment: 
 
 Filename: kvirt/cluster/k3s/kcli_default.yml
 Comment: 
 
 Filename: kvirt/cluster/k3s/keepalived.conf
@@ -168,20 +162,14 @@
 
 Filename: kvirt/cluster/kubeadm/ctlplanes.yml
 Comment: 
 
 Filename: kvirt/cluster/kubeadm/deploy.sh
 Comment: 
 
-Filename: kvirt/cluster/kubeadm/gcp-hack.service
-Comment: 
-
-Filename: kvirt/cluster/kubeadm/gcp-hack.sh
-Comment: 
-
 Filename: kvirt/cluster/kubeadm/join.sh
 Comment: 
 
 Filename: kvirt/cluster/kubeadm/kcli_default.yml
 Comment: 
 
 Filename: kvirt/cluster/kubeadm/keepalived.conf
@@ -519,23 +507,14 @@
 
 Filename: kvirt/cluster/openshift/fake_kubeconfig.json
 Comment: 
 
 Filename: kvirt/cluster/openshift/fake_pull.json
 Comment: 
 
-Filename: kvirt/cluster/openshift/gcp-hack.preset
-Comment: 
-
-Filename: kvirt/cluster/openshift/gcp-hack.service
-Comment: 
-
-Filename: kvirt/cluster/openshift/gcp-hack.sh
-Comment: 
-
 Filename: kvirt/cluster/openshift/haproxy.cfg
 Comment: 
 
 Filename: kvirt/cluster/openshift/haproxy.cfg.kubevirt
 Comment: 
 
 Filename: kvirt/cluster/openshift/httpd.yaml
@@ -1017,14 +996,20 @@
 
 Filename: kvirt/providers/fake/__init__.py
 Comment: 
 
 Filename: kvirt/providers/gcp/__init__.py
 Comment: 
 
+Filename: kvirt/providers/gcp/gcp-hack.service
+Comment: 
+
+Filename: kvirt/providers/gcp/gcp-hack.sh
+Comment: 
+
 Filename: kvirt/providers/ibm/__init__.py
 Comment: 
 
 Filename: kvirt/providers/kubevirt/__init__.py
 Comment: 
 
 Filename: kvirt/providers/kvm/__init__.py
@@ -1779,26 +1764,26 @@
 
 Filename: kvirt/web/templates/vms.html
 Comment: 
 
 Filename: kvirt/web/templates/vmstable.html
 Comment: 
 
-Filename: kcli-99.0.202305260939.dist-info/LICENSE
+Filename: kcli-99.0.202305261953.dist-info/LICENSE
 Comment: 
 
-Filename: kcli-99.0.202305260939.dist-info/METADATA
+Filename: kcli-99.0.202305261953.dist-info/METADATA
 Comment: 
 
-Filename: kcli-99.0.202305260939.dist-info/WHEEL
+Filename: kcli-99.0.202305261953.dist-info/WHEEL
 Comment: 
 
-Filename: kcli-99.0.202305260939.dist-info/entry_points.txt
+Filename: kcli-99.0.202305261953.dist-info/entry_points.txt
 Comment: 
 
-Filename: kcli-99.0.202305260939.dist-info/top_level.txt
+Filename: kcli-99.0.202305261953.dist-info/top_level.txt
 Comment: 
 
-Filename: kcli-99.0.202305260939.dist-info/RECORD
+Filename: kcli-99.0.202305261953.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kvirt/cluster/k3s/bootstrap.sh

```diff
@@ -2,19 +2,14 @@
 {% set extra_args = extra_ctlplane_args %}
 {% endif %}
 
 {% if 'ubuntu' in image %}
 apt-get -y install curl
 {% endif %}
 
-{% if config_type == 'gcp' %}
-systemctl enable --now gcp-hack
-ufw allow from any to any port 6443,2379,2380 proto tcp
-{% endif %}
-
 export IP={{ api_ip if cloud_lb else "$(curl -s ifconfig.me)" if config_type in ['aws', 'gcp', 'ibmcloud'] else '$(hostname -I | cut -f1 -d" ")' }}
 curl -sfL https://get.k3s.io | {{ install_k3s_args }} K3S_TOKEN={{ token }} sh -s - server {{ '--cluster-init' if ctlplanes > 1 else '' }} {{ extra_args|join(" ") }} {{ '--tls-san $IP' if not cloud_lb and config_type in ['aws', 'gcp', 'ibmcloud'] else '' }}
 export K3S_TOKEN=$(cat /var/lib/rancher/k3s/server/node-token)
 sed "s/127.0.0.1/$IP/" /etc/rancher/k3s/k3s.yaml > /root/kubeconfig
 if [ -d /root/manifests ] ; then
   mv /root/manifests {{ data_dir|default("/var/lib/rancher/k3s/server") }}
 fi
```

## kvirt/cluster/k3s/ctlplanes.sh

```diff
@@ -1,15 +1,11 @@
 {% if extra_ctlplane_args %}
 {% set extra_args = extra_ctlplane_args %}
 {% endif %}
 
-{% if config_type == 'gcp' %}
-systemctl enable --now gcp-hack
-ufw allow from any to any port 6443,2379,2380 proto tcp
-{% endif %}
 {% if 'ubuntu' in image %}
 apt-get -y install curl
 {% endif %}
 {% if sdn != None and sdn == 'cilium' %}
 echo bpffs /sys/fs/bpf bpf defaults 0 0 >> /etc/fstab
 mount /sys/fs/bpf
 {% endif %}
```

## kvirt/cluster/k3s/ctlplanes.yml

```diff
@@ -8,17 +8,14 @@
 {% endif %}
 
 {% set all_files = files|default([]) %}
 {% set all_scripts = ["ctlplanes.sh"] %}
 {% if config_type not in ['aws', 'gcp', 'ibm'] and api_ip != None %}
 {% do all_files.append("keepalived.conf") %}
 {% do all_scripts.append("keepalived.sh") %}
-{% elif config_type == 'gcp' %}
-{% do all_files.append({"path" : "/usr/local/bin/gcp-hack.sh", "origin": 'gcp-hack.sh', "mode": 755}) %}
-{% do all_files.append({"path" : "/usr/lib/systemd/system/gcp-hack.service", "origin": 'gcp-hack.service', "mode": 644}) %}
 {% endif %}
 
 {% set default_ctlplane = cluster + '-ctlplane-' + number|string %}
 {% set ctlplane = vmrules_names[number] if vmrules_names is defined else default_ctlplane %}
 
 {{ ctlplane }}:
  image: {{ image }}
```

## kvirt/cluster/k3s/workers.sh

```diff
@@ -1,10 +1,7 @@
-{% if config_type == 'gcp' %}
-systemctl enable --now gcp-hack
-{% endif %}
 {% if 'ubuntu' in image %}
 apt-get -y install curl
 {% endif %}
 {% if sdn != None and sdn == 'cilium' %}
 mount bpffs -t bpf /sys/fs/bpf
 {% endif %}
 bash /root/join.sh
```

## kvirt/cluster/k3s/workers.yml

```diff
@@ -15,18 +15,10 @@
  keys: {{ keys }}
  numcpus: {{ worker_numcpus | default(numcpus, numcpus) }}
  memory: {{ worker_memory | default(memory, memory) }}
  nets: {{ [network] + extra_networks }}
  disks: {{ [disk_size] + extra_disks }}
  files:
  - join.sh
-{% if config_type == 'gcp' %}
- - path: /usr/local/bin/gcp-hack.sh
-   origin: gcp-hack.sh
-   mode: 755
- - path: /usr/lib/systemd/system/gcp-hack.service
-   origin: gcp-hack.service
-   mode: 644
-{% endif %}
  scripts:
  - workers.sh
 {% endfor %}
```

## kvirt/cluster/kubeadm/ctlplanes.yml

```diff
@@ -17,21 +17,14 @@
  domain: {{ domain }}
  nets: {{ [primary_network] + extra_networks }}
  disks: {{ [disk_size] + extra_disks }}
  files:
 {% if config_type not in ['aws', 'gcp', 'ibm'] %}
  - keepalived.conf
  - keepalived.sh
-{% elif config_type == 'gcp' %}
- - path: /usr/local/bin/gcp-hack.sh
-   origin: gcp-hack.sh
-   mode: 755
- - path: /usr/lib/systemd/system/gcp-hack.service
-   origin: gcp-hack.service
-   mode: 644
 {% endif %}
  - path: /root/pre.sh
    origin: pre_{{ 'ubuntu' if ubuntu|default(False) else 'el' }}.sh
  - join.sh
  - deploy.sh
 {% if engine == 'containerd' %}
  - path: /etc/crictl.yaml
```

## kvirt/cluster/kubeadm/deploy.sh

```diff
@@ -1,14 +1,11 @@
 #!/usr/bin/env bash
 
 export PATH=/root:$PATH
 test -f /etc/profile.d/kcli.sh && source /etc/profile.d/kcli.sh
-{% if config_type == 'gcp' %}
-systemctl enable --now gcp-hack
-{% endif %}
 pre.sh
 {% if config_type not in ['aws', 'gcp', 'ibm'] and '%s-ctlplane' % cluster in name %}
 keepalived.sh
 {% endif %}
 
 {% set deploy_script = 'bootstrap.sh' if '%s-ctlplane-0' % cluster in name else 'join.sh' %}
```

## kvirt/cluster/kubeadm/workers.yml

```diff
@@ -17,22 +17,14 @@
  nets: {{ [network] + extra_networks }}
  disks: {{ [disk_size] + extra_disks }}
  files:
  - path: /root/pre.sh
    origin: pre_{{ 'ubuntu' if ubuntu|default(False) else 'el' }}.sh
  - deploy.sh
  - join.sh
-{% if config_type == 'gcp' %}
- - path: /usr/local/bin/gcp-hack.sh
-   origin: gcp-hack.sh
-   mode: 755
- - path: /usr/lib/systemd/system/gcp-hack.service
-   origin: gcp-hack.service
-   mode: 644
-{% endif %}
 {% if engine == 'containerd' %}
  - path: /etc/crictl.yaml
    content: |
      runtime-endpoint: unix:///run/containerd/containerd.sock
      image-endpoint: unix:///run/containerd/containerd.sock
      timeout: 10
 {% endif %}
```

## kvirt/cluster/openshift/cloud_ctlplanes.yml

```diff
@@ -18,26 +18,15 @@
  enableroot: false
  numcpus: {{ ctlplane_numcpus | default(numcpus, numcpus) }}
  memory: {{ ctlplane_memory | default(memory, memory) }}
  nets:
  - name: {{ network }}
  disks:
  - size: {{ disk_size }}
-{% if config_type == 'gcp' %}
- files:
- - path: /usr/local/bin/gcp-hack.sh
-   origin: gcp-hack.sh
-   mode: 755
- - path: /etc/systemd/system/gcp-hack.service
-   origin: gcp-hack.service
-   mode: 644
- - path: /etc/systemd/system-preset/00-gcp-hack.preset
-   origin: gcp-hack.preset
-   mode: 644
-{% elif config_type == 'ibm' %}
+{% if config_type == 'ibm' %}
  files:
   - path: /etc/NetworkManager/dispatcher.d/99-forcedns
     origin: 99-forcedns-ibm
     mode: 755
 {% endif %}
 {% if cloud_tag != None %}
  tags: [{{ cloud_tag }}]
```

## kvirt/providers/gcp/__init__.py

```diff
@@ -9,14 +9,15 @@
 from kvirt.common import pprint, error, warning, get_ssh_pub_key
 from kvirt.defaults import UBUNTUS, METADATA_FIELDS
 from dateutil import parser as dateparser
 from getpass import getuser
 import googleapiclient.discovery
 from google.cloud import dns, storage
 import os
+import re
 from time import sleep
 import webbrowser
 
 binary_types = ['bz2', 'deb', 'jpg', 'gz', 'jpeg', 'iso', 'png', 'rpm', 'tgz', 'zip']
 
 
 class Kgcp(object):
@@ -99,14 +100,15 @@
                metadata={}, securitygroups=[], vmuser=None):
         conn = self.conn
         project = self.project
         zone = self.zone
         region = self.region
         if self.exists(name):
             return {'result': 'failure', 'reason': f"VM {name} already exists"}
+        kubetype = metadata.get('kubetype')
         if flavor is None:
             if numcpus != 1 and numcpus % 2 != 0:
                 return {'result': 'failure', 'reason': "Number of cpus is not even"}
             if memory != 512 and memory % 1024 != 0:
                 return {'result': 'failure', 'reason': "Memory is not multiple of 1024"}
             if numcpus > 1 and memory < 2048:
                 pprint("Rounding memory to 2048Mb as more than one cpu is used")
@@ -220,14 +222,23 @@
                 enablerootcmds = ['sed -i "s/.*PermitRootLogin.*/PermitRootLogin yes/" /etc/ssh/sshd_config',
                                   'systemctl restart sshd']
                 cmds = enablerootcmds + cmds
             newval = {'key': 'ssh-keys', 'value': '\n'.join(finalkeys)}
             body['metadata']['items'].append(newval)
             newval = {'key': 'block-project-ssh-keys', 'value': 'TRUE'}
             body['metadata']['items'].append(newval)
+        ctlplane_node = kubetype is not None and 'ctlplane' in name
+        bootstrap_node = ctlplane_node and kubetype != 'openshift' and name.endswith('ctlplane-0')
+        need_gcp_hack = ctlplane_node and not bootstrap_node
+        if need_gcp_hack:
+            gcpdir = os.path.dirname(Kgcp.create.__code__.co_filename)
+            overrides['kube_service'] = 'k3s' if kubetype == 'k3s' else 'kubelet'
+            files.append({"path": "/usr/local/bin/gcp-hack.sh", "origin": f'{gcpdir}/gcp-hack.sh', "mode": 755})
+            files.append({"path": "/etc/systemd/system/gcp-hack.service",
+                          "origin": f'{gcpdir}/gcp-hack.service', "mode": 644})
         if cloudinit:
             if image is not None and common.needs_ignition(image):
                 version = common.ignition_version(image)
                 userdata = common.ignition(name=name, keys=keys, cmds=cmds, nets=nets, gateway=gateway, dns=dns,
                                            domain=domain, files=files, enableroot=enableroot,
                                            overrides=overrides, version=version, plan=plan, image=image,
                                            vmuser=vmuser)
@@ -237,25 +248,26 @@
                                             overrides=overrides, fqdn=True, storemetadata=storemetadata,
                                             vmuser=vmuser)[0]
                 if 'ubuntu' in image.lower() or [entry for entry in UBUNTUS if entry in image]:
                     pkgmgr = "apt-get"
                 else:
                     pkgmgr = "yum"
                 startup_script = "test -f /root/.kcli_startup && exit 0\n"
+                if need_gcp_hack:
+                    startup_script += "systemctl start gcp-hack\n"
                 startup_script += "sleep 10\nwhich cloud-init && touch /root/.kcli_startup && exit 0\n"
                 startup_script += f"{pkgmgr} install -y cloud-init\n"
                 startup_script += "systemctl enable --now cloud-init\n"
                 startup_script += "touch /root/.kcli_startup\nreboot"
                 newval = {'key': 'startup-script', 'value': startup_script}
                 body['metadata']['items'].append(newval)
             newval = {'key': 'user-data', 'value': userdata}
             body['metadata']['items'].append(newval)
-        if 'kubetype' in metadata and metadata['kubetype'] in ["generic", "openshift", "k3s"] and not use_xproject:
+        if kubetype is not None and kubetype in ["generic", "openshift", "k3s"] and not use_xproject:
             kube = metadata['kube']
-            kubetype = metadata['kubetype']
             firewalls = conn.firewalls().list(project=project).execute()
             firewalls = firewalls['items'] if 'items' in firewalls else []
             if not firewalls or not [r for r in firewalls if r['name'] == kube]:
                 pprint(f"Adding vm to security group {kube}")
                 tcp_ports = [22, 443, 2379, 2380]
                 firewall_body = {"name": kube, "direction": "INGRESS", "targetTags": [kube],
                                  "allowed": [{"IPProtocol": "tcp", "ports": tcp_ports}]}
@@ -378,22 +390,23 @@
         return status
 
     def list(self):
         conn = self.conn
         project = self.project
         zone = self.zone
         vms = []
-        results = conn.instances().list(project=project, zone=zone).execute()
-        if 'items' not in results:
-            return []
-        for vm in results['items']:
+        instances = conn.instances().list(project=project, zone=zone).execute()
+        instances_items = instances.get('items', [])
+        for vm in instances_items:
             try:
                 vms.append(self.info(vm['name'], vm=vm))
             except:
                 continue
+        if not vms:
+            return []
         return sorted(vms, key=lambda x: x['name'])
 
     def console(self, name, tunnel=False, web=False):
         project = self.project
         zone = self.zone
         resource = googleapiclient.discovery.build('cloudresourcemanager', 'v1')
         projectinfo = resource.projects().get(projectId=project).execute()
@@ -546,22 +559,22 @@
     def volumes(self, iso=False):
         projects = ['centos-cloud', 'coreos-cloud', 'cos-cloud', 'debian-cloud', 'fedora-coreos-cloud', 'rhel-cloud',
                     'suse-cloud', 'ubuntu-os-cloud', self.project]
         conn = self.conn
         images = []
         for project in projects:
             results = conn.images().list(project=project, orderBy="creationTimestamp desc").execute()
-            if 'items' in results:
-                for image in results['items']:
-                    if project == self.project:
-                        images.append(image['name'])
-                    elif 'family' not in image:
-                        continue
-                    elif image['family'] not in images:
-                        images.append(image['family'])
+            image_items = results.get('items', [])
+            for image in image_items:
+                if project == self.project:
+                    images.append(image['name'])
+                elif 'family' not in image:
+                    continue
+                elif image['family'] not in images:
+                    images.append(image['family'])
         return sorted(images)
 
     def delete(self, name, snapshots=False):
         conn = self.conn
         project = self.project
         zone = self.zone
         try:
@@ -737,21 +750,21 @@
 
     def list_disks(self):
         disks = {}
         conn = self.conn
         project = self.project
         zone = self.zone
         alldisks = conn.disks().list(zone=zone, project=project).execute()
-        if 'items' in alldisks:
-            for disk in alldisks['items']:
-                if self.debug:
-                    print(disk)
-                diskname = disk['name']
-                pool = os.path.basename(disk['type'])
-                disks[diskname] = {'pool': pool, 'path': zone}
+        alldisks_items = alldisks.get('items', [])
+        for disk in alldisks_items:
+            if self.debug:
+                print(disk)
+            diskname = disk['name']
+            pool = os.path.basename(disk['type'])
+            disks[diskname] = {'pool': pool, 'path': zone}
         return disks
 
     def add_nic(self, name, network):
         print("not implemented")
         return
 
     def delete_nic(self, name, interface):
@@ -835,20 +848,19 @@
 
 # should return a dict of pool strings
     def list_pools(self):
         print("not implemented")
         return []
 
     def list_project_networks(self, project):
+        networks = {}
         conn = self.conn
         nets = conn.networks().list(project=project).execute()
-        if 'items' not in nets:
-            return {}
-        networks = {}
-        for net in nets['items']:
+        nets_items = nets.get('items', [])
+        for net in nets_items:
             if self.debug:
                 print(net)
             networkname = net['name']
             cidr = net['IPv4Range'] if 'IPv4Range' in net else ''
             dhcp = True
             domainname = ''
             mode = ''
@@ -1073,17 +1085,16 @@
 
     def list_flavors(self):
         conn = self.conn
         project = self.project
         zone = self.zone
         flavors = []
         results = conn.machineTypes().list(project=project, zone=zone).execute()
-        if 'items' not in results:
-            return []
-        for flavor in results['items']:
+        flavors_items = results.get('items', [])
+        for flavor in flavors_items:
             if self.debug:
                 print(flavor)
             name = flavor['name']
             numcpus = flavor['guestCpus']
             memory = flavor['memoryMb']
             flavors.append([name, numcpus, memory])
         return flavors
@@ -1115,22 +1126,30 @@
         conn_beta = self.conn_beta
         project = self.project
         zone = self.zone
         region = self.region
         instances = []
         vmpath = f"https://www.googleapis.com/compute/v1/projects/{project}/zones/{zone}/instances"
         use_xproject, vm_subnets = False, []
-        if vms:
-            for index, vm in enumerate(vms):
-                update = self.update_metadata(vm, 'loadbalancer', sane_name, append=True)
-                if update == 0:
-                    instances.append({"instance": f"{vmpath}/{vm}"})
-                if index == 0:
-                    vm_subnets = self.vm_ports(vm)
-                    use_xproject = self.xproject in [self.list_subnets()[n]['az'] for n in vm_subnets]
+        if not vms:
+            msg = "Creating a load balancer requires to specify some vms"
+            error(msg)
+            return {'result': 'failure', 'reason': msg}
+        for vm in vms:
+            if not self.exists(vm):
+                msg = f"Vm {vm} not found"
+                error(msg)
+                return {'result': 'failure', 'reason': msg}
+        for index, vm in enumerate(vms):
+            update = self.update_metadata(vm, 'loadbalancer', sane_name, append=True)
+            if update == 0:
+                instances.append({"instance": f"{vmpath}/{vm}"})
+            if index == 0:
+                vm_subnets = self.vm_ports(vm)
+                use_xproject = self.xproject in [self.list_subnets()[n]['az'] for n in vm_subnets]
         # add checkpath handling (and default to http when defined)
         health_check_body = {"checkIntervalSec": "10", "timeoutSec": "10", "unhealthyThreshold": 3,
                              "healthyThreshold": 3, "name": sane_name}
         health_check_body["type"] = "TCP"
         health_check_body["tcpHealthCheck"] = {"port": checkport}
         pprint(f"Creating healthcheck {name}")
         if internal:
@@ -1191,16 +1210,17 @@
             forwarding_rule_body["subnetwork"] = f'projects/{network_project}/regions/{region}/subnetworks/{netname}'
         pprint(f"Creating forwarding rule {forwarding_name}")
         operation = conn.forwardingRules().insert(project=project, region=region, body=forwarding_rule_body).execute()
         self._wait_for_operation(operation)
         if not use_xproject:
             firewall_body = {"name": sane_name, "direction": "INGRESS",
                              "allowed": [{"IPProtocol": "tcp", "ports": ports}]}
-            if sane_name.startswith('api-') or sane_name.startswith('apps-'):
-                kube = '-'.join(sane_name.split('-')[1:])
+            first_vm = vms[0]
+            if '-ctlplane-' in first_vm or '-worker-' in first_vm and re.search(r'\d+$', first_vm):
+                kube = first_vm.split('-')[0]
                 firewall_body["targetTags"] = [kube]
             pprint(f"Creating firewall rule {sane_name}")
             operation = conn.firewalls().insert(project=project, body=firewall_body).execute()
             self._wait_for_operation(operation)
         if domain is not None:
             if dnsclient is not None:
                 return ip
@@ -1213,112 +1233,112 @@
         name = name.replace('.', '-')
         conn = self.conn
         conn_beta = self.conn_beta
         project = self.project
         zone = self.zone
         region = self.region
         firewall_rules = conn.firewalls().list(project=project).execute()
-        if 'items' in firewall_rules:
-            for firewall_rule in firewall_rules['items']:
-                firewall_rule_name = firewall_rule['name']
-                if firewall_rule_name == name:
-                    pprint(f"Deleting firewall rule {name}")
-                    operation = conn.firewalls().delete(project=project, firewall=name).execute()
-                    self._wait_for_operation(operation)
+        firewall_rules_items = firewall_rules.get('items', [])
+        for firewall_rule in firewall_rules_items:
+            firewall_rule_name = firewall_rule['name']
+            if firewall_rule_name == name:
+                pprint(f"Deleting firewall rule {name}")
+                operation = conn.firewalls().delete(project=project, firewall=name).execute()
+                self._wait_for_operation(operation)
         forwarding_rules = conn.forwardingRules().list(project=project, region=region).execute()
-        if 'items' in forwarding_rules:
-            for forwarding_rule in forwarding_rules['items']:
-                forwarding_rule_name = forwarding_rule['name']
-                if forwarding_rule_name == name or forwarding_rule_name.startswith(f'{name}-'):
-                    pprint(f"Deleting forwarding rule {forwarding_rule_name}")
-                    operation = conn.forwardingRules().delete(project=project, region=region,
-                                                              forwardingRule=forwarding_rule_name).execute()
-                    self._wait_for_operation(operation)
-                    pprint("Waiting to make sure forwarding rule is gone")
-                    timeout = 0
-                    deleted = False
-                    while not deleted:
-                        new_forwarding_rules = conn.forwardingRules().list(project=project, region=region).execute()
-                        if 'items' not in new_forwarding_rules:
-                            deleted = True
-                        elif [f['name'] for f in new_forwarding_rules['items'] if f['name'] == forwarding_rule_name]:
-                            sleep(5)
-                            timeout += 5
-                        elif timeout >= 60:
-                            warning("Timeout waiting for forwarding rule to be gone")
-                            break
+        forwarding_rules_items = forwarding_rules.get('items', [])
+        for forwarding_rule in forwarding_rules_items:
+            forwarding_rule_name = forwarding_rule['name']
+            if forwarding_rule_name == name or forwarding_rule_name.startswith(f'{name}-'):
+                pprint(f"Deleting forwarding rule {forwarding_rule_name}")
+                operation = conn.forwardingRules().delete(project=project, region=region,
+                                                          forwardingRule=forwarding_rule_name).execute()
+                self._wait_for_operation(operation)
+                pprint("Waiting to make sure forwarding rule is gone")
+                timeout = 0
+                while True:
+                    if timeout >= 60:
+                        warning("Timeout waiting for forwarding rule to be gone")
+                        break
+                    new_forwarding_rules = conn.forwardingRules().list(project=project, region=region).execute()
+                    items = new_forwarding_rules.get('items', [])
+                    if not items or not [f for f in items if f['name'] == forwarding_rule_name]:
+                        break
+                    else:
+                        sleep(5)
+                        timeout += 5
         try:
             address = conn_beta.addresses().get(project=project, region=region, address=name).execute()
             if 'labels' in address and 'domain' in address['labels'] and 'dnsclient' not in address['labels']:
                 domain = address["labels"]["domain"].replace('-', '.')
                 pprint(f"Deleting DNS {name}.{domain}")
                 self.delete_dns(name, domain=domain)
             pprint(f"Deleting address {name}")
             operation = conn.addresses().delete(project=project, region=region, address=name).execute()
             self._wait_for_operation(operation)
         except Exception as e:
             if self.debug:
                 print(e)
             pass
         backendservices = conn.regionBackendServices().list(project=project, region=region).execute()
-        if 'items' in backendservices:
-            for backendservice in backendservices['items']:
-                backendservice_name = backendservice['name']
-                if backendservice_name == name:
-                    internal = True if backendservice['loadBalancingScheme'] == 'INTERNAL' else False
-                    pprint(f"Deleting backend service {name}")
-                    operation = conn.regionBackendServices().delete(project=project, region=region,
-                                                                    backendService=name).execute()
+        backendservices_items = backendservices.get('items', [])
+        for backendservice in backendservices_items:
+            backendservice_name = backendservice['name']
+            if backendservice_name == name:
+                internal = True if backendservice['loadBalancingScheme'] == 'INTERNAL' else False
+                pprint(f"Deleting backend service {name}")
+                operation = conn.regionBackendServices().delete(project=project, region=region,
+                                                                backendService=name).execute()
+                self._wait_for_operation(operation)
+                for healthcheck in backendservice.get('healthChecks', []):
+                    healthcheck_short = os.path.basename(healthcheck)
+                    pprint(f"Deleting healthcheck {healthcheck_short}")
+                    if internal:
+                        operation = conn.healthChecks().delete(project=project,
+                                                               healthCheck=healthcheck_short).execute()
+                    else:
+                        operation = conn.regionHealthChecks().delete(project=project, region=region,
+                                                                     healthCheck=healthcheck_short).execute()
                     self._wait_for_operation(operation)
-                    for healthcheck in backendservice.get('healthChecks', []):
-                        healthcheck_short = os.path.basename(healthcheck)
-                        pprint(f"Deleting healthcheck {healthcheck_short}")
-                        if internal:
-                            operation = conn.healthChecks().delete(project=project,
-                                                                   healthCheck=healthcheck_short).execute()
-                        else:
-                            operation = conn.regionHealthChecks().delete(project=project, region=region,
-                                                                         healthCheck=healthcheck_short).execute()
-                        self._wait_for_operation(operation)
         instancegroups = conn.instanceGroups().list(project=project, zone=zone).execute()
-        if 'items' in instancegroups:
-            for instancegroup in instancegroups['items']:
-                instancegroup_name = instancegroup['name']
-                if instancegroup_name == name:
-                    pprint(f"Deleting instance group {name}")
-                    operation = conn.instanceGroups().delete(project=project, zone=zone, instanceGroup=name).execute()
-                    self._wait_for_operation(operation)
+        instancegroups_items = instancegroups.get('items', [])
+        for instancegroup in instancegroups_items:
+            instancegroup_name = instancegroup['name']
+            if instancegroup_name == name:
+                pprint(f"Deleting instance group {name}")
+                operation = conn.instanceGroups().delete(project=project, zone=zone, instanceGroup=name).execute()
+                self._wait_for_operation(operation)
         if dnsclient is not None:
             return dnsclient
         return {'result': 'success'}
 
     def list_loadbalancers(self):
         conn = self.conn
         project = self.project
         region = self.region
         results = []
-        results1 = conn.globalForwardingRules().list(project=project).execute()
-        results2 = conn.forwardingRules().list(project=project, region=region).execute()
-        if 'items' in results1:
-            for lb in results1['items']:
-                name = lb['name']
-                ip = lb['IPAddress']
-                protocol = lb['IPProtocol']
-                port = lb['port']
-                target = os.path.basename(lb['target'])
-                results.append([name, ip, protocol, port, target])
-        if 'items' in results2:
-            for lb in results2['items']:
-                name = lb['name']
-                ip = lb['IPAddress']
-                protocol = lb['IPProtocol']
-                port = lb['portRange'] if 'portRange' in lb else ','.join(lb['ports'])
-                target = lb['target'] if 'target' in lb else lb['backendService']
-                target = os.path.basename(target)
-                results.append([name, ip, protocol, port, target])
+        global_forwarding_rules = conn.globalForwardingRules().list(project=project).execute()
+        global_forwarding_rules_items = global_forwarding_rules.get('items', [])
+        forwarding_rules = conn.forwardingRules().list(project=project, region=region).execute()
+        forwarding_rules_items = forwarding_rules.get('items', [])
+        for lb in global_forwarding_rules_items:
+            name = lb['name']
+            ip = lb['IPAddress']
+            protocol = lb['IPProtocol']
+            port = lb['port']
+            target = os.path.basename(lb['target'])
+            results.append([name, ip, protocol, port, target])
+        for lb in forwarding_rules_items:
+            name = lb['name']
+            ip = lb['IPAddress']
+            protocol = lb['IPProtocol']
+            port = lb['portRange'] if 'portRange' in lb else ','.join(lb['ports'])
+            target = lb['target'] if 'target' in lb else lb['backendService']
+            target = os.path.basename(target)
+            results.append([name, ip, protocol, port, target])
         return results
 
     def create_bucket(self, bucket, public=False):
         client = storage.Client(self.project)
         if bucket in self.list_buckets():
             error(f"Bucket {bucket} already there")
             return
```

## kvirt/version/git

```diff
@@ -1 +1 @@
-71f857a 2023/05/26
+4d570af 2023/05/26
```

## Comparing `kcli-99.0.202305260939.dist-info/LICENSE` & `kcli-99.0.202305261953.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kcli-99.0.202305260939.dist-info/METADATA` & `kcli-99.0.202305261953.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kcli
-Version: 99.0.202305260939
+Version: 99.0.202305261953
 Summary: Provisioner/Manager for Libvirt/Vsphere/Aws/Gcp/Kubevirt/Ovirt/Openstack/IBM Cloud and containers
 Home-page: http://github.com/karmab/kcli
 Author: Karim Boumedhel
 Author-email: karimboumedhel@gmail.com
 License: ASL
 Platform: UNKNOWN
 License-File: LICENSE
```

## Comparing `kcli-99.0.202305260939.dist-info/RECORD` & `kcli-99.0.202305261953.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -33,47 +33,43 @@
 kvirt/cluster/hypershift/nmstateconfig.yml.j2,sha256=EjNalSAXko4ZVEN-tnMJn3l59s2_-uBYSDN_C2SWZ6c,1587
 kvirt/cluster/hypershift/nodepool.yaml,sha256=CMRrPOwGSLCZNkO3oZU5JePksgwggxR4w556UqEikJw,752
 kvirt/cluster/hypershift/nonlocalbind.conf,sha256=eRCLfWYHqx2UgY3QE1pbXm2iFwERatyihNySEEbeuE8,60
 kvirt/cluster/hypershift/staticpods/coredns.yml,sha256=eWg3JyDJBEajn_jwvlx8SfvgEpe2GQUif-QWkPOFdW4,1992
 kvirt/cluster/hypershift/staticpods/keepalived.yml,sha256=3IP1snMk0P3l30qaCFAMtC2gGBYoAocRQ2UX5T2Gzoc,2244
 kvirt/cluster/hypershift/staticpods/mdns.yml,sha256=ttElI3ATZ2Y1kR1t5AJrcf-kdA6_t3RifaLOo4wU-IY,1721
 kvirt/cluster/k3s/__init__.py,sha256=1fLj2IKBx7sck9oRieeCpOFYTY5cbZWAzZ_Uv1DtlJY,11453
-kvirt/cluster/k3s/bootstrap.sh,sha256=AEuqTS8ISbHFnRABxCaVzOJhYl2rfGPtHoFEN1EhHEk,1248
+kvirt/cluster/k3s/bootstrap.sh,sha256=INB2JoqetAaYwB7TX3gVtvwpAHQ2N-sKX-a-dZjnh_0,1117
 kvirt/cluster/k3s/bootstrap.yml,sha256=hQ6SyufxcFXp4p93_92lhL0mWh_Hr1ixg9kmHL5QeU8,1050
 kvirt/cluster/k3s/cloud_lb_api.yml,sha256=FaXCkoCEn1jzlrUJv3LD8f2d0MNRi5FO_9za--W_tDw,409
-kvirt/cluster/k3s/ctlplanes.sh,sha256=2dPSucNNtgow8Q9_m7kuzGQ5el1LteX7MzObpZpeSfs,568
-kvirt/cluster/k3s/ctlplanes.yml,sha256=jG47m2RTA8iI-8sSXARab0EzWOC-digfFWv-CV7GM4Q,1329
-kvirt/cluster/k3s/gcp-hack.service,sha256=_qXIYflGx3ASpkA7CcawuQoTUAq3WW03Qc4esJWyIiY,214
-kvirt/cluster/k3s/gcp-hack.sh,sha256=58eqb_9l1sFR27n7IJOTLqYQtlyZC_TGqXRraB_MyP8,424
+kvirt/cluster/k3s/ctlplanes.sh,sha256=6ZoabY5couHlvgcUFJUBK4YURSQ5iYsMZhEnlTAtStQ,438
+kvirt/cluster/k3s/ctlplanes.yml,sha256=yUSEMtcTrp88s7FvD2Bu7SHbzPOu8dxs1iOuEPGV8ZE,1068
 kvirt/cluster/k3s/join.sh,sha256=C_WUN5T2i87wfDe7bosWfE3bi_G0qV1f7jXGKpr77HQ,338
 kvirt/cluster/k3s/kcli_default.yml,sha256=Acehe-2P2QlrgG0HoQHKgZ3WexjMr9yKbah0UjqwgQk,1245
 kvirt/cluster/k3s/keepalived.conf,sha256=XBC6ezpHtjHF2lUU9l3z7zvjp5YYHzGuAz30TXvsFCo,511
 kvirt/cluster/k3s/keepalived.sh,sha256=CpUcNspJekNZGqTBmLk6m_tCaulL5hmKEQLYj-Pxc5w,352
-kvirt/cluster/k3s/workers.sh,sha256=oVlb9rcwQtTiaz7bAC4PRIt6YfCwcBwjmZw_syJbsno,240
-kvirt/cluster/k3s/workers.yml,sha256=q2HenMnv0oAzZK28V1tADewZqIbYY0UlTxAh50TuPfo,914
+kvirt/cluster/k3s/workers.sh,sha256=ErZ5T8uEV8iV7PczVHY4bHXtFC3fsKVtF3k5tS_0vkc,166
+kvirt/cluster/k3s/workers.yml,sha256=HD1MkMcRKwvFndoMJOS8fC1f_O1vfzi27PVwR4GN_7k,709
 kvirt/cluster/kubeadm/__init__.py,sha256=kMiMe-yQQL3jewhQ6Xl4gppNTOAD_Jht-37eZKdheWI,13543
 kvirt/cluster/kubeadm/bootstrap.sh,sha256=bM-p97BDmSlYvof0MehCaqASOycYtSDzDg_0jaowv_k,2707
 kvirt/cluster/kubeadm/bootstrap.yml,sha256=_ir1VAcHlggxsLlclaypz7VZxQUN2_ly7bEqfFcXt9A,1621
 kvirt/cluster/kubeadm/cloud_lb_api.yml,sha256=GnSSmlp-GVhUgPpd3fqyXSxgilyKqA6BmadyQ9z_jO4,325
-kvirt/cluster/kubeadm/ctlplanes.yml,sha256=PHkpHWdyapgr3M81uGc5GPv2LgtzUnsQjWwalL-5ICI,1367
-kvirt/cluster/kubeadm/deploy.sh,sha256=SjiS3NMTheOrfE6HZyqGpuI8iIFS24fNniCfQ0lXDSM,417
-kvirt/cluster/kubeadm/gcp-hack.service,sha256=_qXIYflGx3ASpkA7CcawuQoTUAq3WW03Qc4esJWyIiY,214
-kvirt/cluster/kubeadm/gcp-hack.sh,sha256=EaQ8EbzluHe6dSY5HJ-LGsNMrsNZLHjjlrqhA_s3w8c,355
+kvirt/cluster/kubeadm/ctlplanes.yml,sha256=qgStzWZSSMmIq-qAamSK3sFipdocawNTNWDKRdpGpPc,1172
+kvirt/cluster/kubeadm/deploy.sh,sha256=iCqoY0QHMltWKYRPmhu4DdsVrn4WIsRe9LugeRZzxpk,343
 kvirt/cluster/kubeadm/join.sh,sha256=L-fjfac_zJifQl3tKyE6kJBPCB3jZIYAEKYjmvfWD7s,412
 kvirt/cluster/kubeadm/kcli_default.yml,sha256=cE53vjnAG5RgFN3fP5E8XhyrfNwqQsYRP0-wp28cyB8,1822
 kvirt/cluster/kubeadm/keepalived.conf,sha256=BrQJvLnzLnI3-bf4fJtAt1xYsRyY1FqPYcQEWEJmVbU,563
 kvirt/cluster/kubeadm/keepalived.sh,sha256=QMLjKiVtOa4S4-zBEnXWOoN8a6-FhNxKbSgovw-koOg,424
 kvirt/cluster/kubeadm/kubernetes.repo,sha256=GWh2FNI9B4kd1ADx3piQe9FI7jK39kjeZXsHEe8RiTg,140
 kvirt/cluster/kubeadm/multus.sh,sha256=wfCFekktOYLiXIkRo6Szi_3YTgCKj7i5KX6BLWYCJ-I,179
 kvirt/cluster/kubeadm/nfs.sh,sha256=TUT-ImtcVQyNYek8bsNc0hwzexyN6YgUwhJVqAf6Z9c,572
 kvirt/cluster/kubeadm/nfs.yml,sha256=js0KtTYqI1dtnc018wBXefyVPsCVn_sSneShMCJWUe4,226
 kvirt/cluster/kubeadm/pre_el.sh,sha256=PTqJt5unutNiTV7wY5LWmOjr1zGBpenxo-JSlG8Q-ag,4021
 kvirt/cluster/kubeadm/pre_ubuntu.sh,sha256=LDE0nySnPoxzRMJcnP7QxMZkjG4DTj0QxkqYNBpkI9k,3906
 kvirt/cluster/kubeadm/registry.yml,sha256=olLPTvazYAuwMVmDHjCDWeC2n7Elo2smAqH0xUSsD_M,2127
-kvirt/cluster/kubeadm/workers.yml,sha256=lxyrFJn1Yty-LqMO3ze1RjKfAS1j_gW7HDfprGNrQBY,1154
+kvirt/cluster/kubeadm/workers.yml,sha256=bozEotFmtc_Op6APuMdreF86i3t_2BrS_KVOFBQtAK0,949
 kvirt/cluster/kubeadm/apps/argocd/ingress.yml,sha256=t6U1QnaTq4_yxjQMsMQaMiddx2ROg2vr9kCZeta4v5Y,487
 kvirt/cluster/kubeadm/apps/argocd/install.sh,sha256=e9OM3g4QaWX4yDI3DEjyx_sb09yR95mgl3tdwZET4c4,2134
 kvirt/cluster/kubeadm/apps/argocd/kcli_default.yml,sha256=Zp_vKiNLNtMnOwxM4beKjBAZOzt-rw2c9PS0xk0eC64,71
 kvirt/cluster/kubeadm/apps/argocd/uninstall.sh,sha256=81yj7KCDrdmgnXwAGNepJC8BK8LUSPO-3iUQfwma5VA,314
 kvirt/cluster/kubeadm/apps/autolabeller/install.sh,sha256=WdBcqqlvi59rIJsqkZrlTZUbHN79vIe4gwgjNXz_080,90
 kvirt/cluster/kubeadm/apps/autolabeller/uninstall.sh,sha256=fnH5aHzNpi4tr-7vDyKkAQqcDBhUH6Q9oTNUx7Zovrg,91
 kvirt/cluster/kubeadm/apps/certmanager/install.sh,sha256=4kKTZqQ4fzJdgiVVEwmo86820PLwODtx7CmUE8_XJJ4,380
@@ -150,15 +146,15 @@
 kvirt/cluster/openshift/__init__.py,sha256=Ew47LajY4MguoCqRvU_Aiw_FshHpwNsQA8ERapjEg3Q,81595
 kvirt/cluster/openshift/autoapprovercron.yml,sha256=MjxtA9fg-TzpQP3mu7tIc--IpmdOaze8hYoCKFSvx8E,1326
 kvirt/cluster/openshift/autorules.yml,sha256=YigI0IlT0ah7WhdqQTxJfsJgWnJvNdvjs00wDsmUQM4,987
 kvirt/cluster/openshift/bootstrap.yml,sha256=qAQFBBBofSxotTTqV-knV0h1H2qqNNSB14v-TQv4tlc,1630
 kvirt/cluster/openshift/calico.sh.j2,sha256=6HH46S3eM3V7sHIXzWiYk739QwUAqAWl5M0hmFqyKNU,250
 kvirt/cluster/openshift/chrony.conf,sha256=WYo7cseCaZMx-JP6p9RFnsmmwlHg8whKQA4DxLZx_jI,107
 kvirt/cluster/openshift/cloud_bootstrap.yml,sha256=X5-ib8HK_4iuJ4JnFYIG39LBXhbr7cdGIHP473wnlJ4,629
-kvirt/cluster/openshift/cloud_ctlplanes.yml,sha256=qZ7g1rxboh3_HVFPzJgmfiSUhrFYSUnwXBdlHwPfG3o,1086
+kvirt/cluster/openshift/cloud_ctlplanes.yml,sha256=YyOZbZq7S9I8W4UQHKujBUJrS1Wy5gtAo7Ey5Ql9qus,792
 kvirt/cluster/openshift/cloud_dns.yml,sha256=ydqv3cOV7xMpvxm-52ktBI8VivjEZN7aKWWHJciJVsU,217
 kvirt/cluster/openshift/cloud_lb_api.yml,sha256=J5TSZxmZy-2iOJclqgHBud03xZNSVUOx_JUW1bv0g14,616
 kvirt/cluster/openshift/cloud_lb_apps.yml,sha256=EyCGRluLJO1AxfqeXTRtIZMnYHxsDimYjgl104TzcLo,204
 kvirt/cluster/openshift/cloud_workers.yml,sha256=z2sxSOUk0wNMiOJO2pS0nOBegvtv0vs0fNTFWEcqkoA,703
 kvirt/cluster/openshift/cluster-ingress-02-config.yml,sha256=HQZiT7gFAeL1UXqWFSZMSnUAf7pHQC3j31yuH1DnXBc,123
 kvirt/cluster/openshift/cluster-scheduler-02-config.yml,sha256=qpbRXIsn_GLnZaG6RgfKe2VY5kzX53A1aMcRGz2u7S8,159
 kvirt/cluster/openshift/config.hcl.templ,sha256=H1uWG66pGmPDlfuJQUlYjC0BwK2ZXKIGdivlhdLhQ4s,224
@@ -169,17 +165,14 @@
 kvirt/cluster/openshift/ctlplanes.yml,sha256=XEimn8FutO5G07j5CrQJX_W9BYxZYpGCgnfBDZn92Go,2278
 kvirt/cluster/openshift/dhcp.conf,sha256=8Rzp2F9q7Hij49sOkz8DokUwrrvPs6o5QgGK78MD5eQ,326
 kvirt/cluster/openshift/dhcp.sh,sha256=LbzXUmRCUieNs1FVhKNVkoa7ZUKDPLjHke6fyIR39eU,106
 kvirt/cluster/openshift/dhcp.yml,sha256=rQok85vJDgSPXtSONY3XFEDLBZJNq0yWeE53x-_GhGc,536
 kvirt/cluster/openshift/disconnected.yml,sha256=TqPZEtKQDev57p6FjehMXKEKQJubX6vTqqEHFMWgB0M,836
 kvirt/cluster/openshift/fake_kubeconfig.json,sha256=XxFI3MSxrYbA6-4U8W5vSVFxrQmOeTOxAVzc7e1ngNc,8945
 kvirt/cluster/openshift/fake_pull.json,sha256=FMotW4LO1fkynpj-hCMCQYQ6LA5if7uNAAL6sqyHdKQ,35
-kvirt/cluster/openshift/gcp-hack.preset,sha256=nvUq6njQw6zLDnd7lCr24TR3YtYIn1KRLjKhZEumXQI,24
-kvirt/cluster/openshift/gcp-hack.service,sha256=urrMkMFFpNsb4f8ebrebn9ghrwh8ZJf__o_bS1Dhedc,320
-kvirt/cluster/openshift/gcp-hack.sh,sha256=EaQ8EbzluHe6dSY5HJ-LGsNMrsNZLHjjlrqhA_s3w8c,355
 kvirt/cluster/openshift/haproxy.cfg,sha256=IpADcEMF4BC2Xbk2MLgQluCvW0M7F1be_OMBRw83ODo,1792
 kvirt/cluster/openshift/haproxy.cfg.kubevirt,sha256=7X7TcU6qLFjPpaayWYROnsjmQroHVZzoTskyeHoB-1U,2483
 kvirt/cluster/openshift/httpd.yaml,sha256=KES_fEXyFkC0Uw8Mp4czJPze-ReAxSl-Ux6-F85ql4k,902
 kvirt/cluster/openshift/ignition.j2,sha256=lMjNuMVciXjGcf66ZLOaO-BCgd7eTP1FOYauSSNPM7I,524
 kvirt/cluster/openshift/install-config.yaml,sha256=CTtWGZR6pW-dPzlL1J5oTQpVxo0kCvbvqPNr7HYX3UQ,3562
 kvirt/cluster/openshift/iso.sh,sha256=JdcEzxsNYW0HW7n5SU1IDlI9gCEYT0MXtf6W_t8HKQE,2691
 kvirt/cluster/openshift/kcli-ipv6.conf.j2,sha256=y2KAdA2fGNUO-Nazj9EEgUawrzFQeFb1Y_USBN9BySI,237
@@ -334,28 +327,30 @@
 kvirt/ksushy/templates/virtualmedias.json,sha256=IocFk2ecKvgnzO8nyxsBhJEdU62X_KvX0m4EunVQscw,705
 kvirt/miniconsole/__init__.py,sha256=jCaDAk4Yq2fjOR_4GrnRxMq9CPLolxIJR81_hAk1eZg,2780
 kvirt/nameutils/__init__.py,sha256=f_9tUVxw9yIz_JRGU-L39ZHoYPjfkclabHjC7CVl1QQ,3488
 kvirt/providers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kvirt/providers/sampleprovider.py,sha256=IJHdRbhSrL10r-i1OLwiKhFxhHXewTyzso9SWlotVnQ,8935
 kvirt/providers/aws/__init__.py,sha256=SmkNTfX22BYyWjV0kV5VcwO1sO6rpMtfbSugbhuplKY,65799
 kvirt/providers/fake/__init__.py,sha256=ufPQ7JdEkz7fQAiwb-LfHwrKzBFZrpiwk-8Hh8oI_XI,479
-kvirt/providers/gcp/__init__.py,sha256=7oB_YFmn8pqrI9rSxnKdbKgT3qBluWB3XPreh7UJJCg,65306
+kvirt/providers/gcp/__init__.py,sha256=copl6sCBXjACWMt3gcs4Pw-m0HNs__b6xQAMlNsJi10,66344
+kvirt/providers/gcp/gcp-hack.service,sha256=gG35O6KTLlGqIMwrSBqb_id-h3SWm_us_yLkLfQelOw,175
+kvirt/providers/gcp/gcp-hack.sh,sha256=K4ZDgWo9AoysBEMAZW3pj_5_1KmQAz0th49EqamsLVY,231
 kvirt/providers/ibm/__init__.py,sha256=MjwZU6J4yJ6usf3ZXjO19HsqVLhs2hs6kW6htr9ar9c,65035
 kvirt/providers/kubevirt/__init__.py,sha256=bAf3kSFjApkKCZEbOpV2uaWS5B4XJZ95gHONWt1XEM8,80949
 kvirt/providers/kvm/__init__.py,sha256=oafQ7M4bgE6emiZ4yxW6XxNRxbuyYuM3ZqIPmGuXK4w,184146
 kvirt/providers/kvm/helpers.py,sha256=t2CLczaU-gWPXL6iglK2Mlu-85ErH59nkdSA50v18lM,1965
 kvirt/providers/openstack/__init__.py,sha256=X6M0jV3NGD6JQJoLQlNF495l_QpNKI6b75pLGgHOnL4,57063
 kvirt/providers/ovirt/__init__.py,sha256=9znli5vpUeJOcNFqX4FuiQHJKRnm84ccOJ5uDGMbEPo,62531
 kvirt/providers/packet/__init__.py,sha256=QvNdslKLsv5BmPpr7mNUtleUa9L9sDKK7JEJdUfPff8,31099
 kvirt/providers/vsphere/__init__.py,sha256=pEMaRkkDegS77VbMR_Q8I0W4nqdnOMCFmiT1WG3Meio,73086
 kvirt/providers/vsphere/helpers.py,sha256=F1rB_AHISd8TFYQ6eRolQmCVqU8KFAa36CCwjDj-vqw,13655
 kvirt/providers/vsphere/tagging.py,sha256=7RqFIUETSzHAjS0F_8-j145-_8lca7aDUsCxs4DhQVQ,4893
 kvirt/providers/web/__init__.py,sha256=jHLAJAVGJ-1m5530cs6zPCR7Mo8OieiAgC3ZPczpesk,21273
 kvirt/version/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kvirt/version/git,sha256=K6KJ0BpeW6hKg6Wf_qfK3_bbfWe-oOZYJVzQq62b1h0,19
+kvirt/version/git,sha256=vEnKA5RMwzj6JKAudYdRMi5Qm5Q5GSGha6fvqOjWCnY,19
 kvirt/web/__init__.py,sha256=jR0jOtI73-MJQmyVnH4MHuf5UQpdWZe-lCFk1YtXy54,46592
 kvirt/web/main.py,sha256=DIb6tW3ce7wCc83kD9HBCG4ALJuLItp9uaP6tzdsm_Y,261
 kvirt/web/static/css/bootstrap-notify.css,sha256=ibUTW-jDj-F8d1T1KZ4DOujRmVTFfvMKL9y14QgEaPQ,408
 kvirt/web/static/css/bootstrap-theme.min.css,sha256=ZT4HPpdCOt2lvDkXokHuhJfdOKSPFLzeAJik5U_Q-l4,23409
 kvirt/web/static/css/bootstrap.min.css,sha256=E-dwlJxOS7dOrKCvR-5WCqiHCbIHLl59MMDVsfU4oiU,121125
 kvirt/web/static/css/dataTables.checkboxes.css,sha256=H-x4lWeyX3jMsghnkCUUTO2lXjRpJ8pxhUj3YAqaBrQ,399
 kvirt/web/static/css/jquery.dataTables.min.css,sha256=-Z1rYa3ys5OdZNUck5G7lBvb8A13OrYwvf-d8PfEaHQ,13587
@@ -589,13 +584,13 @@
 kvirt/web/templates/repos.html,sha256=HaFCTQjX3zSaqyV05Y_wG0vSkOWDpc-wj6Uj5TLbiFg,475
 kvirt/web/templates/repostable.html,sha256=6HH8sgdppR-yojQspdcI59ju4e9HZYVvV6uvnPxqbeo,1203
 kvirt/web/templates/vmcreate.html,sha256=FG3OoQEKTpeo8spJ1WiqYVkOp672saYRQKujNWOA3uQ,958
 kvirt/web/templates/vmprofiles.html,sha256=T65Cv7povhBtD2dyuWkWJE6byaA9EYtLSk5gtcQlHIU,486
 kvirt/web/templates/vmprofilestable.html,sha256=-8viNOqSvN_yzimENxq7Q0187zbflOn8p8zpgx0Vyek,1420
 kvirt/web/templates/vms.html,sha256=k2ptKeiLFdpzgfbk6xi__sduu0UALYXXrnrmDEmAfaQ,470
 kvirt/web/templates/vmstable.html,sha256=ikuYkIm_ocvGIBXFyJt1-tBjwQWCyqkgC08leoXgR54,4894
-kcli-99.0.202305260939.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-kcli-99.0.202305260939.dist-info/METADATA,sha256=0ZzBfsJ4E3E_1clFN7jrLWcXR2tNb9t1JbecySMZasE,2914
-kcli-99.0.202305260939.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-kcli-99.0.202305260939.dist-info/entry_points.txt,sha256=Rks05_15yZkzTe2QTbrkV_O8uruW_WjUDzmfMApHUvw,209
-kcli-99.0.202305260939.dist-info/top_level.txt,sha256=FwVTxtMIWdr8QBk5mTfd0f_GheFlRR_vn4zl6p5N57s,6
-kcli-99.0.202305260939.dist-info/RECORD,,
+kcli-99.0.202305261953.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+kcli-99.0.202305261953.dist-info/METADATA,sha256=X6BdDfozIh9rwke_gCn-LPYzNzMCiu80LHisfcrd3Ho,2914
+kcli-99.0.202305261953.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+kcli-99.0.202305261953.dist-info/entry_points.txt,sha256=Rks05_15yZkzTe2QTbrkV_O8uruW_WjUDzmfMApHUvw,209
+kcli-99.0.202305261953.dist-info/top_level.txt,sha256=FwVTxtMIWdr8QBk5mTfd0f_GheFlRR_vn4zl6p5N57s,6
+kcli-99.0.202305261953.dist-info/RECORD,,
```

