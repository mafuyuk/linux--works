```bash
$ cc -o sched sched.c
$ taskset -c 0 ./sched 1 100 1
# 論理CPUの数を出す
$ grep -c processor /proc/cpuinfo
2
$ taskset -c 0,1 ./sched 2 200 1
```