Commands and what they do
1. printenv: show all environment variables

Prints every currently set environment variable and its value ,a long list.

2. printenv HOME: show one specific variable

Same command, but narrowed to just one variable's value instead of the whole list.

3. echo $VAR: the more common way to check a single variable

$ → tells the shell treat what follows as a variable name, give me its value, not the literal text
Without the $, echo PATH would just print the word "PATH, the $ is what makes it look the value up

4. export: create or update a variable for this session and makes the variable available not just to your current shell, but to any program launched from this shell too

Note: This only lasts for your current terminal session but when the terminal closes, and it's gone. 

5. unset: remove a variable

Deletes the variable entirely from the current session. After this, echo variable would print nothing.

6. env: similar to printenv, slightly different tool

Env also lists environment variables, but env can additionally be used to run a command with a modified environment temporarily. 

7. source: reload a file's contents into your current shell

when running a script it starts a new process, any variables it sets disappear when it finishes
source instead runs the file's commands directly in your current shell, so anything it sets actually sticks around afterward

8. echo $PATH:specifically inspecting the search path

It searches through folders in order until it finds where a program is located with it's name.

9. export PATH=$PATH: add a folder to PATH

PATH=$PATH: → take PATH's current value, then add a new folder onto the end, separated by a colon.

10. cat /etc/environment: view system-wide default variables

This is a file that sets environment variables for every user on the system, applied at login different from your personal, session-only export commands.