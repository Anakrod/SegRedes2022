# Nombre del reto
### wave a flag
## Objetivo
```
Can you invoke help flags for a tool or binary? [This program](https://mercury.picoctf.net/static/beec4f433e5ee5bfcd71bba8d5863faf/warm) has extraordinarily helpful information...
HINT1:This program will only work in the webshell or another Linux computer.
HINT2: To get the file accessible in your shell, enter the following in the Terminal prompt: `$ wget https://mercury.picoctf.net/static/beec4f433e5ee5bfcd71bba8d5863faf/warm`
HINT3: Run this program by entering the following in the Terminal prompt: `$ ./warm`, but you'll first have to make it executable with `$ chmod +x warm`
HINT4: -h and --help are the most common arguments to give to programs to get more information from them!
HINT5: Not every program implements help features like -h and --help.
```
## Solucion
```` shell
┌──(anitars㉿kali)-[~/Descargas]
└─$ wget https://mercury.picoctf.net/static/beec4f433e5ee5bfcd71bba8d5863faf/warm
--2022-09-22 22:20:25--  https://mercury.picoctf.net/static/beec4f433e5ee5bfcd71bba8d5863faf/warm
Resolviendo mercury.picoctf.net (mercury.picoctf.net)... 18.189.209.142
Conectando con mercury.picoctf.net (mercury.picoctf.net)[18.189.209.142]:443... conectado.
Petición HTTP enviada, esperando respuesta... 200 OK
Longitud: 10936 (11K) [application/octet-stream]
Grabando a: «warm.1»

warm.1              100%[================>]  10.68K  --.-KB/s    en 0s      

2022-09-22 22:20:26 (47.2 MB/s) - «warm.1» guardado [10936/10936]

                                                                             
┌──(anitars㉿kali)-[~/Descargas]
└─$ chmod +x warm
                                                                             
┌──(anitars㉿kali)-[~/Descargas]
└─$ ./warm 
Hello user! Pass me a -h to learn what I can do!
                                                                             
┌──(anitars㉿kali)-[~/Descargas]
└─$ ./warm -h
Oh, help? I actually don't do much, but I do have this flag here: picoCTF{b1scu1ts_4nd_gr4vy_616f7182}

````
## Referencias
```
seguimos solo los pasos de las pistas para llegar a la bandera.
```
