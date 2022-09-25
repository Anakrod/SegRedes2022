# Nombre del reto
### PW Crack 3
## Objetivo
```
Can you crack the password to get the flag? Download the password checker [here](https://artifacts.picoctf.net/c/23/level3.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/23/level3.flag.txt.enc) and the [hash](https://artifacts.picoctf.net/c/23/level3.hash.bin) in the same directory too. There are 7 potential passwords with 1 being correct. You can find these by examining the password checker script.

HINT1: To view the level3.hash.bin file in the webshell, do: `$ bvi level3.hash.bin`
HINT2: To exit `bvi` type `:q` and press enter.
HINT3: The `str_xor` function does not need to be reverse engineered for this challenge.
```
## Solucion
``` shell
┌──(anitars㉿kali)-[~/Descargas]
└─$ python3 level3.py   
Please enter correct password for flag: 6997
That password is incorrect
                                                                                                                                                                       
┌──(anitars㉿kali)-[~/Descargas]
└─$ python3 level3.py
Please enter correct password for flag: 3ac8
That password is incorrect
                                                                                                                                                                       
┌──(anitars㉿kali)-[~/Descargas]
└─$ python3 level3.py
Please enter correct password for flag: 865e
That password is incorrect
                                                                                                                                                                       
┌──(anitars㉿kali)-[~/Descargas]
└─$ python3 level3.py
Please enter correct password for flag: 4e66
That password is incorrect
                                                                                                                                                                       
┌──(anitars㉿kali)-[~/Descargas]
└─$ python3 level3.py
Please enter correct password for flag: ec27
That password is incorrect
                                                                                                                                                                       
┌──(anitars㉿kali)-[~/Descargas]
└─$ python3 level3.py
Please enter correct password for flag: 4b17
Welcome back... your flag, user:
picoCTF{m45h_fl1ng1ng_2b072a90}
                                                                                                                                                                       
┌──(anitars㉿kali)-[~/Descargas]
└─$ 


Revisamos los scripts descargados, en level3.py nos muestra las posibles contraseñas, al no encontrar nada en los demas scripts procedemos a intentar con cada contraseña dada hasta entrar y obtener la bandera.
```
## Referencias