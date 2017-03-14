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
```
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
```
$ touch test1
Usage: touch [OPTION]... FILE...
Update the access and modification times of each FILE to the current time.

A FILE argument that does not exist is created empty, unless -c or -h
is supplied.

A FILE argument string of - is handled specially and causes touch to
change the times of the file associated with standard output.

Mandatory arguments to long options are mandatory for short options too.
  -a                     change only the access time
  -c, --no-create        do not create any files
  -d, --date=STRING      parse STRING and use it instead of current time
  -f                     (ignored)
  -h, --no-dereference   affect each symbolic link instead of any referenced
                         file (useful only on systems that can change the
                         timestamps of a symlink)
  -m                     change only the modification time
  -r, --reference=FILE   use this file's times instead of current time
  -t STAMP               use [[CC]YY]MMDDhhmm[.ss] instead of current time
      --time=WORD        change the specified time:
                           WORD is access, atime, or use: equivalent to -a
                           WORD is modify or mtime: equivalent to -m
      --help     display this help and exit
      --version  output version information and exit

Note that the -d and -t options accept different time-date formats.

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
Report touch translation bugs to <http://translationproject.org/team/>
Full documentation at: <http://www.gnu.org/software/coreutils/touch>
or available locally via: info '(coreutils) touch invocation'

```

### COPY FILE
```
$ cp test1 test2
Usage: cp [OPTION]... [-T] SOURCE DEST
  or:  cp [OPTION]... SOURCE... DIRECTORY
  or:  cp [OPTION]... -t DIRECTORY SOURCE...
Copy SOURCE to DEST, or multiple SOURCE(s) to DIRECTORY.

Mandatory arguments to long options are mandatory for short options too.
  -a, --archive                same as -dR --preserve=all
      --attributes-only        don't copy the file data, just the attributes
      --backup[=CONTROL]       make a backup of each existing destination file
  -b                           like --backup but does not accept an argument
      --copy-contents          copy contents of special files when recursive
  -d                           same as --no-dereference --preserve=links
  -f, --force                  if an existing destination file cannot be
                                 opened, remove it and try again (this option
                                 is ignored when the -n option is also used)
  -i, --interactive            prompt before overwrite (overrides a previous -n
                                  option)
  -H                           follow command-line symbolic links in SOURCE
  -l, --link                   hard link files instead of copying
  -L, --dereference            always follow symbolic links in SOURCE
  -n, --no-clobber             do not overwrite an existing file (overrides
                                 a previous -i option)
  -P, --no-dereference         never follow symbolic links in SOURCE
  -p                           same as --preserve=mode,ownership,timestamps
      --preserve[=ATTR_LIST]   preserve the specified attributes (default:
                                 mode,ownership,timestamps), if possible
                                 additional attributes: context, links, xattr,
                                 all
      --no-preserve=ATTR_LIST  don't preserve the specified attributes
      --parents                use full source file name under DIRECTORY
  -R, -r, --recursive          copy directories recursively
      --reflink[=WHEN]         control clone/CoW copies. See below
      --remove-destination     remove each existing destination file before
                                 attempting to open it (contrast with --force)
      --sparse=WHEN            control creation of sparse files. See below
      --strip-trailing-slashes  remove any trailing slashes from each SOURCE
                                 argument
  -s, --symbolic-link          make symbolic links instead of copying
  -S, --suffix=SUFFIX          override the usual backup suffix
  -t, --target-directory=DIRECTORY  copy all SOURCE arguments into DIRECTORY
  -T, --no-target-directory    treat DEST as a normal file
  -u, --update                 copy only when the SOURCE file is newer
                                 than the destination file or when the
                                 destination file is missing
  -v, --verbose                explain what is being done
  -x, --one-file-system        stay on this file system
  -Z                           set SELinux security context of destination
                                 file to default type
      --context[=CTX]          like -Z, or if CTX is specified then set the
                                 SELinux or SMACK security context to CTX
      --help     display this help and exit
      --version  output version information and exit

By default, sparse SOURCE files are detected by a crude heuristic and the
corresponding DEST file is made sparse as well.  That is the behavior
selected by --sparse=auto.  Specify --sparse=always to create a sparse DEST
file whenever the SOURCE file contains a long enough sequence of zero bytes.
Use --sparse=never to inhibit creation of sparse files.

When --reflink[=always] is specified, perform a lightweight copy, where the
data blocks are copied only when modified.  If this is not possible the copy
fails, or if --reflink=auto is specified, fall back to a standard copy.

The backup suffix is '~', unless set with --suffix or SIMPLE_BACKUP_SUFFIX.
The version control method may be selected via the --backup option or through
the VERSION_CONTROL environment variable.  Here are the values:

  none, off       never make backups (even if --backup is given)
  numbered, t     make numbered backups
  existing, nil   numbered if numbered backups exist, simple otherwise
  simple, never   always make simple backups

As a special case, cp makes a backup of SOURCE when the force and backup
options are given and SOURCE and DEST are the same name for an existing,
regular file.

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
Report cp translation bugs to <http://translationproject.org/team/>
Full documentation at: <http://www.gnu.org/software/coreutils/cp>
or available locally via: info '(coreutils) cp invocation'

```

### RENAME FILE
```
$ mv test2 test6
Usage: mv [OPTION]... [-T] SOURCE DEST
  or:  mv [OPTION]... SOURCE... DIRECTORY
  or:  mv [OPTION]... -t DIRECTORY SOURCE...
Rename SOURCE to DEST, or move SOURCE(s) to DIRECTORY.

Mandatory arguments to long options are mandatory for short options too.
      --backup[=CONTROL]       make a backup of each existing destination file
  -b                           like --backup but does not accept an argument
  -f, --force                  do not prompt before overwriting
  -i, --interactive            prompt before overwrite
  -n, --no-clobber             do not overwrite an existing file
If you specify more than one of -i, -f, -n, only the final one takes effect.
      --strip-trailing-slashes  remove any trailing slashes from each SOURCE
                                 argument
  -S, --suffix=SUFFIX          override the usual backup suffix
  -t, --target-directory=DIRECTORY  move all SOURCE arguments into DIRECTORY
  -T, --no-target-directory    treat DEST as a normal file
  -u, --update                 move only when the SOURCE file is newer
                                 than the destination file or when the
                                 destination file is missing
  -v, --verbose                explain what is being done
  -Z, --context                set SELinux security context of destination
                                 file to default type
      --help     display this help and exit
      --version  output version information and exit

