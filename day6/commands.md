commands and what it does                                         
ls -l : Shows files together with their permissions, owner, group, size, and other details.              
chmod: Changes the permissions of a file or directory.                                                  
chmod 755 file : Gives the owner full permission and gives the group and others read and execute permission.      
chmod 644 file: Gives the owner read and write permission, while group and others can only read.                 
chmod 600 file: Gives the owner read and write permission, while everyone else has no permission.                
chmod - R:Changes permissions recursively, meaning it applies to a directory and everything inside it. 
umask :Shows the default permission settings used when new files and directories are created.           
umask -S: Shows the umask permissions in an easier-to-read symbolic format.                              
chmod u+x file: Adds execute permission for the file's owner.                                                    
stat -c '%A %U %G' file: Shows the file's permissions, owner, and group in a simple format.                               
