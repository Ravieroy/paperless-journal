1. Replace a string in a file with a newstring 
2. Find and delete a line 
3. Remove empty lines 
4. Remove the first or n lines in a file 
5. To replace tabs with spaces 
6. Show defined lines from a file 
7. Substitute within [[Vim]] editor 
8. And many more 

## Examples 
!!! tip
	The flag -i makes the changes permanent while running the sed command 

#### Replace the *oldWord* with the *newWord* globally (Only on screen)
```bash
sed 's/oldWord/newWord/g' fileName
```

#### Replace the *oldWord* with the *newWord* globally (make changes permanent)
```bash
sed -i 's/oldWord/newWord/g' fileName
```

#### Find and delete the *keyWord*
```bash
sed 'keyWord/d' fileName
```

Delete an empty line from a file
```bash
sed '/^$/d' fileName
```

Delete first line
```bash
sed '1d' fileName
```

Delete first two lines
```bash
sed '1,2d' fileName
```

Replace Tabs with Spaces
```bash
sed 's/\t/ /g' fileName
```

View from line i to j
```bash
sed -n i,jp fileName
sed -n 12,18p fileName #view from line 12 to 18
```

View all *except* from i to j 
```bash
sed i,jd fileName
```

Add space after each line
```bash
sed G fileName
```

Replace *oldWord* with *newWord* except the ith occurence
```bash
sed 'i!s/oldWord/newWord/g' fileName
```

Search and replace in the [[Vim]] editor 
```vim
:s/oldWord/newWord
```
