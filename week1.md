## Week 1 lab report
**1. Installing VScode**
- You should visit https://code.visualstudio.com/ in order to download the Visual Studio Code program
- Next download the program by navigating to this screen by pressing the blue download button in the top right corner <img width="1091" alt="CleanShot 2023-01-11 at 14 16 23@2x" src="https://user-images.githubusercontent.com/36582468/211929688-ab291953-7733-47a6-a9ed-fcfa5b628b1f.png">
- Download the appropriate files based on the operating system you are on

**2. Remotely Connecting**
- In order to remotely connect to the server, you should first find your determine your email and password login using https://sdacs.ucsd.edu/~icc/index.php
- To connect to the remote server, you should run the following command on terminal
`ssh cs15lwi23anc@ieng6.ucsd.edu` 
- Make sure to type the correct password and the following should display
- <img width="529" alt="CleanShot 2023-01-11 at 14 22 14@2x" src="https://user-images.githubusercontent.com/36582468/211930597-c0946bba-d805-4754-97a3-5afbb0f3f144.png">

**3. Trying Some Commands**
- After connecting to the remote server you can run the following commands
```
cd ~
cd
ls -lat
ls -a
ls <directory> where <directory> is /home/linux/ieng6/cs15lwi23/cs15lwi23abc, where the abc is one of the other group members’ username
cp /home/linux/ieng6/cs15lwi23/public/hello.txt ~/
cat /home/linux/ieng6/cs15lwi23/public/hello.txt
```
- Running these commands will give these results: 
<img width="1502" alt="CleanShot 2023-01-11 at 14 26 43@2x" src="https://user-images.githubusercontent.com/36582468/211931316-83436ae6-5b77-45ff-ba70-d79221fd0e76.png">
- *Sidenote: You can use Ctrl-D or the exit command to exit the remote server*
