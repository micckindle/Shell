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
Usage: ls [OPTION]... [FILE]...
List information about the FILEs (the current directory by default).
Sort entries alphabetically if none of -cftuvSUX nor --sort is specified.

Mandatory arguments to long options are mandatory for short options too.
  -a, --all                  do not ignore entries starting with .
  -A, --almost-all           do not list implied . and ..
      --author               with -l, print the author of each file
  -b, --escape               print C-style escapes for nongraphic characters
      --block-size=SIZE      scale sizes by SIZE before printing them; e.g.,
                               '--block-size=M' prints sizes in units of
                               1,048,576 bytes; see SIZE format below
  -B, --ignore-backups       do not list implied entries ending with ~
  -c                         with -lt: sort by, and show, ctime (time of last
                               modification of file status information);
                               with -l: show ctime and sort by name;
                               otherwise: sort by ctime, newest first
  -C                         list entries by columns
      --color[=WHEN]         colorize the output; WHEN can be 'always' (default
                               if omitted), 'auto', or 'never'; more info below
  -d, --directory            list directories themselves, not their contents
  -D, --dired                generate output designed for Emacs' dired mode
  -f                         do not sort, enable -aU, disable -ls --color
  -F, --classify             append indicator (one of */=>@|) to entries
      --file-type            likewise, except do not append '*'
      --format=WORD          across -x, commas -m, horizontal -x, long -l,
                               single-column -1, verbose -l, vertical -C
      --full-time            like -l --time-style=full-iso
  -g                         like -l, but do not list owner
      --group-directories-first
                             group directories before files;
                               can be augmented with a --sort option, but any
                               use of --sort=none (-U) disables grouping
  -G, --no-group             in a long listing, don't print group names
  -h, --human-readable       with -l and/or -s, print human readable sizes
                               (e.g., 1K 234M 2G)
      --si                   likewise, but use powers of 1000 not 1024
  -H, --dereference-command-line
                             follow symbolic links listed on the command line
      --dereference-command-line-symlink-to-dir
                             follow each command line symbolic link
                               that points to a directory
      --hide=PATTERN         do not list implied entries matching shell PATTERN
                               (overridden by -a or -A)
      --indicator-style=WORD  append indicator with style WORD to entry names:
                               none (default), slash (-p),
                               file-type (--file-type), classify (-F)
  -i, --inode                print the index number of each file
  -I, --ignore=PATTERN       do not list implied entries matching shell PATTERN
  -k, --kibibytes            default to 1024-byte blocks for disk usage
  -l                         use a long listing format
  -L, --dereference          when showing file information for a symbolic
                               link, show information for the file the link
                               references rather than for the link itself
  -m                         fill width with a comma separated list of entries
  -n, --numeric-uid-gid      like -l, but list numeric user and group IDs
  -N, --literal              print raw entry names (don't treat e.g. control
                               characters specially)
  -o                         like -l, but do not list group information
  -p, --indicator-style=slash
                             append / indicator to directories
  -q, --hide-control-chars   print ? instead of nongraphic characters
      --show-control-chars   show nongraphic characters as-is (the default,
                               unless program is 'ls' and output is a terminal)
  -Q, --quote-name           enclose entry names in double quotes
      --quoting-style=WORD   use quoting style WORD for entry names:
                               literal, locale, shell, shell-always,
                               shell-escape, shell-escape-always, c, escape
  -r, --reverse              reverse order while sorting
  -R, --recursive            list subdirectories recursively
  -s, --size                 print the allocated size of each file, in blocks
  -S                         sort by file size, largest first
      --sort=WORD            sort by WORD instead of name: none (-U), size (-S),
                               time (-t), version (-v), extension (-X)
      --time=WORD            with -l, show time as WORD instead of default
                               modification time: atime or access or use (-u);
                               ctime or status (-c); also use specified time
                               as sort key if --sort=time (newest first)
      --time-style=STYLE     with -l, show times using style STYLE:
                               full-iso, long-iso, iso, locale, or +FORMAT;
                               FORMAT is interpreted like in 'date'; if FORMAT
                               is FORMAT1<newline>FORMAT2, then FORMAT1 applies
                               to non-recent files and FORMAT2 to recent files;
                               if STYLE is prefixed with 'posix-', STYLE
                               takes effect only outside the POSIX locale
  -t                         sort by modification time, newest first
  -T, --tabsize=COLS         assume tab stops at each COLS instead of 8
  -u                         with -lt: sort by, and show, access time;
                               with -l: show access time and sort by name;
                               otherwise: sort by access time, newest first
  -U                         do not sort; list entries in directory order
  -v                         natural sort of (version) numbers within text
  -w, --width=COLS           set output width to COLS.  0 means no limit
  -x                         list entries by lines instead of by columns
  -X                         sort alphabetically by entry extension
  -Z, --context              print any security context of each file
  -1                         list one file per line.  Avoid '\n' with -q or -b
      --append-exe           append .exe if cygwin magic was needed
      --help     display this help and exit
      --version  output version information and exit

The SIZE argument is an integer and optional unit (example: 10K is 10*1024).
Units are K,M,G,T,P,E,Z,Y (powers of 1024) or KB,MB,... (powers of 1000).

Using color to distinguish file types is disabled both by default and
with --color=never.  With --color=auto, ls emits color codes only when
standard output is connected to a terminal.  The LS_COLORS environment
variable can change the settings.  Use the dircolors command to set it.

Exit status:
 0  if OK,
 1  if minor problems (e.g., cannot access subdirectory),
 2  if serious trouble (e.g., cannot access command-line argument).

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
Report ls translation bugs to <http://translationproject.org/team/>
Full documentation at: <http://www.gnu.org/software/coreutils/ls>
or available locally via: info '(coreutils) ls invocation'

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




