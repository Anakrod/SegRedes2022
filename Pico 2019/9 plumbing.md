# Nombre del reto
### plumbing
## Objetivo
```
	Sometimes you need to handle process data outside of a file. Can you find a way to keep the output from this program and search for the flag? Connect to `jupiter.challenges.picoctf.org 14291`.
	HINT1: Remember the flag format is picoCTF{XXXX}
	HINT2: What's a pipe? No not that kind of pipe... This [kind](http://www.linfo.org/pipes.html)
```
## Solucion
``` shell
	──(anitars㉿kali)-[~/Descargas]
	└─$ nc jupiter.challenges.picoctf.org 14291 | grep pico
	picoCTF{digital_plumb3r_ea8bfec7}
```
## Referencias
```
	Utilizamos el comando grep, con un pipe "|" para conectarnos y seguido del pipe ponemos el comando grep para identificar la bandera.
```
