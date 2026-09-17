commands and what they do
1. ps aux:snapshot of every running process

ps → process status, a → show processes for all users, not just yours, u → show in user-friendly format, x → include processes not attached to a terminal i.e background orsystem processes

2. ps -ef: an alternative full-format listing

what each character mean -e → every process, -f → full format, including parent process ID

Similar information to ps aux, but shows the PPID (Parent Process ID), useful for understanding what launched what.

3. ps -u: processes for a specific user

Filters the listing down to just one user's processes, useful on a shared/multi-user system when you only care about your own activity.

4. top: live, constantly updating process view

Unlike ps (a one-time snapshot), top refreshes continuously, sorted by CPU usage by default. Press q to quit.

5. htopa: friendlier, colorized version of top

Same concept as top, but with color, mouse support, and easier-to-read bars for CPU/memory usage per core.

6. pgrep: find a process's PID by name

 process grep searches running processes by name instead of scrolling through a full list.

7. pstree: view processes as a parent-child tree

Shows visually which processes spawned which others.

8. lsof -i: see which process is using network connections

lsof: list open files, -i filters to network (internet) connections specifically.

Shows exactly which process, if any, is using port 80 (the standard web traffic port) — genuinely useful when something says "port already in use."

9. jobs: see background jobs in your current shell

Lists any commands you've sent to run in the background in this specific terminal session.

10. nice / renice: adjust a process's priority

The meaning: — a number from -20 (highest priority) to 19 (lowest), controlling how much CPU attention the scheduler gives a process relative to others.

