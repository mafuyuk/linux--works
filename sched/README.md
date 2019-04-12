```bash
$ cc -o sched sched.c
$ taskset -c 0 ./sched 1 100 1
```