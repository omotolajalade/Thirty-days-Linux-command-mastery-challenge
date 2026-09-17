Commands and what they do

1. systemctl start: start a service now

2. systemctl stop: stop a service now

3. systemctl restart: stop then start a service

Useful after changing a service's configuration, many services need a restart to pick up changes.

4. systemctl reload: reload config without a full restart

Gentler than restart, it tells the service to reread its config while continuing to run, avoiding any brief downtime a full restart causes.

5. systemctl enable: make a service start automatically at boot

 Important distinction: enable does NOT start the service now, it only sets it to start on the next reboot.

6. systemctl disable: stop a service from auto-starting at boot

Same distinction in reverse: doesn't stop it running now, just prevents it from starting automatically next time.

7. systemctl enable --now: enable AND start in one command

Combines both actions and starts it immediately and sets it to persist across reboots.

8. systemctl status: check detailed current state

Shows whether it's active/inactive, enabled/disabled, recent log lines, and the process ID, your main diagnostic tool.

9. systemctl is-active: A quick yes/no check if the systrm is running

10. systemctl is-enabled: A quick yes/no check if the system is set to auto-start