## User management 
#### User Management in Linux refers to the process of creating, modifying, deleting, and managing user accounts and their permissions on a Linux system. It helps administrators control who can access the system and what actions they are allowed to perform, ensuring security and proper resource usage.

### Types of user
#### 1) Root user
#### 2) local user
#### 3) system user

### add user
```bash
adduser username
```
```bash
useradd -m username
```
### to check the password of the user 
```bash
cat/ etc/shadow
```
### To check the content of the password 
```bash
cat /etc/passwd
```
### To delete the user 
```bash
userdel -r username
```
### to  set the password to user 
```bash
passwd username
```
### fields into etc/passwd
1. username <br>
2. password placeholder<br>
3. userid<br>
4. groupid<br>
5. user information<br>
6. home directory<br>
7. login shell<br>
#### fields in etc/shadow
1. username <br>
2. encrypted password<br>
3. last time password change<br>
4. minimum days between password change<br>
5. maximum days between password changes<br>
6. warning days<br>
7. inactive days<br>
8. account expiry<br>
9. future use<br>

## Group management
#### Group management in Linux is the process of organizing users into groups and managing those groups to control permissions and access to system resources.”
### to create a group 
```bash
groupadd groupname
```
### to check group info 
```bash
tail-1 /etc/group
```
### to show specific group info 
```bash
cat  /etc/group |grep groupname
```
### to add memeber in group
```bash
gpasswd -a username groupname
usermod -aG groupname username
```
### to remove the user from group 
```bash
gpasswd -d username groupname
```
### to remove the group
```bash
gpasswd -f groupname
```
### to add multiple member in group 
```bash
gpasswd -M user1 ,user2 ,user3 groupname
```
### to make group member to admin 
```bash
gpasswd -A username groupname
```
### to remove group admin 
```bash
gpasswd -A '   ' groupname
```
