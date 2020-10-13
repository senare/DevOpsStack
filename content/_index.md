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

## Java {#java}

[go to slides]({{% relref "/java" %}})

---

## Git {#git}

[go to slides]({{% relref "/git" %}})

---

{{% section %}}

## GOGS {#gogs}

[go to slides]({{% relref "/gogs" %}})

---

[![GOGS](/senare/images/gogs.png)](https://gogs.io/)

{{% /section %}}

---

## JUnit {#junit}

[go to slides]({{% relref "/junit" %}})

---

## NEXUS {#nexus}

[go to slides]({{% relref "/nexus" %}})

---

## GO {#golang}

[go to slides]({{% relref "/golang" %}})

---

## Python {#python}

[go to slides]({{% relref "/python" %}})

---

## Bash {#bash}

[go to slides]({{% relref "/bash" %}})

---

## Kubernetes {#kubernetes}

[go to slides]({{% relref "/kubernetes" %}})

---

{{% section %}}

## Rook {#rook}

[go to slides]({{% relref "/rook" %}})

---

[![GOGS](/senare/images/rook.svg)](https://github.com/rook/rook)

{{% /section %}}

---

{{% section %}}

## Ceph {#ceph}

[go to slides]({{% relref "/ceph" %}})

---

[![GOGS](/senare/images/ceph.png)](https://ceph.io/)

{{% /section %}}

---

## Terraform {#terraform}

[go to slides]({{% relref "/terraform" %}})

---

## Terragrunt {#terragrunt}

[go to slides]({{% relref "/terragrunt" %}})

---

## Etcd {#etcd}

[go to slides]({{% relref "/etcd" %}})

---

## Ansible {#ansible}

[go to slides]({{% relref "/ansible" %}})

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

## MicroK8s {#microk8s}

[go to slides]({{% relref "/microk8s" %}})

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

## Kubevirt {#kubevirt}

[go to slides]({{% relref "/kubevirt" %}})

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

## Bastion Jump Host {#bastion}

[go to slides]({{% relref "/bastion" %}})

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

{{% /section %}}

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

https://smallstep.com/blog/use-ssh-certificates/#:~:text=Most%20SSH%20deployments%20use%20public,each%20user%20%26%20host%20to%20authenticate.&text=Certificate%20authentication%20works%20the%20same,get%20to%20in%20a%20moment.

---

{{< slide background-image="/senare/images/ssh-certificate-authentication.png" >}}

---

{{< slide background-image="/senare/images/ssh-deploy-rgm.png" >}}


{{% /section %}}

---

# End

[return]({{% relref "/#" %}})

