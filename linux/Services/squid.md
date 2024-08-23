Squid with auth (digest mode) for ubuntu 16.04

apt update && apt -y upgrade

apt install  iptables-persistent

iptables -A INPUT -p tcp -m tcp --dport 3128 -j ACCEPT

#iptables -A INPUT -m tcp -p tcp --dport 22  -j ACCEPT

iptables -P INPUT DROP

netfilter-persistent save

apt install squid

 sudo cp /etc/squid/squid.conf /etc/squid/squid.conf.original

 sudo chmod a-w /etc/squid/squid.conf.original

apt install apache2-utils

cat /etc/squid/squid.conf

    auth_param digest program /usr/lib/squid3/digest_file_auth -c /etc/squid/passwords

    auth_param digest realm proxy

    auth_param digest authenticate_cache_garbage_interval 5 minutes

        #auth_param digest authenticate_cache_garbage_interval 3 hour

    auth_param digest authenticate_ttl 3 hour

        #auth_param digest authenticate_ip_ttl 0 seconds

    auth_param digest authenticate_ip_ttl 3 hour

    auth_param digest children 5

    auth_param digest nonce_max_duration 30 minutes

    auth_param digest nonce_max_count 50

    auth_param digest nonce_strictness on

    auth_param digest check_nonce_count on

    acl authenticated proxy_auth REQUIRED

    http_access allow authenticated

    http_port 3128

new pass file:

htdigest -c /etc/squid/passwords proxy user1

# proxy = realm from /etc/squid/squid.conf

add user:

htdigest /etc/squid/passwords proxy user2