Commands and what they do

1. grep: search text for a pattern and prints every line in the file containing the keyword.

2. grep -r — search recursively through a whole folder

 The-r means recursive instead of one file, search every file inside a folder and its subfolders.

3. grep -i: case-insensitive search

The  -i ignores the difference between uppercase and lowercase and matches "error," "Error," "ERROR," all the same.

4. sort: sort lines alphabetically

Rearranges the file's lines into alphabetical (or numeric-as-text) order.

5. sort -n: sort numerically

What each character does -n tells sort to treat the content as actual numbers, not just text — important because plain sort would put "10" before "9" comparing them as text, character by character, while sort -n correctly puts 9 before 10.

6. uniq — remove consecutive duplicate lines

The uniq command only removes duplicates that are next to each other, which is exactly why it's almost always used right after sort, since sorting groups identical lines together first.

7. cut -d',' -f: extract a specific column from delimited text

what each character represent -d',' → the delimiter is a comma (could be any character ,a comma here since we're imagining CSV-style data)
-f → extract field number 

8. awk '{print $1}': A  powerful column extractor

The awk command is a full text-processing mini-language; {print $1} tells it to print just the first field of each line, where fields are automatically split by whitespace by default.

9. sed 's/old/new/g': find and replace text 
 what each character represent s for substitute, old/new, g for global.
 Note: It run directly from the terminal against a file, not inside an editor.

10. Pipe chains (|) :combining commands together

The | command  takes the output of one command and feeds it directly as input to the next, letting you chain several tools into one pipeline.