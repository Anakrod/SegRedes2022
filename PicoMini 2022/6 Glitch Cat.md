# Nombre del reto
### Glitch Cat
## Objetivo
``` shell
Our flag printing service has started glitching! `$ nc saturn.picoctf.net 51109`

HINT1: ASCII is one of the most common encodings used in programming
HINT2: We know that the glitch output is valid Python, somehow!
HINT3: Press Ctrl and c on your keyboard to close your connection and return to the command prompt.
```
## Solucion
``` shell
┌──(anitars㉿kali)-[~/Descargas]
└─$ nc saturn.picoctf.net 51109
'picoCTF{gl17ch_m3_n07_' + chr(0x62) + chr(0x64) + chr(0x61) + chr(0x36) + chr(0x38) + chr(0x66) + chr(0x37) + chr(0x35) + '}'
                                                                                                                                                                       
┌──(anitars㉿kali)-[~/Descargas]
└─$ nano glitch.py                                                                                                                                                                                    
┌──(anitars㉿kali)-[~/Descargas]
└─$ python3 glitch.py          
picoCTF{gl17ch_m3_n07_bda68f75}
                                                                                                                                                                       
┌──(anitars㉿kali)-[~/Descargas]

Nos conectamos como se nos indica en el objetivo, nos da la bandera a medias, para poder decifrarla crearemos un script con los siguiente:
print('picoCTF{gl17ch_m3_n07_' + chr(0x62) + chr(0x64) + chr(0x61) + chr(0x36) + chr(0x38) + chr(0x66) + chr(0x37) + chr(0x35) + '}')
lo guardamos y lo corremos, obtiendo la bandera completa.
```
## Referencias