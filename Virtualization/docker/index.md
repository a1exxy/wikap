Запуск контейнера в фоне:

    docker run -d -ti -p 2222:22 -m 256m --restart unless-stopped  --name ub1 ubuntu /bin/bash

        -d = фон

        -t = tty

        -i = interactive

        -p = мапинг портов 2222 хостовой машины в 22 контенера

        -m = максимальный размер памяти

   --restart = старт при перезагрузке (no, on-failure[:max-retry], always, unless-stopped)

        --name = имя контейнера

        ubuntu = имя образа.

        /bin/bash = запущенная команда

Подключение к запущенному контейнеру:

    docker attach --detach-keys="ctrl-q" contener_name

Коммит образа с новым названием

    docker commit serene_bohr git2

Создание сети:

    docker network create --driver=bridge  --subnet=172.19.0.0/24 net        

Подключение сети к контейнеру:

    docker network connect net1 condescending_galileo

Запуск контейнера с сетью:

    docker run -tid -p 2222:22 --net net1 --ip=172.19.0.100    --restart unless-stopped   --name sqi squid /bin/bash

Подключенин стандартной сети:

    docker network connect bridge sqi

docker commit nginx username/nginx

docker login

docker push username/nginx

 pwd

/etc/systemd/system/docker.service.d

-rw-r--r--  1 root root  121 Feb 17 12:05 http-proxy.conf

cat http-proxy.conf 

[Service]

Environment="HTTP_PROXY=http://10.77.128.254:3128/" "NO_PROXY=localhost,127.0.0.1,docker-registry.as0485.net"

///////////////////////////HTTPS////////////////////

pwd

/etc/systemd/system/docker.service.d

-rw-r--r--  1 root root  121 Jul 19 08:31 https-proxy.conf

cat https-proxy.conf 

[Service]

Environment="HTTPS_PROXY=http://10.77.127.254:3128/" "NO_PROXY=localhost,127.0.0.1,docker-registry.as0485.net"

Удаление пустых образов:

for i in $(docker images | grep "<none>" | awk '{print $3}'); do docker rmi $i; done

Локальный репо:

docker run -d -p 5000:5000 --restart=always --name registry registry:2

You can now use it with docker.

Get any image from the hub and tag it to point to your registry:

docker pull ubuntu && docker tag ubuntu localhost:5000/ubuntu

… then push it to your registry:

docker push localhost:5000/ubuntu

… then pull it back from your registry:

docker pull localhost:5000/ubuntu

To stop your registry, you would:

docker stop registry && docker rm -v registry

View images:

curl http://localhost:5000/v2/_catalog