# Nombre del reto
### fixme1.py
## Objetivo
```
Fix the syntax error in this Python script to print the flag. [Download Python script](https://artifacts.picoctf.net/c/39/fixme1.py)

HINT1: Indentation is very meaningful in Python
HINT2: To view the file in the webshell, do: `$ nano fixme1.py`
HINT3: To exit `nano`, press Ctrl and x and follow the on-screen prompts.
HINT4: The `str_xor` function does not need to be reverse engineered for this challenge.
```
## Solucion
``` shell
┌──(anitars㉿kali)-[~/Descargas]
└─$ python3 fixme1.py 
  File "/home/anitars/Descargas/fixme1.py", line 20
    print('That is correct! Here\'s your flag: ' + flag)
IndentationError: unexpected indent
                                                                             
┌──(anitars㉿kali)-[~/Descargas]
└─$ nano fixme1.py 
                                                                                                                                                                       
┌──(anitars㉿kali)-[~/Descargas]
└─$ python3 fixme1.py
That is correct! Here's your flag: picoCTF{1nd3nt1ty_cr1515_182342f7}'
                                                                                                                                                                       
┌──(anitars㉿kali)-[~/Descargas]
└─$ 


Descargamos el script y lo corremos, nos manda el error que es de identacion, revisamos el script con el comando "nano" el cual nos permitira editarlo, arreglamos la identacion en la ultima linea, guardamos, volvemos a correr y si esta bien nos dara la bandera.
```
## Referencias