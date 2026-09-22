Commands and what they do

1. #!/bin/bash (shebang): the very first line of a script, telling the system which program should run it.

2. chmod +x script.sh: make a script executable (you've done this before).

3. ./script.sh: run a script from the current directory.

Thw ./ command explicitly means in this current folder needed because, for security reasons, the current directory usually isn't in your PATH by default.

4. VAR=value: set a variable inside a script.

5. $(): command substitution: run a command and capture its output into a variable.

6. read -p: prompt the user for input.

What each character means -p shows a prompt message before waiting for input.

7. if / elif / else / fi: conditional logic.

if [ condition ]; then

elif [ other_condition ]; then
    
else
    
fi

8. -gt / -lt / -eq: numeric comparison operators inside if conditions.

What each character means  -gt = greater than, -lt = less than, -eq = equal to.

9. for loop: repeat an action for each item in a list.

10. while loop: repeat an action as long as a condition remains true.