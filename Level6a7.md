# Level 6 a 7

## Objetivo
	La contraseña para el siguiente nivel se almacena **en algún lugar del servidor** y tiene todas las siguientes propiedades:
	-   owned by user bandit7
	-   owned by group bandit6
	-   33 bytes in size
## Datos de acceso
	Usuario: bandit6
	Contraseña: DXjZPULLxYr17uwoI01bNLQbtFemEgo7  
## Solución
bandit6@bandit:~$ find -user bandit7 -group bandit6 -size 33c 2>/dev/null
bandit6@bandit:~$ cat /var/lib/dpkg/info/bandit7.password
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
## Notas adicionales
	Volvemos a utilizar el comando "find" para encontrar el archivo con las caracteristicas correctas.
## Referencias 
