Day 10 Drill: . Produce a one-page mini security audit of a server: who has logged in recently,
who is logged in right now, which accounts have never logged in, and every sudo command run in this session

Step 1 — Check SUID files: Run sudo find / -perm /4000  to search the system for files with the SUID permission. These files are important to review because they can run with the permissions of their owner.

Step 2: Run last to see who has recently logged into the system and when.

Step 3: Run lastlog to see the most recent login information for the different user accounts.

Step 4: Run w to see who is currently logged in and what they are doing.

Step 5: Run who to see the users currently connected to the system.

Step 6: Run groups to see which groups your current account belongs to.

Step 7: Run sudo passwd -S username, replacing username with your actual Linux username. This gives you basic information about the account's password status.

Step 8: Run chage -l username, replacing username with your Linux username. This shows password expiry and account-aging information.

Step 9: Run sudo lastb to see unsuccessful login attempts. This can help identify suspicious login activity.

Step 10: Run history | grep sudo to search your command history and display commands where you used sudo.
