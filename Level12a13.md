
# Level 12 a 13

## Objetivo
	The password for the next level is stored in the file **data.txt**, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work using mkdir. For example: mkdir /tmp/myname123. Then copy the datafile using cp, and rename it using mv (read the manpages!)
## Datos de acceso
	Usuario: bandit12
	Contraseña: 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu
## Solución
	bandit12@bandit:~$ cat data.txt | xxd -r | file -
	/dev/stdin: gzip compressed data, was "data2.bin", last modified: Thu May  7 18:14:30 2020, max compression, from Unix
	bandit12@bandit:~$ cat data.txt | xxd -r | zcat | file -
	/dev/stdin: bzip2 compressed data, block size = 900k
	bandit12@bandit:~$ cat data.txt | xxd -r | zcat | bzcat | file -
	/dev/stdin: gzip compressed data, was "data4.bin", last modified: Thu May  7 18:14:30 2020, max compression, from Unix
	bandit12@bandit:~$ cat data.txt | xxd -r | zcat | bzcat | zcat | file -
	/dev/stdin: POSIX tar archive (GNU)
	bandit12@bandit:~$ cat data.txt | xxd -r | zcat | bzcat | zcat | tar xO | file -
	/dev/stdin: POSIX tar archive (GNU)
	bandit12@bandit:~$ cat data.txt | xxd -r | zcat | bzcat | zcat | tar xO | tar xO | file -
	/dev/stdin: bzip2 compressed data, block size = 900k
	bandit12@bandit:~$ cat data.txt | xxd -r | zcat | bzcat | zcat | tar xO | tar xO | bzcat | file -
	/dev/stdin: POSIX tar archive (GNU)
	bandit12@bandit:~$ cat data.txt | xxd -r | zcat | bzcat | zcat | tar xO | tar xO | bzcat | tar xO | file -
	/dev/stdin: gzip compressed data, was "data9.bin", last modified: Thu May  7 18:14:30 2020, max compression, from Unix
	bandit12@bandit:~$ cat data.txt | xxd -r | zcat | bzcat | zcat | tar xO | tar xO | bzcat | tar xO | zcat | file -
	/dev/stdin: ASCII text
	bandit12@bandit:~$ cat data.txt | xxd -r | zcat | bzcat | zcat | tar xO | tar xO | bzcat | tar xO | zcat
	The password is 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL
	bandit12@bandit:~$
## Notas adicionales
	Algo largo y complicado, utilizamos decomprension, "zcat", "bzcat", "tar xO" para poder ir descomprimiendo cada archivo.
	El comando "file -" lo utilizamos para que nos muestre que tipo de archivo es.
## Referencias 