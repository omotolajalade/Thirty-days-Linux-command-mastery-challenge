Day 12 drill:Create a group named devs, add two users to it, confirm membership with getent, remove one
member, then delete the group entirely.

Step 1 — Create the group

sudo groupadd devs

Step 2 — Add two users to it

sudo gpasswd -a omotola devs

Step 3 — Confirm membership using getent

getent group devs

Step 4 — Confirm membership a second way

id -Gn omotola

Step 5 — Remove one member

sudo gpasswd -d omotola devs

Step 6 — Confirm the removal

getent group devs

Step 7 — Delete the group entirely

sudo groupdel devs

Step 8 — Confirm it's gone

getent group devs
