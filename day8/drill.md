Day 8 Drill :Attempt a command that fails for lack of permission, re-run it instantly with sudo !!, then list
exactly which commands your account is permitted to run as another user.


Step 1: Run whoami to see the username you are currently logged in as.

Step 2: Run id to see your user ID, group ID, and the groups your account belongs to.

Step 3: Run sudo -l to see which commands your account is allowed to run with administrator privileges.

Step 4: Run cat /etc/shadow to try accessing a protected system file. Note: Your normal account will usually get “Permission denied.”

Step 5: Run sudo !!. The !! means the previous command, so Linux repeats it with administrator privileges.

Step 6: Run sudo -i to open a root shell. Then run whoami to confirm that you are now root.

Step 7: Run id while you are root to see the root user ID and groups.

Step 8: Run exit to leave the root shell. Then run whoami again to confirm that you are back to your normal user.

Step 9: Run sudo -u username whoami, replacing username with an actual user on your system. This shows how sudo can run a command as another user.


