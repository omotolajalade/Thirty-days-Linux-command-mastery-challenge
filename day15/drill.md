Day 15 drill: Provision a complete new team member account (user, groups, password) and
install the three tools they need for their role, in a single documented sequence. 

Step 1 — Create the group for their role 

sudo groupadd devs

Step 2 — Create the user, home folder, shell, AND assign their group all at once

sudo useradd -m -s /bin/bash -G devs newhire

Step 3 — Set their password

sudo passwd newhire

Step 4 — Confirm the account and group membership

id newhire
getent passwd newhire

Step 5 — Refresh the package index and install their three role tools

Pick three small, safe example tools:

sudo apt update
sudo apt install -y tree cowsay curl

Step 6 — Confirm all three installed successfully

apt list --installed > installed.txt

Then check installed.txt for tree, cowsay, and curl.