# k8s-work
k8s-work is learning workbench

$ vangrant up

# This should bring up one Kmaster and three Kworker nodes


$ vagrant status

#To run kubectl command from host machin, you have to copy .kube/config folder.

mkdir .kube
scp vagrant@kmaster:.kube/config .kube

#In case it prompt for password type 'vagrant' as password
