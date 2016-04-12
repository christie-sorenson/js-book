# Ace Editor


{% ace lang="javascript", edit=true %}

var a = parseInt("3.5dog",10); //3
var b = parseFloat("3.5dog");//3.6
var c = parseInt("foo3",10); //NaN
var trouble = parseInt("011");
alert(trouble);  
/* 9 w/o radix assumes octal  in older versions */
var hex = parseInt("0xFF"); // 255

{% endace %}