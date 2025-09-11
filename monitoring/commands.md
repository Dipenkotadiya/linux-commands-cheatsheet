# Monitoring Commands

## df – Show disk space usage
df -h
# Shows the disk usage in human-readable format (sizes in GB/MB).

df -i
# Displays inode usage and availability for each mounted filesystem.

## free – Show memory usage
free -h
# Displays memory usage in human-readable format (total, used, available memory).

## top – Display real-time processes
top
# Shows all running processes, CPU and memory usage in real-time.

top -o %MEM
# Sorts the processes by memory usage, showing the highest at the top.

## ps – List running processes
ps aux
# Shows all running processes with user, CPU %, memory %, and more.

ps aux | grep sleep
# Searches for processes related to 'sleep'.

## kill – Terminate processes
kill -9 <PID>
# Forcefully kills the process with the specified Process ID.

## uptime – Show system load
uptime
# Displays how long the system has been running and the load averages.

## htop (optional, if installed)
htop
# Interactive process viewer with easy sorting and filtering.
