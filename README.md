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

To run kubectl command from host machin, you have to copy .kube/config folder.o go 

$ mkdir .kube
$ scp vagrant@kmaster:.kube/config .kube

In case above command prompt for password type 'vagrant' as password


$ Vagrant destroy 
command will remove all the nodes.

Edit /etc/hosts file and add below entries

172.16.16.100 kmaster.delixus.com kmaster

172.16.16.101 kworker1.delixus.com kworker1

172.16.16.102 kworker2.delixus.com kworker2

172.16.16.103 kworker2.delixus.com kworker3

You are good to go for application installation.


