```bash
$ cc -o loop loop.c
$ ./loop &
[1] 29839
$ sar -P ALL 1 1
Linux 4.15.0-43-generic (150-95-153-54) 	04/08/2019 	_x86_64_	(1 CPU)

12:12:19 AM     CPU     %user     %nice   %system   %iowait    %steal     %idle
12:12:20 AM     all    100.00      0.00      0.00      0.00      0.00      0.00
12:12:20 AM       0    100.00      0.00      0.00      0.00      0.00      0.00

Average:        CPU     %user     %nice   %system   %iowait    %steal     %idle
Average:        all    100.00      0.00      0.00      0.00      0.00      0.00
Average:          0    100.00      0.00      0.00      0.00      0.00      0.00
$ kill 29839
```