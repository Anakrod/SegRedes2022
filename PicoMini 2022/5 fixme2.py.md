# Nombre del reto
### fixme2.py
## Objetivo
```
Fix the syntax error in the Python script to print the flag. [Download Python script](https://artifacts.picoctf.net/c/65/fixme2.py)

HINT1: Are equality and assignment the same symbol?
HINT2: To view the file in the webshell, do: `$ nano fixme2.py`
HINT3: To exit `nano`, press Ctrl and x and follow the on-screen prompts.
HINT4: The `str_xor` function does not need to be reverse engineered for this challenge.
```
## Solucion
``` shell
┌──(anitars㉿kali)-[~/Descargas]
└─$ ls
Addadshashanammu      code.py       file       fixme2.py  ltdis.sh                  runme.py  strings  warm.1
Addadshashanammu.zip  convertme.py  fixme1.py  flag       Obsidian-0.15.9.AppImage  static    warm
                                                                                                                                                                       
┌──(anitars㉿kali)-[~/Descargas]
└─$ python3 fixme2.py
  File "/home/anitars/Descargas/fixme2.py", line 22
    if flag = "":
       ^^^^^^^^^
SyntaxError: invalid syntax. Maybe you meant '==' or ':=' instead of '='?
                                                                                                                                                                       
┌──(anitars㉿kali)-[~/Descargas]
└─$ nano fixme2.py
                                                                                                                                                                       
┌──(anitars㉿kali)-[~/Descargas]
└─$ python3 fixme2.py
That is correct! Here's your flag: picoCTF{3qu4l1ty_n0t_4551gnm3nt_e8814d03}'
                                                                                                                                                                       
┌──(anitars㉿kali)-[~/Descargas]
└─$ 

Descargamos el script, lo corremos y nos marca un error en un if, entramos a revisarlo con el comando 'nano', corregimos, guardamos y volvemos a correr obteniendo la bandera.
```
## Referencias