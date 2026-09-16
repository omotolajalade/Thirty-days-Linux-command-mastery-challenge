Commands and what they do
1. vim <file>: open a file in Vim

If the file doesn't exist yet, Vim creates it fresh once you save. You'll open into command mode by default.

2. i: enter insert mode

 i stands for insert. Pressing this switches you from command mode into insert mode.

3. Esc: return to command mode

This is the single most important key to remember today, pressing Esc at any time takes you out of insert mode and back into command mode, ready to issue instructions again.

4. :w — save (write) the file

 :w starts a command-line instruction inside Vim, w means write (save) the current file to disk, without quitting.

5. :q: quit 

 :q means quit. This only works cleanly if there are no unsaved changes.

6. :wq / :x: save and quit in one step

:wq explicitly means write, then quit. :x is a shorthand that does almost the same thing, with one subtle difference: :x only actually writes if something changed, while :wq always writes regardless. 

7. :q!: quit WITHOUT saving, discarding changes

The ! forces the quit even though there are unsaved changes.

8. dd: delete an entire line

the meaning: d for delete, pressed twice as a shortcut for "delete this whole line." Deletes the line your cursor is currently sitting on.

9. yy / p: copy (yank) and paste a line

the meaning: y stands for yank (Vim's word for copy), pressed twice for "yank the whole current line." p then pastes it directly below your cursor's current position.

10. u / Ctrl+r: undo and redo

the meaning: u undoes your last change, and can be pressed repeatedly to keep undoing further back. Ctrl+r reverses an undo.