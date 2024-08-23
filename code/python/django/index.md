Установка: sudo apt install postgresql postgresql-contrib  docker run --name some-postgres -e POSTGRES_PASSWORD=mysecretpassword -d postgresПодключение к БД: psql -h 172.17.0.2 -U postgres -d postgres -W

add to ./project/settings.py

DATABASES = {

   'default': {

       'ENGINE': 'django.db.backends.postgresql',

       'NAME': 'postgres',

       'USER': 'postgres',

       'PASSWORD': 'mysecretpassword',

       'HOST': '172.17.0.2',

       'PORT': '5432',

   }

}

postgres:

 \l \list - просмотр списка баз

\c <database> - подключение к БД

\d \dt - просмотр таблиц

\conninfo - просмотр подключений

Создание базы:

CREATE DATABASE имя_базы OWNER имя_роли;

createdb -O имя_роли имя_базы

Дамп с командой создания БД:

pg_dump -h localhost -p 5432 -U someuser -C -F p -b -v -f mydb.backup mydb

Создание бекапа базы mydb, в сжатом виде:

pg_dump -h localhost -p 5440 -U someuser -F c -b -v -f mydb.backup mydb

Удаление таблиц:

DROP TABLE [ IF EXISTS ] имя [, ...] [ CASCADE | RESTRICT ]

Удаление базы:

DROP DATABASE имя;

Бекап: 

pg_dump -h 172.17.0.2 -U postgres -d postgres -W > dump2.sql

psql -h 172.17.0.2 -U postgres -d postgres -W -f dump2.sql