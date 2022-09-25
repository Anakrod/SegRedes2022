# Nombre del reto
### PW Crack 2
## Objetivo
```
Can you crack the password to get the flag? Download the password checker [here](https://artifacts.picoctf.net/c/18/level2.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/18/level2.flag.txt.enc) in the same directory too.

HINT1: Does that encoding look familiar?
HINT2: The `str_xor` function does not need to be reverse engineered for this challenge.
```
## Solucion
``` shell
┌──(anitars㉿kali)-[~/Descargas]
└─$ ls
Addadshashanammu      code.py       file       fixme2.py  glitch.py            level1.py            level2.py  Obsidian-0.15.9.AppImage  static   warm
Addadshashanammu.zip  convertme.py  fixme1.py  flag       level1.flag.txt.enc  level2.flag.txt.enc  ltdis.sh   runme.py                  strings  warm.1
                                                                                                                                                                       
┌──(anitars㉿kali)-[~/Descargas]
└─$ python3 level2.py
Please enter correct password for flag: hola
That password is incorrect
                                                                                                                                                                       
┌──(anitars㉿kali)-[~/Descargas]
└─$ nano level2.py
                                                                                                                                                                       
┌──(anitars㉿kali)-[~/Descargas]
└─$ nano pwd.py   
                                                                                                                                                                       
┌──(anitars㉿kali)-[~/Descargas]
└─$ python3 pwd.py   
39ce
                                                                                                                                                                       
┌──(anitars㉿kali)-[~/Descargas]
└─$ python3 level2.py
Please enter correct password for flag: 39ce
Welcome back... your flag, user:
picoCTF{tr45h_51ng1ng_502ec42e}
                                                                                                                                                                       
┌──(anitars㉿kali)-[~/Descargas]
└─$ 


Descargamos lo que nos indica, verificamos que esten en la misma carpeta. Corremos el script y nos pedira una contraseña, introducimos cualquiera y nos dara un error, revisamos el codigo con 'nano' y nos damos cuenta que la contraseña esta encriptada, procedemos a copiar la contraseña y creamos un script en python que la desencriptara, lo corremos para obtener la contraseña, entramos a el primer script y obtenemos la bandera.
```
## Referencias