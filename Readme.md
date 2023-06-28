A set of Ansible scripts to setup a k8s cluster on Debian 12

Uses k3s for the k8s solution

99 percent of this work comes from https://github.com/onedr0p/flux-cluster-template

Will leave a k3s cluster with cilium installed and coredns, nothing else.

LoadBalancing is removed as I use HAProxy on PFsense to achieve this.

Steps:

task precommit:init

task precommit:update

task ansible:prepare

task ansible:install

find the kubeconfig file in the root folder and you have a cluster.