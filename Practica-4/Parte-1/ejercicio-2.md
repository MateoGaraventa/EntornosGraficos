Ejercicio 2:
Indicar si los siguientes códigos son equivalentes.

Inciso a)

Primer codigo
<?php
$i = 1;
while ($i <= 10) {
 print $i++; 
}
?>

Segundo codigo 
<?php
$i = 1;
while ($i <= 10):
 print $i;
 $i++;
endwhile;
?>

Tercer codigo
<?php
$i = 0;
do {
 print ++$i;
} while ($i<10);
?>

Si son equivalentes, todos los códigos muestran los numeros del 1 al 10 inclusive. En el primer caso la variable se postincrementa, por que lo primero muestra el valor 1 y despues aumenta su valor,mientras que en el último caso es un preincremento, es decir primero aumenta su valor de 0 a 1 y despues se muestra el 1.

Inciso b)

Primer codigo
<?php
for ($i = 1; $i <= 10; $i++) {
 print $i;
}
?>

Segundo codigo
<?php
for ($i = 1; $i <= 10; print $i, $i++) ;
?>

Tercer codigo
<?php
for ($i = 1; ;$i++) {
 if ($i > 10) {
 break;
 }
 print $i;
}
?>

Cuarto codigo
<?php
$i = 1;
for (;;) {
 if ($i > 10) {
 break;
 }
 print $i;
 $i++;
}
?>

Los códigos son equivalentes, muestran el valor de la variabe $i que va desde 1 a 10 inlcusive

Inciso c)

Primer codigo
<?php
…
…
if ($i == 0) {
 print "i equals 0";
} elseif ($i == 1) {
 print "i equals 1";
} elseif ($i == 2) {
 print "i equals 2";
}
?>

Segundo codigo
<?php
…
…
switch ($i) {
 case 0:
 print "i equals 0";
 break;
 case 1:
 print "i equals 1";
 break;
 case 2:
 print "i equals 2";
 break;
}
?>

Si son equivalentes