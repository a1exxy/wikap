Установка:

sudo apt install openjdk-8-jre

java -version

#  Разработчики рекомендуют использовать Java 8 версии 1.8.0_131 или выше

wget -qO - https://artifacts.elastic.co/GPG-KEY-elasticsearch | sudo apt-key add -

sudo apt-get install apt-transport-https

echo "deb https://artifacts.elastic.co/packages/6.x/apt stable main" | sudo tee -a /etc/apt/sources.list.d/elastic-6.x.list

sudo apt-get update && sudo apt-get install elasticsearch

файл /etc/elasticsearch/jvm.options

 измените значение опций -Xms и -Xmx на то количество памяти, которое вы хотите, чтобы программа использовала. Например:

    -Xms512m

    -Xmx512m

sudo systemctl start elasticsearch

sudo systemctl enable elasticsearch

Проверка:

curl -XGET http://localhost:9200