# Nombre del reto
### convertme.py
## Objetivo
```
Run the Python script and convert the given number from decimal to binary to get the flag. [Download Python script](https://artifacts.picoctf.net/c/31/convertme.py)

HINT1: Look up a decimal to binary number conversion app on the web or use your computer's calculator!
HINT2: The `str_xor` function does not need to be reverse engineered for this challenge.
HINT3: If you have Python on your computer, you can download the script normally and run it. Otherwise, use the `wget` command in the webshell.
HINT4: To use `wget` in the webshell, first right click on the download link and select 'Copy Link' or 'Copy Link Address'
HINT5: Type everything after the dollar sign in the webshell: `$ wget` , then paste the link after the space after `wget` and press enter. This will download the script for you in the webshell so you can run it!
HINT6: Finally, to run the script, type everything after the dollar sign and then press enter: `$ python3 convertme.py`
```
## Solucion
``` shell
┌──(anitars㉿kali)-[~/Descargas]
└─$ ls
Addadshashanammu      file      Obsidian-0.15.9.AppImage  strings
Addadshashanammu.zip  flag      runme.py                  warm
convertme.py          ltdis.sh  static                    warm.1
                                                                             
┌──(anitars㉿kali)-[~/Descargas]
└─$ python3 convertme.py
If 29 is in decimal base, what is it in binary base?
Answer: 11101
That is correct! Here's your flag: picoCTF{4ll_y0ur_b4535_9c3b7d4d}
                                                                             
┌──(anitars㉿kali)-[~/Descargas]
└─$ 

Corremos el script descargado previamente, seguido nos preguntara cual es X numero en binario, en este caso nos pregunto por el "29", para lo cual utilizamos un convertidor (adjunto en las referencias), al obtener la respuesta la tecleamos y de esa forma nos da la bandera.
```
## Referencias
``` shell
convertidor: 
https://www.rapidtables.org/convert/number/decimal-to-binary.html
```