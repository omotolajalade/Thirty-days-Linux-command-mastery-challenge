Day 23 drill:Pick a service, stop it, confirm it is inactive, restart it, enable it to auto-start at boot in a single
combined command, and confirm both its active and enabled state.

Step 1 — Pick a service and check its current state

systemctl status ssh

Step 2 — Stop it

sudo systemctl stop ssh

Step 3 — Confirm it's inactive

systemctl is-active ssh

Step 4 — Restart it

sudo systemctl restart ssh

Step 5 — Enable it to auto-start at boot, starting it now too, in one combined command

sudo systemctl enable --now ssh

Step 6 — Confirm both active and enabled states

systemctl is-active ssh
systemctl is-enabled ssh