# Nombre del reto
### strings it
## Objetivo
```
	Can you find the flag in [file](https://jupiter.challenges.picoctf.org/static/94d00153b0057d37da225ee79a846c62/strings) without running it?
	
```
## Solucion
``` shell 
	┌──(anitars㉿kali)-[~/Descargas]
└─$ strings strings | grep pico
picoCTF{5tRIng5_1T_d66c7bb7}
                                                                             
┌──(anitars㉿kali)-[~/Descargas]
└─$ 

```
## Referencias
	Hacemos uso del comando 'strings' como nos recomienda, y pedimos nos muestre donde este la palabra 'pico' con el comando grep para de esa manera encontremos la bandera.
