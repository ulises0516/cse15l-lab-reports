``` ==Question== ```       ``` Post```
Title: Confused on why my code is wrong
Categroy ```==Debugging==```

What environment are you using (computer, operating system, web browser, terminal/editor, and so on)?
I am on mac using visual studio code.

Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead. Screenshots are great, copy-pasted terminal output is also great. Avoid saying “it doesn't work”.

The symptom Im seeing is that when I am running my bash script it is saying I need to implement public static void which is very confusing because im certain we dont need to do this or a JavaFX application class must extend javafx.application.Application. Im confused on what this mean I have never seen error before .
                         
Detail the failure-inducing input and context. That might mean any or all of the command you're running, a test case, command-line arguments, working directory, even the last few commands you ran. Do your best to provide as much context as you can.

I didnt run any special commands. I ran the bash script that included the javac and java steps to compile and run my code. So it would be faster in writing. I dont know why this is happening. Just in case I will provide my bash script.




![Screenshot 2023-06-05 at 4 59 55 PM](https://github.com/ulises0516/cse15l-lab-reports/assets/125671517/adc8044a-0866-46ce-945f-e7a273d7912e)



## TA response 

Hi, thanks for being specific in your response. Your problem is in your bash script you need to  use org.junit.runner.JUnitCore to actually run your tests from the command line.




