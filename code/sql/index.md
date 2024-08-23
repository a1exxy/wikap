SHOW DATABASES; - список баз данных SHOW TABLES [FROM db_name]; -  список таблиц в базе  SHOW COLUMNS FROM таблица [FROM db_name]; - список столбцов в таблице SHOW CREATE TABLE table_name; - показать структуру таблицы в формате "CREATE TABLE" SHOW INDEX FROM tbl_name; - список индексов SHOW GRANTS FOR user [FROM db_name]; - привилегии для пользователя.   SHOW VARIABLES; - значения системных переменных SHOW [FULL] PROCESSLIST; - статистика по mysqld процессам SHOW STATUS; - общая статистика SHOW TABLE STATUS [FROM db_name]; - статистика по всем таблицам в базе

SELECT DISTINCT используется для возврата только разных значений из таблицы.

Синтаксис SQL SELECT DISTINCT
1 2

SELECT DISTINCT column_name(s)FROM table_name

Пример SELECT DISTINCT
Есть таблица "Persons":
P_Id	LastName	FirstName	Address	City
1	Hansen	Ola	Timoteivn 10	Sandnes
2	Svendson	Tove	Borgvn 23	Sandnes
3	Pettersen	Kari	Storgt 20	Stavanger

Итак, мы хотим выбрать только разные значения из колонки "City".

Для этого используем такой запрос:

1

SELECT DISTINCT City FROM Persons