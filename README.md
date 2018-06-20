# AnitaR_rep

<?php

$radijus = 4.0; 
$pi = 3.14;
$title1="povrsina kruga";
$title2="opseg kruga";
$a = 5.0; //stranica-osnovica trokuta a
$b = 3.0; //stranica trokuta b
$c = 4.0; //stranica trokuta c
$Va = 4; //visina na osnovicu trokuta a
$title3="povrsina trokuta";
$title4="opseg trokuta";

echo "<html> <head> <title1> $title1 = </title1></head> <body>"; 

function KrugPovrsina($radijus, $pi) 
{
    $povrsina = $radijus * $radijus * $pi; 
    return $povrsina; 
} 

function KrugOpseg($radijus, $pi) 
{
    $opseg = 2 * $radijus * $pi; 
    return $opseg; 
} 

function TrokutPovrsina($a, $b, $c, $Va) 
{
    $povrsina = 0.5 * $a * $Va; 
    return $povrsina; 
} 

function TrokutOpseg($a, $b, $c, $Va) 
{
    $opseg = $a + $b + $c; 
    return $opseg; 
} 

echo KrugPovrsina($radijus, $pi) . "<br>"; 

echo "$title2 = " . KrugOpseg($radijus, $pi) . "<br>"; 

echo "$title3 = " . TrokutPovrsina ($a, $b, $c, $Va) . "<br>"; 

echo "$title4 = " . TrokutOpseg($a, $b, $c, $Va); 

echo "</body> </html>";
