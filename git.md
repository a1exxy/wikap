Подключение репо:

cat /etc/docker/daemon.json
{
       "registry-mirrors": ["https://repo.maya:1112/repository/docker/"]
}

Проверка docker info

Отключение tls:

cat /etc/docker/daemon.json
{
        "insecure-registries": ["10.0.2.2:8181"],
           "registry-mirrors": ["http://10.0.2.2:8181"]
}

--------------------------------------------------------------------

Поиск интерфейса контейнера

root@c3edc77fd4fc:/# cat /sys/class/net/eth0/iflink
45

# ip a | grep 45
45: veth3c17edb@if44: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu


docker inspect p12_test_nginx | grep -i pid
"Pid": 185925,

nsenter -t 185925 -n ifconfig
eth0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
       inet 172.18.0.7  netmask 255.255.0.0  broadcast 172.18.255.255

nsenter -t 185925 -n tcpdump -nni eth0


