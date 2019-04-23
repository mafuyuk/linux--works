# filemap
```bash
$ cc -o filemap filemap.c
$ ./filemap
*** memory map before mapping file ***
55b84c166000-55b84c167000 r-xp 00000000 08:01 531171                     /home//filemap
55b84c367000-55b84c368000 r--p 00001000 08:01 531171                     /home//filemap
55b84c368000-55b84c369000 rw-p 00002000 08:01 531171                     /home//filemap
55b84d9ad000-55b84d9ce000 rw-p 00000000 00:00 0                          [heap]
7f2587f64000-7f25880f9000 r-xp 00000000 08:01 393319                     /lib/x86_64-linux-gnu/libc-2.24.so
7f25880f9000-7f25882f9000 ---p 00195000 08:01 393319                     /lib/x86_64-linux-gnu/libc-2.24.so
7f25882f9000-7f25882fd000 r--p 00195000 08:01 393319                     /lib/x86_64-linux-gnu/libc-2.24.so
7f25882fd000-7f25882ff000 rw-p 00199000 08:01 393319                     /lib/x86_64-linux-gnu/libc-2.24.so
7f25882ff000-7f2588303000 rw-p 00000000 00:00 0
7f2588303000-7f2588326000 r-xp 00000000 08:01 393315                     /lib/x86_64-linux-gnu/ld-2.24.so
7f258851f000-7f2588521000 rw-p 00000000 00:00 0
7f2588526000-7f2588527000 r--p 00023000 08:01 393315                     /lib/x86_64-linux-gnu/ld-2.24.so
7f2588527000-7f2588528000 rw-p 00024000 08:01 393315                     /lib/x86_64-linux-gnu/ld-2.24.so
7f2588528000-7f2588529000 rw-p 00000000 00:00 0
7ffdd85d2000-7ffdd85f3000 rw-p 00000000 00:00 0                          [stack]
7ffdd85fb000-7ffdd85fd000 r--p 00000000 00:00 0                          [vvar]
7ffdd85fd000-7ffdd85ff000 r-xp 00000000 00:00 0                          [vdso]
ffffffffff600000-ffffffffff601000 r-xp 00000000 00:00 0                  [vsyscall]
filemap: open() failed: No such file or directory
```