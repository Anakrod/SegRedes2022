# Nombre del reto
### PW Crack 1
## Objetivo
```
Can you crack the password to get the flag? Download the password checker [here](https://artifacts.picoctf.net/c/52/level1.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/52/level1.flag.txt.enc) in the same directory too.

HINT1: To view the file in the webshell, do: `$ nano level1.py`
HINT2: To exit `nano`, press Ctrl and x and follow the on-screen prompts.
HINT3: The `str_xor` function does not need to be reverse engineered for this challenge.
```
## Solucion
``` shell
┌──(anitars㉿kali)-[~/Descargas]
└─$ nano level1.py
                                                                                                                                                                       
┌──(anitars㉿kali)-[~/Descargas]
└─$ python3 level1.py
Please enter correct password for flag: 1e1a
Welcome back... your flag, user:
picoCTF{545h_r1ng1ng_fa343060}
                                                                                                                                                                       
┌──(anitars㉿kali)-[~/Descargas]
└─$ 


Descargamos lo indicado, corremos el script 'level1.py' nos pide una contraseña la cual no sabemos, recurrimos a leer el script por medio del comando 'nano', revisamos el codigo y encontramos la contraseña que se necesita para que nos de la bandera, la copiamos y la introduciomos para que nos de la bandera.
```
## Referencias