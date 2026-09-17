Day 24 drill: List every failed service on the box, then pull today's logs for one specific service, filtered to errors
only, and follow it live for one minute.

Step 1 — List every failed service

systemctl list-units --state=failed

Step 2 — Pull today's logs for one specific service

journalctl -u ssh --since today

Step 3 — Filter those same logs to errors only

journalctl -u ssh --since today -p err

Step 4 — Follow it live for one minute

journalctl -u ssh -f