The backup suffix is '~', unless set with --suffix or SIMPLE_BACKUP_SUFFIX.
The version control method may be selected via the --backup option or through
the VERSION_CONTROL environment variable.  Here are the values:

  none, off       never make backups (even if --backup is given)
  numbered, t     make numbered backups
  existing, nil   numbered if numbered backups exist, simple otherwise
  simple, never   always make simple backups

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
Report mv translation bugs to <http://translationproject.org/team/>
Full documentation at: <http://www.gnu.org/software/coreutils/mv>
or available locally via: info '(coreutils) mv invocation'

```

### DELETE FILE
```
$ rm test2
Usage: rm [OPTION]... [FILE]...
Remove (unlink) the FILE(s).

  -f, --force           ignore nonexistent files and arguments, never prompt
  -i                    prompt before every removal
  -I                    prompt once before removing more than three files, or
                          when removing recursively; less intrusive than -i,
                          while still giving protection against most mistakes
      --interactive[=WHEN]  prompt according to WHEN: never, once (-I), or
                          always (-i); without WHEN, prompt always
      --one-file-system  when removing a hierarchy recursively, skip any
                          directory that is on a file system different from
                          that of the corresponding command line argument
      --no-preserve-root  do not treat '/' specially
      --preserve-root   do not remove '/' (default)
  -r, -R, --recursive   remove directories and their contents recursively
  -d, --dir             remove empty directories
  -v, --verbose         explain what is being done
      --help     display this help and exit
      --version  output version information and exit

By default, rm does not remove directories.  Use the --recursive (-r or -R)
option to remove each listed directory, too, along with all of its contents.

To remove a file whose name starts with a '-', for example '-foo',
use one of these commands:
  rm -- -foo

  rm ./-foo

Note that if you use rm to remove a file, it might be possible to recover
some of its contents, given sufficient expertise and/or time.  For greater
assurance that the contents are truly unrecoverable, consider using shred.

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
Report rm translation bugs to <http://translationproject.org/team/>
Full documentation at: <http://www.gnu.org/software/coreutils/rm>
or available locally via: info '(coreutils) rm invocation'

```

### CREATE DIRECTORY
```
$ mkdir dir3
Usage: mkdir [OPTION]... DIRECTORY...
Create the DIRECTORY(ies), if they do not already exist.

Mandatory arguments to long options are mandatory for short options too.
  -m, --mode=MODE   set file mode (as in chmod), not a=rwx - umask
  -p, --parents     no error if existing, make parent directories as needed
  -v, --verbose     print a message for each created directory
  -Z                   set SELinux security context of each created directory
                         to the default type
      --context[=CTX]  like -Z, or if CTX is specified then set the SELinux
                         or SMACK security context to CTX
      --help     display this help and exit
      --version  output version information and exit

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
Report mkdir translation bugs to <http://translationproject.org/team/>
Full documentation at: <http://www.gnu.org/software/coreutils/mkdir>
or available locally via: info '(coreutils) mkdir invocation'

```

### REMOVE DIRECTORY
```
$ rmdir dir3
Usage: rmdir [OPTION]... DIRECTORY...
Remove the DIRECTORY(ies), if they are empty.

      --ignore-fail-on-non-empty
                  ignore each failure that is solely because a directory
                    is non-empty
  -p, --parents   remove DIRECTORY and its ancestors; e.g., 'rmdir -p a/b/c' is
                    similar to 'rmdir a/b/c a/b a'
  -v, --verbose   output a diagnostic for every directory processed
      --help     display this help and exit
      --version  output version information and exit

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
Report rmdir translation bugs to <http://translationproject.org/team/>
Full documentation at: <http://www.gnu.org/software/coreutils/rmdir>
or available locally via: info '(coreutils) rmdir invocation'

```

### VIEW FILE STATISTICS
```
$ stat test10
Usage: stat [OPTION]... FILE...
Display file or file system status.

Mandatory arguments to long options are mandatory for short options too.
  -L, --dereference     follow links
  -f, --file-system     display file system status instead of file status
  -c  --format=FORMAT   use the specified FORMAT instead of the default;
                          output a newline after each use of FORMAT
      --printf=FORMAT   like --format, but interpret backslash escapes,
                          and do not output a mandatory trailing newline;
                          if you want a newline, include \n in FORMAT
  -t, --terse           print the information in terse form
      --append-exe      append .exe if cygwin magic was needed
      --help     display this help and exit
      --version  output version information and exit

The valid format sequences for files (without --file-system):

  %a   access rights in octal (note '#' and '0' printf flags)
  %A   access rights in human readable form
  %b   number of blocks allocated (see %B)
  %B   the size in bytes of each block reported by %b
  %C   SELinux security context string
  %d   device number in decimal
  %D   device number in hex
  %f   raw mode in hex
  %F   file type
  %g   group ID of owner
  %G   group name of owner
  %h   number of hard links
  %i   inode number
  %m   mount point
  %n   file name
  %N   quoted file name with dereference if symbolic link
  %o   optimal I/O transfer size hint
  %s   total size, in bytes
  %t   major device type in hex, for character/block device special files
  %T   minor device type in hex, for character/block device special files
  %u   user ID of owner
  %U   user name of owner
  %w   time of file birth, human-readable; - if unknown
  %W   time of file birth, seconds since Epoch; 0 if unknown
  %x   time of last access, human-readable
  %X   time of last access, seconds since Epoch
  %y   time of last data modification, human-readable
  %Y   time of last data modification, seconds since Epoch
  %z   time of last status change, human-readable
  %Z   time of last status change, seconds since Epoch

Valid format sequences for file systems:

  %a   free blocks available to non-superuser
  %b   total data blocks in file system
  %c   total file nodes in file system
  %d   free file nodes in file system
  %f   free blocks in file system
  %i   file system ID in hex
  %l   maximum length of filenames
  %n   file name
  %s   block size (for faster transfers)
  %S   fundamental block size (for block counts)
  %t   file system type in hex
  %T   file system type in human readable form

