Просмотр пути файла конфигурации

psql -U user -d db1  -c 'SHOW config_file;'

----------------------------------------------------------------------------------

Команды:

\l  - список БД

\c <имя бд> - подключение к БД

\dt - список таблиц

\d <таблица> - список полей таблицы

----------------------------------------------------------------------------------

Создание таблицы

CREATE TABLE products (
    product_no integer,
    name text,
    price numeric
);

Основные типы данных:

integer

char(размер)

serial - инкрементный счетчик

Добавление данных:

insert into test(id,name,age) values (3, 'c', 45);