# filemap
```bash
$ echo hello > testfile
$ cc -o filemap filemap.c
$ ./filemap
*** memory map before mapping file ***
557440538000-557440539000 r-xp 00000000 08:01 531171                     /home//filemap
557440739000-55744073a000 r--p 00001000 08:01 531171                     /home//filemap
55744073a000-55744073b000 rw-p 00002000 08:01 531171                     /home//filemap
5574417fe000-55744181f000 rw-p 00000000 00:00 0                          [heap]
7f1b15219000-7f1b153ae000 r-xp 00000000 08:01 393319                     /lib/x86_64-linux-gnu/libc-2.24.so
7f1b153ae000-7f1b155ae000 ---p 00195000 08:01 393319                     /lib/x86_64-linux-gnu/libc-2.24.so
7f1b155ae000-7f1b155b2000 r--p 00195000 08:01 393319                     /lib/x86_64-linux-gnu/libc-2.24.so
7f1b155b2000-7f1b155b4000 rw-p 00199000 08:01 393319                     /lib/x86_64-linux-gnu/libc-2.24.so
7f1b155b4000-7f1b155b8000 rw-p 00000000 00:00 0
7f1b155b8000-7f1b155db000 r-xp 00000000 08:01 393315                     /lib/x86_64-linux-gnu/ld-2.24.so
7f1b157d4000-7f1b157d6000 rw-p 00000000 00:00 0
7f1b157db000-7f1b157dc000 r--p 00023000 08:01 393315                     /lib/x86_64-linux-gnu/ld-2.24.so
7f1b157dc000-7f1b157dd000 rw-p 00024000 08:01 393315                     /lib/x86_64-linux-gnu/ld-2.24.so
7f1b157dd000-7f1b157de000 rw-p 00000000 00:00 0
7ffee6173000-7ffee6194000 rw-p 00000000 00:00 0                          [stack]
7ffee61ca000-7ffee61cc000 r--p 00000000 00:00 0                          [vvar]
7ffee61cc000-7ffee61ce000 r-xp 00000000 00:00 0                          [vdso]
ffffffffff600000-ffffffffff601000 r-xp 00000000 00:00 0                  [vsyscall]
*** succeeded to map file: address = 0x7f1b0ee19000; size = 6400000 ***
*** memory map after mapping file ***
557440538000-557440539000 r-xp 00000000 08:01 531171                     /home//filemap
557440739000-55744073a000 r--p 00001000 08:01 531171                     /home//filemap
```