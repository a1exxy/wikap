echo 'http_proxy="http://10.77.128.254:3128/"' >> /etc/environment

echo 'https_proxy="https://10.77.128.254:3128/"' >> /etc/environment

echo 'ftp_proxy="ftp://10.77.128.254:3128/"' >> /etc/environment

echo 'no_proxy=".tk.net,.as0485.net"' >> /etc/environment

export http_proxy="http://proxysrv:8080/"

export https_proxy="https://proxysrv:8080/"

export ftp_proxy="ftp://proxysrv:8080/"

export no_proxy=".mylan.local,.domain1.com,host1,host2"

 

echo 'proxy=http://proxysrv:8080/' >> /etc/yum.conf