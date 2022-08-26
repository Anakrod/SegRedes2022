# Level 1 a 2

## Objetivo
	La contraseña para el siguiente nivel se almacena en un archivo llamado **-** ubicado en el directorio de inicio
## Datos de acceso
	usuario: bandit1
	contraseña: boJ9jbbUNNfktd78OOpsqOltutMc3MY1
## Solución

bandit1@bandit:~$ ls
-
bandit1@bandit:~$ cat -
^C
bandit1@bandit:~$ cat ./-
CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9
bandit1@bandit:~$

## Notas adicionales
	Utilizaremos el comando 'CAT' para leer lo que hay dentro del archivo solicitado.
	
	El comando cat confunde al "-" como parte de la entrada estandar, por lo tanto hay que poner ./ antes del nombre
## Referencias 