# Lab Report 2 


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
**What did the new implmenetation Do**

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








