sudo apt-get install nginx fcgiwrap curl

#--------------------------------------------------

cat /etc/nginx/sites-enabled/default

server {

    listen 80 default_server;

    listen [::]:80 default_server ipv6only=on;

    charset utf-8;

    root /home/ubuntu/www;

    index index.html index.htm;

    server_name localhost;

    location / {

        try_files $uri $uri/ =404;

    }

    location /cgi-bin/ {

        fastcgi_pass unix:/var/run/fcgiwrap.socket;

        include /etc/nginx/fastcgi_params;

        fastcgi_param SCRIPT_FILENAME /home/ubuntu/www$fastcgi_script_name;

    }

}

#--------------------------------------------------

mkdir /home/ubuntu/www

#--------------------------------------------------

cat /home/ubuntu/www/cgi-bin/test.py

#!/usr/bin/env python3

import sys

import codecs

sys.stdout = codecs.getwriter("utf-8")(sys.stdout.detach())

print ("Content-type: text/html\n")

print("hi")

#--------------------------------------------------

chmod 755 /home/ubuntu/www/cgi-bin/test.py

sudo service nginx restart

sudo service fcgiwrap restart

curl localhost/cgi-bin/test.py