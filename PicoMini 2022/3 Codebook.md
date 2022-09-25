# Nombre del reto
### Codebook
## Objetivo
```
Run the Python script `code.py` in the same directory as `codebook.txt`.

-   [Download code.py](https://artifacts.picoctf.net/c/102/code.py)
-   [Download codebook.txt](https://artifacts.picoctf.net/c/102/codebook.txt)
```
## Solucion
``` shell
┌──(anitars㉿kali)-[~/Descargas]
└─$ ls
Addadshashanammu      convertme.py  Obsidian-0.15.9.AppImage  warm
Addadshashanammu.zip  file          runme.py                  warm.1
codebook.txt          flag          static
code.py               ltdis.sh      strings
                                                                             
┌──(anitars㉿kali)-[~/Descargas]
└─$ python3 code.py     
picoCTF{c0d3b00k_455157_197a982c}
                                                                             
┌──(anitars㉿kali)-[~/Descargas]
└─$ 

Descargamos el script y libro que se nos pide, al momento de descargarlo se guardaran en la misma carpeta, por lo cual al correr el script nos dara la bandera, pero si por el contrario, el libro no esta en la misma carpeta esta no se nos dara:

"EJEMPLO"
┌──(anitars㉿kali)-[~/Descargas]
└─$ ls
Addadshashanammu      file                      runme.py  warm.1
Addadshashanammu.zip  flag                      static
code.py               ltdis.sh                  strings
convertme.py          Obsidian-0.15.9.AppImage  warm
                                                                             
┌──(anitars㉿kali)-[~/Descargas]
└─$ python3 code.py
Couldn't find codebook.txt. Did you download that file into the same directory as this script?'
                                                                             
┌──(anitars㉿kali)-[~/Descargas]
└─$ 

```
## Referencias