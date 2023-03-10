## Week 5 lab report

I am improving on lab report 4 and creating a bash script to do the task very quickly. 
1. To begin, create a bash script called speed.sh
2. You still need to do the setup setup steps manually so...
3. Delete any existing forks of the repository you have on your account<br>
I ran the command ```rm -rf lab7``` to delete the lab7 folder. Then I deleted any forks of the repository that I had on my account on Github. <br>
![CleanShot 2023-02-23 at 19 03 52](https://user-images.githubusercontent.com/36582468/221081949-5b1a7df1-90bc-45d7-983b-00503075e39b.png)
<img width="322" alt="CleanShot 2023-02-23 at 19 04 26@2x" src="https://user-images.githubusercontent.com/36582468/221082017-e846da58-1f89-4178-a802-9e0e8b2366f3.png">

4. Setup Fork the repository <br>
![CleanShot 2023-02-23 at 19 17 28](https://user-images.githubusercontent.com/36582468/221083600-2f52edaa-d062-4987-992b-276837dfe341.png) <br>
I pressed the fork button on the top right of the screen which took me to this page. I pressed the green create fork button in order to fork the repository. <br>

5. Now is when you can start using the bash script to speed things up<br>

6. Log into ieng6 by typing ```ssh cs15lwi23anc@ieng6.ucsd.edu``` into the bash script<br>

7. To clone your fork of the repository from your Github account, run the command ```git clone git@github.com:Jasonnyang/lab7.git``` but you need to press the fork button on github before running the script. 

8. Run the tests, demonstrating that they fail <br>
I entered the commands ```cd lab7/``` to enter the lab7 directory and then I ran ```javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java``` in order to compile the java files in the directory. Then I ran ```java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests``` to actually run the test file. All of these commands went into the bash script. 

9. Now is where the first bash script ends and this is what the bash script should look like when you type it out and run it. 
<img width="834" alt="CleanShot 2023-03-09 at 20 21 25@2x" src="https://user-images.githubusercontent.com/36582468/224222684-ac03dbe7-aea0-4d1d-8697-67ae832d3310.png">

10. Edit the code file to fix the failing test <br>
Because there was an error, I used the command ```nano ListExample.java``` to open up the ListExample file to fix the error. The error was a line where it says ```index1 += 1;``` which I changed to ```index2 += 1;``` to fix the issue. 
<img width="976" alt="CleanShot 2023-02-23 at 19 29 32@2x" src="https://user-images.githubusercontent.com/36582468/221085119-d5377680-6483-453f-9800-a09cf053d4a5.png">
I then used ```Ctrl-O, <Enter>, Ctrl-X``` to save the edits. 

11. Create a second bash script called speed1.sh to complete the rest of the tasks. 
12. I used these commands from earlier and put them in my second script. ```javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java``` and ```java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests```

13. Commit and push the resulting change to your Github account (you can pick any commit message!)
I added ```git add .``` to add all the files to be staged. Then I added ```git commit -m "Commit"``` to get my code committed. Then I added ```git push origin main``` in order to push my committed code to Github.
14. The final script should look like this when you run it 
