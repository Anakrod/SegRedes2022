# Level 26 a 27

## Objetivo
	Good job getting a shell! Now hurry and grab the password for bandit27!
## Datos de acceso
	Usuario: bandit26
	contraseña: c7GvcKlw9mC7aUQaPx7nwFstuAIBw1o1
## Solución
``` Shell 
	En el modo edicion ponemos lo siguiente
:set shell=/bin/bash
despues un 
"shell"

bandit26@bandit:~$ ./bandit27-do cat /etc/bandit_pass/bandit27
YnQpBuifNMas1hcUFk70ZmqkhUU2EuaS
bandit26@bandit:~$
```
## Notas adicionales
	Hacemos uso del more y la tecla 'v' para pasar al modo de edicion
	Despues de eso ingresamos el siguiente comando "./bandit27-do cat /etc/bandit_pass/bandit27" que es donde se encuentra la contraseña para el siguiente nivel.
## Referencias 