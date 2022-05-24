# k8s-notes

give permission to execute the script chmod u+x docker-installation.sh
run this docker-installation.sh script to install docker and kubeadm.


error --The connection to the server x.x.x.:6443 was refused - did you specify the right host or port? Kubernetes

solution-

$ sudo systemctl stop kubelet
$ sudo systemctl start kubelet
$ strace -eopenat kubectl version
