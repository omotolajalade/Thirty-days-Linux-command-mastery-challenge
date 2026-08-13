1.mkdir -p practice/2026/april
Create the nested folder structure in one command

2. Create three empty files inside it
touch newfile1.txt newfile2.txt newfille3.txt

 3. Copy the whole folder (with its contents) to a backup location
cp -r  ~\pratice/2026/april ~/practice/2026/backup

 4. Rename one file (mv also works for renaming)
mv newfile1.txt Linux txt 

 5. Now safely delete the empty directory (rmdir refuses if anything is still inside — that's the safety check)
rmdir practice
