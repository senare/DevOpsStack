+++
title = "Kubernetes"
outputs = ["Reveal"]
+++

# Kubernetes

---

{{< slide background-color="#000000" >}}

[![K8S](/senare/images/k8s.svg)](https://kubernetes.io/)

---

{{< slide background-color="#000000" >}}

{{< youtube PH-2FfFD2PU >}}

---

# Why should I use Kubernetes

# %

---

Kubernetes is ridiculous hard to deploy and manage (i.e day 2 operations)...

… Docker Swarm is equally ridiculous easy to get started with.

---

Kubernetes master isn’t particularly scalable, architecture supports only primary/standby and practical limit today is around 5k nodes …

… Mesos (DC/OS ?) is hot/hot and clusters supporting 80k+ nodes have been found in the wild.

---

K8s is 2nd to linux kernel

When we look at the hype K8s have already reached “plateau of productivity’’

---

{{< slide background-image="/senare/images/hypecycle.png" >}}

---

{{% section %}}

# Is it really that complicated

---

{{< slide background-image="/senare/images/k8s/inner.png" >}}

{{% /section %}}

---

{{% section %}}

{{< slide background-image="/senare/images/k8s/zoo.png" >}}

---

{{< slide background-image="/senare/images/k8s/pods.png" >}}

---

{{< slide background-image="/senare/images/k8s/deployments.png" >}}

---

{{< slide background-image="/senare/images/k8s/secrets.png" >}}

---

{{< slide background-image="/senare/images/k8s/daemonsets.png" >}}

---

{{< slide background-image="/senare/images/k8s/replicasets.png" >}}

---

{{< slide background-image="/senare/images/k8s/ingress.png" >}}

---

{{< slide background-image="/senare/images/k8s/cronjobs.png" >}}

---

{{< slide background-image="/senare/images/k8s/crd.png" >}}

{{% /section %}}

---

{{% section %}}

# Containers VS Virtual Machines

# YES

---

{{< slide background-image="/senare/images/virt/seperate.png" >}}

---

{{< slide background-image="/senare/images/virt/combined.png" >}}

{{% /section %}}

---

{{% section %}}

[![CNCF](/senare/images/cncf.png)](https://www.cncf.io/)

---

[![CNCF Landscape](/senare/images/cloudnativelandscape.svg)](https://landscape.cncf.io/)

---

{{< slide background-image="/senare/images/cncf_landcape.png" >}}

{{% /section %}}

---

{{% section %}}

# Batteries not included

---

{{< slide background-image="/senare/images/virt/openstack.png" >}}

---

{{< slide background-image="/senare/images/virt/openstackandk8s.png" >}}

{{% /section %}}

---

# End

[return]({{% relref "/#" %}})
