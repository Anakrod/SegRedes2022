# Nombre del reto
### Runme.py
## Objetivo
```
Run the `runme.py` script to get the flag. Download the script with your browser or with `wget` in the webshell. [Download runme.py Python script](https://artifacts.picoctf.net/c/86/runme.py)

HINT1: If you have Python on your computer, you can download the script normally and run it. Otherwise, use the `wget` command in the webshell.
HINT2: To use `wget` in the webshell, first right click on the download link and select 'Copy Link' or 'Copy Link Address'
HINT3: Type everything after the dollar sign in the webshell: `$ wget` , then paste the link after the space after `wget` and press enter. This will download the script for you in the webshell so you can run it!
HINT4: Finally, to run the script, type everything after the dollar sign and then press enter: `$ python3 runme.py` You should have the flag now!
```
## Solucion
``` shell
┌──(anitars㉿kali)-[~]
└─$ cd Descargas
                                                                             
┌──(anitars㉿kali)-[~/Descargas]
└─$ ls                     
Addadshashanammu      flag                      runme.py  warm
Addadshashanammu.zip  ltdis.sh                  static    warm.1
file                  Obsidian-0.15.9.AppImage  strings
                                                                             
┌──(anitars㉿kali)-[~/Descargas]
└─$ python3 runme.py 
picoCTF{run_s4n1ty_run}
                                                                             
┌──(anitars㉿kali)-[~/Descargas]
└─$  

Descargamos el script que nos indica y simplemente lo corremos, escribiendo "python3 [nombre del script]" para que nos mande lo que hace o en este caso, encontrar la bandera.
```
## Referencias