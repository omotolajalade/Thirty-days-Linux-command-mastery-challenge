Commands and what they do

1. systemctl list-units --type=service: list all services

Shows every currently loaded service and its state.

2. systemctl list-units --state=failed: list only failed services

Instantly surfaces anything broken, without scanning the full list manually.

3. systemctl daemon-reload: reload systemd's own configuration

Needed after manually editing a service's config file, so systemd notices the change.

4. journalctl: view the full system log

The centralized log system reads from every service's output funnels here.

5. journalctl -f: follow the log live

What each character means -f = follow — like a live feed, showing new entries as they happen. Press Ctrl+C to stop.

6. journalctl -u: logs for one specific service or unit.

7. journalctl --since: filter logs by time

8. journalctl -p err: filter logs by priority level

What each character means  -p = priority, err = error-level and above only

9. tail -f /var/log/syslog: it follows a traditional log file live

An older-style equivalent to journalctl -f, for systems/logs still using plain text files.

10. tail -f /var/log/auth.log : it follows authentication events live

Shows real-time login attempts, sudo usage, and authentication events, directly connects to your Day 10 audit work.