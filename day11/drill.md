Day 11 drill:Create a new user with a home directory and Bash shell, set their password, add them to a
secondary group, rename the account, then remove it along with its home directory.

Step 1 — Create a new user with a home directory and Bash shell

sudo useradd -m -s /bin/bash testuser

Step 2 — Confirm the account was created correctly

ls /home

It shows a new testuser folder alongside your own.

Step 3 — Set the account's password

sudo passwd testuser

Step 4 — Add the account to a secondary group

sudo usermod -aG sudo testuser

Step 5 — Confirm the group was added without wiping anything else

groups testuser

Step 6 — Rename the account

sudo usermod -l renameduser testuser

Step 7 — Confirm the rename

id renameduser

Step 8 — Remove the account along with its home directory

sudo userdel -r renameduser

Step 9 — Confirm it is gone.

ls /home
id renameduser