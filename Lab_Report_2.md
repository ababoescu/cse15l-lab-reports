**Lab Report 2 - Servers and Bugs:**


**Part 1**: Writing a web server called StringServer that stores and print string inputs, concatenating a new line each time a string is added.

Code:

![Image 1-28-23 at 11 22 PM](https://user-images.githubusercontent.com/122492492/215312049-1dd26071-1f5c-433e-baf6-2fb1dd741e03.jpg)

Output 1 (when typing /add-message?s=Hello):

![Image 1-28-23 at 11 24 PM](https://user-images.githubusercontent.com/122492492/215312166-b1f8433b-adab-4356-8c12-c47b73789731.jpg)
To achieve the output of the image above, I had to first create a method that handles the a url request and in this method I created a url path that contains the string "/add-message", from this path I had then to create a query that asks for a string variable _s_ that the user would input and be printed on the web page. 
