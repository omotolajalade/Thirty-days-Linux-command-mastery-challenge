Day 17 drill:Add a permanent environment variable and a custom alias to your .bashrc, reload it without
opening a new terminal, and confirm both persist in a fresh session.


Step 1 — Open your .bashrc for editing

nano ~/.bashrc

Step 2 — Scroll to the bottom and add two new lines

export FAVORITE_FRUIT=banana
alias ll='ls -la'

Save and exit (Ctrl+O, Enter, then Ctrl+X).

Step 3 — Reload it into your current session, without opening a new terminal

source ~/.bashrc

Step 4 — Confirm both took effect immediately

echo $FAVORITE_FRUIT
ll