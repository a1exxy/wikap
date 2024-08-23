Экспорт напрямую из MySql в csv-файл:



SELECT id, name, email INTO OUTFILE '/tmp/result.csv'

FIELDS TERMINATED BY ',' OPTIONALLY ENCLOSED BY '"'

ESCAPED BY ‘\\’

LINES TERMINATED BY '\n'

FROM users WHERE 1

Используя PHP-скрипт:


// Параметры доступа к БД

 

$host="localhost";

$uname="root";

$pass="";

$database = "testDb";

 

$connection=mysql_connect($host,$uname,$pass);

 

echo mysql_error();

 

$selectdb=mysql_select_db($database) or

die("Database could not be selected");

$result=mysql_select_db($database)

or die("database cannot be selected <br>");

 

// Получение данных из БД

 

$output = "";// Строка-результат

$sql = mysql_query("select * from 'test'");

$columns_total = mysql_num_fields($sql);

 

// Первая строка - название полей

 

for ($i = 0; $i < $columns_total; $i++) {

    $heading = mysql_field_name($sql, $i);

    $output .= '"'.$heading.'",';

}

$output .="\n";

 

// Получить данные для записи в файл

 

while ($row = mysql_fetch_array($sql)) {

    for ($i = 0; $i < $columns_total; $i++) {

        $output .='"'.$row["$i"].'",';

    }

    $output .="\n";

}

 

// Скачать файл

 

$filename = "myFile.csv";

header('Content-type: application/csv');

header('Content-Disposition: attachment; filename='.$filename);

 

echo $output;

exit;