NOTE: your shell may have its own version of stat, which usually supersedes
the version described here.  Please refer to your shell's documentation
for details about the options it supports.

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
Report stat translation bugs to <http://translationproject.org/team/>
Full documentation at: <http://www.gnu.org/software/coreutils/stat>
or available locally via: info '(coreutils) stat invocation'

```

### VIEW FILE TYPE
```
$ file test1
Usage: file [OPTION...] [FILE...]
Determine type of FILEs.

      --help                 display this help and exit
  -v, --version              output version information and exit
  -m, --magic-file LIST      use LIST as a colon-separated list of magic
                               number files
  -z, --uncompress           try to look inside compressed files
  -Z, --uncompress-noreport  only print the contents of compressed files
  -b, --brief                do not prepend filenames to output lines
  -c, --checking-printout    print the parsed form of the magic file, use in
                               conjunction with -m to debug a new magic file
                               before installing it
  -e, --exclude TEST         exclude TEST from the list of test to be
                               performed for file. Valid tests are:
                               apptype, ascii, cdf, compress, elf, encoding,
                               soft, tar, text, tokens
  -f, --files-from FILE      read the filenames to be examined from FILE
  -F, --separator STRING     use string as separator instead of `:'
  -i, --mime                 output MIME type strings (--mime-type and
                               --mime-encoding)
      --apple                output the Apple CREATOR/TYPE
      --extension            output a slash-separated list of extensions
      --mime-type            output the MIME type
      --mime-encoding        output the MIME encoding
  -k, --keep-going           don't stop at the first match
  -l, --list                 list magic strength
  -L, --dereference          follow symlinks
  -h, --no-dereference       don't follow symlinks (default)
  -n, --no-buffer            do not buffer output
  -N, --no-pad               do not pad output
  -0, --print0               terminate filenames with ASCII NUL
  -p, --preserve-date        preserve access times on files
  -P, --parameter            set file engine parameter limits
                               indir        15 recursion limit for indirection
                               name         30 use limit for name/use magic
                               elf_notes   256 max ELF notes processed
                               elf_phnum   128 max ELF prog sections processed
                               elf_shnum 32768 max ELF sections processed
  -r, --raw                  don't translate unprintable chars to \ooo
  -s, --special-files        treat special (block/char devices) files as
                             ordinary ones
  -C, --compile              compile file specified by -m
  -d, --debug                print debugging messages

Report bugs to http://bugs.gw.com/

```

### VIEW THE ENTIRE FIEL
```
$ cat test1
Usage: cat [OPTION]... [FILE]...
Concatenate FILE(s) to standard output.

With no FILE, or when FILE is -, read standard input.

  -A, --show-all           equivalent to -vET
  -b, --number-nonblank    number nonempty output lines, overrides -n
  -e                       equivalent to -vE
  -E, --show-ends          display $ at end of each line
  -n, --number             number all output lines
  -s, --squeeze-blank      suppress repeated empty output lines
  -t                       equivalent to -vT
  -T, --show-tabs          display TAB characters as ^I
  -u                       (ignored)
  -v, --show-nonprinting   use ^ and M- notation, except for LFD and TAB
      --help     display this help and exit
      --version  output version information and exit

Examples:
  cat f - g  Output f's contents, then standard input, then g's contents.
  cat        Copy standard input to standard output.

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
Report cat translation bugs to <http://translationproject.org/team/>
Full documentation at: <http://www.gnu.org/software/coreutils/cat>
or available locally via: info '(coreutils) cat invocation'

$ more test1(advantage)
$ less test1(more advantage)
```

### VIEW SOME OF THE FILE
```
$ tail 
Usage: tail [OPTION]... [FILE]...
Print the last 10 lines of each FILE to standard output.
With more than one FILE, precede each with a header giving the file name.

With no FILE, or when FILE is -, read standard input.

Mandatory arguments to long options are mandatory for short options too.
  -c, --bytes=[+]NUM       output the last NUM bytes; or use -c +NUM to
                             output starting with byte NUM of each file
  -f, --follow[={name|descriptor}]
                           output appended data as the file grows;
                             an absent option argument means 'descriptor'
  -F                       same as --follow=name --retry
  -n, --lines=[+]NUM       output the last NUM lines, instead of the last 10;
                             or use -n +NUM to output starting with line NUM
      --max-unchanged-stats=N
                           with --follow=name, reopen a FILE which has not
                             changed size after N (default 5) iterations
                             to see if it has been unlinked or renamed
                             (this is the usual case of rotated log files);
                             with inotify, this option is rarely useful
      --pid=PID            with -f, terminate after process ID, PID dies
  -q, --quiet, --silent    never output headers giving file names
      --retry              keep trying to open a file if it is inaccessible
  -s, --sleep-interval=N   with -f, sleep for approximately N seconds
                             (default 1.0) between iterations;
                             with inotify and --pid=P, check process P at
                             least once every N seconds
  -v, --verbose            always output headers giving file names
  -z, --zero-terminated    line delimiter is NUL, not newline
      --help     display this help and exit
      --version  output version information and exit

NUM may have a multiplier suffix:
b 512, kB 1000, K 1024, MB 1000*1000, M 1024*1024,
GB 1000*1000*1000, G 1024*1024*1024, and so on for T, P, E, Z, Y.

With --follow (-f), tail defaults to following the file descriptor, which
means that even if a tail'ed file is renamed, tail will continue to track
its end.  This default behavior is not desirable when you really want to
track the actual name of the file, not the file descriptor (e.g., log
rotation).  Use --follow=name in that case.  That causes tail to track the
named file in a way that accommodates renaming, removal and creation.

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
Report tail translation bugs to <http://translationproject.org/team/>
Full documentation at: <http://www.gnu.org/software/coreutils/tail>
or available locally via: info '(coreutils) tail invocation'

$ head
Usage: head [OPTION]... [FILE]...
Print the first 10 lines of each FILE to standard output.
With more than one FILE, precede each with a header giving the file name.

With no FILE, or when FILE is -, read standard input.

Mandatory arguments to long options are mandatory for short options too.
  -c, --bytes=[-]NUM       print the first NUM bytes of each file;
                             with the leading '-', print all but the last
                             NUM bytes of each file
  -n, --lines=[-]NUM       print the first NUM lines instead of the first 10;
                             with the leading '-', print all but the last
                             NUM lines of each file
  -q, --quiet, --silent    never print headers giving file names
  -v, --verbose            always print headers giving file names
  -z, --zero-terminated    line delimiter is NUL, not newline
      --help     display this help and exit
      --version  output version information and exit

NUM may have a multiplier suffix:
b 512, kB 1000, K 1024, MB 1000*1000, M 1024*1024,
GB 1000*1000*1000, G 1024*1024*1024, and so on for T, P, E, Z, Y.

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
Report head translation bugs to <http://translationproject.org/team/>
Full documentation at: <http://www.gnu.org/software/coreutils/head>
or available locally via: info '(coreutils) head invocation'

```

