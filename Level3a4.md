# Retos Bandit
Para documentar los retos bandit, usaremos la siguiente estructura:

# Level 3 a 4

## Objetivo
	La contraseña para el siguiente nivel se almacena en un archivo oculto en el directorio **inhere** .
## Datos de acceso
	Usaurio: bandit3
	Contraseña: UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK
## Solución
bandit3@bandit:~$ ls
inhere
bandit3@bandit:~$ cd inhere/
bandit3@bandit:~/inhere$ ls
bandit3@bandit:~/inhere$ ls -a
.  ..  .hidden
bandit3@bandit:~/inhere$ cat .hidden
pIwrPrtPN36QITSp3EQaw936yaFoFgAB
bandit3@bandit:~/inhere$

## Notas adicionales
	El comando ls -a me permite ver documentos/archivos ocultos
## Referencias 