Day 29 drill: Turn yesterday's script into a reusable function that accepts a service name as an argument, checks
its status, restarts it if stopped, and schedule it to run hourly with cron.

Step 1 — Write the function-based script

bash
#!/bin/bash

check_service() {
    local service_name=$1
    if systemctl is-active --quiet "$service_name"; then
        echo "$service_name is running."
    else
        echo "$service_name is stopped. Restarting..."
        sudo systemctl restart "$service_name"
        logger "day29script restarted $service_name"
    fi
}

check_service "$1"

Step 2 — Save, make executable, and test it
chmod +x ~/linux-practice/day29script.sh
~/linux-practice/day29script.sh cron

Step 3 — Schedule it hourly with cron

crontab -e