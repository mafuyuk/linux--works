# sched
```bash
$ cc -o sched sched.c
$ taskset -c 0 ./sched 1 100 1
# 論理CPUの数を出す
$ grep -c processor /proc/cpuinfo
2
$ taskset -c 0,1 ./sched 2 200 1
```

# sched_nice
```bash
$ cc -o sched_nice sched_nice.c
$ taskset -c 0 ./sched_nice 100 1

```