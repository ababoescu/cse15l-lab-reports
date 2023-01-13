Week 1 Lab Report: a tutorial to log into a course-specific account on ieng6


Step 1: Downloading and Installing Visual Studio Code (VScode)
![image](https://user-images.githubusercontent.com/122492492/211933489-5f24d739-67df-4201-b66a-ef0b010a79d2.png)

For this step I already have Visual Studio Code downloaded into my own computer and could skip the installation step (the installation can be skipped as well when using a computer from one of the labs in the Engineering building). If you have not already downloaded Visual Studio Code, go to there website through this link: https://code.visualstudio.com/, and follow the instructions provided to install it onto your computer (pay attention to the different versions being offered for Macs and Windows). Once installed, you should be able to open a window that looks similar to the image above. If you are accessing Visual Studio Code from a computer in the lab, you simply need to search for it in the search bar on the bottom left of the screen and click on it to open a window that looks like the image provided above.




Step 2: Remotely Connecting

Part 1: For this step, if you are connecting through a computer in the lab (as I was) you just need to open a terminal in VScode. You can do this by clicking "Terminal" on upper left of the window then clicking the "New Terminal" menu option, another method is pressing Ctrl/Command + '. When you are in the terminal, type "ssh cs15lwi23zz@ieng6.ucsd.edu" where "zz" are the letters in your course-specific account (for example: ssh cs15lwi23bc@ieng6.ucsd.edu). Press enter.
You should receive a message such as the one in the image below:

<img width="634" alt="Screen Shot 2023-01-13 at 1 12 50 PM" src="https://user-images.githubusercontent.com/122492492/212420132-49ac6f78-67b6-435d-befc-d287451d94fc.png">

You will be asked "Are you sure you want to continue connecting (yes/no/[fingerprint])? Answer: "Yes", as shown in the image above.
Your screen would appear like this:
<img width="635" alt="Screen Shot 2023-01-13 at 1 15 47 PM" src="https://user-images.githubusercontent.com/122492492/212420582-ff0373bb-a2ab-419c-a7c0-ec58b23f4075.png">

Part 2: Since it is most likely your first time connecting to a server, you will need to set up a password (If this is not your first time or your password is already set up, skip to Part 3 of Step 2). For CSE15L, you can access your course-specific account through this link: https://sdacs.ucsd.edu/~icc/index.php. Once you have accessed your account, there should be a link prompting you to change your password, click the link and follow the instructions provided to create your password (Make sure your password is at least 13 characters long!). Make sure to answer the following questions with these answers:

Change MyTritonLink password? [No]

Change course-specific account passwords? [Yes]

Once you have reached the end, DO NOT click "Check Password" just press your enter key.
Once your password is set, you'll have to wait at least 15 minutes before using it.

Part 3: Once your password is set up, type your password next to the prompt "Password: " displayed on your terminal. Password will not appear when you type it (don't worry, it is there). Once you are done, press enter and your terminal should display something similar to the image below:
<img width="350" alt="Screen Shot 2023-01-13 at 1 45 01 PM" src="https://user-images.githubusercontent.com/122492492/212424960-88226b4c-4e80-452f-b8cc-621145172627.png">


Step 3: Trying Some Commands
<img width="513" alt="Screen Shot 2023-01-13 at 2 20 02 PM" src="https://user-images.githubusercontent.com/122492492/212429830-b8950e70-6524-4d61-a779-29a4ae46103a.png">
