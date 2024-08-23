81  yum install -y mc nano vim wget open-ssh openssh-clients man bind-utils bzip2 unzip zip ntp sysstat bash-completion vnstat net-tools lsof tcpdump

   82  yum install -y epel-release

   83  vim /etc/selinux/config

   84  yum remove firewalld

   85  yum  install -y kvm libvirt python-virtinst qemu-kvm bridge-utils virt-install

   86  cd /etc/libvirt/

   87  mkdir hooks

   88  cat > /etc/libvirt/hooks/qemu

   89  chmod +x /etc/libvirt/hooks/qemu

   90  ll /etc/libvirt/hooks/qemu

   91  cat /etc/libvirt/hooks/qemu

   92  reboot 

   93  wget ftp://pelican/soft/VIRTUAL_ROUTERS/vrr-bundle-kvm-16.2R2.8.tgz

   94  mc

   95  cd /var/lib/libvirt/images/

   97  virt-install --name clk71rr --ram 16384 --import --disk=/var/lib/libvirt/images/junos-x86-64-16.2R2.8.img  --import --disk=/var/lib/libvirt/images/metadata.img