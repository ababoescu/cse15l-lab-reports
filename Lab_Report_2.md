**Lab Report 2 - Servers and Bugs:**


**Part 1**: Writing a web server called StringServer that stores and print string inputs, concatenating a new line each time a string is added.

Code:

![Image 1-28-23 at 11 22 PM](https://user-images.githubusercontent.com/122492492/215312049-1dd26071-1f5c-433e-baf6-2fb1dd741e03.jpg)

Output 1 (when typing /add-message?s=Hello):

![Image 1-28-23 at 11 24 PM](https://user-images.githubusercontent.com/122492492/215312166-b1f8433b-adab-4356-8c12-c47b73789731.jpg)

To achieve the output of the image above, I had to first create a method that handles the a url request and in this method I created a url path that contains the string "/add-message", from this path I had then to create a query that asks for a string variable _s_ that the user would input and be printed on the web page. 

Relevant arguments used in this method are two string variables assigned to the args parameters, the first string being "s" and the second string an input that the user would insert into the url. Another revelant argument is an array list that was created to store the memory of the strings inputed by the user, so that they may be displayed when the user types in a new string into the url.

Values that are relevant are the strings that take the user's input, that are labeled parameters, and the array list that stores the string.


Output 2 (when typing /add-message?s=How are you):

![Image 1-28-23 at 11 25 PM](https://user-images.githubusercontent.com/122492492/215393805-e58c8c1e-914a-4d1e-8ecd-9955c57ac2d8.jpg)


This output follows the same methods as the output above, with the same relevant arguments to these methods. This output helps to demonstrate how the string is being stored in an array list (the memory), that each time the 
user writes a new string at the end of "/add-message?s=" that string would be printed below the string previosly inputed before it, as shown in the image. This specific output, with the next string appearing below the previous string is a achieved by concatinating "\n" to the end of each string inputed.

The only value that changes for this output is the string inputed by the user into the url ("How are you"), leading to it being stored into an array list and being printed out below the first string ("Hello").
