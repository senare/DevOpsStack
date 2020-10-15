+++
title = "Infra Presentation"
outputs = ["Reveal"]
+++

{{% section %}}

## Infra Structure Resources

* Continuous integration
* Continuous delivery
* Infrastructure as Code
* Automated configuration management
* DevSecOps

---

# about me

I'm Manfred Nilsson

---

I like :

* DevOps
* Cloud Native Apps
* Linux
* Kubernetes

---

# End

[return]({{% relref "/#" %}})

{{% /section %}}

---

{{% section %}}

# Development workflow

---
    
#### We keep the code in a 'source code repository'

[[GIT]]({{% relref "/git" %}})

[[GOGS]]({{% relref "/gogs" %}})

---

#### We create pipelines to build code

[[Tekton]]({{% relref "/tekton" %}})

---

#### We publish binaries from the code

[[Nexus]]({{% relref "/nexus" %}})

[[Tekton]]({{% relref "/tekton" %}})

---

#### We create pipelines to test the code

[[JUnit]]({{% relref "/junit" %}})

[[Tekton]]({{% relref "/tekton" %}})


---

#### We create pipelines to lint the code

[[Sonar Qube]]({{% relref "/sonarqube" %}})

[[Tekton]]({{% relref "/tekton" %}})

---

#### We ensure that we have a known environment to execute the code

[[Docker]]({{% relref "/docker" %}})

---

#### We deploy the code

????

---

{{% /section %}}

---

{{% section %}}

# We can treat infrastructure as code

---

#### Life cycle Infra structure

- We keep the code in a 'source code repository'
- We create pipelines to build code
- We create pipelines to test the code
- We create pipelines to lint the code

---

#### Create infrastructure

i.e storage, network and compute

[[Terraform]]({{% relref "/terraform" %}})

---

#### Configure infrastructure

i.e install packages and configure firewalls

[[Ansible]]({{% relref "/ansible" %}})

---

#### Cluster available resources to reduce overhead

[[Kubernetes]]({{% relref "/kubernetes" %}})


{{% /section %}}

---

{{% section %}}

# Configuration Management

---

{{< slide background-image="/senare/images/cicd_flow.png" >}}

---

- If it isn't really needed by your production environment it isn’t really part of you production environment.

- Separate CI from CD

- KISS, and as few moving parts as possible (in production)

{{% /section %}}

---

{{% section %}}

## Java {#java}

[go to slides]({{% relref "/java" %}})

---

