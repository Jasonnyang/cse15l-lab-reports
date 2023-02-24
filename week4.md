## Week 4 lab report
1. Setup Delete any existing forks of the repository you have on your account<br>
I ran the command ```rm -rf lab7``` to delete the lab7 folder. Then I deleted any forks of the repository that I had on my account on Github. <br>
![CleanShot 2023-02-23 at 19 03 52](https://user-images.githubusercontent.com/36582468/221081949-5b1a7df1-90bc-45d7-983b-00503075e39b.png)
<img width="322" alt="CleanShot 2023-02-23 at 19 04 26@2x" src="https://user-images.githubusercontent.com/36582468/221082017-e846da58-1f89-4178-a802-9e0e8b2366f3.png">

2. Setup Fork the repository <br>
![CleanShot 2023-02-23 at 19 17 28](https://user-images.githubusercontent.com/36582468/221083600-2f52edaa-d062-4987-992b-276837dfe341.png) <br>
I pressed the fork button on the top right of the screen which took me to this page. I pressed the green create fork button in order to fork the repository. <br>

3. The real deal Start the timer!<br>
<img width="659" alt="CleanShot 2023-02-23 at 19 01 26@2x" src="https://user-images.githubusercontent.com/36582468/221081595-0ed7f8c2-271c-4aba-b968-a2138dc2fe6b.png"> <br>
Started the timer! <br>

4. Log into ieng6 <br>
<img width="761" alt="CleanShot 2023-02-23 at 19 00 00@2x" src="https://user-images.githubusercontent.com/36582468/221081401-f98cad12-8323-4830-b733-81c942e43c21.png">
I logged into ieng6 by typing 
```
ssh cs15lwi23anc@ieng6.ucsd.edu
``` 
Because I ran the command earlier that day, I was able to type ```<up><up><up><up><up><up><enter>``` to save some typing. <br>

5. Clone your fork of the repository from your Github account
<img width="722" alt="CleanShot 2023-02-23 at 19 18 38@2x" src="https://user-images.githubusercontent.com/36582468/221083758-26f5157c-0b60-4f31-a78a-fb2dd362ee32.png">
I ran the command ```git clone git@github.com:Jasonnyang/lab7.git``` in order to clone. I got the url by going to my forked repository and clicking ssh and copying the url, shown in the image below. <br>
![CleanShot 2023-02-23 at 19 23 53](https://user-images.githubusercontent.com/36582468/221084403-6486567a-7f5e-440f-bfb6-57c5de556b04.png) <br>

6. Run the tests, demonstrating that they fail <br>
I ran the commands ```cd lab7/``` to enter the lab7 directory and then I ran ```javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java``` in order to compile the java files in the directory. Then I ran ```java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests``` to actually run the test file. 
<img width="966" alt="CleanShot 2023-02-23 at 19 27 27@2x" src="https://user-images.githubusercontent.com/36582468/221084904-426ad797-3ed3-4d3a-bedb-4425ca2b1b64.png">

7. Edit the code file to fix the failing test <br>
Because there was an error, I used the command ```nano ListExample.java``` to open up the ListExample file to fix the error. The error was a line where it says ```index1 += 1;``` which I changed to ```index2 += 1;``` to fix the issue. 
<img width="976" alt="CleanShot 2023-02-23 at 19 29 32@2x" src="https://user-images.githubusercontent.com/36582468/221085119-d5377680-6483-453f-9800-a09cf053d4a5.png">
I then used ```Ctrl-O, <Enter>, Ctrl-X``` to save the edits. 

8. Run the tests, demonstrating that they now succeed <br>
I then reran the javac and java commands by typing ```<up><up><up><enter>``` to run the javac commmand and then ```<up><up><up><enter>``` to run the java command. <br>
<img width="966" alt="CleanShot 2023-02-23 at 19 31 47@2x" src="https://user-images.githubusercontent.com/36582468/221085368-d0304e04-9207-4f2b-849d-77d4ce5981f5.png">

9. Commit and push the resulting change to your Github account (you can pick any commit message!)
Finally I ran ```git add .``` to add all the files to be tracked. Then I ran ```git commit -m "Commit"``` to get my code ready to be committed. Then I ran ```git push origin main ``` in order to push my code to Github. 
<img width="505" alt="CleanShot 2023-02-23 at 19 33 15@2x" src="https://user-images.githubusercontent.com/36582468/221085533-3984257c-48c0-4be9-abbe-c13cd82bc8a2.png">
