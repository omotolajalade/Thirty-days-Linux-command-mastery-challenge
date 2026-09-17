Commands and what they do

1. kill: send a termination signal to a process

kill by default, sends signal 15 (SIGTERM) which is a polite request asking the process to shut down cleanly, giving it a chance to save data first.

2. kill -9: force-kill a process immediately

kill -9 signal 9 (SIGKILL) can't be ignored or cleaned up after the process is terminated instantly, no chance to save anything.

3. kill -HUP: ask a process to reload its configuration

The  HUP (hangup) traditionally tells a process to reread its config files without fully restarting, many services use this specifically for that purpose.

4. killall: kill processes by name instead of PID

Kills every process matching that name, it is  useful when a program has spawned multiple related processes.

5. pkill: kill by pattern match 

Matches process names by pattern, not requiring an exact full name match.

6. fg: bring a background job to the foreground

 Foreground command resumes a paused or backgrounded job, bringing it back to actively occupy your terminal.

7. bg: resume a paused job, but in the background

Background command resumes a job you'd paused, but lets it keep running without taking over your terminal, freeing you to keep typing other commands.

8. Ctrl+Z: suspend the current foreground process

Keyboard shortcut, not a typed command: pausing whatever's currently running in your terminal, returning you to the prompt without killing it.

9. nohup: run a command that survives you logging out

No hangup commad normally, closing your terminal sends a hangup signal that kills anything still running in it. nohup makes a command immune to that.

10. disown: detach an already-running background job from your shell

Similar goal to nohup, but applied after a job is already running in the background, rather than at launch time.