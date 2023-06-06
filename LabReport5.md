# Lab Report 5

## Student question
``` ruby
Question
```       

```ruby
Post
```

**Title:** Why is My script producing a different output 

Category
```ruby
Debugging
```

**What environment are you using (computer, operating system, web browser, terminal/editor, and so on)?**

I am on mac using visual studio code.



**Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead. Screenshots are great, copy-pasted terminal output is also great. Avoid saying “it doesn't work”.**


The symptom Im seeing is that it is saying that Im using an import statement when im not. It producing and printing the message that im using an import statement. I provided screenshots below.


                         
**Detail the failure-inducing input and context. That might mean any or all of the command you're running, a test case, command-line arguments, working directory, even the last few commands you ran. Do your best to provide as much context as you can.**



I didnt run any special commands. I ran the bash script that included the javac and java steps to compile and run my code. So it would warn me if I accidentally used an import that I wasnt suppose to use


**SideNote:**

I provided some extra information on what each screen shot shows.





This shows the file my bash Script is running on and running the test.

![Screenshot 2023-06-05 at 7 58 01 PM](https://github.com/ulises0516/cse15l-lab-reports/assets/125671517/fd5dec35-6c4b-4476-ae72-e6b7797560c9)

This shows the code of my bash script and what it does

![Screenshot 2023-06-05 at 7 58 08 PM](https://github.com/ulises0516/cse15l-lab-reports/assets/125671517/b590dfaa-9a46-4d4a-9ae3-2b70b171f5ce)


This shows my working directory and files 

![Screenshot 2023-06-05 at 8 15 37 PM](https://github.com/ulises0516/cse15l-lab-reports/assets/125671517/3b62bdbc-8c8f-424a-ac00-2b3d3ffc9651)





## TA Response 

Hi, thanks for being specific in your response. Your problem is in your bash script you need to be more specific in your grep command instead of using and remeber the function of grep -q. Which doesnt need to match exact line but rather a partially of the line. So if you have a slashed out import statement which techincally means you're not using an import statement your bash script would read this line as still valid. I suggest using grep -x instead which has to match your given import statement you're not allowed to use exactly.


## Students Response

Hey Thanks! The example you gave was in fact the same thing happening to me. I previously slashed out an import statement and forgot about it when i made the bash script. The bug was produced by the command ```grep -q``` on the line ```//import java.util.ArrayList;``` although it was slashed out so technically Im not using the import statment and should not say dont use import. My bash script would still read it because it still ```grep -q``` will still partially matches the input(import java.util.ArrayList;) I gave it. When I used grep -x it gave me the right produced output. I was looking for because it matches the exact input I gave the bash script to look out for which was ```import java.util.ArrayList;``` . Thanks for the help it was a difficult bug and I spent hours on it.


This shows my code working and the slashed out import statement I was using.
![Screenshot 2023-06-05 at 8 07 53 PM](https://github.com/ulises0516/cse15l-lab-reports/assets/125671517/1273fb0f-6ee2-4147-a72a-4ce2286b54cd)







