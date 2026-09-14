Create a shared project folder, apply the SGID permission so new files inherit the folder's group, then search the system for files with the SUID permission.

Step 1: Create a folder called shared-project.

Step 2: Use ls -ld to see who owns the folder and which group it belongs to.

Step 3: Create a group called projectgroup.

Step 4 : Use chgrp to make projectgroup the group that owns shared-project.

Step 5: Use chmod g+s on the folder.

i.e : This makes new files created inside the folder inherit the folder's group.

Step 6:Use ls -ld shared-project and check that the group permissions contain an s.

Step 7: Create a file inside shared-project.

Step 8:Check the file's group and confirm that it inherited the project folder's group.

Step 9: Use find -perm /4000 to search for files on the system that have the SUID permission.

Step 10: Use getfacl on your shared project folder to view its detailed permissions.