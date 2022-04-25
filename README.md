# lab

1. Create a php webpage and print “hello world”.
Aim:-
To Create a php webpage and print “hello world”.
Program:
<!DOCTYPE html>
<html>
<body>
<h1>My first PHP page</h1>
<?php
echo "Hello World!";
?>
</body>
</html>
Output:
My first PHP page

2.Write a PHP program to swap two numbers.
Aim:
To Create a PHP program to swap two numbers.
Program:
<html>
<head>
<title>Swapping of Two numbers</title>
</head>
<body>
<?php
$a = 15;
$b = 27;
// Swap Logic
echo "\nThe number before swapping is:\n";
echo "Number a =".$a." and b=".$b;
$temp = $a;
$a = $b;
$b = $temp;
echo "\nThe number after swapping is: \n";
echo "Number a =".$a." and b=".$b."\n";
?>
</body>
</html>
Output:
The number before swapping is: 
Number a =15 and b=27 
The number after swapping is: 
Number a =27 and b=15

3. Write a PHP Program to demonstrate the variable function: Gettype():
Aim:
To create a PHP Program to demonstrate the variable function: Gettype():
Program:
<html>
<head>
<title>Gettype() Function</title>
</head>
<body>
<?php
echo gettype(102).'<br>';
echo gettype(true).'<br>';
echo gettype(' ').'<br>';
echo gettype(null).'<br>';
echo gettype(array()).'<br>';
echo gettype(new stdclass());
?>
</body>
</html>
Output:
integer
boolean
string
NULL
array
object 

4.Write a PHP Program to demonstrate the variable unction: unset()
Aim:
To create a PHP Program to demonstrate the variable unction: unset()
Program:
<html>
<head>
<title>Unset Function</title>
</head>
<body>
<?php
function unset_val1()
{
global $val1;
echo $val1;
unset($val1);
}
$val1 = "Bipin";
unset_val1();
?>
</body>
</html>
Output:
Bipin

5.Give the example of string function: substr()
Aim:
To create a PHP program for string function: substr()
Program:
<html>
<head>
<title>Sub string Function</title>
</head>
<body>
<?php
$string1="Welcome to Rathinamcollege.com";
echo $string1;
echo '<br>';
echo substr($string1,1);
echo '<br>';
echo substr($string1,1,5);
echo '<br>';
echo substr($string1,0,10);
echo '<br>';
echo substr($string1,-1,1);
echo '<br>';
?>
</body>
</html>
Output:
Welcome to Rathinamcolleg

6.Give the example of string function: strcmp()
Aim:
To create a PHP program for using the string function: strcmp()
Program:
<html>
<head>
<title>String Compare Function</title>
</head>
<body>
<?php
$str1 = 'a';
$str2 = 'b';
echo strcmp($str1, $str2)."<br>";
$str3 = 'b';
$str4 = 'a';
echo strcmp($str3, $str4)."<br>";
$str5 = "Anil";
$str6 = "anil";
echo strcmp($str5, $str6)."<br>";
?>
</body>
</html>

7. Write a PHP program to create a database using MySQL.
Aim:
PHP program to create a database using MySQL.
Program:
<html>
<head>
<title>Create a Database using MySQL</title>
</head>
<body>
<?php
$con = mysql_connect("localhost","root","");
if(!$con)
{
die("not opened");
}
echo "Connection open"."<br>";
$query = "create database std";
$crdb = mysql_query($query,$con);
if(!$crdb) 
{ 
die("not created. .!".mysql_error()); 
}
echo "database created.. !";
?>
</body>
</html>
Output:
Connection open 
database created.. 
