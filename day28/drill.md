Day 28 drill: Write and execute a script that reads the user's name, checks whether a config file exists using an
if statement, and loops through three server names pinging each one.

Step 1 — Create and open the script

nano ~/linux-practice/day28script.sh

Step 2 — Write it

bash
#!/bin/bash

read -p "Enter your name: " username
echo "Hello, $username"

if [ -f ~/linux-practice/config50.txt ]; then
    echo "Config file exists."
else
    echo "Config file does not exist."
fi
     for server in google.com github.com wikipedia.org; do
    echo "Pinging $server..."
    ping -c 1 "$server"
done

Step 3 — Make it executable and run it

chmod +x ~/linux-practice/day28script.sh
~/linux-practice/day28script.sh