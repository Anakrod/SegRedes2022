
# Level 13 a 14

## Objetivo
	The password for the next level is stored in **/etc/bandit_pass/bandit14 and can only be read by user bandit14**. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. **Note:** **localhost** is a hostname that refers to the machine you are working on
## Datos de acceso
	Usuario: bandit13
	Contraseña: 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL
## Solución
	´´´ bash bandit13@bandit:~$ ssh -i sshkey.private  bandit14@localhost
	bandit14@bandit:~$ cat /etc/bandit_pass/bandit14
	4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e

## Notas adicionales
	Entramos a el usuario "bandit14" por medio de una sshkey
## Referencias 