### VIEW PROCESS
```
$ ps
Usage: ps [-aefls] [-u UID] [-p PID]

Report process status

 -a, --all       show processes of all users
 -e, --everyone  show processes of all users
 -f, --full      show process uids, ppids
 -h, --help      output usage information and exit
 -l, --long      show process uids, ppids, pgids, winpids
 -p, --process   show information for specified PID
 -s, --summary   show process summary
 -u, --user      list processes owned by UID
 -V, --version   output version information and exit
 -W, --windows   show windows as well as cygwin processes

With no options, ps outputs the long format by default

```

### STOP PROCESS
```
$ kill PID
$ killall
```

### MOUNT MEDIA
```
$ mount
Usage: mount [OPTION] [<win32path> <posixpath>]
       mount -a
       mount <posixpath>

Display information about mounted filesystems, or mount a filesystem

  -a, --all                     mount all filesystems mentioned in fstab
  -c, --change-cygdrive-prefix  change the cygdrive path prefix to <posixpath>
  -f, --force                   force mount, don't warn about missing mount
                                point directories
  -h, --help                    output usage information and exit
  -m, --mount-entries           write fstab entries to replicate mount points
                                and cygdrive prefixes
  -o, --options X[,X...]        specify mount options
  -p, --show-cygdrive-prefix    show user and/or system cygdrive path prefix
  -V, --version                 output version information and exit

Valid options are: acl,auto,binary,bind,cygexec,dos,exec,ihash,noacl,nosuid,notexec,nouser,override,posix=0,posix=1,sparse,text,user

$ unmount
```

### VIEW DISK SPACE
```
$ df
Usage: df [OPTION]... [FILE]...
Show information about the file system on which each FILE resides,
or all file systems by default.

Mandatory arguments to long options are mandatory for short options too.
  -a, --all             include pseudo, duplicate, inaccessible file systems
  -B, --block-size=SIZE  scale sizes by SIZE before printing them; e.g.,
                           '-BM' prints sizes in units of 1,048,576 bytes;
                           see SIZE format below
  -h, --human-readable  print sizes in powers of 1024 (e.g., 1023M)
  -H, --si              print sizes in powers of 1000 (e.g., 1.1G)
  -i, --inodes          list inode information instead of block usage
  -k                    like --block-size=1K
  -l, --local           limit listing to local file systems
      --no-sync         do not invoke sync before getting usage info (default)
      --output[=FIELD_LIST]  use the output format defined by FIELD_LIST,
                               or print all fields if FIELD_LIST is omitted.
  -P, --portability     use the POSIX output format
      --sync            invoke sync before getting usage info
      --total           elide all entries insignificant to available space,
                          and produce a grand total
  -t, --type=TYPE       limit listing to file systems of type TYPE
  -T, --print-type      print file system type
  -x, --exclude-type=TYPE   limit listing to file systems not of type TYPE
  -v                    (ignored)
      --help     display this help and exit
      --version  output version information and exit

Display values are in units of the first available SIZE from --block-size,
and the DF_BLOCK_SIZE, BLOCK_SIZE and BLOCKSIZE environment variables.
Otherwise, units default to 1024 bytes (or 512 if POSIXLY_CORRECT is set).

The SIZE argument is an integer and optional unit (example: 10K is 10*1024).
Units are K,M,G,T,P,E,Z,Y (powers of 1024) or KB,MB,... (powers of 1000).

FIELD_LIST is a comma-separated list of columns to be included.  Valid
field names are: 'source', 'fstype', 'itotal', 'iused', 'iavail', 'ipcent',
'size', 'used', 'avail', 'pcent', 'file' and 'target' (see info page).

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
Report df translation bugs to <http://translationproject.org/team/>
Full documentation at: <http://www.gnu.org/software/coreutils/df>
or available locally via: info '(coreutils) df invocation'

```

### VIEW FILE SIZE ON DISK
```
$ du
Usage: du [OPTION]... [FILE]...
  or:  du [OPTION]... --files0-from=F
Summarize disk usage of the set of FILEs, recursively for directories.

Mandatory arguments to long options are mandatory for short options too.
  -0, --null            end each output line with NUL, not newline
  -a, --all             write counts for all files, not just directories
      --apparent-size   print apparent sizes, rather than disk usage; although
                          the apparent size is usually smaller, it may be
                          larger due to holes in ('sparse') files, internal
                          fragmentation, indirect blocks, and the like
  -B, --block-size=SIZE  scale sizes by SIZE before printing them; e.g.,
                           '-BM' prints sizes in units of 1,048,576 bytes;
                           see SIZE format below
  -b, --bytes           equivalent to '--apparent-size --block-size=1'
  -c, --total           produce a grand total
  -D, --dereference-args  dereference only symlinks that are listed on the
                          command line
  -d, --max-depth=N     print the total for a directory (or file, with --all)
                          only if it is N or fewer levels below the command
                          line argument;  --max-depth=0 is the same as
                          --summarize
      --files0-from=F   summarize disk usage of the
                          NUL-terminated file names specified in file F;
                          if F is -, then read names from standard input
  -H                    equivalent to --dereference-args (-D)
  -h, --human-readable  print sizes in human readable format (e.g., 1K 234M 2G)
      --inodes          list inode usage information instead of block usage
  -k                    like --block-size=1K
  -L, --dereference     dereference all symbolic links
  -l, --count-links     count sizes many times if hard linked
  -m                    like --block-size=1M
  -P, --no-dereference  don't follow any symbolic links (this is the default)
  -S, --separate-dirs   for directories do not include size of subdirectories
      --si              like -h, but use powers of 1000 not 1024
  -s, --summarize       display only a total for each argument
  -t, --threshold=SIZE  exclude entries smaller than SIZE if positive,
                          or entries greater than SIZE if negative
      --time            show time of the last modification of any file in the
                          directory, or any of its subdirectories
      --time=WORD       show time as WORD instead of modification time:
                          atime, access, use, ctime or status
      --time-style=STYLE  show times using STYLE, which can be:
                            full-iso, long-iso, iso, or +FORMAT;
                            FORMAT is interpreted like in 'date'
  -X, --exclude-from=FILE  exclude files that match any pattern in FILE
      --exclude=PATTERN    exclude files that match PATTERN
  -x, --one-file-system    skip directories on different file systems
      --help     display this help and exit
      --version  output version information and exit

Display values are in units of the first available SIZE from --block-size,
and the DU_BLOCK_SIZE, BLOCK_SIZE and BLOCKSIZE environment variables.
Otherwise, units default to 1024 bytes (or 512 if POSIXLY_CORRECT is set).

The SIZE argument is an integer and optional unit (example: 10K is 10*1024).
Units are K,M,G,T,P,E,Z,Y (powers of 1024) or KB,MB,... (powers of 1000).

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
Report du translation bugs to <http://translationproject.org/team/>
Full documentation at: <http://www.gnu.org/software/coreutils/du>
or available locally via: info '(coreutils) du invocation'

```

