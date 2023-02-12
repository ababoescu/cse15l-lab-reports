**Lab Report 2 - Servers and Bugs:**


**Part 1**: Writing a web server called StringServer that stores and print string inputs, concatenating a new line each time a string is added.

Code:



<img width="425" alt="Screen Shot 2023-02-11 at 10 28 22 PM" src="https://user-images.githubusercontent.com/122492492/218296608-3ec1e369-acf3-4b03-9f16-34100be22fd3.png">





Output 1 (when typing /add-message?s=Hello):

![Image 1-28-23 at 11 24 PM](https://user-images.githubusercontent.com/122492492/215312166-b1f8433b-adab-4356-8c12-c47b73789731.jpg)

To achieve the output of the image above, I had to first create a method called HandleRequest that handles a url request and in this method I created a url path that contains the string "/add-message", from this path I had to then create a query that asks for a string variable _s_ that the user would input and be printed on the web page. 

Relevant arguments used in this method are two string variables assigned to the args parameters, the first string being "s" and the second string an input that the user would insert into the url. Another revelant field is an array list that was created to store the memory of the strings inputed by the user, so that they may be displayed when the user types in a new string into the url.

Values that are relevant are the strings that take the user's input, that are labeled parameters, and the array list that stores the string.


Output 2 (when typing /add-message?s=How are you):

![Image 1-28-23 at 11 25 PM](https://user-images.githubusercontent.com/122492492/215393805-e58c8c1e-914a-4d1e-8ecd-9955c57ac2d8.jpg)


This output follows the same methods as the output above, with the same relevant arguments to these methods. This output helps to demonstrate how the string is being stored in an array list (the memory), that each time the 
user writes a new string at the end of "/add-message?s=" that string would be printed below the string previosly inputed before it, as shown in the image. This specific output, with the next string appearing below the previous string is a achieved by concatenating "\n" to the end of each string inputed.

The only value that changes for this output is the string inputed by the user into the url ("How are you"), leading to it being stored into an array list and being printed out below the first string ("Hello"). From the image below you can see how the strings are being stored in the array list in the terminal.

<img width="455" alt="Screen Shot 2023-01-30 at 6 08 28 PM" src="https://user-images.githubusercontent.com/122492492/215641739-76e6b812-6fba-425d-be65-d4762eebf8ea.png">



**Part 2:** Choosing a bug from lab 3

Code being tested:
```
#code block
static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
}
```

A failure-inducing input for the buggy program:
```
# code block
@Test
public void testReversed2(){
  // the input array
  int[] input2 = {1,2,3};
  // expected output of test case: {3,2,1}
  assertArrayEquals(new int[]{3,2,1}, ArrayExamples.reversed(input2));
}
 ```

An input that doesn't induce a failure:
```
#code block
@Test
public void testReversed() {
  // the input array
  int[] input1 = { };
  // expected output of the test case: { }
  assertArrayEquals(new int[]{ }, ArrayExamples.reversed(input1));
}
```


<img width="537" alt="Screen Shot 2023-02-11 at 10 27 11 PM" src="https://user-images.githubusercontent.com/122492492/218296564-7a87a11c-ca0e-460a-b7c8-97e77fbfdcff.png">



```
#code after
static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[arr.length - i - 1]; //this line is changed
    }
    return newArray; //this line is changed
}
```
Fix: The array should be creating a new array with the newArray being assigned on the left rather than the right. So it’s supposed to be newArray[i] = arr[arr.length-i-1]. The reason the previous code was wrong was because arr was getting assigned with an empty array (newArray).


**Part 3:** Something I learned
Something that I learned about, that I didn't know about before, was using URLS to create a web server. More specifically on taking a URL as an input and respond with the text of a web page (an example of this can be demonstrated in Part 1). I also learned how to run the server on my local computer.

