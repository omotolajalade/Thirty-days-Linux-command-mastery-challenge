Day 21 drill:Find the PID of a running process by name, view it in top, show it as part of the process tree, and
identify which process is using port 80.

Step 1 — Find the PID of a running process by name

pgrep firefox

(Substitute any program you know is running — Firefox is a safe bet since it's in your dock.)

Step 2 — View it live in top

top

Once open, you can also press Shift+M to sort by memory usage, or just visually locate your PID from Step 1 in the list. Press q to exit.

Step 3 — See it in the process tree

pstree -p | grep firefox

Step 4 — Check what's using port 80

sudo lsof -i :80