Day 13 drill:Refresh the package index, search for and install a small utility, inspect its package details, then
purge it completely along with its configuration files.

Step 1 — Refresh the package index

sudo apt update

Step 2 — Search for a small utility

apt search cowsay

Step 3 — Install it

sudo apt install cowsay

Step 4 — Inspect its package details
apt show cowsay

Step 5 — See exactly what files it placed on your system

dpkg -L cowsay

Step 6 — Purge it completely

sudo apt purge cowsay

Step 7 — Clean up any leftover dependencies

sudo apt autoremove

Step 8 — Confirm it's really gone

dpkg -l | grep cowsay