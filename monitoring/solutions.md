# Solutions – System Monitoring

### Exercise 1 – top sorted by memory
$ top -o %MEM
# The top processes by memory usage are displayed. Below is a sample output:
PID USER      %MEM COMMAND
413 root      3.8  /usr/lib/snapd/snapd
162 root      2.7  /sbin/multipathd
...

✔ Screenshot captured showing top 5 processes using the most memory.

---

### Exercise 2 – Find and kill dummy process
$ ps aux | grep sleep
ubuntu   1347  0.0  0.1  6192 1920 pts/0  S 17:26  0:00 sleep 1000
ubuntu   1349  0.0  0.2  7008 2304 pts/0  S+ 17:26  0:00 grep --color=auto sleep

$ kill -9 1347

$ ps aux | grep sleep
ubuntu   1351  0.0  0.2  7008 2304 pts/0  S+ 17:26  0:00 grep --color=auto sleep

✔ The dummy process is successfully terminated.

---

### Exercise 3 – Check disk space
$ df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/root      7.6G  1.8G  5.9G  24% /
...

✔ Screenshot captured showing disk usage.

$ df -i
Filesystem     Inodes IUsed IFree IUse% Mounted on
/dev/root    1032192 75680 956512    8% /
...

✔ Screenshot captured showing inode usage.

---

### Exercise 4 – Check memory usage
$ free -h
              total   used   free   shared  buff/cache  available
Mem:           957M   202M   227M    0.0K    527M     597M
Swap:            0B     0B      0B

✔ Screenshot captured showing memory usage.

---

### Exercise 5 – Show system uptime
$ uptime
 17:15:23 up 35 min, 1 user, load average: 0.00, 0.00, 0.00

✔ Screenshot/log shows system uptime and load averages.
