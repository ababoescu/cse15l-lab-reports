# Lab Report 4: Get ready... Get set... CODE!

## Step 4: Log into ieng6

<img width="465" alt="Screen Shot 2023-02-27 at 6 31 18 PM" src="https://user-images.githubusercontent.com/122492492/221738120-7163ef7a-929b-462b-8666-e4173df26b98.png">

Keys pressed: `ssh c<tab><enter>`

The `ssh cs15lwi23abg@ieng6.ucsd.edu` command was in my computer's search history, so I was able to simply access it by only ssh and the first letter of the server.


## Step 5: Clone fork of the repository from Github account

<img width="595" alt="Screen Shot 2023-02-27 at 6 37 47 PM" src="https://user-images.githubusercontent.com/122492492/221739132-f1dbb907-f00f-4074-b2bc-bf4d71e04bb7.png">

Keys pressed: `<Ctrl-R>git c<enter>`

The `git clone git@github.com:ababoescu/lab7.git` command was in my command history, so I used Ctrl-R to access it.


## Step 6: Run tests, demonstrating that they fail

<img width="626" alt="Screen Shot 2023-02-27 at 7 26 18 PM" src="https://user-images.githubusercontent.com/122492492/221745732-2afad855-7e0a-4605-8204-eba9c3a9a34a.png">


Keys pressed: `cd l<tab><enter>`,`<Ctrl-R>javac -<enter>`,`<Ctrl-R>java -<enter>`

I changed directories with the `cd lab7/` command by simply typing 'cd l' and tabing to auto-complete. Then I ran the tests, first using the `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` command, which was in my bash history, so I used Ctrl-R to access it. The same was with the `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests`, so I accessed and ran it in the same way.


## Step 7: Edit code file to fix failing test

<img width="627" alt="Screen Shot 2023-02-27 at 6 58 40 PM" src="https://user-images.githubusercontent.com/122492492/221742228-1ab24529-8329-4f7b-9572-41befa9ea43e.png">
<img width="612" alt="Screen Shot 2023-02-27 at 6 59 07 PM" src="https://user-images.githubusercontent.com/122492492/221742287-92cc7ac4-97b5-435e-a74a-e57573debfb5.png">

Keys pressed: `<Ctrl-R>n<enter>`,`<Ctrl-W>while(index2<enter><down><down><right><right><right><right><right><right><right><right><delete>2`,`<Ctrl-O><enter>`,`<Ctrl-X>`

The `nano ListExamples.java` command, to access and edit my code file, was in my command history, so I used Ctrl-R to access it. I then used Ctrl-W to search for the closes unique line of code closest to the line which I hope to fix, that line of code being `while(index2 < list2.size()) {`. I then moved the cursor down twice and right eight times before deleting the 1 and replacing it with 2. I then used `<Ctrl-O><enter>` to save and `<Ctrl-X>` to exit.

## Step 8: Run tests, demonstrate that they now succeed

<img width="626" alt="Screen Shot 2023-02-27 at 7 11 32 PM" src="https://user-images.githubusercontent.com/122492492/221743944-e99134de-5a0e-4a0a-a0cd-e991482a5b8c.png">

Keys pressed: `<Ctrl-R>javac -<enter>`,`<Ctrl-R>java -<enter>`

I accessed and ran the same test commands as I did in **Step 6**, using Ctrl-R since the commands are already saved in my bash history. This time the tests are shown to all be passing.


## Step 9: Commit and push resulting change to Github account

<img width="627" alt="Screen Shot 2023-02-27 at 7 16 47 PM" src="https://user-images.githubusercontent.com/122492492/221744636-76eb1291-5ef3-41ab-9998-fb2c292f3e5a.png">

Keys pressed: `<Ctrl-R>git a<enter>`,`<Ctrl-R>git c<enter>`,`<Ctrl-R>git p<enter>`

The `git add ListExamples.java` command was in my bash history, so I used Ctrl-R to access and run it. I did the same with the commands `git commit -m "Update"` and `git push origin main` to access them and run them.
