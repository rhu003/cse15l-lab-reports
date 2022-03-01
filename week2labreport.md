## Installing VScode
![image](Screenshot (65).png)
First you should download vs code from visual studio's website.
go to [Link](http://code.visualstudio.com)
When you finished, it should look like this. 

## Remotely Connecting
![image](Screenshot (66).png)
Try to remotely connect to our course by using course account for cse15l.
Type in course-specific account and enter password.

## Trying Some Commands
![image](Screenshot (67).png)
Now, let's try some commands like ```cd```, ```ls```, ```ls lat```.
Enter them in the command window.

## Moving files with ```scp```
![image](Screenshot (68).png)
Now we try to learn to move files with ```scp```. 
Do the above ```scp``` command with file name and username.

## Setting an SSH Key
![image](Screenshot (70).png)
Try to set an ssh key as the figure suggests.
Using ```ssh-Keygen```.

## Optimizing Remote Running
![image](Screenshot (121).png)
Now we need to optimizing remote running.
We can add ```ls``` command to ssh to have it list the home directory.
1. edit ```whereami.java``` in local computer
2. ```scp WhereAmI.java cs15lwi22zz@ieng6.ucsd.edu:~/```
3. run whereami on server
we get a total of about 80+ keystrokes, it runs slower as type ssh command into terminal counts a lot of strokes. 
However, if we save the ssh command and run it, it would take much less keystrokes and run faster, so the remote running is supposed to run faster.
click local file - 1 keystroke
write comment in local file - 10 keystrokes
save local file - 2 keystrokes

copy scp command from website - 3 keystrokes
pasted scp into terminal and pressed enter - 3 key strokes
type ssh command into terminal - 70 keystrokes
total keystrokes: 89
