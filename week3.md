## Week 3 lab report
**Using the Grep command** <br>
*Using the -c argument* <br>
<img width="815" alt="CleanShot 2023-02-07 at 17 26 14@2x" src="https://user-images.githubusercontent.com/36582468/217404917-18d44186-113d-4a5c-9413-13b54de88cd3.png"> <br>
When using the -c argument on a directory, it shows all of the files in the directory and the number of times the target word shows up in file. <br>
<img width="879" alt="CleanShot 2023-02-07 at 17 28 19@2x" src="https://user-images.githubusercontent.com/36582468/217405185-122bf0f8-dcc7-49af-b027-92762e1fe273.png"> <br>
When using the -c argument on a file, the file name no longer shows up and only the number of times the target word shows up is displayed in the output. <br>

*Using the -l argument* <br>
<img width="879" alt="CleanShot 2023-02-07 at 17 50 14@2x" src="https://user-images.githubusercontent.com/36582468/217408106-30824cbc-eb13-41a9-a2f9-f9d5f770092e.png"> <br>
When using the -l argument on a file, the file will show back up in the output only if it contains the specified phrase or word in it. The file did not show up because the file does contain the word recommend so nothing is returned. <br> 
<img width="793" alt="CleanShot 2023-02-07 at 18 19 30@2x" src="https://user-images.githubusercontent.com/36582468/217412023-38816bbd-084a-4cf2-bbaa-1859f7872517.png"> <br>
When using the -l argument on a directory, the files with the word recommend will show up. These files match the output from the -c command. <br>

*Using the -L argument* <br>
<img width="872" alt="CleanShot 2023-02-07 at 17 49 55@2x" src="https://user-images.githubusercontent.com/36582468/217408059-bfad7a31-26f5-4842-8857-ec3fb1067cab.png"> <br>
When using the -L argument on a file, the file will show back up in the output only if it does not contains the specified phrase or word in it. The file showed up because the file does not contain the word recommend. <br>
<img width="777" alt="CleanShot 2023-02-07 at 18 21 26@2x" src="https://user-images.githubusercontent.com/36582468/217412301-65c68495-bc85-4285-b1f7-a8efa25b0277.png"> <br>
When using the -L argument on a directory, the files without the word in the files will show up again. The files that showed up when using -l will not show up again if you use -L because a file either contains or does not contain the target word. <br>

*Using the -v argument* <br>
<img width="983" alt="CleanShot 2023-02-07 at 18 25 16@2x" src="https://user-images.githubusercontent.com/36582468/217412872-94e802d5-20f2-4fc9-a349-5d6f04ea0503.png"><br>
When using the -v argument on a directory as typed below, it causes all the lines in the directory without the target word to be displayed. In this case, the directory is giant and many lines were printed out since there are a lot of lines without the word recommend. <br>
<img width="948" alt="CleanShot 2023-02-07 at 18 27 20@2x" src="https://user-images.githubusercontent.com/36582468/217413100-08f09185-b35d-4ec9-8bca-b2771b8f0e78.png"> <br>
When using the -v argument on a file, it prints out all the lines in the file that don't contain the word recommend. It is interesting how it also prints out empty lines. <br>
 
**Sources** <br>
I used the ```man grep``` command in the terminal to get a list of all the command line arguments that I could use for grep. I found the examples section to be useful. In addition I referred to the lab materials from week 4 in order to refresh my understanding of grep. 
