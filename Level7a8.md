comando grep# Retos Bandit
Para documentar los retos bandit, usaremos la siguiente estructura:

# Level 7 a 8

## Objetivo
	La contraseña para el siguiente nivel se almacena en el archivo **data.txt** junto a la palabra **millionth**
## Datos de acceso
	Usuario: bandit7
	Contraseña: HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
## Solución
	bandit7@bandit:~$ grep millionth data.txt
millionth       cvX2JJa4CFALtqS87jk27qwqGhBM9plV
## Notas adicionales
	Utilizaremos el comando "grep" ya que buscamos una palabra exacta, (millionth) que es la que contiene la contraseña.
## Referencias 