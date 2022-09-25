# Nombre del reto
### Static aint always noise
## Objetivo
```
Can you look at the data in this binary: [static](https://mercury.picoctf.net/static/66932732825076cad4ba43e463dae82f/static)? This [BASH script](https://mercury.picoctf.net/static/66932732825076cad4ba43e463dae82f/ltdis.sh) might help!
```
## Solucion
``` shell
┌──(anitars㉿kali)-[~/Descargas]
└─$ strings static | grep pico
picoCTF{d15a5m_t34s3r_f5aeda17}
                                 
```
## Referencias
```
Usamos el comando strings para convertir lo que hay en el documento, y agrupamos para que solamente nos salga donde hay la palabra "pico"
```
