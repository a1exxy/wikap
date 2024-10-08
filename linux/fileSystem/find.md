# ОСНОВНАЯ ИНФОРМАЦИЯ О FIND
Find - это одна из наиболее важных и часто используемых утилит системы Linux. Это команда для поиска файлов и каталогов на основе специальных условий. Ее можно использовать в различных обстоятельствах, например, для поиска файлов по разрешениям, владельцам, группам, типу, размеру и другим подобным критериям.

Утилита find предустановлена по умолчанию во всех Linux дистрибутивах, поэтому вам не нужно будет устанавливать никаких дополнительных пакетов. Это очень важная находка для тех, кто хочет использовать командную строку наиболее эффективно.

Команда find имеет такой синтаксис:

find [папка] [параметры] критерий шаблон [действие]

Папка - каталог в котором будем искать

Параметры - дополнительные параметры, например, глубина поиска, и т д

Критерий - по какому критерию будем искать: имя, дата создания, права, владелец и т д.

Шаблон - непосредственно значение по которому будем отбирать файлы.

ОСНОВНЫЕ ПАРАМЕТРЫ КОМАНДЫ FIND
Я не буду перечислять здесь все параметры, рассмотрим только самые полезные.

-P никогда не открывать символические ссылки

-L - получает информацию о файлах по символическим ссылкам. Важно для дальнейшей обработки, чтобы обрабатывалась не ссылка, а сам файл.

-maxdepth - максимальная глубина поиска по подкаталогам, для поиска только в текущем каталоге установите 1.

-depth - искать сначала в текущем каталоге, а потом в подкаталогах

-mount искать файлы только в этой файловой системе.

-version - показать версию утилиты find

-print - выводить полные имена файлов

-type f - искать только файлы

-type d - поиск папки в Linux

КРИТЕРИИ
Критериев у команды find в Linux очень много, и мы опять же рассмотрим только основные.

-name - поиск файлов по имени

-perm - поиск файлов в Linux по режиму доступа

-user - поиск файлов по владельцу

-group - поиск по группе

-mtime - поиск по времени модификации файла

-atime - поиск файлов по дате последнего чтения

-nogroup - поиск файлов, не принадлежащих ни одной группе

-nouser - поиск файлов без владельцев

-newer - найти файлы новее чем указанный

-size - поиск файлов в Linux по их размеру

ПРИМЕРЫ ИСПОЛЬЗОВАНИЯ
А теперь давайте рассмотрим примеры find, чтобы вы лучше поняли, как использовать эту утилиту.

## 1. ПОИСК ВСЕХ ФАЙЛОВ
Показать все файлы в текущей директории:

 find

 find .

 find . -print

## 2. ПОИСК ФАЙЛОВ В ОПРЕДЕЛЕННОЙ ПАПКЕ
Показать все файлы в указанной директории:

 find ./test

Искать файлы по имени в текущей папке:

 find . -name "*.jpg"

Не учитывать регистр при поиске по имени:

 find . -iname "test*"

## 3. ОГРАНИЧЕНИЕ ГЛУБИНЫ ПОИСКА
Поиска файлов по имени в Linux только в этой папке:

 find . -maxdepth 1 -name "*.php"

## 4. ИНВЕРТИРОВАНИЕ ШАБЛОНА
Найти файлы, которые не соответствуют шаблону:

 find . -not -name "test*"

## 5. НЕСКОЛЬКО КРИТЕРИЕВ
Поиск командой find в Linux по нескольким критериям, с оператором исключения:

 find . -name "test" -not -name "*.php"

Найдет все файлы, начинающиеся на test, но без расширения php. А теперь рассмотрим оператор ИЛИ:

 find -name "*.html" -o -name "*.php"

## 6. НЕСКОЛЬКО КАТАЛОГОВ
Искать в двух каталогах одновременно:

 find ./test ./test2 -type f -name "*.c"

## 7. ПОИСК СКРЫТЫХ ФАЙЛОВ
Найти скрытые файлы:

 find ~ -type f -name ".*"

## 8. ПОИСК ПО РАЗРЕШЕНИЯМ
Найти файлы с определенной маской прав, например, 0664:

 find . type f -perm 0664

Найти файлы с установленным флагом suid/guid:

 find / -perm 2644

Или так:

 find / -maxdepth 2 -perm /u=s

Поиск файлов только для чтения:

 find /etc -maxdepth 1 -perm /u=r

Найти только исполняемые файлы:

 find /bin -maxdepth 2 -perm /a=x

## 9. ПОИСК ФАЙЛОВ ПО ГРУППАХ И ПОЛЬЗОВАТЕЛЯХ
Найти все файлы, принадлежащие пользователю:

 find . -user sergiy

Поиск файлов в Linux принадлежащих группе:

 find /var/www -group developer

## 10. ПОИСК ПО ДАТЕ МОДИФИКАЦИИ
Поиск файлов по дате в Linux осуществляется с помощью параметра mtime. Найти все файлы модифицированные 50 дней назад:

 find / -mtime 50

Поиск файлов в Linux открытых N дней назад:

 find / -atime 50

Найти все файлы, модифицированные между 50 и 100 дней назад:

 find / -mtime +50 –mtime -100

Найти файлы измененные в течении часа:

 find . -cmin 60

## 11. ПОИСК ФАЙЛОВ ПО РАЗМЕРУ
Найти все файлы размером 50 мегабайт:

 find / -size 50M

От пятидесяти до ста мегабайт:

 find / -size +50M -size -100M

Найти самые маленькие файлы:

 find . -type f -exec ls -s {} \; | sort -n -r | head -5

Самые большие:

 find . -type f -exec ls -s {} \; | sort -n | head -5

## 12. ПОИСК ПУСТЫХ ФАЙЛОВ И ПАПОК
 find /tmp -type f -empty

$ find ~/ -type d -empty

## 13. ДЕЙСТВИЯ С НАЙДЕННЫМИ ФАЙЛАМИ
Для выполнения произвольных команд для найденных файлов используется опция -exec. Например, выполнить ls для получения подробной информации о каждом файле:

 find . -exec ls -ld {} \;

Удалить все текстовые файлы в tmp

 find /tmp -type f -name "*.txt" -exec rm -f {} \;

Удалить все файлы больше 100 мегабайт:

 find /home/bob/dir -type f -name *.log -size +10M -exec rm -f {} \;