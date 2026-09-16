Day 18 drill:Open a new file in vim, type three lines of text, save it, reopen it, delete the middle line, undo the
deletion, then save and qui

Step 1 — Open a new file

vim ~/linux-practice/vimtest.txt

Step 2 — Enter insert mode and type three lines

Press i, then type the three lines

Step 3 — Return to command mode and save

Press Esc, then type:

:w

and press Enter.

Step 4 — Quit, then reopen the file to prove it saved

:q

Then from the terminal:

vim ~/linux-practice/vimtest.txt

Step 5 — Delete the middle line

Move your cursor to "This is line two" , then in command mode press: dd

Step 6 — Undo the deletion

u

Confirm "This is line two" reappeared.

Step 7 — Save and quit in one step

:wq