require "header.htm"; // Включение файла до начала работы

include имя_файла; // Включение файла во время работы

Подключение к БД

require "db.php";

$link = mysql_connect($DBSERVER, $DBUSER, $DBPASS)

or die("Could not connect : " . mysql_error());

print "Connected successfully<br>";

mysql_select_db($DBNAME) or die("Could not select database");

mysql_query("SET character_set_client = 'utf8'");

mysql_query("SET character_set_connection = 'utf8'");

mysql_query("SET character_set_results = 'utf8'");

mysql_query("SET NAMES utf8");

Вставка данных из формы в БД:

if(isset($_POST['surname']))         $surname = $_POST['surname'];if(isset($_POST['name']))         $name = $_POST['name'];$query = "INSERT INTO sotrud (surname, name) VALUES ('$surname', '$name')";