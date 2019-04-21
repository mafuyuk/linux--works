# mmap
```bash
$ cc -o mmap mmap.c
55dff9605000-55dff9606000 r-xp 00000000 08:01 531161                     /home//mmap
55dff9805000-55dff9806000 r--p 00000000 08:01 531161                     /home//mmap
55dff9806000-55dff9807000 rw-p 00001000 08:01 531161                     /home//mmap
55dffad21000-55dffad42000 rw-p 00000000 00:00 0                          [heap]
7fe65dcf4000-7fe65de89000 r-xp 00000000 08:01 393319                     /lib/x86_64-linux-gnu/libc-2.24.so
7fe65de89000-7fe65e089000 ---p 00195000 08:01 393319                     /lib/x86_64-linux-gnu/libc-2.24.so
7fe65e089000-7fe65e08d000 r--p 00195000 08:01 393319                     /lib/x86_64-linux-gnu/libc-2.24.so
7fe65e08d000-7fe65e08f000 rw-p 00199000 08:01 393319                     /lib/x86_64-linux-gnu/libc-2.24.so
7fe65e08f000-7fe65e093000 rw-p 00000000 00:00 0
7fe65e093000-7fe65e0b6000 r-xp 00000000 08:01 393315                     /lib/x86_64-linux-gnu/ld-2.24.so
7fe65e2af000-7fe65e2b1000 rw-p 00000000 00:00 0
7fe65e2b6000-7fe65e2b7000 r--p 00023000 08:01 393315                     /lib/x86_64-linux-gnu/ld-2.24.so
7fe65e2b7000-7fe65e2b8000 rw-p 00024000 08:01 393315                     /lib/x86_64-linux-gnu/ld-2.24.so
7fe65e2b8000-7fe65e2b9000 rw-p 00000000 00:00 0
7ffd105a5000-7ffd105c6000 rw-p 00000000 00:00 0                          [stack]
7ffd105d9000-7ffd105db000 r--p 00000000 00:00 0                          [vvar]
7ffd105db000-7ffd105dd000 r-xp 00000000 00:00 0                          [vdso]
ffffffffff600000-ffffffffff601000 r-xp 00000000 00:00 0                  [vsyscall]
*** succeeded to allocate  memory: address = 0x7fe6578f4000; size = 0x6400000 ***
*** memory map after memory allocation ***
55dff9605000-55dff9606000 r-xp 00000000 08:01 531161                     /home//mmap
55dff9805000-55dff9806000 r--p 00000000 08:01 531161                     /home//mmap
55dff9806000-55dff9807000 rw-p 00001000 08:01 531161                     /home//mmap
55dffad21000-55dffad42000 rw-p 00000000 00:00 0                          [heap]
7fe6578f4000-7fe65dcf4000 rw-p 00000000 00:00 0
7fe65dcf4000-7fe65de89000 r-xp 00000000 08:01 393319                     /lib/x86_64-linux-gnu/libc-2.24.so
7fe65de89000-7fe65e089000 ---p 00195000 08:01 393319                     /lib/x86_64-linux-gnu/libc-2.24.so
7fe65e089000-7fe65e08d000 r--p 00195000 08:01 393319                     /lib/x86_64-linux-gnu/libc-2.24.so
7fe65e08d000-7fe65e08f000 rw-p 00199000 08:01 393319                     /lib/x86_64-linux-gnu/libc-2.24.so
7fe65e08f000-7fe65e093000 rw-p 00000000 00:00 0
7fe65e093000-7fe65e0b6000 r-xp 00000000 08:01 393315                     /lib/x86_64-linux-gnu/ld-2.24.so
7fe65e2af000-7fe65e2b1000 rw-p 00000000 00:00 0
7fe65e2b6000-7fe65e2b7000 r--p 00023000 08:01 393315                     /lib/x86_64-linux-gnu/ld-2.24.so
7fe65e2b7000-7fe65e2b8000 rw-p 00024000 08:01 393315                     /lib/x86_64-linux-gnu/ld-2.24.so
7fe65e2b8000-7fe65e2b9000 rw-p 00000000 00:00 0
7ffd105a5000-7ffd105c6000 rw-p 00000000 00:00 0                          [stack]
7ffd105d9000-7ffd105db000 r--p 00000000 00:00 0                          [vvar]
7ffd105db000-7ffd105dd000 r-xp 00000000 00:00 0                          [vdso]
ffffffffff600000-ffffffffff601000 r-xp 00000000 00:00 0                  [vsyscall]

$ python -c "print(0x7fe65dcf4000 - 0x7fe6578f4000)"
104857600
```