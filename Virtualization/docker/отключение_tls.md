Отключение tls:

cat /etc/docker/daemon.json
```json
{
"insecure-registries": ["10.0.2.2:8181"],


"registry-mirrors": ["http://10.0.2.2:8181"]
}
```