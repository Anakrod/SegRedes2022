# Retos Bandit
Para documentar los retos bandit, usaremos la siguiente estructura:

# Level 8 a 9

## Objetivo
	La contraseña para el siguiente nivel se almacena en el archivo **data.txt** y es la única línea de texto que aparece una sola vez
## Datos de acceso
	Usuario: bandit8
	Contraseña: cvX2JJa4CFALtqS87jk27qwqGhBM9plV
## Solución
bandit8@bandit:~$ cat data.txt  | sort  | uniq -u
UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR
bandit8@bandit:~$
## Notas adicionales
	Usaremos dos comandos, "sort" y "uniq" que nos permitira ordenar el contenido del archivo y mostrar la linea que no esta repetida,lo que nos permitira encontrar la contraseña.
## Referencias 