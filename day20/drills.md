Day 20 drill: From a raw log file, build one pipeline that filters for 'error' entries, extracts the
timestamp column, sorts the results, and removes duplicates, all in a single chained command.

Step 1: Filter the real authentication log for sudo entries using sudo grep -i sudo /var/log/auth.log > step1.txt

This searches your machine's actual authentication log for every line mentioning sudo genuine records of every time you've used elevated privileges and saves just those matching lines into a new file called step1.txt.

Step 2 : Check what you captured using cat step1.txt

Which displays the contents of step1.txt so you can see the raw filtered lines before processing them further.

Step 3: Extract just the timestamp columns with awk '{print $1, $2, $3}' step1.txt > step2.txt

This takes each line from step1.txt and prints only the first three space-separated fields (month, day, and time), saving the result into step2.txt pulling out just the date/time information and discarding the rest of each line.

Step 4: Sort the extracted timestamps with sort step2.txt > step3.txt

This arranges the lines in step2.txt into alphabetical/chronological order and saves the sorted result into step3.txt.

Step 5: Remove duplicate lines making use of the command uniq step3.txt > final_result.txt

Since uniq only removes duplicates sitting next to each other, this only works correctly because Step 4 already sorted everything first identical timestamps are now grouped together, so uniq can properly collapse them.

Step 6: View your final result with cat final_result.txt

This displays the finished output a clean, sorted, deduplicated list of every unique date/time you've run a sudo command.