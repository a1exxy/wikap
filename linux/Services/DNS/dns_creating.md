CO6:

добавить в /etc/security/limits.conf

* soft nofile 65535

* hard nofile 65535

добавить в /etc/sysctl.conf

fs.file-max = 100000

net.netfilter.nf_conntrack_max=1048576

vm.swappiness = 0 