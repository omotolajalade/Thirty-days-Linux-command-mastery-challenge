Day 4 practice drill
Task:  Find every .conf file under /etc, find every file larger than 1 MB under /var, check the total disk usage of /home, and check the remaining free space on the root filesystem /.
Steps:
We start by opening the terminal and running the first command:
find /etc -type f -name "*.conf"
This searches through /etc and its subdirectories and displays every file whose name ends in .conf. 
Next, search /var for files larger than 1 MB by running:
find /var -type f -size +1M
 The command will then show files under /var that are larger than 1 MB.
After that, check how much storage the /home directory is using:
du -sh /home
This gives you one total figure in a human-readable format. 
Finally, check the available storage on your root filesystem by running:
df -h /
Look at the result and find the Size, Used, Avail, and Use% columns. Size tells you the total storage, Used tells you how much has been used, Avail tells you how much is still available, and Use% tells you the percentage currently being used.
