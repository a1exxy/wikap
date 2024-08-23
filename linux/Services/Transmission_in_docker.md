docker run -tid -v /srv/share/transmission:/mnt -p 9091:9091 --name  transmission  ubuntu

docker exec -ti transmission bash

apt update

apt install iproute2 vim

apt install transmission-daemon

service transmission-daemon stop

vim /etc/transmission-daemon/settings.json 

{

    "blocklist-enabled": 0, 

    "download-dir": "\/var\/lib\/transmission-daemon\/downloads",

    "download-limit": 100, 

    "download-limit-enabled": 0, 

    "encryption": 1, 

    "max-peers-global": 200, 

    "peer-port": 51413, 

    "pex-enabled": 1, 

    "port-forwarding-enabled": 0, 

    "rpc-authentication-required": 1, 

    "rpc-password": "transmission", 

    "rpc-port": 9091, 

    "rpc-username": "transmission", 

    "rpc-whitelist": "127.0.0.1", 

    "upload-limit": 100, 

    "upload-limit-enabled": 0

}

service transmission-daemon start

Open WebGUI:

firefox <ip>:9091