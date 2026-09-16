Day 19 drill: In a 50-line config file, jump straight to line 10, search for a keyword, jump between all matches,
then replace every occurrence of one word with another across the whole file.
Step 1 — Create a 50-line practice file

for i in $(seq 1 50); do echo "This is config line number $i with an error placeholder" >> ~/linux-practice/config50.txt; done

Step 2 — Open it in Vim

vim ~/linux-practice/config50.txt

Step 3 — Jump straight to line 10

:10

Step 4 — Search for the word "error"

/error

Step 5 — Jump between matches

Press n several times, and watch your cursor jump to each occurrence in turn.

Step 6 — Replace every occurrence of "error" with "WARNING" across the whole file

:%s/error/WARNING/g

Step 7 — Confirm the replacement worked

Scroll or use /WARNING to check several lines — they should all now say "WARNING" instead of "error."

Step 8 — Save and quit using the shortcut

ZZ