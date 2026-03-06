 ### Filesystem
 ### to create a file 
 ```bash
touch hello.txt
```
### to create multiple files in linux
```bash
touch file{1..5}.txt
```
### to remove the file 
```bash
rm -rvf hello.txt
```
### to remove multiple files 
```bash
rm -rvf file{1..5}.txt
```
### to write in the file
```bash
cat > filename.txt
```
### to read the file
```bash
cat hello.txt
```
### to copy the content of the file
```bash
cat index.html >> hello.html
``` 


## File permission
### “File permissions in Linux control access to files and directories by defining read, write, and execute permissions for the owner, group, and others.”
## Types of file 
1. - --> Normal file <br>
2. d --> Directory <br>
3. l --> link file <br>
4. b --> block device file <br>
5. c --> character device file <br>
6. p --> pipe <br>

## permission (numerical)
1. r = 4 <br>
2. w = 2 <br>
3. x = 1 <br>

#### To check the permission of file 
```bash
ls-l
```
#### to check the specific file permission 
```bash
ll filename
```
#### to check the permission of the hidden files 
```bash
ls-la
```
#### to show in human redable format 
```bash
ls-lh
```
#### to check particular directory permission
```bash
ll -d dirname
```

## ownership in linux 
### "Ownership in Linux means assigning a file or directory to a specific user and group. It determines who controls the file and works with permissions to manage access.”
1. owner : the user who created file<br>
2. group : the primary group of the file owner<br>
3. other : all other user on the system<br>

### to change ownership of file 
```bash
chown username filename
```
### to change owner of group
```bash
chown groupname filename
```

#### 1) Root user 
1. Default directory permission for root user = 755 <br>
2. Default file permission for root user = 644 <br>
3. Maximum directory permission = 777 <br>
4. Maximum  file permission = 666 <br>
#### 2) Local user 
1. Default directory permission =775 <br>
2. Default file permission = 664

### to set permission to other user 
```bash
chmod o+w filename
```
### to remove the permission to other user 
```bash
chmod o-w filename
```
### to set permission to group 
```bash
chmod g+w filename
```
### to remove the permission to group 
```bash
chmod g-w filename
```
### to set all permission to user group and other 
```bash
chmod ugo = rwx filename
```
##  Umask 
#### used to set default permission for files and directories 
1. Root user umask = 022 <br>
2. Local user umask = 002 <br>

### formula for umask 
umask = max permission - default permission 
  
## ACL (Access control list)
### Acl is used to set specific permisiion to user for particular file or directory .
### to set the permission
```bash
setfacl -m u:username:rwx filename
```
### to view permission 
```bash
getfacl filename
```
### to remove the permission 
```bash
setfacl -x u:username filename
```
