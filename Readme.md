## Linux Commands
###### Linux Practice : <a href="./Linux Practice.pdf">Linux Practice.pdf</a>
###### Linux Practical Exam : <a href="./Linux Practical Exam.pdf">Linux Practical Exam.pdf</a>

### 1. Open Terminal
```
CTRL + ALT + T
```

### 2. Free Space
The df command displays the amount of disk space available on the filesystem with each file name's argument.
```
df
free
```

### 3. Current Working Directory
pwd - Print Working Directory
```
pwd
```


### 4. Directory
View directories
```
dir - (It is like ls)
```
Make directory
```
mkdir dirname
```
Change directory 
```
cd dirpath
cd - (Change to Previous Working Directory)
cd ~ (Change to Home Directory)
('.' - Current Directory, '..' - Parent Directory)
```
Remove directory - But it will delete only empty directory
```
rmdir dirname
```
For deleting whole directory
```
rm -r dirname
```

### 5. Files
Create File
```
touch filename
```
Read File
```
cat filename
less filename
more filename
tac filename (reverse of cat)
```
Remove File
```
rm filename
```
Copy File
```
cp filename path
```
Move File
```
mv filename path
mv oldfilename newfilename (Rename file)
```
Add content to file
```
cat > filename (It will overwrite the content, '>' Redirectional Operator)
cat >> filename (It will append new content to existing content, '>>' Append Operator)
vi filename
```

### 6. Listing
```
ls
ls -l (Long Format)
ls -a (Display all hidden files too)
ls -t (Sorted by Time)
ls -lt --reverse (Reverse Order)
ls -R (Display subdirectories' content too)
ls -p (Each folder has /)
ls -s (Display size of each file)
ls -S (Sort)
ls -h (Human Readable Format)
```

### 7. Links
###### Symbolic Link
Soft links are similar to shortcuts, and can point to another file or directory in any file system.
Removal, deletion will affect the link.
```
ln -s file nameofLink
```

###### Hard Link
Hard links are also shortcuts for files and folders, but a hard link cannot be created for a folder or file in a different file system. 
Removal, deletion will not affect the link.
```
ln file nameofLink
```

### 8. Permissions
-rw-r--r-- : r(read), w(write), x(execute)
1 bit is for d, l, c, b : [ - : Files, d – Directory, l – Symbolik link, c – Character Files, b -  Block Files] 
2nd : rwx : Permissions to User/Owner 
3rd : rwx : Group Permissions 
4th : rwx : Others/Public Permissions 

Change mode of file
```
chmod u=rw filename (For group g=rwx, others o=rwx, all a=rwx)
```
Change owner and group of file
```
chown new_owner filename 
chgrp new_group filename
chown new_owner:new_group filename 
passwd (To change password)
```

### 9. Process
Running Process 
```
top
ps
kill pid
pidof process_name
```

### 10. Extra
```
alias name='string' (Creating Alias)
unalias name

whoami (Display Username)
history (Command History)
type command (Display type of command)
file filename (Describe the content of that file)

su username (Switch User)
sudo command (Run command as a Root user)

sort filename (It will sort the content of that file)
uniq filename (It will show only unique the content of that file)
wc filename (Wordcount)
grep pattern (It will match the pattern)
```
