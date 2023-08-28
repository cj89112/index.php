# index.php

# index.php

//A PHP script can be placed anywhere in the document.

//A PHP script starts with <?php and ends with ?>:

<!DOCTYPE html>
<html>
<body>

<h1>My first PHP page</h1>

//In PHP, keywords (e.g. if, else, while, echo, etc.), classes, functions, and user-defined functions are not case-sensitive.

<?php
ECHO "Hello World!<br>";
echo "Hello World!<br>";
EcHo "Hello World!<br>";
?>

//Look at the example below; only the first statement will display the value of the $color variable! This is because $color, $COLOR, and $coLOR are treated as three different variables:

<?php
$color = "red";
echo "My car is " . $color . "<br>";
echo "My house is " . $COLOR . "<br>";
echo "My boat is " . $coLOR . "<br>";
?>

<?php
/*
This is a multiple-lines comment block
that spans over multiple
lines
*/
?>

//Example

<?php
// You can also use comments to leave out parts of a code line
$x = 5 /* + 15 */ + 5;
echo $x;
?>

//In PHP, a variable starts with the $ sign, followed by the name of the variable:

<?php
$txt = "Hello world!";
$x = 5;
$y = 10.5;
?>

<?php
\*
After the execution of the statements above, the variable $txt will hold the value Hello world!, the variable $x will hold the value 5, and the variable $y will hold the value 10.5.

Note: When you assign a text value to a variable, put quotes around the value.

Note: Unlike other programming languages, PHP has no command for declaring a variable. It is created the moment you first assign a value to it.
*/
?>

//The PHP echo statement is often used to output data to the screen.

<?php
$txt = "W3Schools.com";
echo "I love $txt!";
?>

//The following example will output the sum of two variables:

<?php
$x = 5;
$y = 4;
echo $x + $y;
?>

//A variable declared outside a function has a GLOBAL SCOPE and can only be accessed outside a function:

<?php
$x = 5; // global scope

function myTest() {
  // using x inside this function will generate an error
  echo "<p>Variable x inside function is: $x</p>";
}
myTest();

echo "<p>Variable x outside function is: $x</p>";
?>

//A variable declared within a function has a LOCAL SCOPE and can only be accessed within that function:

<?php
function myTest() {
  $x = 5; // local scope
  echo "<p>Variable x inside function is: $x</p>";
}
myTest();

// using x outside the function will generate an error
echo "<p>Variable x outside function is: $x</p>";
?>

<?php
\*
The global keyword is used to access a global variable from within a function.

To do this, use the global keyword before the variables (inside the function):
*/
?>

<?php
$x = 5;
$y = 10;

function myTest() {
  global $x, $y;
  $y = $x + $y;
}

myTest();
echo $y; // outputs 15
?>



</body>
</html>
