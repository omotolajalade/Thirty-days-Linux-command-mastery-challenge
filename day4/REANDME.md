SEARCHING THE FILESYSTEM
I learned how to search through the Linux filesystem and understand disk usage. I learned that the "find" command can be used to search for files and directories based on different conditions.

I practiced searching for files by name using "find -name", searching specifically for files or directories using "find -type", searching for files based on their size using "find -size", searching according to when files were modified using "find -mtime", and searching based on file permissions using "find -perm".

I also learned about the "locate" command, which provides another way of searching for files. I learned that "updatedb" can be used to update the database that "locate" uses for its searches.

Another important part of Day 4 was understanding disk usage. I learned that "du" means Disk Usage and can be used to determine how much storage files or directories are using. For example, "du -sh /home" provides a human-readable summary of the total space being used by the "/home" directory.

I also learned that "df" means Disk Free and is used to check filesystem storage and available space. Using "df -h /" allows me to see the total storage, used storage, available storage, percentage of storage being used, and the filesystem where the root directory is mounted.

For the Day 4 practical exercise, I searched for configuration files under "/etc" using "find /etc -type f -name "*.conf"". I also searched for files larger than 1 MB under "/var" using "find /var -type f -size +1M". I then checked the total disk usage of "/home" with "du -sh /home" and checked the remaining available space on the root filesystem with "df -h /".
What surprised me how these commands make locating things easier