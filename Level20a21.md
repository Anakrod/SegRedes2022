# Level 20 a 21

## Objetivo
	There is a setuid binary in the homedirectory that does the following: it makes a connection to localhost on the port you specify as a commandline argument. It then reads a line of text from the connection and compares it to the password in the previous level (bandit20). If the password is correct, it will transmit the password for the next level (bandit21).

	**NOTE:** Try connecting to your own network daemon to see if it works as you think
## Datos de acceso
	Usuario: bandit20
	Contraseña: VxCazJaVykI6W36BkBU0mJTCM8rR95XT
## Solución
	bandit20@bandit:~$ nc -lvp 3030 <<< VxCazJaVykI6W36BkBU0mJTCM8rR95XT &
	[3] 634791
	bandit20@bandit:~$ Listening on 0.0.0.0 3030
	
	bandit20@bandit:~$ jobs
	[1]-  Stopped                 nc -lvp 2020
	[2]+  Stopped                 nc localhost 3030
	[3]   Running                 nc -lvp 3030 <<< VxCazJaVykI6W36BkBU0mJTCM8rR95XT &
	bandit20@bandit:~$ ./suconnect 3030
	Connection received on localhost 36486
	Read: VxCazJaVykI6W36BkBU0mJTCM8rR95XT
	Password matches, sending next password
	NvEJF7oVjkddltPSrdKEFOllh9V1IBcq
	[3]   Done                    nc -lvp 3030 <<< VxCazJaVykI6W36BkBU0mJTCM8rR95XT
	bandit20@bandit:~$
## Notas adicionales
	Utilizamos el comando nc -lvp [puerto] seguido de la contraseña que usamos para entrar a el usuario 20 y un & (esto para mandarla a segundo plano y poder hacer lo siguiente)
	Despues ponemos el siguiente comando "./suconnect [puerto]"
## Referencias 