### SORT DATA
```
$ sort
Usage: sort [OPTION]... [FILE]...
  or:  sort [OPTION]... --files0-from=F
Write sorted concatenation of all FILE(s) to standard output.

With no FILE, or when FILE is -, read standard input.

Mandatory arguments to long options are mandatory for short options too.
Ordering options:

  -b, --ignore-leading-blanks  ignore leading blanks
  -d, --dictionary-order      consider only blanks and alphanumeric characters
  -f, --ignore-case           fold lower case to upper case characters
  -g, --general-numeric-sort  compare according to general numerical value
  -i, --ignore-nonprinting    consider only printable characters
  -M, --month-sort            compare (unknown) < 'JAN' < ... < 'DEC'
  -h, --human-numeric-sort    compare human readable numbers (e.g., 2K 1G)
  -n, --numeric-sort          compare according to string numerical value
  -R, --random-sort           shuffle, but group identical keys.  See shuf(1)
      --random-source=FILE    get random bytes from FILE
  -r, --reverse               reverse the result of comparisons
      --sort=WORD             sort according to WORD:
                                general-numeric -g, human-numeric -h, month -M,
                                numeric -n, random -R, version -V
  -V, --version-sort          natural sort of (version) numbers within text

Other options:

      --batch-size=NMERGE   merge at most NMERGE inputs at once;
                            for more use temp files
  -c, --check, --check=diagnose-first  check for sorted input; do not sort
  -C, --check=quiet, --check=silent  like -c, but do not report first bad line
      --compress-program=PROG  compress temporaries with PROG;
                              decompress them with PROG -d
      --debug               annotate the part of the line used to sort,
                              and warn about questionable usage to stderr
      --files0-from=F       read input from the files specified by
                            NUL-terminated names in file F;
                            If F is - then read names from standard input
  -k, --key=KEYDEF          sort via a key; KEYDEF gives location and type
  -m, --merge               merge already sorted files; do not sort
  -o, --output=FILE         write result to FILE instead of standard output
  -s, --stable              stabilize sort by disabling last-resort comparison
  -S, --buffer-size=SIZE    use SIZE for main memory buffer
  -t, --field-separator=SEP  use SEP instead of non-blank to blank transition
  -T, --temporary-directory=DIR  use DIR for temporaries, not $TMPDIR or /tmp;
                              multiple options specify multiple directories
      --parallel=N          change the number of sorts run concurrently to N
  -u, --unique              with -c, check for strict ordering;
                              without -c, output only the first of an equal run
  -z, --zero-terminated     line delimiter is NUL, not newline
      --help     display this help and exit
      --version  output version information and exit

KEYDEF is F[.C][OPTS][,F[.C][OPTS]] for start and stop position, where F is a
field number and C a character position in the field; both are origin 1, and
the stop position defaults to the line's end.  If neither -t nor -b is in
effect, characters in a field are counted from the beginning of the preceding
whitespace.  OPTS is one or more single-letter ordering options [bdfgiMhnRrV],
which override global ordering options for that key.  If no key is given, use
the entire line as the key.  Use --debug to diagnose incorrect key usage.

SIZE may be followed by the following multiplicative suffixes:
% 1% of memory, b 1, K 1024 (default), and so on for M, G, T, P, E, Z, Y.

*** WARNING ***
The locale specified by the environment affects sort order.
Set LC_ALL=C to get the traditional sort order that uses
native byte values.

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
Report sort translation bugs to <http://translationproject.org/team/>
Full documentation at: <http://www.gnu.org/software/coreutils/sort>
or available locally via: info '(coreutils) sort invocation'

```

