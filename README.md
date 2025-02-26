# Kubernetes The Hard Way


This tutorial walks you through setting up Kubernetes the hard way on a local machine using a hypervisor.
This guide is not for people looking for a fully automated command to bring up a Kubernetes cluster.
If that's you then check out [Google Kubernetes Engine](https://cloud.google.com/kubernetes-engine), or the [Getting Started Guides](http://kubernetes.io/docs/getting-started-guides/).

Kubernetes The Hard Way is optimized for learning, which means taking the long route to ensure you understand each task required to bootstrap a Kubernetes cluster. Note that the cluster when built will not be accessible from your laptop browser - that isn't what this is about. If you want a more useable cluster, try [one of these](https://github.com/kodekloudhub/certified-kubernetes-administrator-course/tree/master/kubeadm-clusters).

## Target Audience

The target audience for this tutorial is someone planning to support a production Kubernetes cluster and wants to understand how everything fits together.

## Cluster Details

Kubernetes The Hard Way guides you through bootstrapping a highly available Kubernetes cluster with end-to-end encryption between components and RBAC authentication.

* [Kubernetes](https://github.com/kubernetes/kubernetes) Latest version
* [Container Runtime](https://github.com/containerd/containerd) Latest version
* [Weave Networking](https://www.weave.works/docs/net/latest/kubernetes/kube-addon/)
* [etcd](https://github.com/coreos/etcd) v3.5.9
* [CoreDNS](https://github.com/coredns/coredns) v1.9.4

### Getting Started

This tutorial requires four (4) ARM64 based virtual or physical machines connected to the same network. While ARM64 based machines are used for the tutorial, the lessons learned can be applied to other platforms.

* [Prerequisites](docs/01-prerequisites.md)
* [Setting up the Cluster](docs/02-compute-resources.md)
* [Client tools](03-client-tools.md)
* [Provisioning CA and Generating TLS certificates](docs/04-certificate-authority.md)
* [Generating Kubernetes COnfiguration Files for Authentication](docs/05-kubernetes-configuration-files.md)
