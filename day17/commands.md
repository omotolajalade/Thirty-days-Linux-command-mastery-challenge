Commands and what they do
1. nano ~/ .bashrc: edit your personal shell config file

nano → a simple, beginner-friendly text editor, ~/.bashrc → a hidden file, the leading dot hides it from normal ls in your home folder, automatically read every time you open a new interactive terminal session

2. source ~/.bashrc: apply changes without restarting

 This makes the changes take effect in your current terminal, instead of needing to close and reopen it.

 3. cat ~/.bash_profile: a related, sometimes-confusing sibling file

what each character does .bashrc runs for every new interactive shell,.bash_profile traditionally runs only at login time.
Note: On many desktop Linux setups, .bash_profile may not even exist by default, or may simply load .bashrc itself, worth checking, not assuming.

4. sudo nano /etc/environment: edit the system-wide variables file

5. sudo nano /etc/bash.bashrc: the system-wide equivalent of .bashrc

The ~/.bashrc only affects your account; /etc/bash.bashrc is read by every user's bash session on the system before their personal .bashrc runs. Editing this needs sudo since it affects everyone.

6. alias: create a shortcut for a longer command

 this creates a new, shorter command name (ll) that actually runs a longer one (ls -la) whenever typed.

7. unalias: remove a shortcut

Removes the alias for the current session. To remove it permanently, you'd also need to delete the line from .bashrc where it was defined.
8. type:find out what kind of command something actually is

This is genuinely useful for troubleshooting: it tells you whether something is a real program, a shell built-in, or an alias — important since aliases can sometimes behave unexpectedly compared to the "real" command they're based on.

9. which: find the exact location of a command's program file

it shows exactly which file on disk gets run when you type that command name, useful when multiple versions of a program might exist in different PATH folders.

10. whereis: find a command's binary, source, and manual page locations

Broader than which shows not just the executable, but also documentation and related files if they exist.