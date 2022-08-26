# Level 5 a 6

## Objetivo
	La contraseña para el siguiente nivel se almacena en un archivo en algún lugar del directorio **inhere** y tiene todas las siguientes propiedades:
	-   human-readable
	-   1033 bytes in size
	-   not executable
## Datos de acceso
	Usuario: bandit5
	Contraseña: koReBOKuIDDepwhWk7jZC0RTdopnAYKh
## Solución
	bandit5@bandit:~/inhere$ find -size 1033c
	bandit5@bandit:~/inhere$ cat ./maybehere07/.file2
	DXjZPULLxYr17uwoI01bNLQbtFemEgo7                                      bandit5@bandit:~/inhere$
## Notas adicionales
	Utilizaremos el comando "Find" para buscar el archivo con las caracteristicas que nos pide.
## Referencias 