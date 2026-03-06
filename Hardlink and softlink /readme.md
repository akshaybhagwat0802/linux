## Hardlink
### A Hard Link in Linux is a direct reference to the same inode (data block) of a file.
It means that multiple filenames point to the same file data on disk. 
If you create a hard link, both the original file and the hard link share the same content. Deleting one does not delete the actual data until all hard links are removed.
### Key Characteristics of Hard Link
1. Points to the same inode number <br>
2. Shares the same data as the original file<br>
3. If the original file is deleted, the data still exists through the hard link<br>
4. Cannot be created for directories<br>
5. Cannot be created across different filesystems<br>

### syntax 
```bash
ln filename hardlink name
```

## check inode number 
```bash
ls -li
```

## softlink 
#### A Soft Link (Symbolic Link) in Linux is a special type of file that points to another file or directory.
It acts like a shortcut to the original file.
Unlike a hard link, a soft link does not share the same inode; it only stores the path of the original file.

## Key Characteristics of Soft Link
Has a different inode number <br>
Stores the path of the original file<br>
Can link directories<br>
Can work across different filesystems<br>
If the original file is deleted, the soft link becomes broken<br>
### syntax
```bash
ln-s filename softlink name
```
## Difference between hardlink and softlink 

| features | hardlink | softlink |
|---------|---------|---------|
| 1. Purpose| Backup created    | Shortcut created   |
| 2. filesize  | same as original file   | Different from original file    |
| 3. inode number | same as original file   | Different from original file    |
| 4. linkcount  | link count will be increase or decrease by 1   | link count doesnot increase or decrease by 1    |
| 5.   | original file deleted hardlink remain in file system   | original file deleted softlink will be deleted |
