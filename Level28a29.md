# Retos Bandit

# Level 28 a 29

## Objetivo
	There is a git repository at `ssh://bandit28-git@localhost/home/bandit28-git/repo`. The password for the user `bandit28-git` is the same as for the user `bandit28`.

	Clone the repository and find the password for the next level.
## Datos de acceso
	Usuario: bandit28
	contraseña: AVanL161y9rsbcJIsFHuw35rjaOM19nR
## Solución
``` Shell

	bandit28@bandit:~$ mkdir /tmp/priv/
bandit28@bandit:~$ ls
bandit28@bandit:~$ cd /tmp/priv
bandit28@bandit:/tmp/priv$ ssh://bandit28-git@localhost:2220/home/bandit28-git/repo
-bash: ssh://bandit28-git@localhost:2220/home/bandit28-git/repo: No such file or directory
bandit28@bandit:/tmp/priv$ git clone ssh://bandit28-git@localhost:2220/home/bandit28-git/repo
Cloning into 'repo'...
The authenticity of host '[localhost]:2220 ([127.0.0.1]:2220)' can't be established.
ED25519 key fingerprint is SHA256:C2ihUBV7ihnV1wUXRb4RrEcLfXC5CXlhmAAM/urerLY.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Could not create directory '/home/bandit28/.ssh' (Permission denied).
Failed to add the host to the list of known hosts (/home/bandit28/.ssh/known_hosts).
                         _                     _ _ _
                        | |__   __ _ _ __   __| (_) |_
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_
                        |_.__/ \__,_|_| |_|\__,_|_|\__|


                      This is an OverTheWire game server.
            More information on http://www.overthewire.org/wargames

!!! You are trying to log into this SSH server on port 2220 on localhost.
!!! Please log out and log in again instead.

bandit28-git@localhost's password:
remote: Enumerating objects: 9, done.
remote: Counting objects: 100% (9/9), done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 9 (delta 2), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (9/9), done.
Resolving deltas: 100% (2/2), done.
bandit28@bandit:/tmp/priv$ ls
repo
bandit28@bandit:/tmp/priv$ cd repo
bandit28@bandit:/tmp/priv/repo$ ls
README.md
bandit28@bandit:/tmp/priv/repo$ cat README
cat: README: No such file or directory
bandit28@bandit:/tmp/priv/repo$ cat README.md
# Bandit Notes
Some notes for level29 of bandit.

## credentials

- username: bandit29
- password: xxxxxxxxxx

bandit28@bandit:/tmp/priv/repo$ git show
commit 43032edb2fb868dea2ceda9cb3882b2c336c09ec (HEAD -> master, origin/master, origin/HEAD)
Author: Morla Porla <morla@overthewire.org>
Date:   Thu Sep 1 06:30:25 2022 +0000

    fix info leak

diff --git a/README.md b/README.md
index b302105..5c6457b 100644
--- a/README.md
+++ b/README.md
@@ -4,5 +4,5 @@ Some notes for level29 of bandit.
 ## credentials

 - username: bandit29
-- password: tQKvmcwNYcFS6vmPHIUSI3ShmsrQZK8S
+- password: xxxxxxxxxx

bandit28@bandit:/tmp/priv/repo$
```
## Notas adicionales
```
Clonamos el repositorio indicado en el objetivo en una carpeta que crearemos, entramos al repositorio clonado y leemos lo que hay en el readme, al no encontrar la contraseña, recurrimos a hacer un "git show" que nos mostrara el ultimo cambio en el readme, donde mostrara la contraseña.

```` 

## Referencias 
	Solamente usamos git.