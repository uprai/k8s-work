# k8s-work
k8s-work is learning workbench

Pre-requisite

1. Vagran should be installed on host machin
2. Vitrual box should be installed on host machin

Follow the below step to setup kubernetes cluster with one master and 3 worker nodes.


$ vangrant up

This should bring up one Kmaster node and three Kworker nodes. 
docker engine is installed on all nodes. /etc/hosts file is updated


$ vagrant status

To run kubectl command from host machin, you have to copy .kube/config folder.

$ mkdir .kube
$ scp vagrant@kmaster:.kube/config .kube

In case above command prompt for password type 'vagrant' as password


$ Vagrant destroy 
command will remove all the nodes.
