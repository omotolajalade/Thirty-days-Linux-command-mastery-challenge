Practice Drill

Task: Pick any log file on the system. View it fully with `cat`, page through it with `less`, show the first and last 15 lines, count its lines, identify its file type, and inspect its full metadata with `stat`.

Steps

 1. View the entire file
cat /var/log/syslog

2.. Page through it (press space to scroll, q to quit)
less /var/log/syslog

3. Show the first 15 lines
head -n 15 /var/log/syslog
 4. Show the last 15 lines
tail -n 15 /var/log/syslog

 5. Count how many lines it has
wc -l /var/log/syslog
6. Identify its file type
file /var/log/syslog

7. Inspect its full metadata (size, permissions, owner, timestamps)
stat /var/log/syslog
