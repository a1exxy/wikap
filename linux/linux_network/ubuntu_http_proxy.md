Файл /etc/environment https_proxy="https://user:pass@proxy:port/"  http_proxy="http://user:pass@proxy:port/" ftp_proxy="ftp://user:pass@proxy:port/" socks_proxy="socks://user:pass@proxy:port/"

cat /etc/apt/apt.conf Acquire::http::Proxy "http://10.77.128.254:3128/";