### SEARCH DATA
```
$ grep three file1
Usage: grep [OPTION]... PATTERN [FILE]...
Search for PATTERN in each FILE or standard input.
PATTERN is, by default, a basic regular expression (BRE).
Example: grep -i 'hello world' menu.h main.c

Regexp selection and interpretation:
  -E, --extended-regexp     PATTERN is an extended regular expression (ERE)
  -F, --fixed-strings       PATTERN is a set of newline-separated strings
  -G, --basic-regexp        PATTERN is a basic regular expression (BRE)
  -P, --perl-regexp         PATTERN is a Perl regular expression
  -e, --regexp=PATTERN      use PATTERN for matching
  -f, --file=FILE           obtain PATTERN from FILE
  -i, --ignore-case         ignore case distinctions
  -w, --word-regexp         force PATTERN to match only whole words
  -x, --line-regexp         force PATTERN to match only whole lines
  -z, --null-data           a data line ends in 0 byte, not newline

Miscellaneous:
  -s, --no-messages         suppress error messages
  -v, --invert-match        select non-matching lines
  -V, --version             display version information and exit
      --help                display this help text and exit

Output control:
  -m, --max-count=NUM       stop after NUM matches
  -b, --byte-offset         print the byte offset with output lines
  -n, --line-number         print line number with output lines
      --line-buffered       flush output on every line
  -H, --with-filename       print the file name for each match
  -h, --no-filename         suppress the file name prefix on output
      --label=LABEL         use LABEL as the standard input file name prefix
  -o, --only-matching       show only the part of a line matching PATTERN
  -q, --quiet, --silent     suppress all normal output
      --binary-files=TYPE   assume that binary files are TYPE;
                            TYPE is 'binary', 'text', or 'without-match'
  -a, --text                equivalent to --binary-files=text
  -I                        equivalent to --binary-files=without-match
  -d, --directories=ACTION  how to handle directories;
                            ACTION is 'read', 'recurse', or 'skip'
  -D, --devices=ACTION      how to handle devices, FIFOs and sockets;
                            ACTION is 'read' or 'skip'
  -r, --recursive           like --directories=recurse
  -R, --dereference-recursive  likewise, but follow all symlinks
      --include=FILE_PATTERN  search only files that match FILE_PATTERN
      --exclude=FILE_PATTERN  skip files and directories matching FILE_PATTERN
      --exclude-from=FILE   skip files matching any file pattern from FILE
      --exclude-dir=PATTERN  directories that match PATTERN will be skipped.
  -L, --files-without-match  print only names of FILEs containing no match
  -l, --files-with-matches  print only names of FILEs containing matches
  -c, --count               print only a count of matching lines per FILE
  -T, --initial-tab         make tabs line up (if needed)
  -Z, --null                print 0 byte after FILE name

Context control:
  -B, --before-context=NUM  print NUM lines of leading context
  -A, --after-context=NUM   print NUM lines of trailing context
  -C, --context=NUM         print NUM lines of output context
  -NUM                      same as --context=NUM
      --color[=WHEN],
      --colour[=WHEN]       use markers to highlight the matching strings;
                            WHEN is 'always', 'never', or 'auto'
  -U, --binary              do not strip CR characters at EOL (MSDOS/Windows)
  -u, --unix-byte-offsets   report offsets as if CRs were not there
                            (MSDOS/Windows)

'egrep' means 'grep -E'.  'fgrep' means 'grep -F'.
Direct invocation as either 'egrep' or 'fgrep' is deprecated.
When FILE is -, read standard input.  With no FILE, read . if a command-line
-r is given, - otherwise.  If fewer than two FILEs are given, assume -h.
Exit status is 0 if any line is selected, 1 otherwise;
if any error occurs and -q is not given, the exit status is 2.

Report bugs to: bug-grep@gnu.org
GNU grep home page: <http://www.gnu.org/software/grep/>
General help using GNU software: <http://www.gnu.org/gethelp/>

```

### COMPRESSED DATA
```
$ bzip2 myprog
bzip2, a block-sorting file compressor.  Version 1.0.6, 6-Sept-2010.

   usage: bzip2.exe [flags and input files in any order]

   -h --help           print this message
   -d --decompress     force decompression
   -z --compress       force compression
   -k --keep           keep (don't delete) input files
   -f --force          overwrite existing output files
   -t --test           test compressed file integrity
   -c --stdout         output to standard out
   -q --quiet          suppress noncritical error messages
   -v --verbose        be verbose (a 2nd -v gives more)
   -L --license        display software version & license
   -V --version        display software version & license
   -s --small          use less memory (at most 2500k)
   -1 .. -9            set block size to 100k .. 900k
   --fast              alias for -1
   --best              alias for -9

   If invoked as `bzip2', default action is to compress.
              as `bunzip2',  default action is to decompress.
              as `bzcat', default action is to decompress to stdout.

   If no file names are given, bzip2 compresses or decompresses
   from standard input to standard output.  You can combine
   short flags, so `-v -4' means the same as -v4 or -4v, &c.

$ gzip myprog
Usage: gzip [OPTION]... [FILE]...
Compress or uncompress FILEs (by default, compress FILES in-place).

Mandatory arguments to long options are mandatory for short options too.

  -a, --ascii       ascii text; convert end-of-line using local conventions
  -c, --stdout      write on standard output, keep original files unchanged
  -d, --decompress  decompress
  -f, --force       force overwrite of output file and compress links
  -h, --help        give this help
  -k, --keep        keep (don't delete) input files
  -l, --list        list compressed file contents
  -L, --license     display software license
  -n, --no-name     do not save or restore the original name and time stamp
  -N, --name        save or restore the original name and time stamp
  -q, --quiet       suppress all warnings
  -r, --recursive   operate recursively on directories
      --rsyncable   make rsync-friendly archive
  -S, --suffix=SUF  use suffix SUF on compressed files
      --synchronous synchronous output (safer if system crashes, but slower)
  -t, --test        test compressed file integrity
  -v, --verbose     verbose mode
  -V, --version     display version number
  -1, --fast        compress faster
  -9, --best        compress better

With no FILE, or when FILE is -, read standard input.

Report bugs to <bug-gzip@gnu.org>.

$ zip -r testzip test

```

