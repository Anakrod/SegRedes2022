# Retos Bandit
Para documentar los retos bandit, usaremos la siguiente estructura:

# Level 9 a 10

## Objetivo
	La contraseña para el siguiente nivel se almacena en el archivo **data.txt** en una de las pocas cadenas legibles por humanos, precedida por varios caracteres '='.
## Datos de acceso
	Usuario: bandit9
	Contraseña: UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR
## Solución
	bandit9@bandit:~$ strings data.txt | grep ==
========== the*2i"4
========== password
Z)========== is
&========== truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk
bandit9@bandit:~$
## Notas adicionales
	Usaremos el comando "strings" que nos mostrara solamente los caracteres imprimibles.
## Referencias 