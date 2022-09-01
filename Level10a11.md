# Level 10 a 11

## Objetivo
	The password for the next level is stored in the file **data.txt**, which contains base64 encoded data

## Datos de acceso
	Usuario: bandit10
	Contraseña: truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk
## Solución
	bandit10@bandit:~$ cat data.txt | base64 -d
	The password is IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR
	bandit10@bandit:~$ python
	Python 2.7.13 (default, Sep 26 2018, 18:42:22)
	[GCC 6.3.0 20170516] on linux2
	Type "help", "copyright", "credits" or "license" for more information.
``>>> import codecs 
	
	data = open('data.txt','r').read()
	data
	'VGhlIHBhc3N3b3JkIGlzIElGdWt3S0dzRlc4TU9xM0lSRnFyeEUxaHhUTkViVVBSCg==\n'
	codecs.decode(data, 'base64')
	'The password is IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR\n' 

## Notas adicionales
	Hay 2 maneras de poder solucionar el reto, una de ellas de usando el comando "base64" y la otra solucion seria utilizando python.
	``` 

## Referencias 