### ARCHIVE DATA
```
$ tar -cvf test.tar test/ test2/
Usage: tar [OPTION...] [FILE]...
GNU 'tar' saves many files together into a single tape or disk archive, and can
restore individual files from the archive.

Examples:
  tar -cf archive.tar foo bar  # Create archive.tar from files foo and bar.
  tar -tvf archive.tar         # List all files in archive.tar verbosely.
  tar -xf archive.tar          # Extract all files from archive.tar.

 Local file name selection:

      --add-file=FILE        add given FILE to the archive (useful if its name
                             starts with a dash)
  -C, --directory=DIR        change to directory DIR
      --exclude=PATTERN      exclude files, given as a PATTERN
      --exclude-backups      exclude backup and lock files
      --exclude-caches       exclude contents of directories containing
                             CACHEDIR.TAG, except for the tag file itself
      --exclude-caches-all   exclude directories containing CACHEDIR.TAG
      --exclude-caches-under exclude everything under directories containing
                             CACHEDIR.TAG
      --exclude-ignore=FILE  read exclude patterns for each directory from
                             FILE, if it exists
      --exclude-ignore-recursive=FILE
                             read exclude patterns for each directory and its
                             subdirectories from FILE, if it exists
      --exclude-tag=FILE     exclude contents of directories containing FILE,
                             except for FILE itself
      --exclude-tag-all=FILE exclude directories containing FILE
      --exclude-tag-under=FILE   exclude everything under directories
                             containing FILE
      --exclude-vcs          exclude version control system directories
      --exclude-vcs-ignores  read exclude patterns from the VCS ignore files
      --no-null              disable the effect of the previous --null option
      --no-recursion         avoid descending automatically in directories
      --no-unquote           do not unquote input file or member names
      --no-verbatim-files-from   -T treats file names starting with dash as
                             options (default)
      --null                 -T reads null-terminated names; implies
                             --verbatim-files-from
      --recursion            recurse into directories (default)
  -T, --files-from=FILE      get names to extract or create from FILE
      --unquote              unquote input file or member names (default)
      --verbatim-files-from  -T reads file names verbatim (no option handling)
  -X, --exclude-from=FILE    exclude patterns listed in FILE

 File name matching options (affect both exclude and include patterns):

      --anchored             patterns match file name start
      --ignore-case          ignore case
      --no-anchored          patterns match after any '/' (default for
                             exclusion)
      --no-ignore-case       case sensitive matching (default)
      --no-wildcards         verbatim string matching
      --no-wildcards-match-slash   wildcards do not match '/'
      --wildcards            use wildcards (default for exclusion)
      --wildcards-match-slash   wildcards match '/' (default for exclusion)

 Main operation mode:

  -A, --catenate, --concatenate   append tar files to an archive
  -c, --create               create a new archive
  -d, --diff, --compare      find differences between archive and file system
      --delete               delete from the archive (not on mag tapes!)
  -r, --append               append files to the end of an archive
  -t, --list                 list the contents of an archive
      --test-label           test the archive volume label and exit
  -u, --update               only append files newer than copy in archive
  -x, --extract, --get       extract files from an archive

 Operation modifiers:

      --check-device         check device numbers when creating incremental
                             archives (default)
  -g, --listed-incremental=FILE   handle new GNU-format incremental backup
  -G, --incremental          handle old GNU-format incremental backup
      --hole-detection=TYPE  technique to detect holes
      --ignore-failed-read   do not exit with nonzero on unreadable files
      --level=NUMBER         dump level for created listed-incremental archive
  -n, --seek                 archive is seekable
      --no-check-device      do not check device numbers when creating
                             incremental archives
      --no-seek              archive is not seekable
      --occurrence[=NUMBER]  process only the NUMBERth occurrence of each file
                             in the archive; this option is valid only in
                             conjunction with one of the subcommands --delete,
                             --diff, --extract or --list and when a list of
                             files is given either on the command line or via
                             the -T option; NUMBER defaults to 1
      --sparse-version=MAJOR[.MINOR]
                             set version of the sparse format to use (implies
                             --sparse)
  -S, --sparse               handle sparse files efficiently

 Overwrite control:

  -k, --keep-old-files       don't replace existing files when extracting,
                             treat them as errors
      --keep-directory-symlink   preserve existing symlinks to directories when
                             extracting
      --keep-newer-files     don't replace existing files that are newer than
                             their archive copies
      --no-overwrite-dir     preserve metadata of existing directories
      --one-top-level[=DIR]  create a subdirectory to avoid having loose files
                             extracted
      --overwrite            overwrite existing files when extracting
      --overwrite-dir        overwrite metadata of existing directories when
                             extracting (default)
      --recursive-unlink     empty hierarchies prior to extracting directory
      --remove-files         remove files after adding them to the archive
      --skip-old-files       don't replace existing files when extracting,
                             silently skip over them
  -U, --unlink-first         remove each file prior to extracting over it
  -W, --verify               attempt to verify the archive after writing it

 Select output stream:

      --ignore-command-error ignore exit codes of children
      --no-ignore-command-error   treat non-zero exit codes of children as
                             error
  -O, --to-stdout            extract files to standard output
      --to-command=COMMAND   pipe extracted files to another program

 Handling of file attributes:

      --atime-preserve[=METHOD]   preserve access times on dumped files, either
                             by restoring the times after reading
                             (METHOD='replace'; default) or by not setting the
                             times in the first place (METHOD='system')
      --clamp-mtime          only set time when the file is more recent than
                             what was given with --mtime
      --delay-directory-restore   delay setting modification times and
                             permissions of extracted directories until the end
                             of extraction
      --group=NAME           force NAME as group for added files
      --group-map=FILE       use FILE to map file owner GIDs and names
      --mode=CHANGES         force (symbolic) mode CHANGES for added files
      --mtime=DATE-OR-FILE   set mtime for added files from DATE-OR-FILE
  -m, --touch                don't extract file modified time
      --no-delay-directory-restore
                             cancel the effect of --delay-directory-restore
                             option
      --no-same-owner        extract files as yourself (default for ordinary
                             users)
      --no-same-permissions  apply the user's umask when extracting permissions
                             from the archive (default for ordinary users)
      --numeric-owner        always use numbers for user/group names
      --owner=NAME           force NAME as owner for added files
      --owner-map=FILE       use FILE to map file owner UIDs and names
  -p, --preserve-permissions, --same-permissions
                             extract information about file permissions
                             (default for superuser)
      --same-owner           try extracting files with the same ownership as
                             exists in the archive (default for superuser)
  -s, --preserve-order, --same-order
                             member arguments are listed in the same order as
                             the files in the archive
      --sort=ORDER           directory sorting order: none (default), name or
                             inode

 Handling of extended file attributes:

      --acls                 Enable the POSIX ACLs support
      --no-acls              Disable the POSIX ACLs support
      --no-selinux           Disable the SELinux context support
      --no-xattrs            Disable extended attributes support
      --selinux              Enable the SELinux context support
      --xattrs               Enable extended attributes support
      --xattrs-exclude=MASK  specify the exclude pattern for xattr keys
      --xattrs-include=MASK  specify the include pattern for xattr keys

 Device selection and switching:

  -f, --file=ARCHIVE         use archive file or device ARCHIVE
      --force-local          archive file is local even if it has a colon
  -F, --info-script=NAME, --new-volume-script=NAME
                             run script at end of each tape (implies -M)
  -L, --tape-length=NUMBER   change tape after writing NUMBER x 1024 bytes
  -M, --multi-volume         create/list/extract multi-volume archive
      --rmt-command=COMMAND  use given rmt COMMAND instead of rmt
      --rsh-command=COMMAND  use remote COMMAND instead of rsh
      --volno-file=FILE      use/update the volume number in FILE

 Device blocking:

  -b, --blocking-factor=BLOCKS   BLOCKS x 512 bytes per record
  -B, --read-full-records    reblock as we read (for 4.2BSD pipes)
  -i, --ignore-zeros         ignore zeroed blocks in archive (means EOF)
      --record-size=NUMBER   NUMBER of bytes per record, multiple of 512

 Archive format selection:

  -H, --format=FORMAT        create archive of the given format

 FORMAT is one of the following:

    gnu                      GNU tar 1.13.x format
    oldgnu                   GNU format as per tar <= 1.12
    pax                      POSIX 1003.1-2001 (pax) format
    posix                    same as pax
    ustar                    POSIX 1003.1-1988 (ustar) format
    v7                       old V7 tar format

      --old-archive, --portability
                             same as --format=v7
      --pax-option=keyword[[:]=value][,keyword[[:]=value]]...
                             control pax keywords
      --posix                same as --format=posix
  -V, --label=TEXT           create archive with volume name TEXT; at
                             list/extract time, use TEXT as a globbing pattern
                             for volume name

 Compression options:

  -a, --auto-compress        use archive suffix to determine the compression
                             program
  -I, --use-compress-program=PROG
                             filter through PROG (must accept -d)
  -j, --bzip2                filter the archive through bzip2
  -J, --xz                   filter the archive through xz
      --lzip                 filter the archive through lzip
      --lzma                 filter the archive through lzma
      --lzop                 filter the archive through xz
      --no-auto-compress     do not use archive suffix to determine the
                             compression program
  -z, --gzip, --gunzip, --ungzip   filter the archive through gzip
  -Z, --compress, --uncompress   filter the archive through compress

 Local file selection:

      --backup[=CONTROL]     backup before removal, choose version CONTROL
  -h, --dereference          follow symlinks; archive and dump the files they
                             point to
      --hard-dereference     follow hard links; archive and dump the files they
                             refer to
  -K, --starting-file=MEMBER-NAME
                             begin at member MEMBER-NAME when reading the
                             archive
      --newer-mtime=DATE     compare date and time when data changed only
  -N, --newer=DATE-OR-FILE, --after-date=DATE-OR-FILE
                             only store files newer than DATE-OR-FILE
      --one-file-system      stay in local file system when creating archive
  -P, --absolute-names       don't strip leading '/'s from file names
      --suffix=STRING        backup before removal, override usual suffix ('~'
                             unless overridden by environment variable
                             SIMPLE_BACKUP_SUFFIX)

 File name transformations:

      --strip-components=NUMBER   strip NUMBER leading components from file
                             names on extraction
      --transform=EXPRESSION, --xform=EXPRESSION
                             use sed replace EXPRESSION to transform file
                             names

 Informative output:

      --checkpoint[=NUMBER]  display progress messages every NUMBERth record
                             (default 10)
      --checkpoint-action=ACTION   execute ACTION on each checkpoint
      --full-time            print file time to its full resolution
      --index-file=FILE      send verbose output to FILE
  -l, --check-links          print a message if not all links are dumped
      --no-quote-chars=STRING   disable quoting for characters from STRING
      --quote-chars=STRING   additionally quote characters from STRING
      --quoting-style=STYLE  set name quoting style; see below for valid STYLE
                             values
  -R, --block-number         show block number within archive with each message

      --show-defaults        show tar defaults
      --show-omitted-dirs    when listing or extracting, list each directory
                             that does not match search criteria
      --show-snapshot-field-ranges
                             show valid ranges for snapshot-file fields
      --show-transformed-names, --show-stored-names
                             show file or archive names after transformation
      --totals[=SIGNAL]      print total bytes after processing the archive;
                             with an argument - print total bytes when this
                             SIGNAL is delivered; Allowed signals are: SIGHUP,
                             SIGQUIT, SIGINT, SIGUSR1 and SIGUSR2; the names
                             without SIG prefix are also accepted
      --utc                  print file modification times in UTC
  -v, --verbose              verbosely list files processed
      --warning=KEYWORD      warning control
  -w, --interactive, --confirmation
                             ask for confirmation for every action

 Compatibility options:

  -o                         when creating, same as --old-archive; when
                             extracting, same as --no-same-owner

 Other options:

  -?, --help                 give this help list
      --restrict             disable use of some potentially harmful options
      --usage                give a short usage message
      --version              print program version

Mandatory or optional arguments to long options are also mandatory or optional
for any corresponding short options.

The backup suffix is '~', unless set with --suffix or SIMPLE_BACKUP_SUFFIX.
The version control may be set with --backup or VERSION_CONTROL, values are:

  none, off       never make backups
  t, numbered     make numbered backups
  nil, existing   numbered if numbered backups exist, simple otherwise
  never, simple   always make simple backups

Valid arguments for the --quoting-style option are:

  literal
  shell
  shell-always
  c
  c-maybe
  escape
  locale
  clocale

*This* tar defaults to:
--format=gnu -f- -b20 --quoting-style=escape
--rmt-command=/usr/lib/tar/rmt.exe

```

### GLOBAL ENVIRONMENT VARIABLES
```
$ printenv
Usage: printenv [OPTION]... [VARIABLE]...
Print the values of the specified environment VARIABLE(s).
If no VARIABLE is specified, print name and value pairs for them all.

  -0, --null     end each output line with NUL, not newline
      --help     display this help and exit
      --version  output version information and exit

NOTE: your shell may have its own version of printenv, which usually supersedes
the version described here.  Please refer to your shell's documentation
for details about the options it supports.

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
Report printenv translation bugs to <http://translationproject.org/team/>
Full documentation at: <http://www.gnu.org/software/coreutils/printenv>
or available locally via: info '(coreutils) printenv invocation'

```

### ALL ENVIRONMENT VARIABLES
```
$ set
bash: set: --: invalid option
set: usage: set [-abefhkmnptuvxBCHP] [-o option-name] [--] [arg ...]

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




