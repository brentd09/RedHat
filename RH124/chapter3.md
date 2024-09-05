# Chapter 3 RH124
``` bash

``` 
## Command Syntax
``` bash
ls
pwd; ls
date
date +%R
date +%x
```
## View Contents of a file
``` bash
cat file1
cat file1 file2
cat -v /bin/ls
head /etc/passwd
tail /etc/passwd
wc /etc/passwd
```
## Tab Completion
``` bash
mkdir music
cd mus[TAB]
ls --[TAB][TAB]
``` 
## Write Long Commands on Multiple Lines

## Command History
``` bash
history
!head
!10
mkdir ~/data
^mkdir^cd
```
## Create Empty files
``` bash
mkdir songs
touch file1
touch file1 file2
touch crowdedhouse{1..9}.mp3
copy crowd* songs
```
## Links
``` bash
cd songs
ls -li #i-nodes are the key to understanding this
ln crowdedhouse1.mp3 DontDreamItsOver.mp3
ls -li
ln -s crowdedhouse2.mp3 MeanToMe.mp3
```
## Pattern Matching
``` bash
ls c*
ls crowded?ouse[1-4].mp3
ls crowded?ouse[[:digit:]].mp3
ls crowded?ouse[[:digit:]][[:digit:]].mp3 # this will fail if there are no files ending with two digits
```
## Brace Expansion
``` bash

```
## Tilde 
``` bash
cd ~
cd ~bob
cd ~/songs
```
## Variables 
``` bash
var1="This is a string of characters, that is being stored in a variable called var1"
echo $var1
echo ${var1}
```
## Command Substitution
``` bash
current_date=$(date)
echo current_date # this will fail as we are not displaying the contents of a variable, the $ is missing
echo $current_date
echo \$current_date = $current_date
```
