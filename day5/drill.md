Create a symbolic link to a config file, resolve its real path, print a two-level tree of /etc, and explain to a peer the difference between a hard link and a symbolic link.
Steps:
pwd
Then create the link: ln -s /etc/hosts hosts-link
Check that it exists: ls -l hosts-link
Now resolve it: readlink hosts-link
Then:realpath hosts-link to show the path
Then complete the /etc tree requirement
Run: tree -L 2 /etc
Finally, practice basename and dirname
Run:
basename /etc/hosts to get hosts
Then:
dirname /etc/hosts to get etc

