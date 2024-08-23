Ubuntu 20.04:

 _________________________

|                       notebook                          |

|_________________________|

           |                                            |

        eth0                                      wg0

(192.168.1.2)                          10.0.0.2

           |                                            |

 192.168.1.1                                    |

  <_NAT_>                                    |

     2.2.2.2                                        |tunnel

           |                                             |

  <Internet>                                   |

           |                                             |

      3.3.3.3                                10.0.0.1

        eth0                                      wg0

 ____|_________________|___

|                    Wireguard                           |

|_________________________|

                              |

                           eth1

                      172.16.0.1

                              |

                    172.16.0.21

              <Remote_server>

apt install wireguard

wg genkey | tee /etc/wireguard/client1_privatekey | wg pubkey \

| tee /etc/wireguard/client1_publickey

wg genkey | tee /etc/wireguard/server_privatekey | wg pubkey | \

tee /etc/wireguard/server_publickey

Конфиг сервера:

:/etc/wireguard# cat wg0.conf

# Секция настройки сервера: [Interface] PrivateKey = RRR9VSS1wODfiPwHzmTewRzcC7stcXXXq0BfuPKTXXX= # подставьте сюда приватный ключ сервера (cat server_private_key) Address = 10.0.0.1/24 # Внутренний ip адрес нашего сервера ListenPort = 51194 # Порт на котором наш сервер будет принимать подключения # Добавим правила маскарадинга, чтобы весь трафик проходил через наш сервер # ens3 необходимо заменить на ваш сетевой интерфейс (ip route | grep default) PostUp = iptables -A FORWARD -i %i -j ACCEPT; iptables -t nat -A POSTROUTING -o ens3 -j MASQUERADE PostDown = iptables -D FORWARD -i %i -j ACCEPT; iptables -t nat -D POSTROUTING -o ens3 -j MASQUERADE # Секция настройки клиента # Client1 [Peer] PublicKey = vXXXXS+bW2Az8Eq1Y+pKlVw/3zsevfXXXX4xnkEtXXX= # Подставьте сюда публичный ключ клиента (cat client1_public_key) AllowedIPs = 10.0.0.2/32 # внутренний ip адрес клиента (client1)

Поднятие сервиса:

systemctl start wg-quick@wg0

systemctl enable wg-quick@wg0

---------------------------------------------------------------------------------

Конфиг клиента:

:/etc/wireguard# cat wg0.conf 

# Секция настройки клиента client1

[Interface]

PrivateKey = XXXXNxSmrT8njX7aXXXrH845rXXXQvdIZeoxnXXXXmA= # Скопировать значение с нашего сервера (на сервере: sudo cat /etc/wireguard/client1_private_key)

Address = 10.0.0.2/24 # ip адрес клиента client1

#DNS = 8.8.8.8

# Секция настройки подключения к серверу

[Peer]

PublicKey = XXXXXXbovuDMk7ix8svQSesljJSNYEcXXXTJrx8xXXX= # Скопировать значение с нашего сервера (на сервере: sudo cat /etc/wireguard/server_public_key)

AllowedIPs = 10.0.0.0/24, 172.16.0.0/24 # разрешаем клиенту доступ в сеть

Endpoint = 21.5.23.180:51194 # Публичный IP адрес вашего сервера

PersistentKeepalive = 15

Поднятие:

wg-quick up wg0