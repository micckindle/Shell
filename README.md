# Shell

## Getting start with Linux Shell 

### Linux kernel


- System memory management
- Software program management
- Hardware management
- File system management

-------------------------------------
### Linux desktop environment

- X windows system
- KDE desktop
- GNOME desktop
- other: fluxbox, xfree, fvwm, fvwm95


-------------------------------------
### Linux distributions

1. Slackware
2. Red Hat
3. Fedora
4. Gentoo
5. Mandriva
6. openSuSe
7. Debian
8. Linspire
9. Xandros
10. simpleMEPIS
11. ubuntu
12. PCLinuxOS
13. dyne:bolie
14. Puppy Linux

-------------------------------------
### Shell(terminal)

- terminfo database
- Xterm terminal
- Konsole terminal
- GNOME terminal

-------------------------------------
### Bash shell command
```sh
1. Shell user ID configuration
    /etc/passwd     :rich:x:501:501:Rich Blum:/home/rich:/home/bash
    data stagement: user name: password: user system ID code: user system group ID code: user default home directory: user default shell application


-c string :Read and deal the command from string
-r
-i
-s
```
-------------------------------------
### File System
```
/:The root of the virtual directory
/bin: Storing lots of GNU user-level utilities
/boot: Boot directory
/dev: Equipment directory 
/etc: System configuration file directory 
/home: Home directory, create user directory in this directory 
/lib: library directory, store system and application library file in here 
/media: Media directory
/mnt: Mount directory
/opt: Store optional package directory
/root: Administrator home directory
/sbin: GNU management-level directory
/tmp: temporary directory
/usr: User install application directory
/var: variable directory
```
-------------------------------------
### Browse the Directory
```sh
$ cd destination
$ cd /usr/lib/apache（*absolute file path）
$ cd ../Desktop (*relative file path)
$ cd ../../etc
$ cd ./
```

### LIST OF FIELS AND DIRECTORIES
```sh
$ ls
```

### CREATE FIEL
```sh
$ touch test1
```

### COPY FILE
```sh
$ cp test1 test2
```

### RENAME FILE
```sh
$ mv test2 test6
```

### DELETE FILE
```sh
$ rm test2
```

### CREATE DIRECTORY
```
$ mkdir dir3
```

### REMOVE DIRECTORY
```sh
$ rmdir dir3
```

### VIEW FILE STATISTICS
```sh
$ stat test10
```

### VIEW FILE TYPE
```shsh
$ file test1
```

### VIEW THE ENTIRE FIEL
```sh
$ cat test1
$ more test1(advantage)
$ less test1(more advantage)
```

### VIEW SOME OF THE FILE
```sh
$ tail 
$ head
```

### VIEW PROCESS
```sh
$ ps
```

### STOP PROCESS
```sh
$ kill PID
$ killall
```

### MOUNT MEDIA
```sh
$ mount
$ unmount
```

### VIEW DISK SPACE
```sh
$ df
```

### VIEW FILE SIZE ON DISK
```sh
$ du
```

### SORT DATA
```sh
$ sort
```

### SEARCH DATA
```sh
$ grep three file1
```

### COMPRESSED DATA
```sh
$ bzip2 myprog
$ gzip myprog
$ zip -r testzip test
```

### ARCHIVE DATA
```sh
$ tar -cvf test.tar test/ test2/
```

### GLOBAL ENVIRONMENT VARIABLES
```sh
$ printenv
```

### ALL ENVIRONMENT VARIABLES
```sh
$ set
```

### SET ENVIRONMENT VARIABLES
```sh
$ test=testing
$ echo $test
```

### SET GLOBAL ENVIRONMENT VARIABLES
```sh
$ echo $test
$ ecport test
```

### REMOVE ENVIRONMENT VARIABLES
```sh
$ echo $test
$ unset test
```

### DEFAULT ENVIRONMENT VARIABLES
```sh
*CDPATH
*HOME
*IFS
*MAIL
*MAILPATH
*OPTARG
*OPTIND
*PTAH
*PS1
*PS2
```

### BASH SHELL ENVIRONMENT VARIABLES

### LOGIN SHELL
```sh
*/etc/profile;
*$HOME/.bash_profile;
*$HOME/.bash_login;
*$HOME/.profile;
```

### VARIABLES GROUP
```sh
$ mytest=(one two three four five)
```




