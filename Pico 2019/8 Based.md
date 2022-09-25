# Nombre del reto
### Based
## Objetivo
```
	To get truly 1337, you must understand different data encodings, such as hexadecimal or binary. Can you get the flag from this program to prove you are on the way to becoming 1337? Connect with `nc jupiter.challenges.picoctf.org 15130`.
	HINT1: I hear python can convert things.
	HINT2: It might help to have multiple windows open.
```
## Solucion
``` shell
┌──(anitars㉿kali)-[~/Descargas]
└─$ nc jupiter.challenges.picoctf.org 15130 
Let us see how data is stored
socket
Please give the 01110011 01101111 01100011 01101011 01100101 01110100 as a word.
...
you have 45 seconds.....

Input:
socket
Please give me the  163 157 143 153 145 164 as a word.
Input:
socket
Please give me the 70656172 as a word.
Input:
pear
You've beaten the challenge
Flag: picoCTF{learning_about_converting_values_02167de8}

```
## Referencias
``` shell 
	utilizamos convertidores
	primero de binario a texto
		https://www.rapidtables.com/convert/number/binary-to-ascii.html
	despues de octal a texto
		http://www.unit-conversion.info/texttools/octal/
	y al final de hexa a texto
		https://www.rapidtables.com/convert/number/hex-to-ascii.html
``` 

