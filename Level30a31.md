# Retos Bandit

# Level 30 a 31
	There is a git repository at `ssh://bandit30-git@localhost/home/bandit30-git/repo`. The password for the user `bandit30-git` is the same as for the user `bandit30`.

	Clone the repository and find the password for the next level.
## Objetivo

## Datos de acceso
	Usuario: bandit30
	contraseña: xbhV3HpNGlTIdnjUrdAlPzc2L6y9EOnS
## Solución

``` Shell 
bandit30@bandit:~$ mkdir /tmp/dir/
bandit30@bandit:~$ cd /mkdir/dir
-bash: cd: /mkdir/dir: No such file or directory
bandit30@bandit:~$ cd /tmp/dir
bandit30@bandit:/tmp/dir$ git clone ssh://bandit30-git@localhost:2220/home/bandit30-git/repo
Cloning into 'repo'...
The authenticity of host '[localhost]:2220 ([127.0.0.1]:2220)' can't be established.
ED25519 key fingerprint is SHA256:C2ihUBV7ihnV1wUXRb4RrEcLfXC5CXlhmAAM/urerLY.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Could not create directory '/home/bandit30/.ssh' (Permission denied).
Failed to add the host to the list of known hosts (/home/bandit30/.ssh/known_hosts).
                         _                     _ _ _
                        | |__   __ _ _ __   __| (_) |_
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_
                        |_.__/ \__,_|_| |_|\__,_|_|\__|


                      This is an OverTheWire game server.
            More information on http://www.overthewire.org/wargames

!!! You are trying to log into this SSH server on port 2220 on localhost.
!!! Please log out and log in again instead.

bandit30-git@localhost's password:
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (4/4), done.
bandit30@bandit:/tmp/dir$ ls
repo
bandit30@bandit:/tmp/dir$ cd repo
bandit30@bandit:/tmp/dir/repo$ ls
README.md
bandit30@bandit:/tmp/dir/repo$ cat README.md
just an epmty file... muahaha
bandit30@bandit:/tmp/dir/repo$ git show
commit a325f29e1cc26b0f0dc5f89b4348e389b408cc87 (HEAD -> master, origin/master, origin/HEAD)
Author: Ben Dover <noone@overthewire.org>
Date:   Thu Sep 1 06:30:28 2022 +0000

    initial commit of README.md

diff --git a/README.md b/README.md
new file mode 100644
index 0000000..029ba42
--- /dev/null
+++ b/README.md
@@ -0,0 +1 @@
+just an epmty file... muahaha
bandit30@bandit:/tmp/dir/repo$ git tag
secret
bandit30@bandit:/tmp/dir/repo$ git show secret
OoffzGDlzhAlerFJ2cAiz1D41JW1Mhmt
bandit30@bandit:/tmp/dir/repo$
```

## Notas adicionales
	De nuevo clonamos un repositorio, leemos lo que hay en el readme, investigamos que podemoss hacer y encontramos el "git tag", hacemos uso de el y nos muestra que hay un "secret" lo mostramos con el "git show secret" y ahi se encuentra nuestra contraseña.
## Referencias 
	Hacemos uso de 
		-git tag
		-git show
