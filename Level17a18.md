# Level 17 a 18

## Objetivo
	There are 2 files in the homedirectory: **passwords.old and passwords.new**. The password for the next level is in **passwords.new** and is the only line that has been changed between **passwords.old and passwords.new**

**NOTE: if you have solved this level and see ‘Byebye!’ when trying to log into bandit18, this is related to the next level, bandit19**
## Datos de acceso
	Usuario: bandit17
	Contraseña: VwOSWtCA7lRKkTfbr2IDh6awj9RNZM5e
## Solución
	![[Pasted image 20220901083338.png]]

	bandit17@bandit:~$ ls
	passwords.new  passwords.old
	bandit17@bandit:~$ head passwords.old
	AaRtLcWpaZf2x05CinBQoTjVP6fML7EA
	VyuddgCO0UtJKMwC7H4vxAaIMGjPiqky
	gLdNHXq36zoT1HFfPYk4kw5h1Ixyqcvo
	q6qV3SwGPS7L0cw3aJA21lzhNMrAQcGC
	s1vg97taODeKBsWz5yVTIumCUQGggQEC
	ufsx6BLBrGbOAm5LftWxyvYvEpGPeHhv
	uLgMlo2nIcUwbm4oyKuwwo8KoT9eP6Oe
	dixsvhg78iuQJ5t2c2UbRLvwbJrbZF1n
	Wx2PczEyROiv1UYMIVpmXaljcRWMB52b
	wQs6u5FBMsS4Y1NGzQS7W2sv6NnmbJ2i
	bandit17@bandit:~$ head passwords.new
	AaRtLcWpaZf2x05CinBQoTjVP6fML7EA
	VyuddgCO0UtJKMwC7H4vxAaIMGjPiqky
	gLdNHXq36zoT1HFfPYk4kw5h1Ixyqcvo
	q6qV3SwGPS7L0cw3aJA21lzhNMrAQcGC
	s1vg97taODeKBsWz5yVTIumCUQGggQEC
	ufsx6BLBrGbOAm5LftWxyvYvEpGPeHhv
	uLgMlo2nIcUwbm4oyKuwwo8KoT9eP6Oe
	dixsvhg78iuQJ5t2c2UbRLvwbJrbZF1n
	Wx2PczEyROiv1UYMIVpmXaljcRWMB52b
	wQs6u5FBMsS4Y1NGzQS7W2sv6NnmbJ2i
	bandit17@bandit:~$
	bandit17@bandit:~$ diff passwords.old passwords.new
	42c42
	< 09wUIyMU4YhOzl1Lzxoz0voIBzZ2TUAf
	--- hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg
## Notas adicionales
	Usamos el comando "diff" (que nos servira para comparar) seguido de los documentos que queremos comparar.
## Referencias 