Day 25 drill:Build a one-screen operational snapshot of a server covering uptime, memory,
the status of three key services, and any scheduled cron jobs.

Step 1 — Uptime and load

uptime

Step 2 — Memory

free -h

Step 3 — Status of three key services

systemctl status ssh
systemctl status cron
systemctl status NetworkManager

Step 4 — Scheduled jobs

crontab -l