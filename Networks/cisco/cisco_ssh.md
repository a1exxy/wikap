# Ошибка при подключении по ssh: diffie-hellman-group1-sha1
После обновлении системы на ubuntu 16.04 при подключении по ssh к оборудованию стала появляться ошибка:

Unable to negotiate with 10.10.1.2: no matching key exchange method found. Their offer: diffie-hellman-group1-sha1

Решение:

информацию взял с сайта http://www.openssh.com/legacy.html

В домашней папке /home/user/.ssh

создал файл config

содержание данного файла:

cat /home/user/.ssh/config  
Host myhost   KexAlgorithms +diffie-hellman-group1-sha1  
Host 10.10.1.2   KexAlgorithms +diffie-hellman-group1-sha1

Где myhost — это hostname или ip моего оборудования

ssh -oKexAlgorithms=+diffie-hellman-group1-sha1 user@legacyhost