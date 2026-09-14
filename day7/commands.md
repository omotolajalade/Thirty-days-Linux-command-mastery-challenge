Command and what it does 
chown: Changes the ownerof a file or directory.                                                                  |
chown user:group : Changes both the owner and group of a file or directory.                                                   
chown -R: Changes the owner/group of a directory and everything inside it.                                           
chgrp: Changes the group that owns a file or directory.                                                           
chmod u+s: Adds the SUID permission. It allows a program to run with the permissions of its owner.                    
chmod g+s: Adds the SGID permission. On directories, new files can inherit the directory's group.                     
chmod +t: Adds the sticky bit, commonly used on shared directories so users cannot freely delete other users' files. 
find -perm /4000 : Searches for files that have the SUID permission.                                                          
getfacl: Shows the detailed access permissions, including ACLs, for a file or directory.                            
setfacl -m: Adds or changes a specific ACL permission for a user or group.                                             
