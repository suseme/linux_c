Linux C function() 参考手册
===

本参考手册在PennyHot网络间PennyHot的版本上稍作格式上的调整，整体保留原有内容。
之所以fork一份，因为前段时间pku托管的哪个site访问不了。


> 各位Linux爱好者：
>
>　　你好！本人有幸在坊间得到一名为"Linux C 函数参考"的文本文件, 并在此基础重新排版并制成html文件以方便广大爱好者阅读, 我感到无比的荣幸。在此多谢各位的鼎力支持, 以及日益完善此文件, 希望有朝一日能成为Linux编程爱好者必备的参考文件。在此再次多谢编写"Linux C 函数参考"的朋友。
>
>　　声明：本人不拥有文章所有权。本人会对本文件文章内排版出现的错误或遗漏内容以及日后提出的相关请求作出最大限度修改, 有问题可e-mail：pennyhot@21cn.com, 别炸我的邮箱:-)
>
> PennyHot　
>2003.06.06



- [字符测试篇](01.md)
  [`isalnum`](01.md#isalnum), [`isalpha`](01.md#isalpha), [`isascii`](01.md#isascii), [`iscntrl`](01.md#iscntrl), [`isdigit`](01.md#isdigit), [`isgraph`](01.md#isgraph), [`islower`](01.md#islower), [`isprint`](01.md#isprint), [`isspace`](01.md#isspace), [`ispunct`](01.md#ispunct), [`isupper`](01.md#isupper), [`isxdigit`](01.md#isxdigit)
- [字符串转换篇](02.md)
  [`atof`](02.md#atof), [`atoi`](02.md#atoi), [`atol`](02.md#atol), [`gcvt`](02.md#gcvt), [`strtod`](02.md#strtod), [`strtol`](02.md#strtol), [`strtoul`](02.md#strtoul), [`toascii`](02.md#toascii), [`tolower`](02.md#tolower), [`toupper`](02.md#toupper)
- [内存控制篇](03.md)
  [`calloc`](03.md#calloc), [`free`](03.md#free), [`getpagesize`](03.md#getpagesize), [`malloc`](03.md#malloc), [`mmap`](03.md#mmap), [`munmap`](03.md#munmap)
- [日期时间篇](04.md)
  [`asctime`](04.md#asctime), [`ctime`](04.md#ctime), [`gettimeofday`](04.md#gettimeofday), [`gmtime`](04.md#gmtime), [`localtime`](04.md#localtime), [`mktime`](04.md#mktime), [`settimeofday`](04.md#settimeofday), [`time`](04.md#time)
- [内存及字符串操作篇](05.md)
  [`bcmp`](05.md#bcmp), [`bcopy`](05.md#bcopy), [`bzero`](05.md#bzero), [`index`](05.md#index), [`memccpy`](05.md#memccpy), [`memchr`](05.md#memchr), [`memcmp`](05.md#memcmp), [`memcpy`](05.md#memcpy), [`memmove`](05.md#memmove), [`memset`](05.md#memset), [`rindex`](05.md#rindex), [`strcasecmp`](05.md#strcasecmp), [`strcat`](05.md#strcat), [`strchr`](05.md#strchr), [`strcmp`](05.md#strcmp), [`strcoll`](05.md#strcoll), [`strcpy`](05.md#strcpy), [`strcspn`](05.md#strcspn), [`strdup`](05.md#strdup), [`strlen`](05.md#strlen), [`strncasecmp`](05.md#strncasecmp), [`strncat`](05.md#strncat), [`strncpy`](05.md#strncpy), [`strpbrk`](05.md#strpbrk), [`strrchr`](05.md#strrchr), [`strspn`](05.md#strspn), [`strstr`](05.md#strstr), [`strtok`](05.md#strtok)
- [常用数学函数篇](06.md)
  [`abs`](06.md#abs), [`acos`](06.md#acos), [`asin`](06.md#asin), [`atan`](06.md#atan), [`atan2`](06.md#atan2), [`ceil`](06.md#ceil), [`cos`](06.md#cos), [`cosh`](06.md#cosh), [`exp`](06.md#exp), [`frexp`](06.md#frexp), [`ldexp`](06.md#ldexp), [`log`](06.md#log), [`log10`](06.md#log10), [`pow`](06.md#pow), [`sin`](06.md#sin), [`sinh`](06.md#sinh), [`sqrt`](06.md#sqrt), [`tan`](06.md#tan), [`tanh`](06.md#tanh)
- [用户组篇](07.md)
  [`endgrent`](07.md#endgrent), [`endpwent`](07.md#endpwent), [`endutent`](07.md#endutent), [`fgetgrent`](07.md#fgetgrent), [`fgetpwent`](07.md#fgetpwent), [`getegid`](07.md#getegid), [`geteuid`](07.md#geteuid), [`getgid`](07.md#getgid), [`getgrent`](07.md#getgrent), [`getgrgid`](07.md#getgrgid), [`getgrnam`](07.md#getgrnam), [`getgroups`](07.md#getgroups), [`getpw`](07.md#getpw), [`getpwent`](07.md#getpwent), [`getpwnam`](07.md#getpwnam), [`getpwuid`](07.md#getpwuid), [`getuid`](07.md#getuid), [`getutent`](07.md#getutent), [`getutid`](07.md#getutid), [`getutline`](07.md#getutline), [`initgroups`](07.md#initgroups), [`pututline`](07.md#pututline), [`seteuid`](07.md#seteuid), [`setfsgid`](07.md#setfsgid), [`setfsuid`](07.md#setfsuid), [`setgid`](07.md#setgid), [`setgrent`](07.md#setgrent), [`setgroups`](07.md#setgroups), [`setpwent`](07.md#setpwent), [`setregid`](07.md#setregid), [`setreuid`](07.md#setreuid), [`setuid`](07.md#setuid), [`setutent`](07.md#setutent), [`utmpname`](07.md#utmpname)
- [数据结构及算法篇](08.md)
  [`crypt`](08.md#crypt), [`bsearch`](08.md#bsearch), [`lfind`](08.md#lfind), [`lsearch`](08.md#lsearch), [`qsort`](08.md#qsort), [`rand`](08.md#rand), [`srand`](08.md#srand)
- [文件操作篇](09.md)
  [`close`](09.md#close), [`creat`](09.md#creat), [`dup`](09.md#dup), [`dup2`](09.md#dup2), [`fcntl`](09.md#fcntl), [`flock`](09.md#flock), [`fsync`](09.md#fsync), [`lseek`](09.md#lseek), [`mkstemp`](09.md#mkstemp), [`open`](09.md#open), [`read`](09.md#read), [`sync`](09.md#sync), [`write`](09.md#write)
- [文件内容操作篇](10.md)
  [`clearerr`](10.md#clearerr), [`fclose`](10.md#fclose), [`fdopen`](10.md#fdopen), [`feof`](10.md#feof), [`fflush`](10.md#fflush), [`fgetc`](10.md#fgetc), [`fgets`](10.md#fgets), [`fileno`](10.md#fileno), [`fputc`](10.md#fputc), [`fread`](10.md#fread), [`freopen`](10.md#freopen), [`fseek`](10.md#fseek), [`ftell`](10.md#ftell), [`fwrite`](10.md#fwrite), [`getc`](10.md#getc), [`getchar`](10.md#getchar), [`gets`](10.md#gets), [`mktemp`](10.md#mktemp), [`putc`](10.md#putc), [`putchar`](10.md#putchar), [`rewind`](10.md#rewind), [`setbuf`](10.md#setbuf), [`setbuffer`](10.md#setbuffer), [`setlinebuf`](10.md#setlinebuf), [`setvbuf`](10.md#setvbuf), [`ungetc`](10.md#ungetc)
- [进程操作篇](11.md)
  [`atexit`](11.md#atexit), [`execl`](11.md#execl), [`execlp`](11.md#execlp), [`execv`](11.md#execv), [`execve`](11.md#execve), [`execvp`](11.md#execvp), [`exit`](11.md#exit), [`_exit`](11.md#_exit), [`vfork`](11.md#vfork), [`getpgid`](11.md#getpgid), [`getpgrp`](11.md#getpgrp), [`getpid`](11.md#getpid), [`getppid`](11.md#getppid), [`getpriority`](11.md#getpriority), [`nice`](11.md#nice), [`on_exit`](11.md#on_exit), [`setpgid`](11.md#setpgid), [`setpgrp`](11.md#setpgrp), [`setpriority`](11.md#setpriority), [`system`](11.md#system), [`wait`](11.md#wait), [`waitpid`](11.md#waitpid), [`fprintf`](11.md#fprintf), [`fscanf`](11.md#fscanf), [`printf`](11.md#printf), [`sacnf`](11.md#sacnf), [`sprintf`](11.md#sprintf), [`sscanf`](11.md#sscanf), [`vfprintf`](11.md#vfprintf), [`vfscanf`](11.md#vfscanf), [`vprintf`](11.md#vprintf), [`vscanf`](11.md#vscanf), [`vsprintf`](11.md#vsprintf), [`vsscanf`](11.md#vsscanf)
- [文件权限控制篇](12.md)
  [`access`](12.md#access), [`alphasort`](12.md#alphasort), [`chdir`](12.md#chdir), [`chmod`](12.md#chmod), [`chown`](12.md#chown), [`chroot`](12.md#chroot), [`closedir`](12.md#closedir), [`fchdir`](12.md#fchdir), [`fchmod`](12.md#fchmod), [`fchown`](12.md#fchown), [`fstat`](12.md#fstat), [`ftruncate`](12.md#ftruncate), [`getcwd`](12.md#getcwd), [`link`](12.md#link), [`lstat`](12.md#lstat), [`opendir`](12.md#opendir), [`readdir`](12.md#readdir), [`readlink`](12.md#readlink), [`remove`](12.md#remove), [`rename`](12.md#rename), [`rewinddir`](12.md#rewinddir), [`seekdir`](12.md#seekdir), [`stat`](12.md#stat), [`symlink`](12.md#symlink), [`telldir`](12.md#telldir), [`truncate`](12.md#truncate), [`umask`](12.md#umask), [`unlink`](12.md#unlink), [`utime`](12.md#utime), [`utimes`](12.md#utimes)
- [信号处理篇](13.md)
  [`alarm`](13.md#alarm), [`kill`](13.md#kill), [`pause`](13.md#pause), [`sigaction`](13.md#sigaction), [`sigaddset`](13.md#sigaddset), [`sigdelset`](13.md#sigdelset), [`sigemptyset`](13.md#sigemptyset), [`sigfillset`](13.md#sigfillset), [`sigismember`](13.md#sigismember), [`signal`](13.md#signal), [`sigpending`](13.md#sigpending), [`sigprocmask`](13.md#sigprocmask), [`sleep`](13.md#sleep), [`ferror`](13.md#ferror), [`perror`](13.md#perror), [`strerror`](13.md#strerror), [`mkfifo`](13.md#mkfifo), [`pclose`](13.md#pclose), [`pipe`](13.md#pipe), [`popen`](13.md#popen)
- [接口处理篇](14.md)
  [`accept`](14.md#accept), [`bind`](14.md#bind), [`connect`](14.md#connect), [`endprotoent`](14.md#endprotoent), [`endservent`](14.md#endservent), [`getsockopt`](14.md#getsockopt), [`htonl`](14.md#htonl), [`htons`](14.md#htons), [`inet_addr`](14.md#inet_addr), [`inet_aton`](14.md#inet_aton), [`inet_ntoa`](14.md#inet_ntoa), [`listen`](14.md#listen), [`ntohl`](14.md#ntohl), [`ntohs`](14.md#ntohs), [`recv`](14.md#recv), [`recvfrom`](14.md#recvfrom), [`recvmsg`](14.md#recvmsg), [`send`](14.md#send), [`sendmsg`](14.md#sendmsg), [`sendto`](14.md#sendto), [`setprotoent`](14.md#setprotoent), [`setservent`](14.md#setservent), [`setsockopt`](14.md#setsockopt), [`shutdown`](14.md#shutdown), [`socket`](14.md#socket)
- [环境变量篇](15.md)
  [`getenv`](15.md#getenv), [`putenv`](15.md#putenv), [`setenv`](15.md#setenv)
- [终端控制篇](16.md)
  [`getopt`](16.md#getopt), [`isatty`](16.md#isatty), [`select`](16.md#select), [`ttyname`](16.md#ttyname)