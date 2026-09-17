Day 22 drill: Start a long-running command in the background, suspend it, resume it in the background, then
start a second one that survives you logging out, using nohup.

Step 1 — Start a long-running command in the background

sleep 300 &

The & at the end sends it straight to the background it show a job number and PID printed.

Step 2 — Confirm it's running

jobs

Step 3 — Bring it to the foreground, then suspend it

fg and then immediately press Ctrl+Z.

Step 4 — Resume it in the background

bg

Step 5 — Confirm it's running again

jobs

Step 6 — Start a second one that survives logout, using nohup

nohup sleep 300 &

Step 7 — Confirm both, then clean up when done testing

jobs
kill %1
kill %2