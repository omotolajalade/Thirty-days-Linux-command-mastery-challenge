Commands and what they do
1. gg / G :jump to the very top or very bottom of a file

 gg (lowercase, pressed together) jumps to line 1. G (uppercase, single press) jumps to the last line of the file.

2. :10: jump to a specific line number

typing a colon followed by just a number jumps your cursor directly to that line, instant navigation instead of scrolling.

3. /: search forward for text

 / starts a forward search. Vim jumps to the first match after your cursor's current position.
4. ?: search backward for text

Same idea as /, but searches backward from your cursor's position instead of forward.

5. n / N: jump to the next or previous match

Once you've searched once, these let you hop between every occurrence without retyping the search.

6. :%s/old/new/g: search and replace across the entire file

: → start a command, % → apply it to the whole file (every line), not just the current one, s → substitute, old → the text you're searching for, new → the text to replace it with, g → global — replace every occurrence on each line, not just the first one per line

This single command replaces every instance of "error" with "ERROR" across the entire file.

7. dw: delete a single word

 d for delete, w for word  deletes from your cursor's position to the end of the current word.

8. x: delete a single character

Deletes just the one character your cursor is sitting on the smallest, most precise deletion available.

9. o / O: open a new line and enter insert mode

 both immediately drop you into insert mode on the new blank line, a fast way to add content without manually navigating and pressing i.

10. ZZ: save and quit (an alternative to :wq)

A quicker keyboard shortcut for the same save-and-quit action as :wq, no colon or Enter needed.

