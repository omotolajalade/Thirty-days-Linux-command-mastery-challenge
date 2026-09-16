Day 16 drill: Set a temporary environment variable, confirm it exists, unset it, then add a directory to your
PATH for the current session only and prove the shell can now find a script inside it.


Step 1 — Set a temporary environment variable

export FAVORITE_FRUIT=Banana

Step 2 — Confirm it exists

echo $FAVORITE_FRUIT

Step 3 — Remove it

unset FAVORITE_FRUIT
echo $FAVORITE_FRUIT

The second line should print nothing — confirming it's gone.
Step 4 — Create a practice folder with a simple script inside

mkdir -p ~/linux-practice/code
echo 'echo "This is awesome"' > ~/linux-practice/scripts/the_code.sh
chmod +x ~/linux-practice/scripts/the_code.sh

Step 5 — Add the folder to PATH for this session

export PATH=$PATH:~/linux-practice/code

Step 6 — Now try running it by name alone again

the_code.sh