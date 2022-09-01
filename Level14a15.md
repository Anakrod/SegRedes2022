
# Level 14 a 15

## Objetivo
	  
	The password for the next level can be retrieved by submitting the password of the current level to **port 30000 on localhost**.
## Datos de acceso
	Usuario: bandit14
	Contraseña: 4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
## Solución
	bandit14@bandit:~$ nc localhost 30000
	bandit14@bandit:~$ nc -v localhost 30000
	localhost [127.0.0.1] 30000 (?) open
	4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
	Correct!
	BfMYroe26WYalil77FoDi9qh59eK5xNr
## Notas adicionales
	Utilizamoes el comando "nc" para entrar a nuestro localhost, seguido de el puerto donde se encontrara la contraseña. Para que me de la contraseña debo introducir la contraseña con la que entramos a este nivel (14)
## Referencias 