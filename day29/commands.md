Commands and what they do

1. function_name() { }: defining a reusable function.

2. $1 / $2: positional arguments passed into a script or function.

3. $# / $* / $@: $# = number of arguments passed, $*/$@ = all arguments (slightly different handling of spacing, $@ generally preferred).

4. $0: the script's own name/path.

5. exit codes ($?): every command returns a number when it finishes; 0 means success, anything else means some kind of failure. $? holds the most recent exit code.

6. crontab syntax: the five-field time format cron uses.

7. cron scheduling (0 * * * *): breaking down the five fields: minute, hour, day-of-month, month, day-of-week. 0 * * * * means "at minute 0 of every hour".

8. nohup script.sh &: run a script in the background, immune to logout.

9. trap: catch a signal (like Ctrl+C) and run custom cleanup code before exiting.

10. logger: send a custom message into the system log (journalctl/syslog), useful for scripts to leave a record of what they did.