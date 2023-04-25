# Lab Report 2 



---
## Part 1
---

**String Server Code implementation**

*This is my code*
```
 StringBuilder s= new StringBuilder();
    public String handleRequest(URI url) {
        if (url.getPath().contains("/add")) {
            String[] parameter0 = url.getQuery().split("=");
            if (parameter0[0].equals("s")) {
                s.append( parameter0[1] + "\n");
                return s.toString();

            }
        }

        return "404 Not Found!";

    }
}
```
![Server in Real time with 1 Request](<img width="776" alt="Screenshot 2023-04-24 at 10 17 04 PM" src="https://user-images.githubusercontent.com/125671517/234181596-d37b3bc0-3acb-4339-9db4-6d7d96abcd47.png">
)


![Server in Real time with 2 request](<img width="794" alt="Screenshot 2023-04-24 at 10 17 14 PM" src="https://user-images.githubusercontent.com/125671517/234181724-0ac90eb3-391a-4bda-88f8-5a84427a4d60.png">
)	

---
**Methods Called(in previous two images)**

 *Server start is called 
 *Handle is called
 *Append is called
 *toString is called
 *.equals() is called
 *getPath() is called 
 *contains is called 
 *HandleRequest is called

---

**Relevant arguments to those method**

Revelant Arguments is the url , the path , what is placed after the "=" sign
and what is before the equals sign.

---

**How do the values of any relevant fields of the class change from this specific request?**
 An invalid path would return an "error 404" or if the value before the "=" is not s which will throw an error as well. If there is "=" the values can be split and so an error woould occur. 


---


## Part 2
---


**Failure Inducing Junit test**
```ruby
@Test
public void testReverseMultipleInPlace() {
    int[] input1 = { 1, 2, 3 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[] { 3, 2, 1 }, input1);
  }
```
**SideNote:** This Junit test failed because the Progam didnt account for. 
an **Array** size of more than 1 element causing the program to fail. 

**Passed Junit test**
```ruby
@Test
public void testReverseInPlace() {
    int[] input1 = { 3 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[] { 3 }, input1);
  }
```
**Side Note**This this Junit test passed because of the array size. 
the program worked because the code for ReverseInPlace was correct
for an **Array** that holds a singular element.

---
**What was the Symptom?** 

To see faulty program behavior you can see outputed look at figure 1.1. 

![Figure 1.1 ](<img width="699" alt="Screenshot 2023-04-20 at 4 33 45 PM" src="https://user-images.githubusercontent.com/125671517/234164381-a73c6a90-0c6a-4889-91a6-fde18129de32.png">
)
---
**What was the Bug?**



   *Program with bug*
```ruby
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }
```
  *Program without bug(fixed)* 
 ```ruby
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length/2; i += 1) {
      int temp = arr[i];
      arr[i] = arr[arr.length - i - 1];
      arr[arr.length - i - 1]= temp;
    }
    
  }
```
---
**What did the new implmenetation actually do**

* I implemented ```i < arr.length/2``` to stop the code from looping twice. 
 ``` i < arr.length```essentially reverses the array then reverses again which goes back to the original array position.
* I also added ``` int temp = arr[i]``` as a temp variable to hold the value of the original 
value at i index in the arr Array. Which makes the middle value stay the same. ``` arr arr[arr.length - i - 1]= temp; ``` then sets the changed index to original value .
---

---
## Part 3 
---

**What I learned**

I learned thatt Junit test can be quite helpful in debugging your code. In testing from the ground up can unveil new bugs in your program. I learned to closely look at your symptom what ever you output to know where to look to find the bug. I also learned how to start up a server which is very cool!.








