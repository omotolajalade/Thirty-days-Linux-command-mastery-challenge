Commands and what they do

1. ps aux | grep: search running processes.

2. systemctl status:check detailed current state

Shows whether it's active/inactive, enabled/disabled, recent log lines, and the process ID, your main diagnostic tool.

3. journalctl -u: logs for one specific service

4. kill -0: a liveness check without actually killing anything

What each character means  -0 sends no real signal at all, it only checks whether the process exists and you have permission to signal it, returning success or failure silently.

5. uptime: how long the system has been running, plus load average

6. free -h: memory usage in human-readable form

What each command means -h = human-readable (shows GB/MB instead of raw bytes)
7. vmstat: virtual memory and system activity statistics

Snapshot of memory, CPU, and I/O activity in one compact table.

8. iostat: disk input/output statistics

9. watch: repeat a command automatically at intervals

What each character means free -h every 2 seconds, turning any one-off command into a live-updating view.

10. crontab -e / crontab -l: scheduled recurring tasks

What each character means  -e = edit your scheduled jobs, -l = list them