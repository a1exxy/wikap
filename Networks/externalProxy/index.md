# Поднятие локального прокси

### Запуск контейнера
```bash
lxc launch ubuntu:24.04 externalProxy
```

### Установка постоянного ip адреса для контейнера
```bash
sudo lxc config device override externalProxy eth0 ipv4.address=10.2.217.254
```

### Подключение к контейнеру
```bash
lxc exec externalProxy bash
```
### Обновление и установка пакетов
```bash
apt update
apt upgrade
apt install squid wireguard
```

### Настройки прокси
```bash
root@externalProxy:~# cat /etc/squid/squid.conf
http_access allow all
http_port 3128
coredump_dir /var/spool/squid
logfile_rotate 0
```

**Настройки vpn**
```bash
root@externalProxy:~# cat /etc/wireguard/wg0.conf 
[Interface]
PrivateKey = <private_key>
Address = <wg_local_ip>/32
DNS = 8.8.8.8,8.8.4.4

[Peer]
PublicKey = <public_key>
PresharedKey = <preshared_key>
Endpoint = <wg_gateway_ip>:<wg_gateway_port>
AllowedIPs = 0.0.0.0/0
```

### Автозапуск vpn
```bash
systemctl enable --now wg-quick@wg0
```
