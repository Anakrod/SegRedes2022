# Level 11 a 12

## Objetivo
	The password for the next level is stored in the file **data.txt**, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions
## Datos de acceso
	Usuario: bandit11
	Contraseña: IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR
## Solución
	bandit11@bandit:~$ cat data.txt
Gur cnffjbeq vf 5Gr8L4qetPEsPk8htqjhRK8XSP6x2RHh
bandit11@bandit:~$ cat data.txt | tr [a-zA-Z] [n-za-mN-ZA-M]  
bandit11@bandit:~$ cat data.txt | tr [a-zA-Z] [n-za-mN-ZA-M]
The password is 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu
bandit11@bandit:~$
## Notas adicionales
	Lo podemos resolver usando el comando "tr" y de igual manera usando python
## Referencias 