[[JPS]](https://docs.oracle.com/javase/7/docs/technotes/tools/share/jps.html)

[[Base64]](https://docs.oracle.com/javase/8/docs/api/java/util/Base64.html)
[[Understanding Java 9 Modules]](https://www.oracle.com/corporate/features/understanding-java-9-modules.html)
[[A Guide to Java 9 Modularity]](https://www.baeldung.com/java-9-modularity)

---

[[Apache Commons CLI]](http://commons.apache.org/proper/commons-cli/usage.html)

{{% /section %}}

---

{{% section %}}

## Git {#git}

[go to slides]({{% relref "/git" %}})

---

[[GIT svn]](https://git-scm.com/docs/git-svn)

---

[[svn-to-git]](https://ovasquez.github.io/blog/2017/05/29/svn-to-git/)
[[stackoverflow (how-do-i-migrate-an-svn-repository-with-history-to-a-new-git-repository)]](https://stackoverflow.com/questions/79165/how-do-i-migrate-an-svn-repository-with-history-to-a-new-git-repository/3972103#3972103)
[[GIT migrate]](https://git-scm.com/book/en/v2/Git-and-Other-Systems-Migrating-to-Git)
[[cleanly-migrate-your-subversion-repository-to-a-git-repository]](https://web.archive.org/web/20160314221641/https://jonmaddox.com/2008/03/05/cleanly-migrate-your-subversion-repository-to-a-git-repository/)


{{% /section %}}

---

{{% section %}}

## GOGS {#gogs}

[go to slides]({{% relref "/gogs" %}})

---

[![GOGS](/senare/images/gogs.png)](https://gogs.io/)

---

[[CODE]](https://github.com/gogs/gogs)
[[DOCS]](https://gogs.io/docs)

---

[[nginx-gogs-jenkins]](https://techsparx.com/software-development/docker/damp/nginx-gogs-jenkins.html)
[[How to backup, restore and migrate]](https://discuss.gogs.io/t/how-to-backup-restore-and-migrate/991)
[[Setting up Gogs on Docker]](https://vidhyachari.wordpress.com/2017/09/01/setting-up-gogs-on-docker/)

{{% /section %}}

---

## JUnit {#junit}

[go to slides]({{% relref "/junit" %}})

---

{{% section %}}

## NEXUS {#nexus}

[go to slides]({{% relref "/nexus" %}})

---

[[Nexus Helm Chart]](https://hub.helm.sh/charts/sonatype/nexus-repository-manager)

[[Dockerhub Sonatype Nexus IQ Server]](https://hub.docker.com/r/sonatype/nexus-iq-server/)
[[Dockerhub nexus3]](https://hub.docker.com/r/sonatype/nexus3)

[[Cookbook for Nexus Repository Manager]](https://github.com/sonatype/chef-nexus-repository-manager)
[[Getting Started with IQ Server Deployment]](https://help.sonatype.com/iqserver/getting-started)
[[Running The Nexus Platform Behind Nginx Using Docker]](https://blog.sonatype.com/running-the-nexus-platform-behind-nginx-using-docker)

[[Nexus Storage guide]](https://help.sonatype.com/repomanager3/repository-management/storage-guide)
[[Nexus Blob Store]](https://help.sonatype.com/repomanager3/high-availability/configuring-blob-stores)

{{% /section %}}

---

{{% section %}}

## GO {#golang}

[go to slides]({{% relref "/golang" %}})

---

[[GO PATH]](https://golang.org/doc/gopath_code.html)

[[Upgrade golang deps]](https://golang.cafe/blog/upgrade-dependencies-golang.html)

{{% /section %}}

---

## Python {#python}

[go to slides]({{% relref "/python" %}})

---

## Bash {#bash}

[go to slides]({{% relref "/bash" %}})

---

{{% section %}}

## Docker {#docker}

---

[[Encrypted container images for container image security at rest]](https://developer.ibm.com/articles/encrypted-container-images-for-container-image-security-at-rest/)

{{% /section %}}

---

{{% section %}}

## Kubernetes {#kubernetes}

[go to slides]({{% relref "/kubernetes" %}})

---

[[Storage mini direct csi]](https://github.com/minio/direct-csi)

[[Encryption of Kubernetes Persistent Local Volumes]](https://medium.com/@dfrnascimento/encryption-of-kubernetes-persistent-local-volumes-70da62e0ed68)

---

[[OPENEBS]](https://openebs.io/)

[[DOCS OPENEBS]](https://docs.openebs.io/)

[[How to use encryption with OpenEBS Local PV Hostpath volume]](https://github.com/openebs/openebs-docs/blob/day_2_ops/docs/uglocalpv_volume_encrypt.md)

---

## NFSv4.2

[[NFSv4.2]](https://storagetutorial.com/nas/nfsv4-2/)

---

[[Kubernetes NFS: Quick Tutorials]](https://cloud.netapp.com/blog/kubernetes-nfs-two-quick-tutorials-cvo-blg)
[[Provision Kubernetes NFS clients on a Raspberry Pi homelab]](https://opensource.com/article/20/6/kubernetes-nfs-client-provisioning)
[[Kubernetes NFS-Client Provisioner]](https://github.com/kubernetes-retired/external-storage/tree/master/nfs-client)

{{% /section %}}

---

{{% section %}}

## Rook {#rook}

[go to slides]({{% relref "/rook" %}})

---

[![ROOK](/senare/images/rook.svg)](https://github.com/rook/rook)

{{% /section %}}

---

{{% section %}}

## Ceph {#ceph}

[go to slides]({{% relref "/ceph" %}})

---

[![CEPH](/senare/images/ceph.png)](https://ceph.io/)

---

[[Ceph Persistent Storage for Kubernetes with Cephfs]](https://computingforgeeks.com/ceph-persistent-storage-for-kubernetes-with-cephfs/)

{{% /section %}}

---

{{% section %}}

## Terraform {#terraform}

[go to slides]({{% relref "/terraform" %}})

---

[[SOURCE]](https://github.com/hashicorp/terraform)

---

[[Install Third Party Provider]](https://www.hashicorp.com/blog/automatic-installation-of-third-party-providers-with-terraform-0-13)

---

## Terraform & Ansible


[[Terraform-Ansible]](https://github.com/ernesen/Terraform-Ansible/blob/master/artifacts/scripts/install_software.sh)

[[Building Repeatable Infrastructure with Terraform and Ansible on AWS]](https://medium.com/faun/building-repeatable-infrastructure-with-terraform-and-ansible-on-aws-3f082cd398ad)

{{% /section %}}

---

## Terragrunt {#terragrunt}

[go to slides]({{% relref "/terragrunt" %}})

---

{{% section %}}

## Etcd {#etcd}

[go to slides]({{% relref "/etcd" %}})

---

[[Terraform store etcd3]](https://www.terraform.io/docs/backends/types/etcdv3.html)
[[etcd Security model]](https://etcd.io/docs/v3.2.17/op-guide/security/)
[[etcd authentication]](https://etcd.io/docs/v2/authentication/)

[[Dockerhub bitnami etcd]](https://hub.docker.com/r/bitnami/etcd/)

{{% /section %}}

---

## Ansible {#ansible}

[go to slides]({{% relref "/ansible" %}})

[[FreeIpa dynamic inventory for ansible]](https://github.com/freeipa/freeipa-dyndir)

[[Linode getting started with ansible]](https://www.linode.com/docs/applications/configuration-management/ansible/getting-started-with-ansible/)

[[Ansible as IT Automation Glue]](https://www.ansible.com/blog/ansible-it-automation-glue)

[[Ansible Lab environment using Docker]](https://morioh.com/p/fa458766759f)

[[Howto Writing an Ansible module for a REST API]](https://liquidat.wordpress.com/2016/06/27/howto-writing-an-ansible-module-for-a-rest-api/)

[[How to Install Ansible on Ubuntu 20.04 LTS]](https://linuxhint.com/install_ansible_ubuntu/)

---

{{% section %}}

## Molecule {#molecule}

[go to slides]({{% relref "/molecule" %}})

---

[[Molecule]](https://molecule.readthedocs.io/en/latest/)

{{% /section %}}

---

## Grafana {#grafana}

[go to slides]({{% relref "/grafana" %}})

---

## Prometheus {#prometheus}

[go to slides]({{% relref "/prometheus" %}})

---

## Elasticsearch {#elasticsearch}

[go to slides]({{% relref "/elasticsearch" %}})

---

## Kibana {#kibana}

[go to slides]({{% relref "/kibana" %}})

---

## Sonarqube {#sonarqube}

[go to slides]({{% relref "/sonarqube" %}})

---

{{% section %}}

## MicroK8s {#microk8s}

[go to slides]({{% relref "/microk8s" %}})

---

[[microk8s]](https://microk8s.io/)

---

[[How to setup MicroK8s with RBAC and Storage]](https://igy.cx/posts/setup-microk8s-rbac-storage/)

{{% /section %}}

---

## Istio {#istio}

[go to slides]({{% relref "/istio" %}})

---

{{% section %}}

## Argo CD {#argo}

[go to slides]({{% relref "/argo" %}})

---

[![Argo CD](/senare/images/argo.png)](https://argoproj.github.io/argo-cd/)

{{% /section %}}

---

## Tekton {#tekton}

[go to slides]({{% relref "/tekton" %}})

---

{{% section %}}

## Kubevirt {#kubevirt}

[go to slides]({{% relref "/kubevirt" %}})

---

[[Yes, you can run VMs on Kubernetes with KubeVirt]](https://opensource.com/article/20/9/vms-kubernetes-kubevirt)

{{% /section %}}

---

## KVM {#kvm}

[go to slides]({{% relref "/kvm" %}})

---

## LUKS {#luks}

[go to slides]({{% relref "/luks" %}})

---

## Structure101 {#structure101}

[go to slides]({{% relref "/structure101" %}})

---

{{% section %}}

## Bastion Jump Host {#bastion}

[go to slides]({{% relref "/bastion" %}})

---

[[ansible jumphost]](https://blog.keyboardinterrupt.com/ansible-jumphost/)

{{% /section %}}

---

{{% section %}}

## Ubuntu {#ubuntu}

---

[[UFW Ubuntu 20.04]](https://www.ubuntu18.com/how-to-enable-ubuntu-firewall-in-ubuntu-20-04/)

[[UFW]](https://linuxconfig.org/how-to-install-ufw-and-use-it-to-set-up-a-basic-firewall)

[[Add Users Ubuntu 20.04]](https://linuxconfig.org/how-to-add-user-on-ubuntu-20-04-focal-fossa-linux)

{{% /section %}}

---


{{% section %}}

## CentOS {#centos}

---

[![CentOS](/senare/images/centos.png)](https://www.centos.org/)

---

[[DOCS]](https://wiki.centos.org/)

[[DNF]](https://www.howtoforge.com/centos-8-package-management-with-dnf-on-the-command-line/)

[[FIREWALLD]](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html/security_guide/sec-viewing_current_status_and_settings_of_firewalld)

{{% /section %}}

---

{{% section %}}

## FreeIPA {#freeipa}

[go to slides]({{% relref "/freeipa" %}})

---

[![FreeIPA](/senare/images/freeipa.png)](https://www.freeipa.org/)

---

[[DOCS]](https://freeipa.readthedocs.io/en/latest/index.html)

[[CODE]](https://github.com/freeipa/freeipa)

---

## FreeIpa lab

[[LINK]](https://posts.specterops.io/building-a-freeipa-lab-17f3f52cd8d9)

---

## Complex Application in Container

[[LINK]](https://www.adelton.com/docs/docker/complex-application-in-container)
[[Build an OpenLDAP Docker Image That’s Populated With Users]](https://medium.com/better-programming/ldap-docker-image-with-populated-users-3a5b4d090aa4)

---

## CentOS 8 install

[[LINK]](https://www.howtoforge.com/tutorial/install-and-configure-freeipa-server-on-centos-8/)


{{% /section %}}

---

{{% section %}}

## 389 Directory Service {#389}

---

[![389](/senare/images/389.png)](https://directory.fedoraproject.org/)

---

[[fossies]](https://fossies.org/linux/389-ds-base/docker/README.md)

[[BLOG]](https://fy.blackhats.net.au/blog/html/2019/07/05/using_389ds_with_docker.html)

{{% /section %}}

---

{{% section %}}

## SSSD {#sssd}

[go to slides]({{% relref "/sssd" %}})

---

[[DOC]](https://sssd.io/)

[[CODE]](https://github.com/SSSD/sssd)

{{% /section %}}

---

{{% section %}}

## Markdown {#markdown}

[go to slides]({{% relref "/markdown" %}})

---

[![Markdown](/senare/images/markdown.svg)](https://www.markdownguide.org/)

{{% /section %}}|

---

{{% section %}}

## Hugo {#hugo}

[go to slides]({{% relref "/hugo" %}})

---

[![Hugo](/senare/images/hugo.svg)](https://gohugo.io/)

{{% /section %}}

---

{{% section %}}

## Github Pages {#github}

[go to slides]({{% relref "/github" %}})

---

[![Github Pages](/senare/images/githubpages.svg)](https://pages.github.com/)

---

[[Github Actions Hugo]](https://github.com/peaceiris/actions-hugo)

{{% /section %}}

---

{{% section %}}

## Reveal Hugo {#reveal}

[go to slides]({{% relref "/reveal" %}})

---

[![Reveal Hugo](/senare/images/reveal-hugo.png)](https://themes.gohugo.io/reveal-hugo/)

---

[![Reveal JS](/senare/images/revealjs.svg)](https://revealjs.com/)

{{% /section %}}

---

{{% section %}}

## DeckTape {#decktape}

[go to slides]({{% relref "/decktape" %}})

---

[[DeckTape]](https://github.com/astefanutti/decktape)

{{% /section %}}

---

{{% section %}}

## Let's Encrypt {#letsencrypt}

[go to slides]({{% relref "/letsencrypt" %}})

---

[![Let's Encrypt](/senare/images/letsencrypt.svg)](https://letsencrypt.org/)

{{% /section %}}

---

{{% section %}}

## Cert Bot {#certbot}

[go to slides]({{% relref "/certbot" %}})

---

[![Cert Bot](/senare/images/certbot.svg)](https://certbot.eff.org/)

---

[[FAQ]](https://github.com/ppKrauss/certbot-faq/blob/master/README.md)

{{% /section %}}

---

{{% section %}}

## NGINX {#nginx}

[go to slides]({{% relref "/nginx" %}})

---

[![NGINX](/senare/images/NGINX.svg)](https://www.nginx.com/)

---

[[NGINX Reverse Proxy]](https://docs.nginx.com/nginx/admin-guide/web-server/reverse-proxy/)
[[Nginx 1.19 supports environment variables and templates in Docker]](https://marcofranssen.nl/nginx-1-19-supports-environment-variables-and-templates-in-docker/)

[[Nginx and Letsencrypt with certbot in docker alpine]](https://geko.cloud/nginx-and-ssl-with-certbot-in-docker-alpine/)

[[Nginx and Let’s Encrypt with Docker in Less Than 5 Minutes]](https://medium.com/@pentacent/nginx-and-lets-encrypt-with-docker-in-less-than-5-minutes-b4b8a60d3a71)

---

[[Dockerhub nginx]](https://hub.docker.com/_/nginx)
[[Dockerhub bitnami nginx]](https://hub.docker.com/r/bitnami/nginx)

{{% /section %}}

---

{{% section %}}

## SNORT {#snort}

[go to slides]({{% relref "/snort" %}})

---

[![NGINX](/senare/images/snort.png)](https://www.snort.org/)

{{% /section %}}

---

{{% section %}}

## Clair {#clair}

[go to slides]({{% relref "/clair" %}})

---

[![NGINX](/senare/images/clair.png)](https://github.com/quay/clair)

{{% /section %}}

---

{{% section %}}

## osquery {#osquery}

[go to slides]({{% relref "/osquery" %}})

---

[![NGINX](/senare/images/osquery.png)](https://github.com/osquery/osquery)

{{% /section %}}

---

{{% section %}}

## idea {#idea}

[go to slides]({{% relref "/idea" %}})

---

[[IDEA]](https://www.jetbrains.com/idea/)

[[CLI]](https://emmanuelbernard.com/blog/2017/02/27/start-intellij-idea-command-line/)

{{% /section %}}

---

{{% section %}}

## SSH {#ssh}

[go to slides]({{% relref "/ssh" %}})

---

OpenSSH

---

## IPv6

[[Holding IPv6 Neighbor Discovery to a Higher Standard of Security]](https://blogs.infoblox.com/ipv6-coe/holding-ipv6-neighbor-discovery-to-a-higher-standard-of-security/)
[[IPv6 SSH]](https://techhub.hpe.com/eginfolib/networking/docs/switches/WB/15-18/5998-8170_wb_2920_ipv6_config_guide/content/v33585271.html)

---

## Break the glass ...

[[Smallstep cert based]](https://smallstep.com/blog/ssh-emergency-access/)

---

[[Tunneling SSH]](https://www.ssh.com/ssh/tunneling/example)

[[Cyberciti Tunneling SSH]](https://www.cyberciti.biz/faq/ssh-port-forwarding-tunneling/)

---

[[Mozilla guidlines]](https://infosec.mozilla.org/guidelines/openssh)

---

[[Smallstep use cert for ssh]](https://smallstep.com/blog/use-ssh-certificates/)

[[Smallstep DIY bastion]](https://smallstep.com/blog/diy-ssh-bastion-host/)

[[Linux as a bastion]](https://www.cyberciti.biz/faq/linux-bastion-host/)

[[Linux Audit Blogg]](https://linux-audit.com/linux-security-guide-extended-version/)

---

{{< slide background-image="/senare/images/ssh-certificate-authentication.png" >}}

---

{{< slide background-image="/senare/images/ssh-deploy-rgm.png" >}}


{{% /section %}}

---

{{% section %}}

## Linux Server Hardening

---

[[Linux Kernel Security]](https://www.cyberciti.biz/tips/selinux-vs-apparmor-vs-grsecurity.html)

[[40 tips]](https://www.cyberciti.biz/tips/linux-security.html)

[[Digitalocean guide]](https://www.digitalocean.com/community/tutorials/recommended-security-measures-to-protect-your-servers)

---

## AIDE

[[SOURCE]](https://github.com/aide/aide)

[[Ubuntu Install]](https://www.cyberciti.biz/faq/debian-ubuntu-linux-software-integrity-checking-with-aide/)

---

## HIDS

[[WIKI HIDS]](https://en.wikipedia.org/wiki/Host-based_intrusion_detection_system_comparison)

---

[[fail2ban]](http://www.fail2ban.org/wiki/index.php/Main_Page)

---

[[PortKnocking]](https://help.ubuntu.com/community/PortKnocking)

{{% /section %}}

---

{{% section %}}

## Glesys

---

[[Glesys GO API]](https://github.com/glesys/API)

[[Glesys golang client]](https://github.com/glesys/glesys-go)

[[Glesys TERRAFORM provider]](https://github.com/norrland/terraform-provider-glesys)

[[One Click Installers]](https://github.com/glesys/one-click-installers)

[[GleSYS Kubernetes cloud controller]](https://hub.docker.com/r/glesys/glesys-cloud-controller-manager)

[[Cloud Config KVM]](https://github.com/glesys/API/wiki/Using-cloud-config-to-configure-you-KVM-server)

[[Glesys fail2ban]](https://glesys.se/kb/artikel/skydda-ssh-med-fail2ban-i-linux)

[[GleSYS API/Ansible Demo]](https://github.com/glesys/ansible-wp-auto-deploy)

{{% /section %}}

---

{{% section %}}

## Cloud Config

---

[[KVM: Testing cloud-init locally using KVM for an Ubuntu cloud image]](https://fabianlee.org/2020/02/23/kvm-testing-cloud-init-locally-using-kvm-for-an-ubuntu-cloud-image/)


{{% /section %}}

---

{{% section %}}

## DUF

---

[[DUF]](https://ostechnix.com/how-to-view-disk-usage-with-duf-on-linux-and-unix/)
[[CODE]](https://github.com/muesli/duf)

{{% /section %}}

---

{{% section %}}

## OS X KVM

---

[[CODE OS X KVM]](https://github.com/kholia/OSX-KVM)
[[CODE OS X DOCKER]](https://github.com/Cleafy/sxkdvm)
[[OS X Vagrant]](https://app.vagrantup.com/AndrewDryga/boxes/vagrant-box-osx)
[[macos Vagrant]](https://app.vagrantup.com/ramsey/boxes/macos-catalina)

---

[[Using Vagrant to set up a VM with KVM/qemu without VirtualBox]](https://stackoverflow.com/questions/42155213/using-vagrant-to-set-up-a-vm-with-kvm-qemu-without-virtualbox)

{{% /section %}}

---

{{% section %}}

## Backup & LVM

---

[[bacula]](https://www.bacula.org/documentation/documentation/)
[[Introduction to Bacula, How to install, configure, backup and restore]](https://www.labeightyfour.com/2019/04/08/introduction-to-bacula-how-to-install-configure-backup-and-restore/)
[[Back Up (And Restore) LVM Partitions With LVM Snapshots]](https://www.howtoforge.com/linux_lvm_snapshots)
[[Taking a Backup Using Snapshots]](https://tldp.org/HOWTO/LVM-HOWTO/snapshots_backup.html)
[[LVM snapshots as a backup strategy]](https://serverfault.com/questions/23965/lvm-snapshots-as-a-backup-strategy)
[[Backup and Restore Logical Volume using LVM Snapshot]](http://www.tuxfixer.com/backup-and-restore-logical-volume-using-lvm-snapshot/)

[[Managing LVM Snapshots in LVM2]](https://www.theurbanpenguin.com/maning-lvm-snapshots/)

---
[[Docker Volumes]](https://docs.docker.com/storage/volumes/)
[[Docker StorageDriver]](https://docs.docker.com/storage/storagedriver/device-mapper-driver/)

[[docker lvm plugin]](https://github.com/containers/docker-lvm-plugin)
[[Working with Docker LVM Plugin]](https://www.projectatomic.io/blog/2016/05/docker-lvm-plugin/)


---

[[Docker Data Volume Snapshots and Encryption with LVM and LUKS]](https://medium.com/@kalahari/docker-data-volume-snapshots-and-encryption-with-lvm-and-luks-ce80e0555225)

[[LUKS and loop device]](https://askubuntu.com/questions/599044/luks-and-loop-device)
[[Ubuntu ManualFullSystemEncryption/BasicsLVM]](https://help.ubuntu.com/community/ManualFullSystemEncryption/BasicsLVM)
[[LVM on loopback devices]](https://ops.tips/blog/lvm-on-loopback-devices/)

[[Encrypting Docker containers on a Virtual Server]](https://launchbylunch.com/posts/2014/Jan/13/encrypting-docker-on-digitalocean/)


{{% /section %}}

---

{{% section %}}

## Zero Trust

---

{{< youtube -Why_ZjJUhg >}}

---

{{< youtube tFrbt9s4Fns >}}

---

{{< youtube vWdk3zmeS1M >}}

---

{{< youtube 6q6c0Ld0qx0 >}}

---

{{< youtube EF_0dr8WkX8 >}}

---

{{< youtube X6tUptvmi1w >}}

---

{{< youtube UJubIpMm62U >}}

{{% /section %}}

---

# End

[return]({{% relref "/#" %}})
